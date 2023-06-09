# Comparing `tmp/ydb-3.3.4.tar.gz` & `tmp/ydb-3.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ydb-3.3.4.tar", last modified: Thu May 25 14:36:51 2023, max compression
+gzip compressed data, was "ydb-3.3.5.tar", last modified: Fri Jun  9 15:18:35 2023, max compression
```

## Comparing `ydb-3.3.4.tar` & `ydb-3.3.5.tar`

### file list

```diff
@@ -1,272 +1,272 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:36:51.173507 ydb-3.3.4/
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-05-25 14:36:37.000000 ydb-3.3.4/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (123)    11361 2023-05-25 14:36:37.000000 ydb-3.3.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-25 14:36:37.000000 ydb-3.3.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1669 2023-05-25 14:36:51.173507 ydb-3.3.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-05-25 14:36:37.000000 ydb-3.3.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-25 14:36:37.000000 ydb-3.3.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-25 14:36:37.000000 ydb-3.3.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 14:36:51.173507 ydb-3.3.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-05-25 14:36:42.000000 ydb-3.3.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:36:51.129507 ydb-3.3.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 14:36:37.000000 ydb-3.3.4/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:36:51.133507 ydb-3.3.4/tests/aio/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 14:36:37.000000 ydb-3.3.4/tests/aio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4356 2023-05-25 14:36:37.000000 ydb-3.3.4/tests/aio/test_async_iter_stream.py
--rw-r--r--   0 runner    (1001) docker     (123)     1870 2023-05-25 14:36:37.000000 ydb-3.3.4/tests/aio/test_connection.py
--rw-r--r--   0 runner    (1001) docker     (123)     3822 2023-05-25 14:36:37.000000 ydb-3.3.4/tests/aio/test_connection_pool.py
--rw-r--r--   0 runner    (1001) docker     (123)     3431 2023-05-25 14:36:37.000000 ydb-3.3.4/tests/aio/test_session_pool.py
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-05-25 14:36:37.000000 ydb-3.3.4/tests/aio/test_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     7329 2023-05-25 14:36:37.000000 ydb-3.3.4/tests/aio/test_tx.py
--rw-r--r--   0 runner    (1001) docker     (123)     3188 2023-05-25 14:36:37.000000 ydb-3.3.4/tests/aio/test_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     6006 2023-05-25 14:36:37.000000 ydb-3.3.4/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-05-25 14:36:37.000000 ydb-3.3.4/tests/session_pool.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:36:51.133507 ydb-3.3.4/tests/ssl/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 14:36:37.000000 ydb-3.3.4/tests/ssl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-05-25 14:36:37.000000 ydb-3.3.4/tests/ssl/test_ssl.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:36:51.137507 ydb-3.3.4/tests/table/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 14:36:37.000000 ydb-3.3.4/tests/table/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2334 2023-05-25 14:36:37.000000 ydb-3.3.4/tests/table/table_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6666 2023-05-25 14:36:37.000000 ydb-3.3.4/tests/table/test_tx.py
--rw-r--r--   0 runner    (1001) docker     (123)      531 2023-05-25 14:36:37.000000 ydb-3.3.4/tests/test_errors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:36:51.141507 ydb-3.3.4/tests/topics/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 14:36:37.000000 ydb-3.3.4/tests/topics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-05-25 14:36:37.000000 ydb-3.3.4/tests/topics/test_control_plane.py
--rw-r--r--   0 runner    (1001) docker     (123)     8086 2023-05-25 14:36:37.000000 ydb-3.3.4/tests/topics/test_topic_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)    10281 2023-05-25 14:36:37.000000 ydb-3.3.4/tests/topics/test_topic_writer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:36:51.145507 ydb-3.3.4/ydb/
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3032 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_apis.py
--rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_errors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:36:51.145507 ydb-3.3.4/ydb/_grpc/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_grpc/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:36:51.145507 ydb-3.3.4/ydb/_grpc/common/
--rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_grpc/common/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:36:51.145507 ydb-3.3.4/ydb/_grpc/grpcwrapper/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_grpc/grpcwrapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8860 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_grpc/grpcwrapper/common_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      719 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_grpc/grpcwrapper/ydb_scheme.py
--rw-r--r--   0 runner    (1001) docker     (123)    45284 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_grpc/grpcwrapper/ydb_topic.py
--rw-r--r--   0 runner    (1001) docker     (123)     5865 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_grpc/grpcwrapper/ydb_topic_public_types.py
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_grpc/grpcwrapper/ydb_topic_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:36:51.149507 ydb-3.3.4/ydb/_grpc/v3/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_grpc/v3/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:36:51.157507 ydb-3.3.4/ydb/_grpc/v3/protos/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_grpc/v3/protos/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:36:51.157507 ydb-3.3.4/ydb/_grpc/v3/protos/annotations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_grpc/v3/protos/annotations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12213 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_grpc/v3/protos/annotations/validation_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_grpc/v3/protos/annotations/validation_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6184 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_grpc/v3/protos/ydb_auth_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_grpc/v3/protos/ydb_auth_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    83179 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_grpc/v3/protos/ydb_cms_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_grpc/v3/protos/ydb_cms_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     7124 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_grpc/v3/protos/ydb_common_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_grpc/v3/protos/ydb_common_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)   121326 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_grpc/v3/protos/ydb_coordination_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_grpc/v3/protos/ydb_coordination_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    16470 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_grpc/v3/protos/ydb_discovery_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_grpc/v3/protos/ydb_discovery_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    41176 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_grpc/v3/protos/ydb_export_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_grpc/v3/protos/ydb_export_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4995 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_grpc/v3/protos/ydb_formats_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_grpc/v3/protos/ydb_formats_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    30782 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_grpc/v3/protos/ydb_import_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_grpc/v3/protos/ydb_import_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     7161 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_grpc/v3/protos/ydb_issue_message_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_grpc/v3/protos/ydb_issue_message_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    72285 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_grpc/v3/protos/ydb_monitoring_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_grpc/v3/protos/ydb_monitoring_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    29771 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_grpc/v3/protos/ydb_operation_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_grpc/v3/protos/ydb_operation_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    16311 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_grpc/v3/protos/ydb_query_stats_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_grpc/v3/protos/ydb_query_stats_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    40278 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_grpc/v3/protos/ydb_rate_limiter_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_grpc/v3/protos/ydb_rate_limiter_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    38051 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_grpc/v3/protos/ydb_scheme_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_grpc/v3/protos/ydb_scheme_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    25816 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_grpc/v3/protos/ydb_scripting_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_grpc/v3/protos/ydb_scripting_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6884 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_grpc/v3/protos/ydb_status_codes_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_grpc/v3/protos/ydb_status_codes_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)   332647 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_grpc/v3/protos/ydb_table_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_grpc/v3/protos/ydb_table_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)   234296 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_grpc/v3/protos/ydb_topic_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_grpc/v3/protos/ydb_topic_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    52587 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_grpc/v3/protos/ydb_value_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_grpc/v3/protos/ydb_value_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_grpc/v3/ydb_auth_v1_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2503 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_grpc/v3/ydb_auth_v1_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4418 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_grpc/v3/ydb_cms_v1_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    11170 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_grpc/v3/ydb_cms_v1_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4226 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_grpc/v3/ydb_coordination_v1_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     9797 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_grpc/v3/ydb_coordination_v1_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2610 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_grpc/v3/ydb_discovery_v1_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     4307 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_grpc/v3/ydb_discovery_v1_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_grpc/v3/ydb_export_v1_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     4370 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_grpc/v3/ydb_export_v1_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2527 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_grpc/v3/ydb_import_v1_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     4404 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_grpc/v3/ydb_import_v1_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2622 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_grpc/v3/ydb_monitoring_v1_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     4293 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_grpc/v3/ydb_monitoring_v1_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3688 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_grpc/v3/ydb_operation_v1_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    10345 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_grpc/v3/ydb_operation_v1_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4877 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_grpc/v3/ydb_rate_limiter_v1_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    11754 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_grpc/v3/ydb_rate_limiter_v1_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4012 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_grpc/v3/ydb_scheme_v1_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    10044 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_grpc/v3/ydb_scheme_v1_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3112 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_grpc/v3/ydb_scripting_v1_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6037 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_grpc/v3/ydb_scripting_v1_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    11659 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_grpc/v3/ydb_table_v1_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    36535 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_grpc/v3/ydb_table_v1_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4956 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_grpc/v3/ydb_topic_v1_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    14404 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_grpc/v3/ydb_topic_v1_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:36:51.161507 ydb-3.3.4/ydb/_grpc/v4/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_grpc/v4/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:36:51.165507 ydb-3.3.4/ydb/_grpc/v4/protos/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_grpc/v4/protos/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:36:51.169507 ydb-3.3.4/ydb/_grpc/v4/protos/annotations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_grpc/v4/protos/annotations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2727 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_grpc/v4/protos/annotations/validation_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_grpc/v4/protos/annotations/validation_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_grpc/v4/protos/ydb_auth_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_grpc/v4/protos/ydb_auth_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    12062 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_grpc/v4/protos/ydb_cms_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_grpc/v4/protos/ydb_cms_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_grpc/v4/protos/ydb_common_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_grpc/v4/protos/ydb_common_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    15716 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_grpc/v4/protos/ydb_coordination_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_grpc/v4/protos/ydb_coordination_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2871 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_grpc/v4/protos/ydb_discovery_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_grpc/v4/protos/ydb_discovery_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     9313 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_grpc/v4/protos/ydb_export_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_grpc/v4/protos/ydb_export_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_grpc/v4/protos/ydb_formats_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_grpc/v4/protos/ydb_formats_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6939 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_grpc/v4/protos/ydb_import_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_grpc/v4/protos/ydb_import_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1770 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_grpc/v4/protos/ydb_issue_message_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_grpc/v4/protos/ydb_issue_message_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     9769 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_grpc/v4/protos/ydb_monitoring_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_grpc/v4/protos/ydb_monitoring_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6165 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_grpc/v4/protos/ydb_operation_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_grpc/v4/protos/ydb_operation_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2849 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_grpc/v4/protos/ydb_query_stats_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_grpc/v4/protos/ydb_query_stats_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6057 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_grpc/v4/protos/ydb_rate_limiter_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_grpc/v4/protos/ydb_rate_limiter_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5830 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_grpc/v4/protos/ydb_scheme_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_grpc/v4/protos/ydb_scheme_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5143 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_grpc/v4/protos/ydb_scripting_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_grpc/v4/protos/ydb_scripting_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_grpc/v4/protos/ydb_status_codes_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_grpc/v4/protos/ydb_status_codes_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    46408 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_grpc/v4/protos/ydb_table_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_grpc/v4/protos/ydb_table_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    34953 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_grpc/v4/protos/ydb_topic_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_grpc/v4/protos/ydb_topic_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6618 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_grpc/v4/protos/ydb_value_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_grpc/v4/protos/ydb_value_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_grpc/v4/ydb_auth_v1_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2503 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_grpc/v4/ydb_auth_v1_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1868 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_grpc/v4/ydb_cms_v1_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    11170 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_grpc/v4/ydb_cms_v1_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1937 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_grpc/v4/ydb_coordination_v1_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     9797 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_grpc/v4/ydb_coordination_v1_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_grpc/v4/ydb_discovery_v1_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     4307 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_grpc/v4/ydb_discovery_v1_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_grpc/v4/ydb_export_v1_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     4370 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_grpc/v4/ydb_export_v1_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_grpc/v4/ydb_import_v1_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     4404 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_grpc/v4/ydb_import_v1_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_grpc/v4/ydb_monitoring_v1_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     4293 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_grpc/v4/ydb_monitoring_v1_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1776 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_grpc/v4/ydb_operation_v1_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    10345 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_grpc/v4/ydb_operation_v1_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2097 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_grpc/v4/ydb_rate_limiter_v1_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    11754 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_grpc/v4/ydb_rate_limiter_v1_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1789 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_grpc/v4/ydb_scheme_v1_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    10044 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_grpc/v4/ydb_scheme_v1_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1621 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_grpc/v4/ydb_scripting_v1_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6037 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_grpc/v4/ydb_scripting_v1_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3453 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_grpc/v4/ydb_table_v1_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    36535 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_grpc/v4/ydb_table_v1_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_grpc/v4/ydb_topic_v1_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    14404 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_grpc/v4/ydb_topic_v1_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    16278 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_session_impl.py
--rw-r--r--   0 runner    (1001) docker     (123)    14607 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_sp_impl.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:36:51.169507 ydb-3.3.4/ydb/_topic_common/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_topic_common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4659 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_topic_common/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     7957 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_topic_common/common_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1966 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_topic_common/test_helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:36:51.169507 ydb-3.3.4/ydb/_topic_reader/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_topic_reader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5528 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_topic_reader/datatypes.py
--rw-r--r--   0 runner    (1001) docker     (123)     7350 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_topic_reader/datatypes_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3716 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_topic_reader/topic_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)    23087 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_topic_reader/topic_reader_asyncio.py
--rw-r--r--   0 runner    (1001) docker     (123)    47528 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_topic_reader/topic_reader_asyncio_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5469 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_topic_reader/topic_reader_sync.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:36:51.169507 ydb-3.3.4/ydb/_topic_writer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_topic_writer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8093 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_topic_writer/topic_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)    23342 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_topic_writer/topic_writer_asyncio.py
--rw-r--r--   0 runner    (1001) docker     (123)    24156 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_topic_writer/topic_writer_asyncio_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3477 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_topic_writer/topic_writer_sync.py
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_topic_writer/topic_writer_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5838 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_tx_ctx_impl.py
--rw-r--r--   0 runner    (1001) docker     (123)     4130 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_utilities_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:36:51.169507 ydb-3.3.4/ydb/aio/
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/aio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/aio/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)     8402 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/aio/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)     3402 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/aio/credentials.py
--rw-r--r--   0 runner    (1001) docker     (123)     1877 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/aio/driver.py
--rw-r--r--   0 runner    (1001) docker     (123)     4832 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/aio/iam.py
--rw-r--r--   0 runner    (1001) docker     (123)     8824 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/aio/pool.py
--rw-r--r--   0 runner    (1001) docker     (123)     2128 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/aio/resolver.py
--rw-r--r--   0 runner    (1001) docker     (123)      838 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/aio/scheme.py
--rw-r--r--   0 runner    (1001) docker     (123)    18058 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/aio/table.py
--rw-r--r--   0 runner    (1001) docker     (123)      304 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/auth_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    18813 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)    15178 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/convert.py
--rw-r--r--   0 runner    (1001) docker     (123)     7135 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/credentials.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:36:51.173507 ydb-3.3.4/ydb/dbapi/
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/dbapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2569 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/dbapi/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)     5002 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/dbapi/cursor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2174 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/dbapi/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)   285865 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/default_pem.py
--rw-r--r--   0 runner    (1001) docker     (123)     9311 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/driver.py
--rw-r--r--   0 runner    (1001) docker     (123)     7769 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/export.py
--rw-r--r--   0 runner    (1001) docker     (123)      625 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/global_settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:36:51.173507 ydb-3.3.4/ydb/iam/
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/iam/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6297 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/iam/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     4376 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/import_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2336 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/interceptor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5060 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/issues.py
--rw-r--r--   0 runner    (1001) docker     (123)     2973 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/operation.py
--rw-r--r--   0 runner    (1001) docker     (123)    16647 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/pool.py
--rw-r--r--   0 runner    (1001) docker     (123)     6878 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/resolver.py
--rw-r--r--   0 runner    (1001) docker     (123)    14271 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/scheme.py
--rw-r--r--   0 runner    (1001) docker     (123)      810 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/scheme_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3384 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/scripting.py
--rw-r--r--   0 runner    (1001) docker     (123)     3937 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:36:51.173507 ydb-3.3.4/ydb/sqlalchemy/
--rw-r--r--   0 runner    (1001) docker     (123)     9869 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/sqlalchemy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      662 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/sqlalchemy/types.py
--rw-r--r--   0 runner    (1001) docker     (123)    82321 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/table.py
--rw-r--r--   0 runner    (1001) docker     (123)     4895 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/table_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    13428 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/topic.py
--rw-r--r--   0 runner    (1001) docker     (123)     4768 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/tracing.py
--rw-r--r--   0 runner    (1001) docker     (123)    11729 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/types.py
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-25 14:36:42.000000 ydb-3.3.4/ydb/ydb_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:36:51.173507 ydb-3.3.4/ydb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1669 2023-05-25 14:36:51.000000 ydb-3.3.4/ydb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8651 2023-05-25 14:36:51.000000 ydb-3.3.4/ydb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 14:36:51.000000 ydb-3.3.4/ydb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-25 14:36:51.000000 ydb-3.3.4/ydb.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-25 14:36:51.000000 ydb-3.3.4/ydb.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 15:18:35.439087 ydb-3.3.5/
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-06-09 15:18:18.000000 ydb-3.3.5/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (123)    11361 2023-06-09 15:18:18.000000 ydb-3.3.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-09 15:18:18.000000 ydb-3.3.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1669 2023-06-09 15:18:35.439087 ydb-3.3.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-06-09 15:18:18.000000 ydb-3.3.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-09 15:18:18.000000 ydb-3.3.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-09 15:18:18.000000 ydb-3.3.5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-09 15:18:35.439087 ydb-3.3.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-06-09 15:18:26.000000 ydb-3.3.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 15:18:35.395085 ydb-3.3.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 15:18:18.000000 ydb-3.3.5/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 15:18:35.395085 ydb-3.3.5/tests/aio/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 15:18:18.000000 ydb-3.3.5/tests/aio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4356 2023-06-09 15:18:18.000000 ydb-3.3.5/tests/aio/test_async_iter_stream.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1870 2023-06-09 15:18:18.000000 ydb-3.3.5/tests/aio/test_connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3822 2023-06-09 15:18:18.000000 ydb-3.3.5/tests/aio/test_connection_pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3431 2023-06-09 15:18:18.000000 ydb-3.3.5/tests/aio/test_session_pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-06-09 15:18:18.000000 ydb-3.3.5/tests/aio/test_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7329 2023-06-09 15:18:18.000000 ydb-3.3.5/tests/aio/test_tx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3188 2023-06-09 15:18:18.000000 ydb-3.3.5/tests/aio/test_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6006 2023-06-09 15:18:18.000000 ydb-3.3.5/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-06-09 15:18:18.000000 ydb-3.3.5/tests/session_pool.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 15:18:35.395085 ydb-3.3.5/tests/ssl/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 15:18:18.000000 ydb-3.3.5/tests/ssl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-06-09 15:18:18.000000 ydb-3.3.5/tests/ssl/test_ssl.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 15:18:35.395085 ydb-3.3.5/tests/table/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 15:18:18.000000 ydb-3.3.5/tests/table/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2334 2023-06-09 15:18:18.000000 ydb-3.3.5/tests/table/table_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6666 2023-06-09 15:18:18.000000 ydb-3.3.5/tests/table/test_tx.py
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-06-09 15:18:18.000000 ydb-3.3.5/tests/test_errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 15:18:35.395085 ydb-3.3.5/tests/topics/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 15:18:18.000000 ydb-3.3.5/tests/topics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-06-09 15:18:18.000000 ydb-3.3.5/tests/topics/test_control_plane.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8086 2023-06-09 15:18:18.000000 ydb-3.3.5/tests/topics/test_topic_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10281 2023-06-09 15:18:18.000000 ydb-3.3.5/tests/topics/test_topic_writer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 15:18:35.407086 ydb-3.3.5/ydb/
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-06-09 15:18:18.000000 ydb-3.3.5/ydb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3032 2023-06-09 15:18:18.000000 ydb-3.3.5/ydb/_apis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-06-09 15:18:18.000000 ydb-3.3.5/ydb/_errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 15:18:35.407086 ydb-3.3.5/ydb/_grpc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 15:18:18.000000 ydb-3.3.5/ydb/_grpc/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 15:18:35.407086 ydb-3.3.5/ydb/_grpc/common/
+-rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-06-09 15:18:18.000000 ydb-3.3.5/ydb/_grpc/common/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 15:18:35.407086 ydb-3.3.5/ydb/_grpc/grpcwrapper/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 15:18:18.000000 ydb-3.3.5/ydb/_grpc/grpcwrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8860 2023-06-09 15:18:18.000000 ydb-3.3.5/ydb/_grpc/grpcwrapper/common_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      719 2023-06-09 15:18:18.000000 ydb-3.3.5/ydb/_grpc/grpcwrapper/ydb_scheme.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45284 2023-06-09 15:18:18.000000 ydb-3.3.5/ydb/_grpc/grpcwrapper/ydb_topic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5865 2023-06-09 15:18:18.000000 ydb-3.3.5/ydb/_grpc/grpcwrapper/ydb_topic_public_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-06-09 15:18:18.000000 ydb-3.3.5/ydb/_grpc/grpcwrapper/ydb_topic_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 15:18:35.411086 ydb-3.3.5/ydb/_grpc/v3/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 15:18:18.000000 ydb-3.3.5/ydb/_grpc/v3/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 15:18:35.419086 ydb-3.3.5/ydb/_grpc/v3/protos/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 15:18:18.000000 ydb-3.3.5/ydb/_grpc/v3/protos/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 15:18:35.419086 ydb-3.3.5/ydb/_grpc/v3/protos/annotations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 15:18:18.000000 ydb-3.3.5/ydb/_grpc/v3/protos/annotations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12213 2023-06-09 15:18:18.000000 ydb-3.3.5/ydb/_grpc/v3/protos/annotations/validation_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-09 15:18:18.000000 ydb-3.3.5/ydb/_grpc/v3/protos/annotations/validation_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6184 2023-06-09 15:18:18.000000 ydb-3.3.5/ydb/_grpc/v3/protos/ydb_auth_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-09 15:18:18.000000 ydb-3.3.5/ydb/_grpc/v3/protos/ydb_auth_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    83179 2023-06-09 15:18:18.000000 ydb-3.3.5/ydb/_grpc/v3/protos/ydb_cms_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-09 15:18:18.000000 ydb-3.3.5/ydb/_grpc/v3/protos/ydb_cms_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7124 2023-06-09 15:18:18.000000 ydb-3.3.5/ydb/_grpc/v3/protos/ydb_common_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-09 15:18:18.000000 ydb-3.3.5/ydb/_grpc/v3/protos/ydb_common_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)   121326 2023-06-09 15:18:18.000000 ydb-3.3.5/ydb/_grpc/v3/protos/ydb_coordination_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-09 15:18:18.000000 ydb-3.3.5/ydb/_grpc/v3/protos/ydb_coordination_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16470 2023-06-09 15:18:18.000000 ydb-3.3.5/ydb/_grpc/v3/protos/ydb_discovery_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-09 15:18:18.000000 ydb-3.3.5/ydb/_grpc/v3/protos/ydb_discovery_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41176 2023-06-09 15:18:18.000000 ydb-3.3.5/ydb/_grpc/v3/protos/ydb_export_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-09 15:18:18.000000 ydb-3.3.5/ydb/_grpc/v3/protos/ydb_export_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4995 2023-06-09 15:18:18.000000 ydb-3.3.5/ydb/_grpc/v3/protos/ydb_formats_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-09 15:18:18.000000 ydb-3.3.5/ydb/_grpc/v3/protos/ydb_formats_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30782 2023-06-09 15:18:18.000000 ydb-3.3.5/ydb/_grpc/v3/protos/ydb_import_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-09 15:18:18.000000 ydb-3.3.5/ydb/_grpc/v3/protos/ydb_import_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7161 2023-06-09 15:18:18.000000 ydb-3.3.5/ydb/_grpc/v3/protos/ydb_issue_message_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-09 15:18:18.000000 ydb-3.3.5/ydb/_grpc/v3/protos/ydb_issue_message_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    72285 2023-06-09 15:18:18.000000 ydb-3.3.5/ydb/_grpc/v3/protos/ydb_monitoring_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-09 15:18:18.000000 ydb-3.3.5/ydb/_grpc/v3/protos/ydb_monitoring_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29771 2023-06-09 15:18:18.000000 ydb-3.3.5/ydb/_grpc/v3/protos/ydb_operation_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-09 15:18:18.000000 ydb-3.3.5/ydb/_grpc/v3/protos/ydb_operation_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16311 2023-06-09 15:18:18.000000 ydb-3.3.5/ydb/_grpc/v3/protos/ydb_query_stats_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-09 15:18:18.000000 ydb-3.3.5/ydb/_grpc/v3/protos/ydb_query_stats_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40278 2023-06-09 15:18:18.000000 ydb-3.3.5/ydb/_grpc/v3/protos/ydb_rate_limiter_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-09 15:18:18.000000 ydb-3.3.5/ydb/_grpc/v3/protos/ydb_rate_limiter_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38051 2023-06-09 15:18:18.000000 ydb-3.3.5/ydb/_grpc/v3/protos/ydb_scheme_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-09 15:18:18.000000 ydb-3.3.5/ydb/_grpc/v3/protos/ydb_scheme_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25816 2023-06-09 15:18:18.000000 ydb-3.3.5/ydb/_grpc/v3/protos/ydb_scripting_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-09 15:18:18.000000 ydb-3.3.5/ydb/_grpc/v3/protos/ydb_scripting_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6884 2023-06-09 15:18:18.000000 ydb-3.3.5/ydb/_grpc/v3/protos/ydb_status_codes_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-09 15:18:18.000000 ydb-3.3.5/ydb/_grpc/v3/protos/ydb_status_codes_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)   332647 2023-06-09 15:18:18.000000 ydb-3.3.5/ydb/_grpc/v3/protos/ydb_table_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-09 15:18:18.000000 ydb-3.3.5/ydb/_grpc/v3/protos/ydb_table_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)   234296 2023-06-09 15:18:18.000000 ydb-3.3.5/ydb/_grpc/v3/protos/ydb_topic_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-09 15:18:18.000000 ydb-3.3.5/ydb/_grpc/v3/protos/ydb_topic_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52587 2023-06-09 15:18:18.000000 ydb-3.3.5/ydb/_grpc/v3/protos/ydb_value_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-09 15:18:18.000000 ydb-3.3.5/ydb/_grpc/v3/protos/ydb_value_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-06-09 15:18:18.000000 ydb-3.3.5/ydb/_grpc/v3/ydb_auth_v1_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2503 2023-06-09 15:18:18.000000 ydb-3.3.5/ydb/_grpc/v3/ydb_auth_v1_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4418 2023-06-09 15:18:18.000000 ydb-3.3.5/ydb/_grpc/v3/ydb_cms_v1_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11170 2023-06-09 15:18:18.000000 ydb-3.3.5/ydb/_grpc/v3/ydb_cms_v1_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4226 2023-06-09 15:18:18.000000 ydb-3.3.5/ydb/_grpc/v3/ydb_coordination_v1_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9797 2023-06-09 15:18:18.000000 ydb-3.3.5/ydb/_grpc/v3/ydb_coordination_v1_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2610 2023-06-09 15:18:18.000000 ydb-3.3.5/ydb/_grpc/v3/ydb_discovery_v1_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4307 2023-06-09 15:18:18.000000 ydb-3.3.5/ydb/_grpc/v3/ydb_discovery_v1_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-06-09 15:18:18.000000 ydb-3.3.5/ydb/_grpc/v3/ydb_export_v1_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4370 2023-06-09 15:18:18.000000 ydb-3.3.5/ydb/_grpc/v3/ydb_export_v1_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2527 2023-06-09 15:18:18.000000 ydb-3.3.5/ydb/_grpc/v3/ydb_import_v1_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4404 2023-06-09 15:18:18.000000 ydb-3.3.5/ydb/_grpc/v3/ydb_import_v1_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2622 2023-06-09 15:18:18.000000 ydb-3.3.5/ydb/_grpc/v3/ydb_monitoring_v1_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4293 2023-06-09 15:18:18.000000 ydb-3.3.5/ydb/_grpc/v3/ydb_monitoring_v1_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3688 2023-06-09 15:18:18.000000 ydb-3.3.5/ydb/_grpc/v3/ydb_operation_v1_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10345 2023-06-09 15:18:18.000000 ydb-3.3.5/ydb/_grpc/v3/ydb_operation_v1_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4877 2023-06-09 15:18:18.000000 ydb-3.3.5/ydb/_grpc/v3/ydb_rate_limiter_v1_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11754 2023-06-09 15:18:18.000000 ydb-3.3.5/ydb/_grpc/v3/ydb_rate_limiter_v1_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4012 2023-06-09 15:18:18.000000 ydb-3.3.5/ydb/_grpc/v3/ydb_scheme_v1_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10044 2023-06-09 15:18:18.000000 ydb-3.3.5/ydb/_grpc/v3/ydb_scheme_v1_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3112 2023-06-09 15:18:18.000000 ydb-3.3.5/ydb/_grpc/v3/ydb_scripting_v1_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6037 2023-06-09 15:18:18.000000 ydb-3.3.5/ydb/_grpc/v3/ydb_scripting_v1_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11659 2023-06-09 15:18:18.000000 ydb-3.3.5/ydb/_grpc/v3/ydb_table_v1_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36535 2023-06-09 15:18:18.000000 ydb-3.3.5/ydb/_grpc/v3/ydb_table_v1_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4956 2023-06-09 15:18:18.000000 ydb-3.3.5/ydb/_grpc/v3/ydb_topic_v1_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14404 2023-06-09 15:18:18.000000 ydb-3.3.5/ydb/_grpc/v3/ydb_topic_v1_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 15:18:35.427086 ydb-3.3.5/ydb/_grpc/v4/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 15:18:18.000000 ydb-3.3.5/ydb/_grpc/v4/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 15:18:35.431086 ydb-3.3.5/ydb/_grpc/v4/protos/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 15:18:18.000000 ydb-3.3.5/ydb/_grpc/v4/protos/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 15:18:35.435086 ydb-3.3.5/ydb/_grpc/v4/protos/annotations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 15:18:18.000000 ydb-3.3.5/ydb/_grpc/v4/protos/annotations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2727 2023-06-09 15:18:18.000000 ydb-3.3.5/ydb/_grpc/v4/protos/annotations/validation_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-09 15:18:18.000000 ydb-3.3.5/ydb/_grpc/v4/protos/annotations/validation_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-06-09 15:18:18.000000 ydb-3.3.5/ydb/_grpc/v4/protos/ydb_auth_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-09 15:18:18.000000 ydb-3.3.5/ydb/_grpc/v4/protos/ydb_auth_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12062 2023-06-09 15:18:18.000000 ydb-3.3.5/ydb/_grpc/v4/protos/ydb_cms_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-09 15:18:18.000000 ydb-3.3.5/ydb/_grpc/v4/protos/ydb_cms_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-06-09 15:18:18.000000 ydb-3.3.5/ydb/_grpc/v4/protos/ydb_common_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-09 15:18:18.000000 ydb-3.3.5/ydb/_grpc/v4/protos/ydb_common_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15716 2023-06-09 15:18:18.000000 ydb-3.3.5/ydb/_grpc/v4/protos/ydb_coordination_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-09 15:18:18.000000 ydb-3.3.5/ydb/_grpc/v4/protos/ydb_coordination_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2871 2023-06-09 15:18:18.000000 ydb-3.3.5/ydb/_grpc/v4/protos/ydb_discovery_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-09 15:18:18.000000 ydb-3.3.5/ydb/_grpc/v4/protos/ydb_discovery_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9313 2023-06-09 15:18:18.000000 ydb-3.3.5/ydb/_grpc/v4/protos/ydb_export_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-09 15:18:18.000000 ydb-3.3.5/ydb/_grpc/v4/protos/ydb_export_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-06-09 15:18:18.000000 ydb-3.3.5/ydb/_grpc/v4/protos/ydb_formats_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-09 15:18:18.000000 ydb-3.3.5/ydb/_grpc/v4/protos/ydb_formats_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6939 2023-06-09 15:18:18.000000 ydb-3.3.5/ydb/_grpc/v4/protos/ydb_import_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-09 15:18:18.000000 ydb-3.3.5/ydb/_grpc/v4/protos/ydb_import_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1770 2023-06-09 15:18:18.000000 ydb-3.3.5/ydb/_grpc/v4/protos/ydb_issue_message_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-09 15:18:18.000000 ydb-3.3.5/ydb/_grpc/v4/protos/ydb_issue_message_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9769 2023-06-09 15:18:18.000000 ydb-3.3.5/ydb/_grpc/v4/protos/ydb_monitoring_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-09 15:18:18.000000 ydb-3.3.5/ydb/_grpc/v4/protos/ydb_monitoring_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6165 2023-06-09 15:18:18.000000 ydb-3.3.5/ydb/_grpc/v4/protos/ydb_operation_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-09 15:18:18.000000 ydb-3.3.5/ydb/_grpc/v4/protos/ydb_operation_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2849 2023-06-09 15:18:18.000000 ydb-3.3.5/ydb/_grpc/v4/protos/ydb_query_stats_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-09 15:18:18.000000 ydb-3.3.5/ydb/_grpc/v4/protos/ydb_query_stats_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6057 2023-06-09 15:18:18.000000 ydb-3.3.5/ydb/_grpc/v4/protos/ydb_rate_limiter_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-09 15:18:18.000000 ydb-3.3.5/ydb/_grpc/v4/protos/ydb_rate_limiter_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5830 2023-06-09 15:18:18.000000 ydb-3.3.5/ydb/_grpc/v4/protos/ydb_scheme_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-09 15:18:18.000000 ydb-3.3.5/ydb/_grpc/v4/protos/ydb_scheme_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5143 2023-06-09 15:18:18.000000 ydb-3.3.5/ydb/_grpc/v4/protos/ydb_scripting_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-09 15:18:18.000000 ydb-3.3.5/ydb/_grpc/v4/protos/ydb_scripting_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-06-09 15:18:18.000000 ydb-3.3.5/ydb/_grpc/v4/protos/ydb_status_codes_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-09 15:18:18.000000 ydb-3.3.5/ydb/_grpc/v4/protos/ydb_status_codes_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46408 2023-06-09 15:18:18.000000 ydb-3.3.5/ydb/_grpc/v4/protos/ydb_table_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-09 15:18:18.000000 ydb-3.3.5/ydb/_grpc/v4/protos/ydb_table_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34953 2023-06-09 15:18:18.000000 ydb-3.3.5/ydb/_grpc/v4/protos/ydb_topic_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-09 15:18:18.000000 ydb-3.3.5/ydb/_grpc/v4/protos/ydb_topic_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6618 2023-06-09 15:18:18.000000 ydb-3.3.5/ydb/_grpc/v4/protos/ydb_value_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-09 15:18:18.000000 ydb-3.3.5/ydb/_grpc/v4/protos/ydb_value_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-06-09 15:18:18.000000 ydb-3.3.5/ydb/_grpc/v4/ydb_auth_v1_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2503 2023-06-09 15:18:18.000000 ydb-3.3.5/ydb/_grpc/v4/ydb_auth_v1_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1868 2023-06-09 15:18:18.000000 ydb-3.3.5/ydb/_grpc/v4/ydb_cms_v1_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11170 2023-06-09 15:18:18.000000 ydb-3.3.5/ydb/_grpc/v4/ydb_cms_v1_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1937 2023-06-09 15:18:18.000000 ydb-3.3.5/ydb/_grpc/v4/ydb_coordination_v1_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9797 2023-06-09 15:18:18.000000 ydb-3.3.5/ydb/_grpc/v4/ydb_coordination_v1_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-06-09 15:18:18.000000 ydb-3.3.5/ydb/_grpc/v4/ydb_discovery_v1_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4307 2023-06-09 15:18:18.000000 ydb-3.3.5/ydb/_grpc/v4/ydb_discovery_v1_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-06-09 15:18:18.000000 ydb-3.3.5/ydb/_grpc/v4/ydb_export_v1_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4370 2023-06-09 15:18:18.000000 ydb-3.3.5/ydb/_grpc/v4/ydb_export_v1_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-06-09 15:18:18.000000 ydb-3.3.5/ydb/_grpc/v4/ydb_import_v1_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4404 2023-06-09 15:18:18.000000 ydb-3.3.5/ydb/_grpc/v4/ydb_import_v1_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-06-09 15:18:18.000000 ydb-3.3.5/ydb/_grpc/v4/ydb_monitoring_v1_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4293 2023-06-09 15:18:18.000000 ydb-3.3.5/ydb/_grpc/v4/ydb_monitoring_v1_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1776 2023-06-09 15:18:18.000000 ydb-3.3.5/ydb/_grpc/v4/ydb_operation_v1_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10345 2023-06-09 15:18:18.000000 ydb-3.3.5/ydb/_grpc/v4/ydb_operation_v1_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2097 2023-06-09 15:18:18.000000 ydb-3.3.5/ydb/_grpc/v4/ydb_rate_limiter_v1_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11754 2023-06-09 15:18:18.000000 ydb-3.3.5/ydb/_grpc/v4/ydb_rate_limiter_v1_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1789 2023-06-09 15:18:18.000000 ydb-3.3.5/ydb/_grpc/v4/ydb_scheme_v1_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10044 2023-06-09 15:18:18.000000 ydb-3.3.5/ydb/_grpc/v4/ydb_scheme_v1_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1621 2023-06-09 15:18:18.000000 ydb-3.3.5/ydb/_grpc/v4/ydb_scripting_v1_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6037 2023-06-09 15:18:18.000000 ydb-3.3.5/ydb/_grpc/v4/ydb_scripting_v1_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3453 2023-06-09 15:18:18.000000 ydb-3.3.5/ydb/_grpc/v4/ydb_table_v1_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36535 2023-06-09 15:18:18.000000 ydb-3.3.5/ydb/_grpc/v4/ydb_table_v1_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-06-09 15:18:18.000000 ydb-3.3.5/ydb/_grpc/v4/ydb_topic_v1_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14404 2023-06-09 15:18:18.000000 ydb-3.3.5/ydb/_grpc/v4/ydb_topic_v1_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16278 2023-06-09 15:18:18.000000 ydb-3.3.5/ydb/_session_impl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14607 2023-06-09 15:18:18.000000 ydb-3.3.5/ydb/_sp_impl.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 15:18:35.435086 ydb-3.3.5/ydb/_topic_common/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 15:18:18.000000 ydb-3.3.5/ydb/_topic_common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4659 2023-06-09 15:18:18.000000 ydb-3.3.5/ydb/_topic_common/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7957 2023-06-09 15:18:18.000000 ydb-3.3.5/ydb/_topic_common/common_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1966 2023-06-09 15:18:18.000000 ydb-3.3.5/ydb/_topic_common/test_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 15:18:35.435086 ydb-3.3.5/ydb/_topic_reader/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 15:18:18.000000 ydb-3.3.5/ydb/_topic_reader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5569 2023-06-09 15:18:18.000000 ydb-3.3.5/ydb/_topic_reader/datatypes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7583 2023-06-09 15:18:18.000000 ydb-3.3.5/ydb/_topic_reader/datatypes_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3716 2023-06-09 15:18:18.000000 ydb-3.3.5/ydb/_topic_reader/topic_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23900 2023-06-09 15:18:18.000000 ydb-3.3.5/ydb/_topic_reader/topic_reader_asyncio.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48882 2023-06-09 15:18:18.000000 ydb-3.3.5/ydb/_topic_reader/topic_reader_asyncio_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5469 2023-06-09 15:18:18.000000 ydb-3.3.5/ydb/_topic_reader/topic_reader_sync.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 15:18:35.435086 ydb-3.3.5/ydb/_topic_writer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 15:18:18.000000 ydb-3.3.5/ydb/_topic_writer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8093 2023-06-09 15:18:18.000000 ydb-3.3.5/ydb/_topic_writer/topic_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23384 2023-06-09 15:18:18.000000 ydb-3.3.5/ydb/_topic_writer/topic_writer_asyncio.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24169 2023-06-09 15:18:18.000000 ydb-3.3.5/ydb/_topic_writer/topic_writer_asyncio_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3477 2023-06-09 15:18:18.000000 ydb-3.3.5/ydb/_topic_writer/topic_writer_sync.py
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-06-09 15:18:18.000000 ydb-3.3.5/ydb/_topic_writer/topic_writer_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5838 2023-06-09 15:18:18.000000 ydb-3.3.5/ydb/_tx_ctx_impl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4130 2023-06-09 15:18:18.000000 ydb-3.3.5/ydb/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-06-09 15:18:18.000000 ydb-3.3.5/ydb/_utilities_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 15:18:35.439087 ydb-3.3.5/ydb/aio/
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-09 15:18:18.000000 ydb-3.3.5/ydb/aio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-06-09 15:18:18.000000 ydb-3.3.5/ydb/aio/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8402 2023-06-09 15:18:18.000000 ydb-3.3.5/ydb/aio/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3402 2023-06-09 15:18:18.000000 ydb-3.3.5/ydb/aio/credentials.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1877 2023-06-09 15:18:18.000000 ydb-3.3.5/ydb/aio/driver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4832 2023-06-09 15:18:18.000000 ydb-3.3.5/ydb/aio/iam.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8824 2023-06-09 15:18:18.000000 ydb-3.3.5/ydb/aio/pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2128 2023-06-09 15:18:18.000000 ydb-3.3.5/ydb/aio/resolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)      838 2023-06-09 15:18:18.000000 ydb-3.3.5/ydb/aio/scheme.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18058 2023-06-09 15:18:18.000000 ydb-3.3.5/ydb/aio/table.py
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-06-09 15:18:18.000000 ydb-3.3.5/ydb/auth_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18813 2023-06-09 15:18:18.000000 ydb-3.3.5/ydb/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15178 2023-06-09 15:18:18.000000 ydb-3.3.5/ydb/convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7135 2023-06-09 15:18:18.000000 ydb-3.3.5/ydb/credentials.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 15:18:35.439087 ydb-3.3.5/ydb/dbapi/
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-06-09 15:18:18.000000 ydb-3.3.5/ydb/dbapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2569 2023-06-09 15:18:18.000000 ydb-3.3.5/ydb/dbapi/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5002 2023-06-09 15:18:18.000000 ydb-3.3.5/ydb/dbapi/cursor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2174 2023-06-09 15:18:18.000000 ydb-3.3.5/ydb/dbapi/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)   285865 2023-06-09 15:18:18.000000 ydb-3.3.5/ydb/default_pem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9311 2023-06-09 15:18:18.000000 ydb-3.3.5/ydb/driver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7769 2023-06-09 15:18:18.000000 ydb-3.3.5/ydb/export.py
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-06-09 15:18:18.000000 ydb-3.3.5/ydb/global_settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 15:18:35.439087 ydb-3.3.5/ydb/iam/
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-06-09 15:18:18.000000 ydb-3.3.5/ydb/iam/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6297 2023-06-09 15:18:18.000000 ydb-3.3.5/ydb/iam/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4376 2023-06-09 15:18:18.000000 ydb-3.3.5/ydb/import_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2336 2023-06-09 15:18:18.000000 ydb-3.3.5/ydb/interceptor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5060 2023-06-09 15:18:18.000000 ydb-3.3.5/ydb/issues.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2973 2023-06-09 15:18:18.000000 ydb-3.3.5/ydb/operation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16647 2023-06-09 15:18:18.000000 ydb-3.3.5/ydb/pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6878 2023-06-09 15:18:18.000000 ydb-3.3.5/ydb/resolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14271 2023-06-09 15:18:18.000000 ydb-3.3.5/ydb/scheme.py
+-rw-r--r--   0 runner    (1001) docker     (123)      810 2023-06-09 15:18:18.000000 ydb-3.3.5/ydb/scheme_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3384 2023-06-09 15:18:18.000000 ydb-3.3.5/ydb/scripting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3937 2023-06-09 15:18:18.000000 ydb-3.3.5/ydb/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 15:18:35.439087 ydb-3.3.5/ydb/sqlalchemy/
+-rw-r--r--   0 runner    (1001) docker     (123)     9869 2023-06-09 15:18:18.000000 ydb-3.3.5/ydb/sqlalchemy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      662 2023-06-09 15:18:18.000000 ydb-3.3.5/ydb/sqlalchemy/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    82321 2023-06-09 15:18:18.000000 ydb-3.3.5/ydb/table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4895 2023-06-09 15:18:18.000000 ydb-3.3.5/ydb/table_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13548 2023-06-09 15:18:18.000000 ydb-3.3.5/ydb/topic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4768 2023-06-09 15:18:18.000000 ydb-3.3.5/ydb/tracing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11729 2023-06-09 15:18:18.000000 ydb-3.3.5/ydb/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-09 15:18:26.000000 ydb-3.3.5/ydb/ydb_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 15:18:35.439087 ydb-3.3.5/ydb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1669 2023-06-09 15:18:35.000000 ydb-3.3.5/ydb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8651 2023-06-09 15:18:35.000000 ydb-3.3.5/ydb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 15:18:35.000000 ydb-3.3.5/ydb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-09 15:18:35.000000 ydb-3.3.5/ydb.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-09 15:18:35.000000 ydb-3.3.5/ydb.egg-info/top_level.txt
```

### Comparing `ydb-3.3.4/LICENSE` & `ydb-3.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `ydb-3.3.4/PKG-INFO` & `ydb-3.3.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ydb
-Version: 3.3.4
+Version: 3.3.5
 Summary: YDB Python SDK
 Home-page: http://github.com/ydb-platform/ydb-python-sdk
 Author: Yandex LLC
 Author-email: ydb@yandex-team.ru
 License: Apache 2.0
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2
```

### Comparing `ydb-3.3.4/README.md` & `ydb-3.3.5/README.md`

 * *Files identical despite different names*

### Comparing `ydb-3.3.4/setup.py` & `ydb-3.3.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     for line in r.readlines():
         line = line.strip()
         if line != "":
             requirements.append(line)
 
 setuptools.setup(
     name="ydb",
-    version="3.3.4",  # AUTOVERSION
+    version="3.3.5",  # AUTOVERSION
     description="YDB Python SDK",
     author="Yandex LLC",
     author_email="ydb@yandex-team.ru",
     url="http://github.com/ydb-platform/ydb-python-sdk",
     license="Apache 2.0",
     package_dir={"": "."},
     long_description=long_description,
```

### Comparing `ydb-3.3.4/tests/aio/test_async_iter_stream.py` & `ydb-3.3.5/tests/aio/test_async_iter_stream.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.4/tests/aio/test_connection.py` & `ydb-3.3.5/tests/aio/test_connection.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.4/tests/aio/test_connection_pool.py` & `ydb-3.3.5/tests/aio/test_connection_pool.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.4/tests/aio/test_session_pool.py` & `ydb-3.3.5/tests/aio/test_session_pool.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.4/tests/aio/test_tx.py` & `ydb-3.3.5/tests/aio/test_tx.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.4/tests/aio/test_types.py` & `ydb-3.3.5/tests/aio/test_types.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.4/tests/conftest.py` & `ydb-3.3.5/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.4/tests/session_pool.py` & `ydb-3.3.5/tests/session_pool.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.4/tests/table/table_test.py` & `ydb-3.3.5/tests/table/table_test.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.4/tests/table/test_tx.py` & `ydb-3.3.5/tests/table/test_tx.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.4/tests/test_errors.py` & `ydb-3.3.5/tests/test_errors.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.4/tests/topics/test_control_plane.py` & `ydb-3.3.5/tests/topics/test_control_plane.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.4/tests/topics/test_topic_reader.py` & `ydb-3.3.5/tests/topics/test_topic_reader.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.4/tests/topics/test_topic_writer.py` & `ydb-3.3.5/tests/topics/test_topic_writer.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.4/ydb/__init__.py` & `ydb-3.3.5/ydb/__init__.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.4/ydb/_apis.py` & `ydb-3.3.5/ydb/_apis.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.4/ydb/_errors.py` & `ydb-3.3.5/ydb/_errors.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.4/ydb/_grpc/common/__init__.py` & `ydb-3.3.5/ydb/_grpc/common/__init__.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.4/ydb/_grpc/grpcwrapper/common_utils.py` & `ydb-3.3.5/ydb/_grpc/grpcwrapper/common_utils.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.4/ydb/_grpc/grpcwrapper/ydb_scheme.py` & `ydb-3.3.5/ydb/_grpc/grpcwrapper/ydb_scheme.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.4/ydb/_grpc/grpcwrapper/ydb_topic.py` & `ydb-3.3.5/ydb/_grpc/grpcwrapper/ydb_topic.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.4/ydb/_grpc/grpcwrapper/ydb_topic_public_types.py` & `ydb-3.3.5/ydb/_grpc/grpcwrapper/ydb_topic_public_types.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.4/ydb/_grpc/grpcwrapper/ydb_topic_test.py` & `ydb-3.3.5/ydb/_grpc/grpcwrapper/ydb_topic_test.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.4/ydb/_grpc/v3/protos/annotations/validation_pb2.py` & `ydb-3.3.5/ydb/_grpc/v3/protos/annotations/validation_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.4/ydb/_grpc/v3/protos/ydb_auth_pb2.py` & `ydb-3.3.5/ydb/_grpc/v3/protos/ydb_auth_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.4/ydb/_grpc/v3/protos/ydb_cms_pb2.py` & `ydb-3.3.5/ydb/_grpc/v3/protos/ydb_cms_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.4/ydb/_grpc/v3/protos/ydb_common_pb2.py` & `ydb-3.3.5/ydb/_grpc/v3/protos/ydb_common_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.4/ydb/_grpc/v3/protos/ydb_coordination_pb2.py` & `ydb-3.3.5/ydb/_grpc/v3/protos/ydb_coordination_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.4/ydb/_grpc/v3/protos/ydb_discovery_pb2.py` & `ydb-3.3.5/ydb/_grpc/v3/protos/ydb_discovery_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.4/ydb/_grpc/v3/protos/ydb_export_pb2.py` & `ydb-3.3.5/ydb/_grpc/v3/protos/ydb_export_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.4/ydb/_grpc/v3/protos/ydb_formats_pb2.py` & `ydb-3.3.5/ydb/_grpc/v3/protos/ydb_formats_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.4/ydb/_grpc/v3/protos/ydb_import_pb2.py` & `ydb-3.3.5/ydb/_grpc/v3/protos/ydb_import_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.4/ydb/_grpc/v3/protos/ydb_issue_message_pb2.py` & `ydb-3.3.5/ydb/_grpc/v3/protos/ydb_issue_message_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.4/ydb/_grpc/v3/protos/ydb_monitoring_pb2.py` & `ydb-3.3.5/ydb/_grpc/v3/protos/ydb_monitoring_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.4/ydb/_grpc/v3/protos/ydb_operation_pb2.py` & `ydb-3.3.5/ydb/_grpc/v3/protos/ydb_operation_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.4/ydb/_grpc/v3/protos/ydb_query_stats_pb2.py` & `ydb-3.3.5/ydb/_grpc/v3/protos/ydb_query_stats_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.4/ydb/_grpc/v3/protos/ydb_rate_limiter_pb2.py` & `ydb-3.3.5/ydb/_grpc/v3/protos/ydb_rate_limiter_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.4/ydb/_grpc/v3/protos/ydb_scheme_pb2.py` & `ydb-3.3.5/ydb/_grpc/v3/protos/ydb_scheme_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.4/ydb/_grpc/v3/protos/ydb_scripting_pb2.py` & `ydb-3.3.5/ydb/_grpc/v3/protos/ydb_scripting_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.4/ydb/_grpc/v3/protos/ydb_status_codes_pb2.py` & `ydb-3.3.5/ydb/_grpc/v3/protos/ydb_status_codes_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.4/ydb/_grpc/v3/protos/ydb_table_pb2.py` & `ydb-3.3.5/ydb/_grpc/v3/protos/ydb_table_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.4/ydb/_grpc/v3/protos/ydb_topic_pb2.py` & `ydb-3.3.5/ydb/_grpc/v3/protos/ydb_topic_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.4/ydb/_grpc/v3/protos/ydb_value_pb2.py` & `ydb-3.3.5/ydb/_grpc/v3/protos/ydb_value_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.4/ydb/_grpc/v3/ydb_auth_v1_pb2.py` & `ydb-3.3.5/ydb/_grpc/v3/ydb_auth_v1_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.4/ydb/_grpc/v3/ydb_auth_v1_pb2_grpc.py` & `ydb-3.3.5/ydb/_grpc/v3/ydb_auth_v1_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.4/ydb/_grpc/v3/ydb_cms_v1_pb2.py` & `ydb-3.3.5/ydb/_grpc/v3/ydb_cms_v1_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.4/ydb/_grpc/v3/ydb_cms_v1_pb2_grpc.py` & `ydb-3.3.5/ydb/_grpc/v3/ydb_cms_v1_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.4/ydb/_grpc/v3/ydb_coordination_v1_pb2.py` & `ydb-3.3.5/ydb/_grpc/v3/ydb_coordination_v1_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.4/ydb/_grpc/v3/ydb_coordination_v1_pb2_grpc.py` & `ydb-3.3.5/ydb/_grpc/v3/ydb_coordination_v1_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.4/ydb/_grpc/v3/ydb_discovery_v1_pb2.py` & `ydb-3.3.5/ydb/_grpc/v3/ydb_discovery_v1_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.4/ydb/_grpc/v3/ydb_discovery_v1_pb2_grpc.py` & `ydb-3.3.5/ydb/_grpc/v3/ydb_discovery_v1_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.4/ydb/_grpc/v3/ydb_export_v1_pb2.py` & `ydb-3.3.5/ydb/_grpc/v3/ydb_export_v1_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.4/ydb/_grpc/v3/ydb_export_v1_pb2_grpc.py` & `ydb-3.3.5/ydb/_grpc/v3/ydb_export_v1_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.4/ydb/_grpc/v3/ydb_import_v1_pb2.py` & `ydb-3.3.5/ydb/_grpc/v3/ydb_import_v1_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.4/ydb/_grpc/v3/ydb_import_v1_pb2_grpc.py` & `ydb-3.3.5/ydb/_grpc/v3/ydb_import_v1_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.4/ydb/_grpc/v3/ydb_monitoring_v1_pb2.py` & `ydb-3.3.5/ydb/_grpc/v3/ydb_monitoring_v1_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.4/ydb/_grpc/v3/ydb_monitoring_v1_pb2_grpc.py` & `ydb-3.3.5/ydb/_grpc/v3/ydb_monitoring_v1_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.4/ydb/_grpc/v3/ydb_operation_v1_pb2.py` & `ydb-3.3.5/ydb/_grpc/v3/ydb_operation_v1_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.4/ydb/_grpc/v3/ydb_operation_v1_pb2_grpc.py` & `ydb-3.3.5/ydb/_grpc/v3/ydb_operation_v1_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.4/ydb/_grpc/v3/ydb_rate_limiter_v1_pb2.py` & `ydb-3.3.5/ydb/_grpc/v3/ydb_rate_limiter_v1_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.4/ydb/_grpc/v3/ydb_rate_limiter_v1_pb2_grpc.py` & `ydb-3.3.5/ydb/_grpc/v3/ydb_rate_limiter_v1_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.4/ydb/_grpc/v3/ydb_scheme_v1_pb2.py` & `ydb-3.3.5/ydb/_grpc/v3/ydb_scheme_v1_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.4/ydb/_grpc/v3/ydb_scheme_v1_pb2_grpc.py` & `ydb-3.3.5/ydb/_grpc/v3/ydb_scheme_v1_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.4/ydb/_grpc/v3/ydb_scripting_v1_pb2.py` & `ydb-3.3.5/ydb/_grpc/v3/ydb_scripting_v1_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.4/ydb/_grpc/v3/ydb_scripting_v1_pb2_grpc.py` & `ydb-3.3.5/ydb/_grpc/v3/ydb_scripting_v1_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.4/ydb/_grpc/v3/ydb_table_v1_pb2.py` & `ydb-3.3.5/ydb/_grpc/v3/ydb_table_v1_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.4/ydb/_grpc/v3/ydb_table_v1_pb2_grpc.py` & `ydb-3.3.5/ydb/_grpc/v3/ydb_table_v1_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.4/ydb/_grpc/v3/ydb_topic_v1_pb2.py` & `ydb-3.3.5/ydb/_grpc/v3/ydb_topic_v1_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.4/ydb/_grpc/v3/ydb_topic_v1_pb2_grpc.py` & `ydb-3.3.5/ydb/_grpc/v3/ydb_topic_v1_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.4/ydb/_grpc/v4/protos/annotations/validation_pb2.py` & `ydb-3.3.5/ydb/_grpc/v4/protos/annotations/validation_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.4/ydb/_grpc/v4/protos/ydb_auth_pb2.py` & `ydb-3.3.5/ydb/_grpc/v4/protos/ydb_auth_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.4/ydb/_grpc/v4/protos/ydb_cms_pb2.py` & `ydb-3.3.5/ydb/_grpc/v4/protos/ydb_cms_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.4/ydb/_grpc/v4/protos/ydb_common_pb2.py` & `ydb-3.3.5/ydb/_grpc/v4/protos/ydb_common_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.4/ydb/_grpc/v4/protos/ydb_coordination_pb2.py` & `ydb-3.3.5/ydb/_grpc/v4/protos/ydb_coordination_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.4/ydb/_grpc/v4/protos/ydb_discovery_pb2.py` & `ydb-3.3.5/ydb/_grpc/v4/protos/ydb_discovery_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.4/ydb/_grpc/v4/protos/ydb_export_pb2.py` & `ydb-3.3.5/ydb/_grpc/v4/protos/ydb_export_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.4/ydb/_grpc/v4/protos/ydb_formats_pb2.py` & `ydb-3.3.5/ydb/_grpc/v4/protos/ydb_formats_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.4/ydb/_grpc/v4/protos/ydb_import_pb2.py` & `ydb-3.3.5/ydb/_grpc/v4/protos/ydb_import_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.4/ydb/_grpc/v4/protos/ydb_issue_message_pb2.py` & `ydb-3.3.5/ydb/_grpc/v4/protos/ydb_issue_message_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.4/ydb/_grpc/v4/protos/ydb_monitoring_pb2.py` & `ydb-3.3.5/ydb/_grpc/v4/protos/ydb_monitoring_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.4/ydb/_grpc/v4/protos/ydb_operation_pb2.py` & `ydb-3.3.5/ydb/_grpc/v4/protos/ydb_operation_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.4/ydb/_grpc/v4/protos/ydb_query_stats_pb2.py` & `ydb-3.3.5/ydb/_grpc/v4/protos/ydb_query_stats_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.4/ydb/_grpc/v4/protos/ydb_rate_limiter_pb2.py` & `ydb-3.3.5/ydb/_grpc/v4/protos/ydb_rate_limiter_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.4/ydb/_grpc/v4/protos/ydb_scheme_pb2.py` & `ydb-3.3.5/ydb/_grpc/v4/protos/ydb_scheme_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.4/ydb/_grpc/v4/protos/ydb_scripting_pb2.py` & `ydb-3.3.5/ydb/_grpc/v4/protos/ydb_scripting_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.4/ydb/_grpc/v4/protos/ydb_status_codes_pb2.py` & `ydb-3.3.5/ydb/_grpc/v4/protos/ydb_status_codes_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.4/ydb/_grpc/v4/protos/ydb_table_pb2.py` & `ydb-3.3.5/ydb/_grpc/v4/protos/ydb_table_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.4/ydb/_grpc/v4/protos/ydb_topic_pb2.py` & `ydb-3.3.5/ydb/_grpc/v4/protos/ydb_topic_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.4/ydb/_grpc/v4/protos/ydb_value_pb2.py` & `ydb-3.3.5/ydb/_grpc/v4/protos/ydb_value_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.4/ydb/_grpc/v4/ydb_auth_v1_pb2.py` & `ydb-3.3.5/ydb/_grpc/v4/ydb_auth_v1_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.4/ydb/_grpc/v4/ydb_auth_v1_pb2_grpc.py` & `ydb-3.3.5/ydb/_grpc/v4/ydb_auth_v1_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.4/ydb/_grpc/v4/ydb_cms_v1_pb2.py` & `ydb-3.3.5/ydb/_grpc/v4/ydb_cms_v1_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.4/ydb/_grpc/v4/ydb_cms_v1_pb2_grpc.py` & `ydb-3.3.5/ydb/_grpc/v4/ydb_cms_v1_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.4/ydb/_grpc/v4/ydb_coordination_v1_pb2.py` & `ydb-3.3.5/ydb/_grpc/v4/ydb_coordination_v1_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.4/ydb/_grpc/v4/ydb_coordination_v1_pb2_grpc.py` & `ydb-3.3.5/ydb/_grpc/v4/ydb_coordination_v1_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.4/ydb/_grpc/v4/ydb_discovery_v1_pb2.py` & `ydb-3.3.5/ydb/_grpc/v4/ydb_discovery_v1_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.4/ydb/_grpc/v4/ydb_discovery_v1_pb2_grpc.py` & `ydb-3.3.5/ydb/_grpc/v4/ydb_discovery_v1_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.4/ydb/_grpc/v4/ydb_export_v1_pb2.py` & `ydb-3.3.5/ydb/_grpc/v4/ydb_export_v1_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.4/ydb/_grpc/v4/ydb_export_v1_pb2_grpc.py` & `ydb-3.3.5/ydb/_grpc/v4/ydb_export_v1_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.4/ydb/_grpc/v4/ydb_import_v1_pb2.py` & `ydb-3.3.5/ydb/_grpc/v4/ydb_import_v1_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.4/ydb/_grpc/v4/ydb_import_v1_pb2_grpc.py` & `ydb-3.3.5/ydb/_grpc/v4/ydb_import_v1_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.4/ydb/_grpc/v4/ydb_monitoring_v1_pb2.py` & `ydb-3.3.5/ydb/_grpc/v4/ydb_monitoring_v1_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.4/ydb/_grpc/v4/ydb_monitoring_v1_pb2_grpc.py` & `ydb-3.3.5/ydb/_grpc/v4/ydb_monitoring_v1_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.4/ydb/_grpc/v4/ydb_operation_v1_pb2.py` & `ydb-3.3.5/ydb/_grpc/v4/ydb_operation_v1_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.4/ydb/_grpc/v4/ydb_operation_v1_pb2_grpc.py` & `ydb-3.3.5/ydb/_grpc/v4/ydb_operation_v1_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.4/ydb/_grpc/v4/ydb_rate_limiter_v1_pb2.py` & `ydb-3.3.5/ydb/_grpc/v4/ydb_rate_limiter_v1_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.4/ydb/_grpc/v4/ydb_rate_limiter_v1_pb2_grpc.py` & `ydb-3.3.5/ydb/_grpc/v4/ydb_rate_limiter_v1_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.4/ydb/_grpc/v4/ydb_scheme_v1_pb2.py` & `ydb-3.3.5/ydb/_grpc/v4/ydb_scheme_v1_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.4/ydb/_grpc/v4/ydb_scheme_v1_pb2_grpc.py` & `ydb-3.3.5/ydb/_grpc/v4/ydb_scheme_v1_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.4/ydb/_grpc/v4/ydb_scripting_v1_pb2.py` & `ydb-3.3.5/ydb/_grpc/v4/ydb_scripting_v1_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.4/ydb/_grpc/v4/ydb_scripting_v1_pb2_grpc.py` & `ydb-3.3.5/ydb/_grpc/v4/ydb_scripting_v1_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.4/ydb/_grpc/v4/ydb_table_v1_pb2.py` & `ydb-3.3.5/ydb/_grpc/v4/ydb_table_v1_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.4/ydb/_grpc/v4/ydb_table_v1_pb2_grpc.py` & `ydb-3.3.5/ydb/_grpc/v4/ydb_table_v1_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.4/ydb/_grpc/v4/ydb_topic_v1_pb2.py` & `ydb-3.3.5/ydb/_grpc/v4/ydb_topic_v1_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.4/ydb/_grpc/v4/ydb_topic_v1_pb2_grpc.py` & `ydb-3.3.5/ydb/_grpc/v4/ydb_topic_v1_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.4/ydb/_session_impl.py` & `ydb-3.3.5/ydb/_session_impl.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.4/ydb/_sp_impl.py` & `ydb-3.3.5/ydb/_sp_impl.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.4/ydb/_topic_common/common.py` & `ydb-3.3.5/ydb/_topic_common/common.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.4/ydb/_topic_common/common_test.py` & `ydb-3.3.5/ydb/_topic_common/common_test.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.4/ydb/_topic_common/test_helpers.py` & `ydb-3.3.5/ydb/_topic_common/test_helpers.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.4/ydb/_topic_reader/datatypes.py` & `ydb-3.3.5/ydb/_topic_reader/datatypes.py`

 * *Files 5% similar despite different names*

```diff
@@ -78,14 +78,16 @@
 
         try:
             self._loop = asyncio.get_running_loop()
         except RuntimeError:
             self._loop = None
 
     def add_waiter(self, end_offset: int) -> "PartitionSession.CommitAckWaiter":
+        self._ensure_not_closed()
+
         waiter = PartitionSession.CommitAckWaiter(end_offset, self._create_future())
         if end_offset <= self.committed_offset:
             waiter._finish_ok()
             return waiter
 
         # fast way
         if self._ack_waiters and self._ack_waiters[-1].end_offset < end_offset:
@@ -117,25 +119,25 @@
             waiter._finish_ok()
 
     def close(self):
         if self.closed:
             return
 
         self.state = PartitionSession.State.Stopped
-        exception = topic_reader_asyncio.TopicReaderCommitToExpiredPartition()
+        exception = topic_reader_asyncio.PublicTopicReaderPartitionExpiredError()
         for waiter in self._ack_waiters:
             waiter._finish_error(exception)
 
     @property
     def closed(self):
         return self.state == PartitionSession.State.Stopped
 
     def _ensure_not_closed(self):
         if self.state == PartitionSession.State.Stopped:
-            raise topic_reader_asyncio.TopicReaderCommitToExpiredPartition()
+            raise topic_reader_asyncio.PublicTopicReaderPartitionExpiredError()
 
     class State(enum.Enum):
         Active = 1
         GracefulShutdown = 2
         Stopped = 3
 
     @dataclass(order=True)
```

### Comparing `ydb-3.3.4/ydb/_topic_reader/datatypes_test.py` & `ydb-3.3.5/ydb/_topic_reader/datatypes_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -188,13 +188,19 @@
         assert result == session._ack_waiters
         assert res.future.done() == is_done
 
     async def test_close_notify_waiters(self, session):
         waiter = session.add_waiter(session.committed_offset + 1)
         session.close()
 
-        with pytest.raises(topic_reader_asyncio.TopicReaderCommitToExpiredPartition):
+        with pytest.raises(topic_reader_asyncio.PublicTopicReaderPartitionExpiredError):
             waiter.future.result()
 
     async def test_close_twice(self, session):
         session.close()
         session.close()
+
+    async def test_commit_after_close(self, session):
+        session.close()
+
+        with pytest.raises(topic_reader_asyncio.PublicTopicReaderPartitionExpiredError):
+            session.add_waiter(session.committed_offset + 1)
```

### Comparing `ydb-3.3.4/ydb/_topic_reader/topic_reader.py` & `ydb-3.3.5/ydb/_topic_reader/topic_reader.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.4/ydb/_topic_reader/topic_reader_asyncio.py` & `ydb-3.3.5/ydb/_topic_reader/topic_reader_asyncio.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,15 +35,15 @@
     pass
 
 
 class TopicReaderUnexpectedCodec(YdbError):
     pass
 
 
-class TopicReaderCommitToExpiredPartition(TopicReaderError):
+class PublicTopicReaderPartitionExpiredError(TopicReaderError):
     """
     Commit message when partition read session are dropped.
     It is ok - the message/batch will not commit to server and will receive in other read session
     (with this or other reader).
     """
 
     def __init__(self, message: str = "Topic reader partition session is closed"):
@@ -110,23 +110,30 @@
         return self._reconnector.receive_message_nowait()
 
     def commit(self, batch: typing.Union[datatypes.PublicMessage, datatypes.PublicBatch]):
         """
         Write commit message to a buffer.
 
         For the method no way check the commit result
-        (for example if lost connection - commits will not re-send and committed messages will receive again)
+        (for example if lost connection - commits will not re-send and committed messages will receive again).
         """
-        self._reconnector.commit(batch)
+        try:
+            self._reconnector.commit(batch)
+        except PublicTopicReaderPartitionExpiredError:
+            pass
 
     async def commit_with_ack(self, batch: typing.Union[datatypes.PublicMessage, datatypes.PublicBatch]):
         """
         write commit message to a buffer and wait ack from the server.
 
         use asyncio.wait_for for wait with timeout.
+
+        may raise ydb.TopicReaderPartitionExpiredError, the error mean reader partition closed from server
+        before receive commit ack. Message may be acked or not (if not - it will send in other read session,
+        to this or other reader).
         """
         waiter = self._reconnector.commit(batch)
         await waiter.future
 
     async def close(self, flush: bool = True):
         if self._closed:
             raise TopicReaderClosedError()
@@ -170,14 +177,22 @@
                 retry_info = check_retriable_error(err, self._settings._retry_settings(), attempt)
                 if not retry_info.is_retriable:
                     self._set_first_error(err)
                     return
                 await asyncio.sleep(retry_info.sleep_timeout_seconds)
 
                 attempt += 1
+            finally:
+                if self._stream_reader is not None:
+                    # noinspection PyBroadException
+                    try:
+                        await self._stream_reader.close()
+                    except BaseException:
+                        # supress any error on close stream reader
+                        pass
 
     async def wait_message(self):
         while True:
             if self._first_error.done():
                 raise self._first_error.result()
 
             if self._stream_reader:
@@ -344,36 +359,39 @@
             return None
 
         batch = self._message_batches.popleft()
         self._buffer_release_bytes(batch._bytes_size)
         return batch
 
     def receive_message_nowait(self):
+        if self._get_first_error():
+            raise self._get_first_error()
+
         try:
             batch = self._message_batches[0]
             message = batch.pop_message()
         except IndexError:
             return None
 
         if batch.empty():
-            self._message_batches.popleft()
+            self.receive_batch_nowait()
 
         return message
 
     def commit(self, batch: datatypes.ICommittable) -> datatypes.PartitionSession.CommitAckWaiter:
         partition_session = batch._commit_get_partition_session()
 
         if partition_session.reader_reconnector_id != self._reader_reconnector_id:
             raise TopicReaderError("reader can commit only self-produced messages")
 
         if partition_session.reader_stream_id != self._id:
-            raise TopicReaderCommitToExpiredPartition("commit messages after reconnect to server")
+            raise PublicTopicReaderPartitionExpiredError("commit messages after reconnect to server")
 
         if partition_session.id not in self._partition_sessions:
-            raise TopicReaderCommitToExpiredPartition("commit messages after server stop the partition read session")
+            raise PublicTopicReaderPartitionExpiredError("commit messages after server stop the partition read session")
 
         commit_range = batch._commit_get_offsets_range()
         waiter = partition_session.add_waiter(commit_range.end)
 
         if not waiter.future.done():
             client_message = StreamReadMessage.CommitOffsetRequest(
                 commit_offsets=[
@@ -613,21 +631,23 @@
 
         if futures:
             await asyncio.wait(futures)
 
     async def close(self):
         if self._closed:
             return
+
         self._closed = True
 
         self._set_first_error(TopicReaderStreamClosedError())
         self._state_changed.set()
         self._stream.close()
 
         for session in self._partition_sessions.values():
             session.close()
+        self._partition_sessions.clear()
 
         for task in self._background_tasks:
             task.cancel()
 
         if self._background_tasks:
             await asyncio.wait(self._background_tasks)
```

### Comparing `ydb-3.3.4/ydb/_topic_reader/topic_reader_asyncio_test.py` & `ydb-3.3.5/ydb/_topic_reader/topic_reader_asyncio_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -209,43 +209,54 @@
             data=bytes(),
             _partition_session=partition_session,
             _commit_start_offset=partition_session._next_message_start_commit_offset + offset_delta - 1,
             _commit_end_offset=partition_session._next_message_start_commit_offset + offset_delta,
         )
 
     async def send_message(self, stream_reader, message: PublicMessage):
+        await self.send_batch(stream_reader, [message])
+
+    async def send_batch(self, stream_reader, batch: typing.List[PublicMessage]):
+        if len(batch) == 0:
+            return
+
+        first_message = batch[0]
+        for message in batch:
+            assert message._partition_session is first_message._partition_session
+
         def batch_count():
             return len(stream_reader._message_batches)
 
         initial_batches = batch_count()
 
         stream = stream_reader._stream  # type: StreamMock
         stream.from_server.put_nowait(
             StreamReadMessage.FromServer(
                 server_status=ServerStatus(ydb_status_codes_pb2.StatusIds.SUCCESS, []),
                 server_message=StreamReadMessage.ReadResponse(
                     partition_data=[
                         StreamReadMessage.ReadResponse.PartitionData(
-                            partition_session_id=message._partition_session.id,
+                            partition_session_id=first_message._partition_session.id,
                             batches=[
                                 StreamReadMessage.ReadResponse.Batch(
                                     message_data=[
                                         StreamReadMessage.ReadResponse.MessageData(
                                             offset=message.offset,
                                             seq_no=message.seqno,
                                             created_at=message.created_at,
                                             data=message.data,
                                             uncompresed_size=len(message.data),
                                             message_group_id=message.message_group_id,
                                         )
+                                        for message in batch
                                     ],
-                                    producer_id=message.producer_id,
-                                    write_session_meta=message.session_metadata,
+                                    producer_id=first_message.producer_id,
+                                    write_session_meta=first_message.session_metadata,
                                     codec=Codec.CODEC_RAW,
-                                    written_at=message.written_at,
+                                    written_at=first_message.written_at,
                                 )
                             ],
                         )
                     ],
                     bytes_size=self.default_batch_size,
                 ),
             )
@@ -359,15 +370,15 @@
 
     async def test_close_ack_waiters_when_close_stream_reader(
         self, stream_reader_started: ReaderStream, partition_session
     ):
         waiter = partition_session.add_waiter(self.partition_session_committed_offset + 1)
         await wait_for_fast(stream_reader_started.close())
 
-        with pytest.raises(topic_reader_asyncio.TopicReaderCommitToExpiredPartition):
+        with pytest.raises(topic_reader_asyncio.PublicTopicReaderPartitionExpiredError):
             waiter.future.result()
 
     async def test_flush(self, stream, stream_reader_started: ReaderStream, partition_session):
         offset = self.partition_session_committed_offset + 1
         waiter = partition_session.add_waiter(offset)
 
         with pytest.raises(WaitConditionError):
@@ -1062,21 +1073,23 @@
 
         assert mess == expected_message
         assert list(stream_reader._message_batches) == batches_after
 
     async def test_receive_batch_nowait(self, stream, stream_reader, partition_session):
         assert stream_reader.receive_batch_nowait() is None
 
+        initial_buffer_size = stream_reader._buffer_size_bytes
+
         mess1 = self.create_message(partition_session, 1, 1)
         await self.send_message(stream_reader, mess1)
 
         mess2 = self.create_message(partition_session, 2, 1)
         await self.send_message(stream_reader, mess2)
 
-        initial_buffer_size = stream_reader._buffer_size_bytes
+        assert stream_reader._buffer_size_bytes == initial_buffer_size - 2 * self.default_batch_size
 
         received = stream_reader.receive_batch_nowait()
         assert received == PublicBatch(
             messages=[mess1],
             _partition_session=mess1._partition_session,
             _bytes_size=self.default_batch_size,
             _codec=Codec.CODEC_RAW,
@@ -1086,22 +1099,45 @@
         assert received == PublicBatch(
             messages=[mess2],
             _partition_session=mess2._partition_session,
             _bytes_size=self.default_batch_size,
             _codec=Codec.CODEC_RAW,
         )
 
-        assert stream_reader._buffer_size_bytes == initial_buffer_size + 2 * self.default_batch_size
+        assert stream_reader._buffer_size_bytes == initial_buffer_size
 
         assert StreamReadMessage.ReadRequest(self.default_batch_size) == stream.from_client.get_nowait().client_message
         assert StreamReadMessage.ReadRequest(self.default_batch_size) == stream.from_client.get_nowait().client_message
 
         with pytest.raises(asyncio.QueueEmpty):
             stream.from_client.get_nowait()
 
+    async def test_receive_message_nowait(self, stream, stream_reader, partition_session):
+        assert stream_reader.receive_batch_nowait() is None
+
+        initial_buffer_size = stream_reader._buffer_size_bytes
+
+        await self.send_batch(
+            stream_reader, [self.create_message(partition_session, 1, 1), self.create_message(partition_session, 2, 1)]
+        )
+        await self.send_batch(
+            stream_reader,
+            [
+                self.create_message(partition_session, 10, 1),
+            ],
+        )
+
+        assert stream_reader._buffer_size_bytes == initial_buffer_size - 2 * self.default_batch_size
+
+        for expected_seqno in [1, 2, 10]:
+            mess = stream_reader.receive_message_nowait()
+            assert mess.seqno == expected_seqno
+
+        assert stream_reader._buffer_size_bytes == initial_buffer_size
+
     async def test_update_token(self, stream):
         settings = PublicReaderSettings(
             consumer="test-consumer",
             topic="test-topic",
             update_token_interval=0.1,
         )
         reader = await self.get_started_reader(stream, settings, get_token_function=lambda: "foo-bar")
```

### Comparing `ydb-3.3.4/ydb/_topic_reader/topic_reader_sync.py` & `ydb-3.3.5/ydb/_topic_reader/topic_reader_sync.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.4/ydb/_topic_writer/topic_writer.py` & `ydb-3.3.5/ydb/_topic_writer/topic_writer.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.4/ydb/_topic_writer/topic_writer_asyncio.py` & `ydb-3.3.5/ydb/_topic_writer/topic_writer_asyncio.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import asyncio
 import concurrent.futures
 import datetime
+import functools
 import gzip
 import typing
 from collections import deque
 from typing import Deque, AsyncIterator, Union, List, Optional, Dict, Callable
 
 import logging
 
@@ -71,15 +72,15 @@
             if exc_val is None:
                 raise
 
     def __del__(self):
         if self._closed or self._loop.is_closed():
             return
 
-        self._loop.call_soon(self.close, False)
+        self._loop.call_soon(functools.partial(self.close, flush=False))
 
     async def close(self, *, flush: bool = True):
         if self._closed:
             return
 
         self._closed = True
```

### Comparing `ydb-3.3.4/ydb/_topic_writer/topic_writer_asyncio_test.py` & `ydb-3.3.5/ydb/_topic_writer/topic_writer_asyncio_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -621,15 +621,15 @@
             async with self.lock:
                 futures = [asyncio.Future() for _ in messages]
                 self.messages.extend(messages)
                 self.futures.extend(futures)
                 self.messages_writted.set()
                 return futures
 
-        async def close(self):
+        async def close(self, flush: bool):
             pass
 
     @pytest.fixture
     def default_settings(self) -> PublicWriterSettings:
         return PublicWriterSettings(
             topic="/local/topic",
             producer_id="producer-id",
```

### Comparing `ydb-3.3.4/ydb/_topic_writer/topic_writer_sync.py` & `ydb-3.3.5/ydb/_topic_writer/topic_writer_sync.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.4/ydb/_topic_writer/topic_writer_test.py` & `ydb-3.3.5/ydb/_topic_writer/topic_writer_test.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.4/ydb/_tx_ctx_impl.py` & `ydb-3.3.5/ydb/_tx_ctx_impl.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.4/ydb/_utilities.py` & `ydb-3.3.5/ydb/_utilities.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.4/ydb/aio/connection.py` & `ydb-3.3.5/ydb/aio/connection.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.4/ydb/aio/credentials.py` & `ydb-3.3.5/ydb/aio/credentials.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.4/ydb/aio/driver.py` & `ydb-3.3.5/ydb/aio/driver.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.4/ydb/aio/iam.py` & `ydb-3.3.5/ydb/aio/iam.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.4/ydb/aio/pool.py` & `ydb-3.3.5/ydb/aio/pool.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.4/ydb/aio/resolver.py` & `ydb-3.3.5/ydb/aio/resolver.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.4/ydb/aio/scheme.py` & `ydb-3.3.5/ydb/aio/scheme.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.4/ydb/aio/table.py` & `ydb-3.3.5/ydb/aio/table.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.4/ydb/connection.py` & `ydb-3.3.5/ydb/connection.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.4/ydb/convert.py` & `ydb-3.3.5/ydb/convert.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.4/ydb/credentials.py` & `ydb-3.3.5/ydb/credentials.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.4/ydb/dbapi/__init__.py` & `ydb-3.3.5/ydb/dbapi/__init__.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.4/ydb/dbapi/connection.py` & `ydb-3.3.5/ydb/dbapi/connection.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.4/ydb/dbapi/cursor.py` & `ydb-3.3.5/ydb/dbapi/cursor.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.4/ydb/dbapi/errors.py` & `ydb-3.3.5/ydb/dbapi/errors.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.4/ydb/default_pem.py` & `ydb-3.3.5/ydb/default_pem.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.4/ydb/driver.py` & `ydb-3.3.5/ydb/driver.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.4/ydb/export.py` & `ydb-3.3.5/ydb/export.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.4/ydb/global_settings.py` & `ydb-3.3.5/ydb/global_settings.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.4/ydb/iam/auth.py` & `ydb-3.3.5/ydb/iam/auth.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.4/ydb/import_client.py` & `ydb-3.3.5/ydb/import_client.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.4/ydb/interceptor.py` & `ydb-3.3.5/ydb/interceptor.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.4/ydb/issues.py` & `ydb-3.3.5/ydb/issues.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.4/ydb/operation.py` & `ydb-3.3.5/ydb/operation.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.4/ydb/pool.py` & `ydb-3.3.5/ydb/pool.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.4/ydb/resolver.py` & `ydb-3.3.5/ydb/resolver.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.4/ydb/scheme.py` & `ydb-3.3.5/ydb/scheme.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.4/ydb/scheme_test.py` & `ydb-3.3.5/ydb/scheme_test.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.4/ydb/scripting.py` & `ydb-3.3.5/ydb/scripting.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.4/ydb/settings.py` & `ydb-3.3.5/ydb/settings.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.4/ydb/sqlalchemy/__init__.py` & `ydb-3.3.5/ydb/sqlalchemy/__init__.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.4/ydb/sqlalchemy/types.py` & `ydb-3.3.5/ydb/sqlalchemy/types.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.4/ydb/table.py` & `ydb-3.3.5/ydb/table.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.4/ydb/table_test.py` & `ydb-3.3.5/ydb/table_test.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.4/ydb/topic.py` & `ydb-3.3.5/ydb/topic.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,15 @@
     "TopicDescription",
     "TopicError",
     "TopicMeteringMode",
     "TopicReader",
     "TopicReaderAsyncIO",
     "TopicReaderSelector",
     "TopicReaderSettings",
+    "TopicReaderPartitionExpiredError",
     "TopicStatWindow",
     "TopicWriteResult",
     "TopicWriter",
     "TopicWriterAsyncIO",
     "TopicWriterInitInfo",
     "TopicWriterMessage",
     "TopicWriterSettings",
@@ -36,14 +37,15 @@
     PublicTopicSelector as TopicReaderSelector,
 )
 
 from ._topic_reader.topic_reader_sync import TopicReaderSync as TopicReader
 
 from ._topic_reader.topic_reader_asyncio import (
     PublicAsyncIOReader as TopicReaderAsyncIO,
+    PublicTopicReaderPartitionExpiredError as TopicReaderPartitionExpiredError,
 )
 
 from ._topic_writer.topic_writer import (  # noqa: F401
     PublicWriterSettings as TopicWriterSettings,
     PublicMessage as TopicWriterMessage,
     RetryPolicy as TopicWriterRetryPolicy,
     PublicWriterInitInfo as TopicWriterInitInfo,
```

### Comparing `ydb-3.3.4/ydb/tracing.py` & `ydb-3.3.5/ydb/tracing.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.4/ydb/types.py` & `ydb-3.3.5/ydb/types.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.4/ydb.egg-info/PKG-INFO` & `ydb-3.3.5/ydb.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ydb
-Version: 3.3.4
+Version: 3.3.5
 Summary: YDB Python SDK
 Home-page: http://github.com/ydb-platform/ydb-python-sdk
 Author: Yandex LLC
 Author-email: ydb@yandex-team.ru
 License: Apache 2.0
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2
```

### Comparing `ydb-3.3.4/ydb.egg-info/SOURCES.txt` & `ydb-3.3.5/ydb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

