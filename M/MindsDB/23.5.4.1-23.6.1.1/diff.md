# Comparing `tmp/MindsDB-23.5.4.1.tar.gz` & `tmp/MindsDB-23.6.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/MindsDB-23.5.4.1.tar", last modified: Tue May 23 09:12:35 2023, max compression
+gzip compressed data, was "dist/MindsDB-23.6.1.1.tar", last modified: Thu Jun  8 22:54:03 2023, max compression
```

## Comparing `MindsDB-23.5.4.1.tar` & `MindsDB-23.6.1.1.tar`

### file list

```diff
@@ -1,1331 +1,1362 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:35.000000 MindsDB-23.5.4.1/
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/MANIFEST.in
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/MindsDB.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    23039 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/MindsDB.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    63528 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/MindsDB.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/MindsDB.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      733 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/MindsDB.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/MindsDB.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    23039 2023-05-23 09:12:35.000000 MindsDB-23.5.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    20993 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13583 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/api/common/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/common/check_auth.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/api/http/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/http/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3090 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/http/gui.py
--rw-r--r--   0 runner    (1001) docker     (123)      534 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/http/gunicorn_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)    12972 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/http/initialize.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/api/http/namespaces/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/http/namespaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2954 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/http/namespaces/analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     5466 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/http/namespaces/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     8171 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/http/namespaces/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/api/http/namespaces/configs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/http/namespaces/configs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/http/namespaces/configs/analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/http/namespaces/configs/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/http/namespaces/configs/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/http/namespaces/configs/databases.py
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/http/namespaces/configs/default.py
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/http/namespaces/configs/files.py
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/http/namespaces/configs/handlers.py
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/http/namespaces/configs/projects.py
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/http/namespaces/configs/sql.py
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/http/namespaces/configs/streams.py
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/http/namespaces/configs/tabs.py
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/http/namespaces/configs/tree.py
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/http/namespaces/configs/util.py
--rw-r--r--   0 runner    (1001) docker     (123)    10355 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/http/namespaces/databases.py
--rw-r--r--   0 runner    (1001) docker     (123)     4516 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/http/namespaces/default.py
--rw-r--r--   0 runner    (1001) docker     (123)     5627 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/http/namespaces/file.py
--rw-r--r--   0 runner    (1001) docker     (123)     4781 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/http/namespaces/handlers.py
--rw-r--r--   0 runner    (1001) docker     (123)    10197 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/http/namespaces/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/http/namespaces/projects.py
--rw-r--r--   0 runner    (1001) docker     (123)     4867 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/http/namespaces/sql.py
--rw-r--r--   0 runner    (1001) docker     (123)     4084 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/http/namespaces/stream.py
--rw-r--r--   0 runner    (1001) docker     (123)     1551 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/http/namespaces/tab.py
--rw-r--r--   0 runner    (1001) docker     (123)     2866 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/http/namespaces/tree.py
--rw-r--r--   0 runner    (1001) docker     (123)     2919 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/http/namespaces/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     5393 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/http/namespaces/views.py
--rw-r--r--   0 runner    (1001) docker     (123)     1958 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/http/start.py
--rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/http/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/api/mongo/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/mongo/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/api/mongo/classes/
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/mongo/classes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/mongo/classes/query_sql.py
--rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/mongo/classes/responder.py
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/mongo/classes/responder_collection.py
--rw-r--r--   0 runner    (1001) docker     (123)     3217 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/mongo/classes/scram.py
--rw-r--r--   0 runner    (1001) docker     (123)      812 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/mongo/classes/session.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/api/mongo/functions/
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/mongo/functions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/api/mongo/responders/
--rw-r--r--   0 runner    (1001) docker     (123)     2655 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/mongo/responders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/mongo/responders/add_shard.py
--rw-r--r--   0 runner    (1001) docker     (123)     2364 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/mongo/responders/aggregate.py
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/mongo/responders/buildinfo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1767 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/mongo/responders/coll_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/mongo/responders/company_id.py
--rw-r--r--   0 runner    (1001) docker     (123)      577 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/mongo/responders/connection_status.py
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/mongo/responders/count.py
--rw-r--r--   0 runner    (1001) docker     (123)      825 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/mongo/responders/db_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     4221 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/mongo/responders/delete.py
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/mongo/responders/end_sessions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5601 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/mongo/responders/find.py
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/mongo/responders/get_cmd_line_opts.py
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/mongo/responders/get_free_monitoring_status.py
--rw-r--r--   0 runner    (1001) docker     (123)      602 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/mongo/responders/get_parameter.py
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/mongo/responders/getlog.py
--rw-r--r--   0 runner    (1001) docker     (123)      627 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/mongo/responders/host_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     9502 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/mongo/responders/insert.py
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/mongo/responders/is_master.py
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/mongo/responders/is_master_lower.py
--rw-r--r--   0 runner    (1001) docker     (123)     1536 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/mongo/responders/list_collections.py
--rw-r--r--   0 runner    (1001) docker     (123)      920 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/mongo/responders/list_databases.py
--rw-r--r--   0 runner    (1001) docker     (123)      538 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/mongo/responders/list_indexes.py
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/mongo/responders/ping.py
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/mongo/responders/recv_chunk_start.py
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/mongo/responders/replsetgetstatus.py
--rw-r--r--   0 runner    (1001) docker     (123)      890 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/mongo/responders/sasl_continue.py
--rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/mongo/responders/sasl_start.py
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/mongo/responders/update_range_deletions.py
--rw-r--r--   0 runner    (1001) docker     (123)      481 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/mongo/responders/whatsmyuri.py
--rw-r--r--   0 runner    (1001) docker     (123)    14041 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/mongo/server.py
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/mongo/start.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/api/mongo/utilities/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/mongo/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/mongo/utilities/log.py
--rw-r--r--   0 runner    (1001) docker     (123)     7666 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/mongo/utilities/mongodb_ast.py
--rw-r--r--   0 runner    (1001) docker     (123)     4166 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/mongo/utilities/mongodb_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     2160 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/mongo/utilities/mongodb_query.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/api/mysql/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/mysql/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/api/mysql/mysql_proxy/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/mysql/mysql_proxy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/api/mysql/mysql_proxy/classes/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/mysql/mysql_proxy/classes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3358 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/mysql/mysql_proxy/classes/client_capabilities.py
--rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/mysql/mysql_proxy/classes/com_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/api/mysql/mysql_proxy/classes/fake_mysql_proxy/
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/mysql/mysql_proxy/classes/fake_mysql_proxy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      914 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/mysql/mysql_proxy/classes/fake_mysql_proxy/fake_mysql_proxy.py
--rw-r--r--   0 runner    (1001) docker     (123)      586 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/mysql/mysql_proxy/classes/server_capabilities.py
--rw-r--r--   0 runner    (1001) docker     (123)    56525 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/mysql/mysql_proxy/classes/sql_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     4436 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/mysql/mysql_proxy/classes/sql_statement_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/api/mysql/mysql_proxy/controllers/
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/mysql/mysql_proxy/controllers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3914 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/mysql/mysql_proxy/controllers/session_controller.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/api/mysql/mysql_proxy/data_types/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/mysql/mysql_proxy/data_types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5834 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/mysql/mysql_proxy/data_types/mysql_datum.py
--rw-r--r--   0 runner    (1001) docker     (123)     4839 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packet.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/
--rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4620 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/binary_resultset_row_package.py
--rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/column_count_packet.py
--rw-r--r--   0 runner    (1001) docker     (123)     2982 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/column_definition_packet.py
--rw-r--r--   0 runner    (1001) docker     (123)     5765 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/command_packet.py
--rw-r--r--   0 runner    (1001) docker     (123)     1428 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/eof_packet.py
--rw-r--r--   0 runner    (1001) docker     (123)     1520 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/err_packet.py
--rw-r--r--   0 runner    (1001) docker     (123)      486 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/fast_auth_fail_packet.py
--rw-r--r--   0 runner    (1001) docker     (123)     2927 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/handshake_packet.py
--rw-r--r--   0 runner    (1001) docker     (123)     3770 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/handshake_response_packet.py
--rw-r--r--   0 runner    (1001) docker     (123)     3785 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/ok_packet.py
--rw-r--r--   0 runner    (1001) docker     (123)      421 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/password_answer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/resultset_row_package.py
--rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/stmt_prepare_header.py
--rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/switch_auth_packet.py
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/switch_auth_response_packet.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/api/mysql/mysql_proxy/datahub/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/mysql/mysql_proxy/datahub/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/api/mysql/mysql_proxy/datahub/classes/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/mysql/mysql_proxy/datahub/classes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2786 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/mysql/mysql_proxy/datahub/classes/tables_row.py
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/mysql/mysql_proxy/datahub/datahub.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/api/mysql/mysql_proxy/datahub/datanodes/
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/mysql/mysql_proxy/datahub/datanodes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/mysql/mysql_proxy/datahub/datanodes/datanode.py
--rw-r--r--   0 runner    (1001) docker     (123)    23207 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/mysql/mysql_proxy/datahub/datanodes/information_schema_datanode.py
--rw-r--r--   0 runner    (1001) docker     (123)     6121 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/mysql/mysql_proxy/datahub/datanodes/integration_datanode.py
--rw-r--r--   0 runner    (1001) docker     (123)     4087 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/mysql/mysql_proxy/datahub/datanodes/project_datanode.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/api/mysql/mysql_proxy/executor/
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/mysql/mysql_proxy/executor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      673 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/mysql/mysql_proxy/executor/data_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     7054 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/mysql/mysql_proxy/executor/executor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/mysql/mysql_proxy/executor/executor_client_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)    67108 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/mysql/mysql_proxy/executor/executor_commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     5030 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/mysql/mysql_proxy/executor/executor_grpc_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     9125 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/mysql/mysql_proxy/executor/executor_grpc_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/mysql/mysql_proxy/executor/executor_service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/api/mysql/mysql_proxy/external_libs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/mysql/mysql_proxy/external_libs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4116 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/mysql/mysql_proxy/external_libs/mysql_scramble.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/api/mysql/mysql_proxy/libs/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/mysql/mysql_proxy/libs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/api/mysql/mysql_proxy/libs/constants/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/mysql/mysql_proxy/libs/constants/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    35316 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/mysql/mysql_proxy/libs/constants/mysql.py
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/mysql/mysql_proxy/libs/constants/response_type.py
--rw-r--r--   0 runner    (1001) docker     (123)    31908 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/mysql/mysql_proxy/mysql_proxy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/api/mysql/mysql_proxy/utilities/
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/mysql/mysql_proxy/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/mysql/mysql_proxy/utilities/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      973 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/mysql/mysql_proxy/utilities/functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2341 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/mysql/mysql_proxy/utilities/lightwood_dtype.py
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/mysql/mysql_proxy/utilities/log.py
--rw-r--r--   0 runner    (1001) docker     (123)     2790 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/mysql/mysql_proxy/utilities/sql.py
--rw-r--r--   0 runner    (1001) docker     (123)      422 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/mysql/start.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/api/nlp/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/nlp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/nlp/nlp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/api/postgres/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/postgres/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/api/postgres/postgres_proxy/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/postgres/postgres_proxy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/api/postgres/postgres_proxy/executor/
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/postgres/postgres_proxy/executor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6543 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/postgres/postgres_proxy/executor/executor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/api/postgres/postgres_proxy/postgres_packets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/postgres/postgres_proxy/postgres_packets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12729 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/postgres/postgres_proxy/postgres_packets/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/postgres/postgres_proxy/postgres_packets/postgres_fields.py
--rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/postgres/postgres_proxy/postgres_packets/postgres_message.py
--rw-r--r--   0 runner    (1001) docker     (123)    40804 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/postgres/postgres_proxy/postgres_packets/postgres_message_formats.py
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/postgres/postgres_proxy/postgres_packets/postgres_message_identifiers.py
--rw-r--r--   0 runner    (1001) docker     (123)     8434 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/postgres/postgres_proxy/postgres_packets/postgres_packets.py
--rw-r--r--   0 runner    (1001) docker     (123)    19291 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/postgres/postgres_proxy/postgres_proxy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/api/postgres/postgres_proxy/utilities/
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/postgres/postgres_proxy/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      376 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/api/postgres/start.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/access_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/access_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      633 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/access_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6362 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/access_handler/access_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    32145 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/access_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/access_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/access_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/access_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/access_handler/tests/test_access_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/airtable_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/airtable_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/airtable_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6808 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/airtable_handler/airtable_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     4911 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/airtable_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/airtable_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/airtable_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/airtable_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/airtable_handler/tests/test_airtable_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/altibase_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/altibase_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/altibase_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8296 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/altibase_handler/altibase_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)   342129 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/altibase_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/altibase_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/altibase_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/altibase_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/altibase_handler/tests/test_altibase_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/aurora_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/aurora_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/aurora_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6404 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/aurora_handler/aurora_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    11767 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/aurora_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/aurora_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/aurora_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/aurora_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/aurora_handler/tests/test_aurora_mysql_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/aurora_handler/tests/test_aurora_postgres_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/autokeras_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/autokeras_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      523 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/autokeras_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5616 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/autokeras_handler/autokeras_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/autokeras_handler/functions.py
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/autokeras_handler/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/autosklearn_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/autosklearn_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/autosklearn_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1685 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/autosklearn_handler/autosklearn_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)      710 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/autosklearn_handler/config.py
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/autosklearn_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      745 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/autosklearn_handler/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/bigquery_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/bigquery_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      577 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/bigquery_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5974 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/bigquery_handler/bigquery_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/bigquery_handler/logo.svg
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/bigquery_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/bigquery_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/bigquery_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      941 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/bigquery_handler/tests/test_bigquery_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/binance_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/binance_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/binance_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5238 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/binance_handler/binance_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     7458 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/binance_handler/binance_tables.py
--rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/binance_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/binance_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/byom_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/byom_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/byom_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6723 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/byom_handler/byom_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3469 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/byom_handler/proc_wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/cassandra_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      351 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/cassandra_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/cassandra_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/cassandra_handler/cassandra_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)   176707 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/cassandra_handler/logo.png
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/cassandra_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/cassandra_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/cassandra_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/cassandra_handler/tests/test_cassandra_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/ckan_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/ckan_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      472 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/ckan_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3485 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/ckan_handler/ckan_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    17688 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/ckan_handler/logo.png
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/ckan_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/ckan_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/ckan_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      820 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/ckan_handler/tests/test_ckan_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/clickhouse_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/clickhouse_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/clickhouse_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6531 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/clickhouse_handler/clickhouse_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/clickhouse_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/clickhouse_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/clickhouse_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1458 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/clickhouse_handler/tests/test_clickhouse_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/cloud_spanner_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/cloud_spanner_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      662 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/cloud_spanner_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6308 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/cloud_spanner_handler/cloud_spanner_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     6419 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/cloud_spanner_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/cloud_spanner_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/cloud_spanner_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/cloud_spanner_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/cloud_spanner_handler/tests/test_cloud_spanner_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/cloud_sql_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/cloud_sql_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      618 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/cloud_sql_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5153 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/cloud_sql_handler/cloud_sql_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    37571 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/cloud_sql_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/cloud_sql_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/cloud_sql_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/cloud_sql_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/cloud_sql_handler/tests/test_cloud_sql_mssql_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/cloud_sql_handler/tests/test_cloud_sql_mysql_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/cockroach_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      351 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/cockroach_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/cockroach_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/cockroach_handler/cockroach_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/cockroach_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/cockroach_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/cockroach_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/cockroach_handler/tests/test_cockroachdb_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/confluence_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/confluence_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      710 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/confluence_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2743 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/confluence_handler/confluence_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     4301 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/confluence_handler/confluence_table.py
--rw-r--r--   0 runner    (1001) docker     (123)    76194 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/confluence_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/confluence_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/couchbase_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/couchbase_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/couchbase_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9347 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/couchbase_handler/couchbase_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3371 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/couchbase_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/couchbase_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/couchbase_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/couchbase_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1233 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/couchbase_handler/tests/test_couchbase_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/crate_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/crate_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/crate_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7157 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/crate_handler/crate_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2999 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/crate_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/crate_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/crate_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/crate_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/crate_handler/tests/test_crate_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/d0lt_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/d0lt_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/d0lt_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    85600 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/d0lt_handler/create-db.png
--rw-r--r--   0 runner    (1001) docker     (123)    98275 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/d0lt_handler/create-predictor.png
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/d0lt_handler/d0lt_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1590 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/d0lt_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)    98983 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/d0lt_handler/predict-target.png
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/d0lt_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/d0lt_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/d0lt_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/d0lt_handler/tests/test_d0lt_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/databend_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/databend_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/databend_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/databend_handler/databend_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     6443 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/databend_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/databend_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/databend_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/databend_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/databend_handler/tests/test_databend_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/databricks_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/databricks_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      639 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/databricks_handler/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/databricks_handler/databricks/
--rw-r--r--   0 runner    (1001) docker     (123)    86110 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/databricks_handler/databricks/createdb.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    58645 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/databricks_handler/databricks/createpred.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    35986 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/databricks_handler/databricks/hivmetastore.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    21694 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/databricks_handler/databricks/mindsdbdatabricks.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    62078 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/databricks_handler/databricks/selectfrom.jpg
--rw-r--r--   0 runner    (1001) docker     (123)     7952 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/databricks_handler/databricks_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    12097 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/databricks_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/databricks_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/databricks_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/databricks_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/databricks_handler/tests/test_databricks_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/datastax_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/datastax_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      531 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/datastax_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/datastax_handler/datastax_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    26175 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/datastax_handler/logo.png
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/datastax_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/datastax_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/datastax_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/datastax_handler/tests/test_cassandra_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/db2_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/db2_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/db2_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9099 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/db2_handler/db2_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    19117 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/db2_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/db2_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/db2_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/db2_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/db2_handler/tests/test_db2_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/derby_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/derby_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/derby_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8751 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/derby_handler/derby_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     7305 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/derby_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/derby_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/derby_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/derby_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/derby_handler/tests/test_derby_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/dremio_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/dremio_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/dremio_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7311 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/dremio_handler/dremio_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    52734 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/dremio_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/dremio_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/dremio_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/dremio_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/dremio_handler/tests/test_dremio_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/druid_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/druid_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      602 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/druid_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7324 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/druid_handler/druid_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    29112 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/druid_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/druid_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/druid_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/druid_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/druid_handler/tests/test_druid_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/duckdb_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/duckdb_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      635 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/duckdb_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5486 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/duckdb_handler/duckdb_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    19548 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/duckdb_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/duckdb_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/duckdb_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/duckdb_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/duckdb_handler/tests/test_duckdb_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/dynamodb_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      361 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/dynamodb_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/dynamodb_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6592 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/dynamodb_handler/dynamodb_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    55623 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/dynamodb_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/dynamodb_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/dynamodb_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/dynamodb_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/dynamodb_handler/tests/test_dynamodb_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/edgelessdb_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/edgelessdb_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/edgelessdb_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1871 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/edgelessdb_handler/edgelessdb_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     8768 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/edgelessdb_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/edgelessdb_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/edgelessdb_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/edgelessdb_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/edgelessdb_handler/tests/test_edgelessdb_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/elasticsearch_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/elasticsearch_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/elasticsearch_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7624 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/elasticsearch_handler/elasticsearch_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     4749 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/elasticsearch_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/elasticsearch_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/elasticsearch_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/elasticsearch_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/elasticsearch_handler/tests/test_elasticsearch_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/empress_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/empress_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/empress_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7713 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/empress_handler/empress_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    11249 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/empress_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/empress_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/empress_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/empress_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/empress_handler/tests/test_empress_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/eventstoredb_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/eventstoredb_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/eventstoredb_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9062 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/eventstoredb_handler/eventstoredb_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     6031 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/eventstoredb_handler/icon.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/file_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/file_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      275 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/file_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10883 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/file_handler/file_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/firebird_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      361 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/firebird_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/firebird_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9566 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/firebird_handler/firebird_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    54033 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/firebird_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)        3 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/firebird_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/firebird_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/firebird_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/firebird_handler/tests/test_firebird_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/frappe_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/frappe_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      480 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/frappe_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3412 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/frappe_handler/frappe_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     4986 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/frappe_handler/frappe_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2588 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/frappe_handler/frappe_tables.py
--rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/frappe_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/frappe_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/github_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/github_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/github_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3165 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/github_handler/github_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    21392 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/github_handler/github_tables.py
--rw-r--r--   0 runner    (1001) docker     (123)      963 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/github_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/github_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/gitlab_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/gitlab_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      481 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/gitlab_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/gitlab_handler/gitlab_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     6542 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/gitlab_handler/gitlab_tables.py
--rw-r--r--   0 runner    (1001) docker     (123)     2075 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/gitlab_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/gitlab_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/gmail_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/gmail_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      492 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/gmail_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15215 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/gmail_handler/gmail_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/gmail_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/gmail_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/gmail_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/gmail_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/gmail_handler/tests/test_gmail_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/google_books_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/google_books_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/google_books_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6885 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/google_books_handler/google_books_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     6268 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/google_books_handler/google_books_tables.py
--rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/google_books_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/google_books_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/google_books_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/google_books_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/google_books_handler/tests/test_google_books_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/google_calendar_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/google_calendar_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      516 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/google_calendar_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10399 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/google_calendar_handler/google_calendar_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     8111 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/google_calendar_handler/google_calendar_tables.py
--rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/google_calendar_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/google_calendar_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/google_calendar_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/google_calendar_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2228 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/google_calendar_handler/tests/test_google_calendar_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/google_content_shopping_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/google_content_shopping_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      663 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/google_content_shopping_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16251 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/google_content_shopping_handler/google_content_shopping_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    14279 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/google_content_shopping_handler/google_content_shopping_tables.py
--rw-r--r--   0 runner    (1001) docker     (123)    34337 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/google_content_shopping_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/google_content_shopping_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/google_content_shopping_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/google_content_shopping_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2449 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/google_content_shopping_handler/tests/test_google_content_shopping_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/google_fit_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/google_fit_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/google_fit_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6599 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/google_fit_handler/google_fit_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2496 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/google_fit_handler/google_fit_tables.py
--rw-r--r--   0 runner    (1001) docker     (123)    21355 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/google_fit_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/google_fit_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/google_search_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/google_search_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/google_search_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8170 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/google_search_handler/google_search_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     7375 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/google_search_handler/google_search_tables.py
--rw-r--r--   0 runner    (1001) docker     (123)     8618 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/google_search_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/google_search_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/google_search_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/google_search_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2191 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/google_search_handler/tests/test_google_search_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/hackernews_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/hackernews_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/hackernews_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3044 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/hackernews_handler/hn_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     5425 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/hackernews_handler/hn_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/hackernews_handler/icon.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/hana_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/hana_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/hana_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11104 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/hana_handler/hana_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)      715 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/hana_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/hana_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/hive_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/hive_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/hive_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5947 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/hive_handler/hive_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    14000 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/hive_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/hive_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/hive_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/hive_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/hive_handler/tests/test_hive_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/hsqldb_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/hsqldb_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      627 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/hsqldb_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7491 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/hsqldb_handler/hsqldb_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     5355 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/hsqldb_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/hsqldb_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/huggingface_api_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/huggingface_api_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      549 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/huggingface_api_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6425 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/huggingface_api_handler/huggingface_api_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/huggingface_api_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/huggingface_api_handler/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/huggingface_api_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/huggingface_api_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/huggingface_api_handler/tests/test_huggingface_api_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/huggingface_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/huggingface_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/huggingface_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10843 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/huggingface_handler/huggingface_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/huggingface_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/huggingface_handler/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/ignite_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/ignite_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/ignite_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    45779 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/ignite_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)     7181 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/ignite_handler/ignite_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/ignite_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/ignite_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/ignite_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/ignite_handler/tests/test_ignite_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/impala_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/impala_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/impala_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2542 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/impala_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)     5640 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/impala_handler/impala_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/impala_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/impala_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/impala_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/impala_handler/tests/test_impala_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/influxdb_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/influxdb_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      690 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/influxdb_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    63375 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/influxdb_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)     3359 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/influxdb_handler/influxdb_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3281 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/influxdb_handler/influxdb_tables.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/influxdb_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/informix_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/informix_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/informix_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6694 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/informix_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)     9618 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/informix_handler/informix_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/informix_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/informix_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/informix_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/informix_handler/tests/test_informix_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/ingres_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/ingres_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      627 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/ingres_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3932 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/ingres_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)     7581 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/ingres_handler/ingres_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/ingres_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/ingres_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/ingres_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/ingres_handler/tests/test_ingres_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/jira_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/jira_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      565 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/jira_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16812 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/jira_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)     3244 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/jira_handler/jira_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     5493 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/jira_handler/jira_table.py
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/jira_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/langchain_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/langchain_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/langchain_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16667 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/langchain_handler/langchain_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     6680 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/langchain_handler/mindsdb_database_agent.py
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/langchain_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/langchain_handler/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/lightwood_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/lightwood_handler/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/lightwood_handler/lightwood_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/lightwood_handler/lightwood_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/lightwood_handler/lightwood_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8801 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/lightwood_handler/lightwood_handler/functions.py
--rw-r--r--   0 runner    (1001) docker     (123)    20556 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/lightwood_handler/lightwood_handler/lightwood_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2300 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/lightwood_handler/lightwood_handler/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/lightwood_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      949 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/lightwood_handler/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/lightwood_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/lightwood_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10985 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/lightwood_handler/tests/test_lightwood_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/ludwig_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/ludwig_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/ludwig_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/ludwig_handler/functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2395 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/ludwig_handler/ludwig_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/ludwig_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      740 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/ludwig_handler/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/ludwig_handler/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/mariadb_handler/
--rw-r--r--   0 runner    (1001) docker     (123)    88354 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/mariadb_handler/1-create_db.png
--rw-r--r--   0 runner    (1001) docker     (123)   110633 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/mariadb_handler/2-create_predictor.png
--rw-r--r--   0 runner    (1001) docker     (123)   109269 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/mariadb_handler/3-predict_target.png
--rw-r--r--   0 runner    (1001) docker     (123)    62778 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/mariadb_handler/4-drop_db.png
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/mariadb_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/mariadb_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    99045 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/mariadb_handler/create-db.png
--rw-r--r--   0 runner    (1001) docker     (123)     7657 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/mariadb_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/mariadb_handler/mariadb_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    98530 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/mariadb_handler/predict-db.png
--rw-r--r--   0 runner    (1001) docker     (123)   100718 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/mariadb_handler/predictor.png
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/mariadb_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/materialize_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/materialize_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/materialize_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    47935 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/materialize_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/materialize_handler/materialize_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/materialize_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/materialize_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/materialize_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1774 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/materialize_handler/tests/test_materialize_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/matrixone_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/matrixone_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/matrixone_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    57976 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/matrixone_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)     6870 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/matrixone_handler/matrixone_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/matrixone_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/matrixone_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/matrixone_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1789 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/matrixone_handler/tests/test_matrixone_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/maxdb_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/maxdb_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      635 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/maxdb_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26795 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/maxdb_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)     7507 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/maxdb_handler/maxdb_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/maxdb_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/maxdb_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/maxdb_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1918 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/maxdb_handler/tests/test_maxdb_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/merlion_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/merlion_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/merlion_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8498 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/merlion_handler/adapters.py
--rw-r--r--   0 runner    (1001) docker     (123)     8217 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/merlion_handler/merlion_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/merlion_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      828 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/merlion_handler/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/mlflow_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/mlflow_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      542 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/mlflow_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3802 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/mlflow_handler/mlflow_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/mlflow_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      740 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/mlflow_handler/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/monetdb_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/monetdb_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/monetdb_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   544421 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/monetdb_handler/create-database.png
--rw-r--r--   0 runner    (1001) docker     (123)   423554 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/monetdb_handler/create-predictor.png
--rw-r--r--   0 runner    (1001) docker     (123)    64685 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/monetdb_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)     8118 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/monetdb_handler/monetdb_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/monetdb_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)   445044 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/monetdb_handler/select-predictor.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/monetdb_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/monetdb_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/monetdb_handler/tests/test_monetdb_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/monetdb_handler/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/monetdb_handler/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/monetdb_handler/utils/monet_get_id.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/mongodb_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/mongodb_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/mongodb_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15045 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/mongodb_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)     6792 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/mongodb_handler/mongodb_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/mongodb_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/mongodb_handler/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/mongodb_handler/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6410 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/mongodb_handler/utils/mongodb_render.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/mssql_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/mssql_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/mssql_handler/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    14543 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/mssql_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)     4621 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/mssql_handler/mssql_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/mssql_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/mssql_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/mssql_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/mssql_handler/tests/test_mssql_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/mysql_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/mysql_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/mysql_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7406 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/mysql_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)     6812 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/mysql_handler/mysql_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/mysql_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/neuralforecast_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/neuralforecast_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/neuralforecast_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6300 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/neuralforecast_handler/neuralforecast_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/neuralforecast_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      781 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/neuralforecast_handler/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/newsapi_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/newsapi_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/newsapi_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2790 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/newsapi_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)     6958 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/newsapi_handler/newsapi_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/newsapi_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/newsapi_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/newsapi_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3201 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/newsapi_handler/tests/test_newsapi_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/nuo_jdbc_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/nuo_jdbc_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      602 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/nuo_jdbc_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    95071 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/nuo_jdbc_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)     9833 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/nuo_jdbc_handler/nuo_jdbc_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/nuo_jdbc_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/nuo_jdbc_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/nuo_jdbc_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/nuo_jdbc_handler/tests/test_nuo_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/oceanbase_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/oceanbase_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/oceanbase_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    37289 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/oceanbase_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/oceanbase_handler/oceanbase_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/oceanbase_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/oceanbase_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/oceanbase_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1741 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/oceanbase_handler/tests/test_oceanbase_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/openai_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/openai_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/openai_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5125 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/openai_handler/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    28123 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/openai_handler/openai_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/openai_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/openai_handler/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/opengauss_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/opengauss_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      590 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/opengauss_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1362 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/opengauss_handler/opengauss_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/opengauss_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/opengauss_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/opengauss_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/opengauss_handler/tests/test_opengauss_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/oracle_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/oracle_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/oracle_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1820 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/oracle_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)     6257 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/oracle_handler/oracle_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/oracle_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/oracle_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/oracle_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/oracle_handler/tests/test_oracle_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/orioledb_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/orioledb_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/orioledb_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8388 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/orioledb_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/orioledb_handler/orioledb_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/orioledb_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/orioledb_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/orioledb_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/orioledb_handler/tests/test_orioledb_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/phoenix_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/phoenix_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/phoenix_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4286 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/phoenix_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)     8767 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/phoenix_handler/phoenix_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/phoenix_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/phoenix_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/phoenix_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/phoenix_handler/tests/test_phoenix_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/pinot_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/pinot_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      602 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/pinot_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18645 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/pinot_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)     8577 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/pinot_handler/pinot_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/pinot_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/pinot_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/pinot_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/pinot_handler/tests/test_pinot_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/plaid_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/plaid_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      492 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/plaid_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/plaid_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)     8076 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/plaid_handler/plaid_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     5151 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/plaid_handler/plaid_tables.py
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/plaid_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/plaid_handler/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/planetscale_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/planetscale_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      621 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/planetscale_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    97032 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/planetscale_handler/create-db.png
--rw-r--r--   0 runner    (1001) docker     (123)    98334 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/planetscale_handler/create-predictor.png
--rw-r--r--   0 runner    (1001) docker     (123)    63619 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/planetscale_handler/drop-db.png
--rw-r--r--   0 runner    (1001) docker     (123)      555 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/planetscale_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/planetscale_handler/planetscale_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)   112840 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/planetscale_handler/predict-target.png
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/planetscale_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/postgres_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/postgres_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/postgres_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15261 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/postgres_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)     5725 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/postgres_handler/postgres_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/postgres_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/questdb_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/questdb_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/questdb_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5301 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/questdb_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/questdb_handler/questdb_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/questdb_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/questdb_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/questdb_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/questdb_handler/tests/test_questdb_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/quickbooks_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/quickbooks_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      512 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/quickbooks_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/quickbooks_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)     3370 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/quickbooks_handler/quickbooks_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    13384 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/quickbooks_handler/quickbooks_table.py
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/quickbooks_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/ray_serve_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/ray_serve_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/ray_serve_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2661 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/ray_serve_handler/ray_serve_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/ray_serve_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/ray_serve_handler/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/reddit_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/reddit_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/reddit_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2434 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/reddit_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)     3234 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/reddit_handler/reddit_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     6558 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/reddit_handler/reddit_tables.py
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/reddit_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/redshift_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/redshift_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      629 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/redshift_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17615 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/redshift_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)     7319 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/redshift_handler/redshift_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/redshift_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/redshift_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/redshift_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/redshift_handler/tests/test_redshift_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/rocket_chat_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/rocket_chat_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/rocket_chat_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1923 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/rocket_chat_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/rocket_chat_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4972 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/rocket_chat_handler/rocket_chat_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     6686 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/rocket_chat_handler/rocket_chat_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3327 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/rocket_chat_handler/rocket_chat_tables.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/rockset_handler/
--rw-r--r--   0 runner    (1001) docker     (123)    22361 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/rockset_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/rockset_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/rockset_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)   194064 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/rockset_handler/tests/test.png
--rw-r--r--   0 runner    (1001) docker     (123)   108141 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/rockset_handler/tests/test2.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/s3_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/s3_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      584 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/s3_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24332 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/s3_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/s3_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     7191 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/s3_handler/s3_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/s3_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/s3_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/s3_handler/tests/test_s3_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/scylla_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/scylla_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      545 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/scylla_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    40148 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/scylla_handler/logo.png
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/scylla_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6429 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/scylla_handler/scylla_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/scylla_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/scylla_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/scylla_handler/tests/test_scylla_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/sendinblue_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/sendinblue_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      523 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/sendinblue_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3458 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/sendinblue_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/sendinblue_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2572 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/sendinblue_handler/sendinblue_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3837 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/sendinblue_handler/sendinblue_tables.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/sheets_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/sheets_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/sheets_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27211 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/sheets_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/sheets_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5770 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/sheets_handler/sheets_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/sheets_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/sheets_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/sheets_handler/tests/test_sheets_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/shopify_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/shopify_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/shopify_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26694 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/shopify_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/shopify_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2701 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/shopify_handler/shopify_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     4156 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/shopify_handler/shopify_tables.py
--rw-r--r--   0 runner    (1001) docker     (123)     3189 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/shopify_handler/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/singlestore_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/singlestore_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/singlestore_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/singlestore_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/singlestore_handler/singlestore_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/singlestore_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/singlestore_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/singlestore_handler/tests/test_singlestore_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/slack_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/slack_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      518 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/slack_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/slack_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/slack_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)    13091 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/slack_handler/slack_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/slack_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/slack_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/slack_handler/tests/test_slack.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/snowflake_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/snowflake_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/snowflake_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/snowflake_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4721 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/snowflake_handler/snowflake_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/snowflake_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/snowflake_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/snowflake_handler/tests/test_snowflake_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/solr_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/solr_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/solr_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/solr_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     8302 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/solr_handler/solr.svg
--rw-r--r--   0 runner    (1001) docker     (123)     6903 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/solr_handler/solr_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/solr_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/solr_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/solr_handler/tests/test_solr_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/sqlany_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/sqlany_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/sqlany_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      715 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/sqlany_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/sqlany_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     7009 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/sqlany_handler/sqlany_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/sqlite_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/sqlite_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/sqlite_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   521282 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/sqlite_handler/db_connection.png
--rw-r--r--   0 runner    (1001) docker     (123)   369371 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/sqlite_handler/error.png
--rw-r--r--   0 runner    (1001) docker     (123)    11559 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/sqlite_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)   479779 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/sqlite_handler/model_drop.png
--rw-r--r--   0 runner    (1001) docker     (123)   477242 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/sqlite_handler/prediction_result.png
--rw-r--r--   0 runner    (1001) docker     (123)   552154 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/sqlite_handler/predictor_model.png
--rw-r--r--   0 runner    (1001) docker     (123)     5974 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/sqlite_handler/sqlite_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/sqlite_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/sqlite_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/sqlite_handler/tests/test_sqlite_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/sqreamdb_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/sqreamdb_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/sqreamdb_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2843 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/sqreamdb_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/sqreamdb_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6273 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/sqreamdb_handler/sqreamdb_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/sqreamdb_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/sqreamdb_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/sqreamdb_handler/tests/test_sqreamdb_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/starrocks_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/starrocks_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/starrocks_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    72778 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/starrocks_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/starrocks_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/starrocks_handler/starrocks_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/starrocks_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/starrocks_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/starrocks_handler/tests/test_starrocks_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/statsforecast_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/statsforecast_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/statsforecast_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/statsforecast_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      781 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/statsforecast_handler/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)     7584 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/statsforecast_handler/statsforecast_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/strava_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/strava_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      686 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/strava_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3662 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/strava_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/strava_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3456 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/strava_handler/strava_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     8211 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/strava_handler/strava_tables.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/supabase_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/supabase_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/supabase_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/supabase_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/supabase_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/supabase_handler/supabase_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/supabase_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/supabase_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/supabase_handler/tests/test_supabase_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/surrealdb_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/surrealdb_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/surrealdb_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25475 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/surrealdb_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/surrealdb_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     7116 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/surrealdb_handler/surrealdb_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/surrealdb_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/surrealdb_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1904 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/surrealdb_handler/tests/test_surrealdb_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/surrealdb_handler/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/surrealdb_handler/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      512 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/surrealdb_handler/utils/surreal_get_info.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/tdengine_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/tdengine_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/tdengine_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3770 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/tdengine_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/tdengine_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5356 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/tdengine_handler/tdengine_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/tdengine_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/tdengine_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1577 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/tdengine_handler/tests/test_tdengine_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/teradata_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/teradata_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/teradata_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3924 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/teradata_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/teradata_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     8261 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/teradata_handler/teradata_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/tidb_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/tidb_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      570 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/tidb_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/tidb_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/tidb_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/tidb_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1334 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/tidb_handler/tests/test_tidb_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/tidb_handler/tidb_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/timescaledb_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/timescaledb_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/timescaledb_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11184 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/timescaledb_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/timescaledb_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/timescaledb_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/timescaledb_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1565 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/timescaledb_handler/tests/test_timescaledb_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/timescaledb_handler/timescaledb_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:34.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/tpot_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/tpot_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/tpot_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/tpot_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      738 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/tpot_handler/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/tpot_handler/tpot_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:35.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/trino_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/trino_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      457 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/trino_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13752 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/trino_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/trino_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:35.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/trino_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/trino_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1630 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/trino_handler/tests/test_trino_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/trino_handler/trino_config_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     6788 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/trino_handler/trino_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:35.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/twitter_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/twitter_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      500 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/twitter_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      732 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/twitter_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/twitter_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)    16126 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/twitter_handler/twitter_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:35.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/vertica_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/vertica_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/vertica_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/vertica_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/vertica_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:35.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/vertica_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/vertica_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1676 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/vertica_handler/tests/test_vertica_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     6014 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/vertica_handler/vertica_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:35.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/vitess_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/vitess_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      481 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/vitess_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4744 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/vitess_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/vitess_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:35.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/vitess_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/vitess_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1727 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/vitess_handler/tests/test_vitess_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/vitess_handler/vitess_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:35.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/youtube_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      351 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/youtube_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      692 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/youtube_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6833 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/youtube_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/youtube_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2962 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/youtube_handler/youtube_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     5433 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/youtube_handler/youtube_tables.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:35.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/yugabyte_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/yugabyte_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/yugabyte_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16563 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/yugabyte_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/yugabyte_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:35.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/yugabyte_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/yugabyte_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/yugabyte_handler/tests/test_yugabyte_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     5943 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers/yugabyte_handler/yugabyte_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:35.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers_client/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers_client/db_client_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     5264 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers_client/db_grpc_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers_client/ml_client_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     4043 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers_client/ml_grpc_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:35.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers_wrapper/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers_wrapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7894 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers_wrapper/db_grpc_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)      627 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers_wrapper/db_handler_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     6071 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers_wrapper/ml_grpc_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/handlers_wrapper/ml_handler_service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:35.000000 MindsDB-23.5.4.1/mindsdb/integrations/libs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/libs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6478 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/libs/api_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     7147 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/libs/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/libs/const.py
--rw-r--r--   0 runner    (1001) docker     (123)     2328 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/libs/handler_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    18262 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/libs/ml_exec_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6468 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/libs/ml_handler_proc.py
--rw-r--r--   0 runner    (1001) docker     (123)      966 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/libs/net_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2792 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/libs/response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3512 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/libs/storage_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:35.000000 MindsDB-23.5.4.1/mindsdb/integrations/utilities/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2032 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/utilities/date_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      929 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/utilities/install.py
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/utilities/processes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/utilities/sql_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/utilities/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6300 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/utilities/time_series_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      449 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/integrations/utilities/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:35.000000 MindsDB-23.5.4.1/mindsdb/interfaces/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/interfaces/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:35.000000 MindsDB-23.5.4.1/mindsdb/interfaces/database/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/interfaces/database/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2901 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/interfaces/database/database.py
--rw-r--r--   0 runner    (1001) docker     (123)    23057 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/interfaces/database/integrations.py
--rw-r--r--   0 runner    (1001) docker     (123)     9792 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/interfaces/database/projects.py
--rw-r--r--   0 runner    (1001) docker     (123)     3370 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/interfaces/database/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:35.000000 MindsDB-23.5.4.1/mindsdb/interfaces/file/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/interfaces/file/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4417 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/interfaces/file/file_controller.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:35.000000 MindsDB-23.5.4.1/mindsdb/interfaces/jobs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/interfaces/jobs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13068 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/interfaces/jobs/jobs_controller.py
--rw-r--r--   0 runner    (1001) docker     (123)     3446 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/interfaces/jobs/scheduler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:35.000000 MindsDB-23.5.4.1/mindsdb/interfaces/model/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/interfaces/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4495 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/interfaces/model/functions.py
--rw-r--r--   0 runner    (1001) docker     (123)    22507 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/interfaces/model/model_controller.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:35.000000 MindsDB-23.5.4.1/mindsdb/interfaces/storage/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/interfaces/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9337 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/interfaces/storage/db.py
--rw-r--r--   0 runner    (1001) docker     (123)    10434 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/interfaces/storage/fs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2353 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/interfaces/storage/json.py
--rw-r--r--   0 runner    (1001) docker     (123)     4446 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/interfaces/storage/model_fs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:35.000000 MindsDB-23.5.4.1/mindsdb/interfaces/stream/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/interfaces/stream/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:35.000000 MindsDB-23.5.4.1/mindsdb/interfaces/stream/base/
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/interfaces/stream/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6057 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/interfaces/stream/base/integration.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:35.000000 MindsDB-23.5.4.1/mindsdb/interfaces/stream/kafka/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/interfaces/stream/kafka/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2658 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/interfaces/stream/kafka/kafkadb.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:35.000000 MindsDB-23.5.4.1/mindsdb/interfaces/stream/redis/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/interfaces/stream/redis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2357 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/interfaces/stream/redis/redisdb.py
--rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/interfaces/stream/stream.py
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/interfaces/stream/utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:35.000000 MindsDB-23.5.4.1/mindsdb/microservices_grpc/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/microservices_grpc/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:35.000000 MindsDB-23.5.4.1/mindsdb/microservices_grpc/db/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/microservices_grpc/db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/microservices_grpc/db/common_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/microservices_grpc/db/common_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/microservices_grpc/db/db_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    12845 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/microservices_grpc/db/db_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:35.000000 MindsDB-23.5.4.1/mindsdb/microservices_grpc/executor/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/microservices_grpc/executor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3565 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/microservices_grpc/executor/executor_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    14810 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/microservices_grpc/executor/executor_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:35.000000 MindsDB-23.5.4.1/mindsdb/microservices_grpc/ml/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/microservices_grpc/ml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/microservices_grpc/ml/common_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/microservices_grpc/ml/common_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2170 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/microservices_grpc/ml/ml_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     5430 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/microservices_grpc/ml/ml_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:35.000000 MindsDB-23.5.4.1/mindsdb/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2695 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/migrations/alembic.ini
--rw-r--r--   0 runner    (1001) docker     (123)     2427 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/migrations/env.py
--rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/migrations/migrate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:35.000000 MindsDB-23.5.4.1/mindsdb/migrations/versions/
--rw-r--r--   0 runner    (1001) docker     (123)     5750 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/migrations/versions/2021-11-30_17c3d2384711_init.py
--rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/migrations/versions/2022-01-26_47f97b83cee4_views.py
--rw-r--r--   0 runner    (1001) docker     (123)    10808 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/migrations/versions/2022-02-09_27c5aca9e47e_db_files.py
--rw-r--r--   0 runner    (1001) docker     (123)     6163 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/migrations/versions/2022-05-25_d74c189b87e6_predictor_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)     2773 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/migrations/versions/2022-07-08_999bceb904df_integration_args.py
--rw-r--r--   0 runner    (1001) docker     (123)      849 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/migrations/versions/2022-07-15_b5b53e0ea7f8_training_data_rows_columns_count.py
--rw-r--r--   0 runner    (1001) docker     (123)      998 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/migrations/versions/2022-07-22_6e834843e7e9_training_time.py
--rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/migrations/versions/2022-08-19_976f15a37e6a_predictors_versioning.py
--rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/migrations/versions/2022-08-25_6a54ba55872e_view_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/migrations/versions/2022-08-29_473e8f239481_straighten.py
--rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/migrations/versions/2022-09-06_96d5fef10caa_data_integration_id.py
--rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/migrations/versions/2022-09-08_87b2df2b83e1_predictor_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     1789 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/migrations/versions/2022-09-19_3d5e70105df7_content_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     2366 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/migrations/versions/2022-09-29_cada7d2be947_json_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     3467 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/migrations/versions/2022-10-14_43c52d23845a_projects.py
--rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/migrations/versions/2022-11-07_1e60096fc817_predictor_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     3463 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/migrations/versions/2022-11-11_d429095b570f_data_integration_id.py
--rw-r--r--   0 runner    (1001) docker     (123)      799 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/migrations/versions/2022-12-26_459218b0844c_fix_unique_constraint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/migrations/versions/2023-02-02_b6d0a47294ac_jobs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/migrations/versions/2023-02-17_ee63d868fa84_predictor_integration_null.py
--rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/migrations/versions/2023-02-25_3154382dab17_training_progress.py
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/migrations/versions/2023-02-27_ef04cdbe51ed_jobs_user_class.py
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/migrations/versions/2023-04-11_b8be148dbc85_jobs_history_query.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/migrations/versions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:35.000000 MindsDB-23.5.4.1/mindsdb/utilities/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2336 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/utilities/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     6805 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/utilities/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     5775 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/utilities/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/utilities/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     4064 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/utilities/fs.py
--rw-r--r--   0 runner    (1001) docker     (123)     5046 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/utilities/functions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:35.000000 MindsDB-23.5.4.1/mindsdb/utilities/hooks/
--rw-r--r--   0 runner    (1001) docker     (123)      432 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/utilities/hooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/utilities/hooks/profiling.py
--rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/utilities/json_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     5002 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/utilities/log.py
--rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/utilities/log_controller.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:12:35.000000 MindsDB-23.5.4.1/mindsdb/utilities/profiler/
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/utilities/profiler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3665 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/utilities/profiler/profiler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2339 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/utilities/ps.py
--rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/utilities/telemetry.py
--rw-r--r--   0 runner    (1001) docker     (123)     1708 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/mindsdb/utilities/wizards.py
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      799 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-23 09:12:35.000000 MindsDB-23.5.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-05-23 09:12:22.000000 MindsDB-23.5.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:54:03.000000 MindsDB-23.6.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/MANIFEST.in
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:54:02.000000 MindsDB-23.6.1.1/MindsDB.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    25700 2023-06-08 22:54:01.000000 MindsDB-23.6.1.1/MindsDB.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    65137 2023-06-08 22:54:02.000000 MindsDB-23.6.1.1/MindsDB.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 22:54:01.000000 MindsDB-23.6.1.1/MindsDB.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     9125 2023-06-08 22:54:01.000000 MindsDB-23.6.1.1/MindsDB.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-08 22:54:01.000000 MindsDB-23.6.1.1/MindsDB.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    25700 2023-06-08 22:54:03.000000 MindsDB-23.6.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    20672 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:54:02.000000 MindsDB-23.6.1.1/mindsdb/
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13249 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:54:02.000000 MindsDB-23.6.1.1/mindsdb/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:54:02.000000 MindsDB-23.6.1.1/mindsdb/api/common/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/api/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/api/common/check_auth.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:54:02.000000 MindsDB-23.6.1.1/mindsdb/api/http/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/api/http/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3090 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/api/http/gui.py
+-rw-r--r--   0 runner    (1001) docker     (123)      534 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/api/http/gunicorn_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12885 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/api/http/initialize.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:54:02.000000 MindsDB-23.6.1.1/mindsdb/api/http/namespaces/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/api/http/namespaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2954 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/api/http/namespaces/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5466 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/api/http/namespaces/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7659 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/api/http/namespaces/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:54:02.000000 MindsDB-23.6.1.1/mindsdb/api/http/namespaces/configs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/api/http/namespaces/configs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/api/http/namespaces/configs/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/api/http/namespaces/configs/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/api/http/namespaces/configs/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/api/http/namespaces/configs/databases.py
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/api/http/namespaces/configs/default.py
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/api/http/namespaces/configs/files.py
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/api/http/namespaces/configs/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/api/http/namespaces/configs/projects.py
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/api/http/namespaces/configs/sql.py
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/api/http/namespaces/configs/tabs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/api/http/namespaces/configs/tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/api/http/namespaces/configs/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10355 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/api/http/namespaces/databases.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4516 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/api/http/namespaces/default.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5627 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/api/http/namespaces/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4781 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/api/http/namespaces/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10197 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/api/http/namespaces/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/api/http/namespaces/projects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4867 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/api/http/namespaces/sql.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1551 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/api/http/namespaces/tab.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2866 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/api/http/namespaces/tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2919 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/api/http/namespaces/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5393 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/api/http/namespaces/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/api/http/start.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/api/http/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:54:02.000000 MindsDB-23.6.1.1/mindsdb/api/mongo/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/api/mongo/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:54:02.000000 MindsDB-23.6.1.1/mindsdb/api/mongo/classes/
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/api/mongo/classes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/api/mongo/classes/query_sql.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/api/mongo/classes/responder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/api/mongo/classes/responder_collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3217 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/api/mongo/classes/scram.py
+-rw-r--r--   0 runner    (1001) docker     (123)      812 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/api/mongo/classes/session.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:54:02.000000 MindsDB-23.6.1.1/mindsdb/api/mongo/functions/
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/api/mongo/functions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:54:02.000000 MindsDB-23.6.1.1/mindsdb/api/mongo/responders/
+-rw-r--r--   0 runner    (1001) docker     (123)     2655 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/api/mongo/responders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/api/mongo/responders/add_shard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2364 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/api/mongo/responders/aggregate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/api/mongo/responders/buildinfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1767 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/api/mongo/responders/coll_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/api/mongo/responders/company_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/api/mongo/responders/connection_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/api/mongo/responders/count.py
+-rw-r--r--   0 runner    (1001) docker     (123)      825 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/api/mongo/responders/db_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4221 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/api/mongo/responders/delete.py
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/api/mongo/responders/end_sessions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5601 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/api/mongo/responders/find.py
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/api/mongo/responders/get_cmd_line_opts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/api/mongo/responders/get_free_monitoring_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/api/mongo/responders/get_parameter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/api/mongo/responders/getlog.py
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/api/mongo/responders/host_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9502 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/api/mongo/responders/insert.py
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/api/mongo/responders/is_master.py
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/api/mongo/responders/is_master_lower.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1536 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/api/mongo/responders/list_collections.py
+-rw-r--r--   0 runner    (1001) docker     (123)      920 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/api/mongo/responders/list_databases.py
+-rw-r--r--   0 runner    (1001) docker     (123)      538 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/api/mongo/responders/list_indexes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/api/mongo/responders/ping.py
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/api/mongo/responders/recv_chunk_start.py
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/api/mongo/responders/replsetgetstatus.py
+-rw-r--r--   0 runner    (1001) docker     (123)      890 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/api/mongo/responders/sasl_continue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/api/mongo/responders/sasl_start.py
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/api/mongo/responders/update_range_deletions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/api/mongo/responders/whatsmyuri.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14041 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/api/mongo/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/api/mongo/start.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:54:02.000000 MindsDB-23.6.1.1/mindsdb/api/mongo/utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/api/mongo/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/api/mongo/utilities/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7666 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/api/mongo/utilities/mongodb_ast.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4166 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/api/mongo/utilities/mongodb_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2160 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/api/mongo/utilities/mongodb_query.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:54:02.000000 MindsDB-23.6.1.1/mindsdb/api/mysql/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/api/mysql/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:54:02.000000 MindsDB-23.6.1.1/mindsdb/api/mysql/mysql_proxy/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/api/mysql/mysql_proxy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:54:02.000000 MindsDB-23.6.1.1/mindsdb/api/mysql/mysql_proxy/classes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/api/mysql/mysql_proxy/classes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3358 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/api/mysql/mysql_proxy/classes/client_capabilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/api/mysql/mysql_proxy/classes/com_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:54:02.000000 MindsDB-23.6.1.1/mindsdb/api/mysql/mysql_proxy/classes/fake_mysql_proxy/
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/api/mysql/mysql_proxy/classes/fake_mysql_proxy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      914 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/api/mysql/mysql_proxy/classes/fake_mysql_proxy/fake_mysql_proxy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/api/mysql/mysql_proxy/classes/server_capabilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56525 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/api/mysql/mysql_proxy/classes/sql_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4436 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/api/mysql/mysql_proxy/classes/sql_statement_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:54:02.000000 MindsDB-23.6.1.1/mindsdb/api/mysql/mysql_proxy/controllers/
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/api/mysql/mysql_proxy/controllers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3914 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/api/mysql/mysql_proxy/controllers/session_controller.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:54:02.000000 MindsDB-23.6.1.1/mindsdb/api/mysql/mysql_proxy/data_types/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/api/mysql/mysql_proxy/data_types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5834 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/api/mysql/mysql_proxy/data_types/mysql_datum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4839 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:54:02.000000 MindsDB-23.6.1.1/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/
+-rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4620 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/binary_resultset_row_package.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/column_count_packet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2982 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/column_definition_packet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5765 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/command_packet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1428 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/eof_packet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1520 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/err_packet.py
+-rw-r--r--   0 runner    (1001) docker     (123)      486 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/fast_auth_fail_packet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2927 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/handshake_packet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3770 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/handshake_response_packet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3785 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/ok_packet.py
+-rw-r--r--   0 runner    (1001) docker     (123)      421 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/password_answer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/resultset_row_package.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/stmt_prepare_header.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/switch_auth_packet.py
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/switch_auth_response_packet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:54:02.000000 MindsDB-23.6.1.1/mindsdb/api/mysql/mysql_proxy/datahub/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/api/mysql/mysql_proxy/datahub/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:54:02.000000 MindsDB-23.6.1.1/mindsdb/api/mysql/mysql_proxy/datahub/classes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/api/mysql/mysql_proxy/datahub/classes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2786 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/api/mysql/mysql_proxy/datahub/classes/tables_row.py
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/api/mysql/mysql_proxy/datahub/datahub.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:54:02.000000 MindsDB-23.6.1.1/mindsdb/api/mysql/mysql_proxy/datahub/datanodes/
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/api/mysql/mysql_proxy/datahub/datanodes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/api/mysql/mysql_proxy/datahub/datanodes/datanode.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23207 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/api/mysql/mysql_proxy/datahub/datanodes/information_schema_datanode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6121 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/api/mysql/mysql_proxy/datahub/datanodes/integration_datanode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4087 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/api/mysql/mysql_proxy/datahub/datanodes/project_datanode.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:54:02.000000 MindsDB-23.6.1.1/mindsdb/api/mysql/mysql_proxy/executor/
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/api/mysql/mysql_proxy/executor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/api/mysql/mysql_proxy/executor/data_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7054 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/api/mysql/mysql_proxy/executor/executor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/api/mysql/mysql_proxy/executor/executor_client_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68681 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/api/mysql/mysql_proxy/executor/executor_commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5155 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/api/mysql/mysql_proxy/executor/executor_grpc_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9125 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/api/mysql/mysql_proxy/executor/executor_grpc_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/api/mysql/mysql_proxy/executor/executor_service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:54:02.000000 MindsDB-23.6.1.1/mindsdb/api/mysql/mysql_proxy/external_libs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/api/mysql/mysql_proxy/external_libs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4116 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/api/mysql/mysql_proxy/external_libs/mysql_scramble.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:54:02.000000 MindsDB-23.6.1.1/mindsdb/api/mysql/mysql_proxy/libs/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/api/mysql/mysql_proxy/libs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:54:02.000000 MindsDB-23.6.1.1/mindsdb/api/mysql/mysql_proxy/libs/constants/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/api/mysql/mysql_proxy/libs/constants/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35316 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/api/mysql/mysql_proxy/libs/constants/mysql.py
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/api/mysql/mysql_proxy/libs/constants/response_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31908 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/api/mysql/mysql_proxy/mysql_proxy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:54:02.000000 MindsDB-23.6.1.1/mindsdb/api/mysql/mysql_proxy/utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/api/mysql/mysql_proxy/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/api/mysql/mysql_proxy/utilities/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      973 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/api/mysql/mysql_proxy/utilities/functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2341 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/api/mysql/mysql_proxy/utilities/lightwood_dtype.py
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/api/mysql/mysql_proxy/utilities/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3070 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/api/mysql/mysql_proxy/utilities/sql.py
+-rw-r--r--   0 runner    (1001) docker     (123)      422 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/api/mysql/start.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:54:02.000000 MindsDB-23.6.1.1/mindsdb/api/nlp/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/api/nlp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/api/nlp/nlp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:54:02.000000 MindsDB-23.6.1.1/mindsdb/api/postgres/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/api/postgres/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:54:02.000000 MindsDB-23.6.1.1/mindsdb/api/postgres/postgres_proxy/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/api/postgres/postgres_proxy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:54:02.000000 MindsDB-23.6.1.1/mindsdb/api/postgres/postgres_proxy/executor/
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/api/postgres/postgres_proxy/executor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6543 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/api/postgres/postgres_proxy/executor/executor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:54:02.000000 MindsDB-23.6.1.1/mindsdb/api/postgres/postgres_proxy/postgres_packets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/api/postgres/postgres_proxy/postgres_packets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12729 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/api/postgres/postgres_proxy/postgres_packets/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/api/postgres/postgres_proxy/postgres_packets/postgres_fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/api/postgres/postgres_proxy/postgres_packets/postgres_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40804 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/api/postgres/postgres_proxy/postgres_packets/postgres_message_formats.py
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/api/postgres/postgres_proxy/postgres_packets/postgres_message_identifiers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8434 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/api/postgres/postgres_proxy/postgres_packets/postgres_packets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19291 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/api/postgres/postgres_proxy/postgres_proxy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:54:02.000000 MindsDB-23.6.1.1/mindsdb/api/postgres/postgres_proxy/utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/api/postgres/postgres_proxy/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/api/postgres/start.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:54:02.000000 MindsDB-23.6.1.1/mindsdb/integrations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:54:02.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:54:02.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/access_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/access_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      633 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/access_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6362 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/access_handler/access_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32145 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/access_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/access_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:54:02.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/access_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/access_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/access_handler/tests/test_access_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:54:02.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/airtable_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/airtable_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/airtable_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6808 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/airtable_handler/airtable_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4911 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/airtable_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/airtable_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:54:02.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/airtable_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/airtable_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/airtable_handler/tests/test_airtable_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:54:02.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/altibase_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/altibase_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/altibase_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8296 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/altibase_handler/altibase_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)   342129 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/altibase_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/altibase_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:54:02.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/altibase_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/altibase_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/altibase_handler/tests/test_altibase_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:54:02.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/aurora_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/aurora_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/aurora_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6404 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/aurora_handler/aurora_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11767 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/aurora_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/aurora_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:54:02.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/aurora_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/aurora_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/aurora_handler/tests/test_aurora_mysql_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/aurora_handler/tests/test_aurora_postgres_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:54:02.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/autokeras_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/autokeras_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/autokeras_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5616 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/autokeras_handler/autokeras_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/autokeras_handler/functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/autokeras_handler/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:54:02.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/autosklearn_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/autosklearn_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/autosklearn_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1685 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/autosklearn_handler/autosklearn_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      710 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/autosklearn_handler/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/autosklearn_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      745 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/autosklearn_handler/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:54:02.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/bigquery_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/bigquery_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/bigquery_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5974 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/bigquery_handler/bigquery_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/bigquery_handler/logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/bigquery_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:54:02.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/bigquery_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/bigquery_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      941 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/bigquery_handler/tests/test_bigquery_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:54:02.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/binance_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/binance_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/binance_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5238 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/binance_handler/binance_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7458 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/binance_handler/binance_tables.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/binance_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/binance_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:54:02.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/byom_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/byom_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/byom_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6723 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/byom_handler/byom_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3469 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/byom_handler/proc_wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:54:02.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/cassandra_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/cassandra_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/cassandra_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/cassandra_handler/cassandra_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)   176707 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/cassandra_handler/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/cassandra_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:54:02.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/cassandra_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/cassandra_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/cassandra_handler/tests/test_cassandra_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:54:02.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/ckan_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/ckan_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/ckan_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3485 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/ckan_handler/ckan_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17688 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/ckan_handler/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/ckan_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:54:02.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/ckan_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/ckan_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      820 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/ckan_handler/tests/test_ckan_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:54:02.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/clickhouse_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/clickhouse_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/clickhouse_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6531 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/clickhouse_handler/clickhouse_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/clickhouse_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:54:02.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/clickhouse_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/clickhouse_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1458 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/clickhouse_handler/tests/test_clickhouse_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:54:02.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/cloud_spanner_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/cloud_spanner_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      662 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/cloud_spanner_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6308 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/cloud_spanner_handler/cloud_spanner_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6419 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/cloud_spanner_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/cloud_spanner_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:54:02.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/cloud_spanner_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/cloud_spanner_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/cloud_spanner_handler/tests/test_cloud_spanner_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:54:02.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/cloud_sql_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/cloud_sql_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/cloud_sql_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5153 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/cloud_sql_handler/cloud_sql_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37571 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/cloud_sql_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/cloud_sql_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:54:02.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/cloud_sql_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/cloud_sql_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/cloud_sql_handler/tests/test_cloud_sql_mssql_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/cloud_sql_handler/tests/test_cloud_sql_mysql_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:54:02.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/cockroach_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/cockroach_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/cockroach_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/cockroach_handler/cockroach_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/cockroach_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:54:02.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/cockroach_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/cockroach_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/cockroach_handler/tests/test_cockroachdb_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:54:02.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/cohere_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/cohere_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/cohere_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4099 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/cohere_handler/cohere_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/cohere_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/cohere_handler/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:54:02.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/confluence_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/confluence_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      710 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/confluence_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2743 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/confluence_handler/confluence_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4301 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/confluence_handler/confluence_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)    76194 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/confluence_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/confluence_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:54:02.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/couchbase_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/couchbase_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/couchbase_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9347 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/couchbase_handler/couchbase_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3371 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/couchbase_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/couchbase_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:54:02.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/couchbase_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/couchbase_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1233 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/couchbase_handler/tests/test_couchbase_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:54:02.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/crate_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/crate_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/crate_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7157 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/crate_handler/crate_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2999 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/crate_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/crate_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:54:02.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/crate_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/crate_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/crate_handler/tests/test_crate_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:54:02.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/d0lt_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/d0lt_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/d0lt_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    85600 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/d0lt_handler/create-db.png
+-rw-r--r--   0 runner    (1001) docker     (123)    98275 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/d0lt_handler/create-predictor.png
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/d0lt_handler/d0lt_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1590 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/d0lt_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    98983 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/d0lt_handler/predict-target.png
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/d0lt_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:54:02.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/d0lt_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/d0lt_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/d0lt_handler/tests/test_d0lt_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:54:02.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/databend_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/databend_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/databend_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/databend_handler/databend_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6443 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/databend_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/databend_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:54:02.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/databend_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/databend_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/databend_handler/tests/test_databend_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:54:03.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/databricks_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/databricks_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/databricks_handler/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:54:03.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/databricks_handler/databricks/
+-rw-r--r--   0 runner    (1001) docker     (123)    86110 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/databricks_handler/databricks/createdb.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    58645 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/databricks_handler/databricks/createpred.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    35986 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/databricks_handler/databricks/hivmetastore.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    21694 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/databricks_handler/databricks/mindsdbdatabricks.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    62078 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/databricks_handler/databricks/selectfrom.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)     7952 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/databricks_handler/databricks_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12097 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/databricks_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/databricks_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:54:03.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/databricks_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/databricks_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/databricks_handler/tests/test_databricks_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:54:03.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/datastax_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/datastax_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/datastax_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/datastax_handler/datastax_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26175 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/datastax_handler/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/datastax_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:54:03.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/datastax_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/datastax_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/datastax_handler/tests/test_cassandra_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:54:03.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/db2_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/db2_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/db2_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9099 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/db2_handler/db2_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19117 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/db2_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/db2_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:54:03.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/db2_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/db2_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/db2_handler/tests/test_db2_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:54:03.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/derby_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/derby_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/derby_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8751 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/derby_handler/derby_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7305 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/derby_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/derby_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:54:03.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/derby_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/derby_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/derby_handler/tests/test_derby_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:54:03.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/dremio_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/dremio_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/dremio_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7311 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/dremio_handler/dremio_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52734 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/dremio_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/dremio_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:54:03.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/dremio_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/dremio_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/dremio_handler/tests/test_dremio_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:54:03.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/druid_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/druid_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/druid_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7324 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/druid_handler/druid_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29112 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/druid_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/druid_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:54:03.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/druid_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/druid_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/druid_handler/tests/test_druid_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:54:03.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/duckdb_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/duckdb_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      635 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/duckdb_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5486 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/duckdb_handler/duckdb_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19548 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/duckdb_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/duckdb_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:54:03.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/duckdb_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/duckdb_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/duckdb_handler/tests/test_duckdb_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:54:03.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/dynamodb_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/dynamodb_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/dynamodb_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6592 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/dynamodb_handler/dynamodb_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55623 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/dynamodb_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/dynamodb_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:54:03.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/dynamodb_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/dynamodb_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/dynamodb_handler/tests/test_dynamodb_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:54:03.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/edgelessdb_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/edgelessdb_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/edgelessdb_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1871 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/edgelessdb_handler/edgelessdb_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8768 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/edgelessdb_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/edgelessdb_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:54:03.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/edgelessdb_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/edgelessdb_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/edgelessdb_handler/tests/test_edgelessdb_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:54:03.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/elasticsearch_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/elasticsearch_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/elasticsearch_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7624 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/elasticsearch_handler/elasticsearch_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4749 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/elasticsearch_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/elasticsearch_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:54:03.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/elasticsearch_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/elasticsearch_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/elasticsearch_handler/tests/test_elasticsearch_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:54:03.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/empress_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/empress_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/empress_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7713 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/empress_handler/empress_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11249 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/empress_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/empress_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:54:03.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/empress_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/empress_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/empress_handler/tests/test_empress_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:54:03.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/eventstoredb_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/eventstoredb_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/eventstoredb_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9062 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/eventstoredb_handler/eventstoredb_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6031 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/eventstoredb_handler/icon.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:54:03.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/file_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/file_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/file_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10883 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/file_handler/file_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:54:03.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/firebird_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/firebird_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/firebird_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9566 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/firebird_handler/firebird_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54033 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/firebird_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/firebird_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:54:03.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/firebird_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/firebird_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/firebird_handler/tests/test_firebird_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:54:03.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/flaml_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/flaml_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/flaml_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1619 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/flaml_handler/flaml_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/flaml_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/flaml_handler/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:54:03.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/frappe_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/frappe_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      480 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/frappe_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4250 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/frappe_handler/frappe_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7570 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/frappe_handler/frappe_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2648 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/frappe_handler/frappe_tables.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/frappe_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/frappe_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:54:03.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/github_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/github_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/github_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3165 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/github_handler/github_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21392 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/github_handler/github_tables.py
+-rw-r--r--   0 runner    (1001) docker     (123)      963 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/github_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/github_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:54:03.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/gitlab_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/gitlab_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/gitlab_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2611 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/gitlab_handler/gitlab_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15343 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/gitlab_handler/gitlab_tables.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2075 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/gitlab_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/gitlab_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:54:03.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/gmail_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/gmail_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/gmail_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15215 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/gmail_handler/gmail_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/gmail_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/gmail_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:54:03.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/gmail_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/gmail_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/gmail_handler/tests/test_gmail_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:54:03.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/google_books_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/google_books_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/google_books_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6885 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/google_books_handler/google_books_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6268 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/google_books_handler/google_books_tables.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/google_books_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/google_books_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:54:03.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/google_books_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/google_books_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/google_books_handler/tests/test_google_books_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:54:03.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/google_calendar_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/google_calendar_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      516 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/google_calendar_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10399 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/google_calendar_handler/google_calendar_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8111 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/google_calendar_handler/google_calendar_tables.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/google_calendar_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/google_calendar_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:54:03.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/google_calendar_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/google_calendar_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2228 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/google_calendar_handler/tests/test_google_calendar_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:54:03.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/google_content_shopping_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/google_content_shopping_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      663 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/google_content_shopping_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16251 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/google_content_shopping_handler/google_content_shopping_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14279 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/google_content_shopping_handler/google_content_shopping_tables.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34337 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/google_content_shopping_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/google_content_shopping_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:54:03.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/google_content_shopping_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/google_content_shopping_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2449 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/google_content_shopping_handler/tests/test_google_content_shopping_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:54:03.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/google_fit_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/google_fit_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/google_fit_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6599 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/google_fit_handler/google_fit_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2496 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/google_fit_handler/google_fit_tables.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21355 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/google_fit_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/google_fit_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:54:03.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/google_search_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/google_search_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/google_search_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8170 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/google_search_handler/google_search_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7375 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/google_search_handler/google_search_tables.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8618 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/google_search_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/google_search_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:54:03.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/google_search_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/google_search_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2191 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/google_search_handler/tests/test_google_search_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:54:03.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/hackernews_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/hackernews_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/hackernews_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3044 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/hackernews_handler/hn_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5425 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/hackernews_handler/hn_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/hackernews_handler/icon.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:54:03.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/hana_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/hana_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/hana_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11104 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/hana_handler/hana_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      715 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/hana_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/hana_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:54:03.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/hive_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/hive_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/hive_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5947 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/hive_handler/hive_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14000 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/hive_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/hive_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:54:03.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/hive_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/hive_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/hive_handler/tests/test_hive_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:54:03.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/hsqldb_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/hsqldb_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/hsqldb_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7491 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/hsqldb_handler/hsqldb_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5355 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/hsqldb_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/hsqldb_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:54:03.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/huggingface_api_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/huggingface_api_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      549 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/huggingface_api_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6425 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/huggingface_api_handler/huggingface_api_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/huggingface_api_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/huggingface_api_handler/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:54:03.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/huggingface_api_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/huggingface_api_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/huggingface_api_handler/tests/test_huggingface_api_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:54:03.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/huggingface_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/huggingface_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/huggingface_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10766 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/huggingface_handler/huggingface_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/huggingface_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/huggingface_handler/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:54:03.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/ignite_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/ignite_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/ignite_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45779 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/ignite_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7181 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/ignite_handler/ignite_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/ignite_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:54:03.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/ignite_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/ignite_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/ignite_handler/tests/test_ignite_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:54:03.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/impala_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/impala_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/impala_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2542 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/impala_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     5640 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/impala_handler/impala_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/impala_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:54:03.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/impala_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/impala_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/impala_handler/tests/test_impala_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:54:03.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/influxdb_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/influxdb_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/influxdb_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    63375 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/influxdb_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3359 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/influxdb_handler/influxdb_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3281 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/influxdb_handler/influxdb_tables.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/influxdb_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:54:03.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/informix_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/informix_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/informix_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6694 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/informix_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)     9618 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/informix_handler/informix_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/informix_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:54:03.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/informix_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/informix_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/informix_handler/tests/test_informix_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:54:03.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/ingres_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/ingres_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/ingres_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3932 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/ingres_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     7581 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/ingres_handler/ingres_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/ingres_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:54:03.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/ingres_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/ingres_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/ingres_handler/tests/test_ingres_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:54:03.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/jira_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/jira_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      565 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/jira_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16812 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/jira_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3244 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/jira_handler/jira_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5493 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/jira_handler/jira_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/jira_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:54:03.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/langchain_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/langchain_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/langchain_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21871 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/langchain_handler/langchain_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6680 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/langchain_handler/mindsdb_database_agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/langchain_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/langchain_handler/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:54:03.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/lightwood_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/lightwood_handler/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:54:03.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/lightwood_handler/lightwood_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/lightwood_handler/lightwood_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/lightwood_handler/lightwood_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8801 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/lightwood_handler/lightwood_handler/functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20556 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/lightwood_handler/lightwood_handler/lightwood_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2300 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/lightwood_handler/lightwood_handler/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/lightwood_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/lightwood_handler/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:54:03.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/lightwood_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/lightwood_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10985 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/lightwood_handler/tests/test_lightwood_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:54:03.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/llama_index_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/llama_index_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      655 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/llama_index_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6017 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/llama_index_handler/llama_index_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/llama_index_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/llama_index_handler/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:54:03.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/ludwig_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/ludwig_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/ludwig_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/ludwig_handler/functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2395 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/ludwig_handler/ludwig_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/ludwig_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      740 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/ludwig_handler/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/ludwig_handler/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:54:03.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/mariadb_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/mariadb_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/mariadb_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7657 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/mariadb_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/mariadb_handler/mariadb_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/mariadb_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:54:03.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/materialize_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/materialize_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/materialize_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47935 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/materialize_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/materialize_handler/materialize_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/materialize_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:54:03.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/materialize_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/materialize_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1774 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/materialize_handler/tests/test_materialize_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:54:03.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/matrixone_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/matrixone_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/matrixone_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57976 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/matrixone_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)     6870 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/matrixone_handler/matrixone_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/matrixone_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:54:03.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/matrixone_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/matrixone_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1789 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/matrixone_handler/tests/test_matrixone_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:54:03.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/maxdb_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/maxdb_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      635 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/maxdb_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26795 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/maxdb_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7507 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/maxdb_handler/maxdb_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/maxdb_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:54:03.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/maxdb_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/maxdb_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1918 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/maxdb_handler/tests/test_maxdb_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:54:03.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/merlion_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/merlion_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/merlion_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8498 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/merlion_handler/adapters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8217 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/merlion_handler/merlion_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/merlion_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      828 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/merlion_handler/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:54:03.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/mlflow_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/mlflow_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      542 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/mlflow_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3802 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/mlflow_handler/mlflow_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/mlflow_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      740 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/mlflow_handler/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:54:03.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/monetdb_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/monetdb_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/monetdb_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   544421 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/monetdb_handler/create-database.png
+-rw-r--r--   0 runner    (1001) docker     (123)   423554 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/monetdb_handler/create-predictor.png
+-rw-r--r--   0 runner    (1001) docker     (123)    64685 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/monetdb_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)     8118 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/monetdb_handler/monetdb_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/monetdb_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)   445044 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/monetdb_handler/select-predictor.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:54:03.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/monetdb_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/monetdb_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/monetdb_handler/tests/test_monetdb_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:54:03.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/monetdb_handler/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/monetdb_handler/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/monetdb_handler/utils/monet_get_id.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:54:03.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/mongodb_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/mongodb_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/mongodb_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15045 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/mongodb_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     6792 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/mongodb_handler/mongodb_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/mongodb_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:54:03.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/mongodb_handler/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/mongodb_handler/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6410 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/mongodb_handler/utils/mongodb_render.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:54:03.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/monkeylearn_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/monkeylearn_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/monkeylearn_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3297 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/monkeylearn_handler/monkeylearn_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/monkeylearn_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/monkeylearn_handler/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:54:03.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/mssql_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/mssql_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/mssql_handler/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    14543 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/mssql_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4621 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/mssql_handler/mssql_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/mssql_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:54:03.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/mssql_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/mssql_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/mssql_handler/tests/test_mssql_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:54:03.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/mysql_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/mysql_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/mysql_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7406 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/mysql_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     6812 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/mysql_handler/mysql_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/mysql_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:54:03.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/neuralforecast_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/neuralforecast_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/neuralforecast_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6300 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/neuralforecast_handler/neuralforecast_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/neuralforecast_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/neuralforecast_handler/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:54:03.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/newsapi_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/newsapi_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/newsapi_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2790 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/newsapi_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)     6958 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/newsapi_handler/newsapi_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/newsapi_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:54:03.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/newsapi_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/newsapi_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3201 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/newsapi_handler/tests/test_newsapi_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:54:03.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/nuo_jdbc_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/nuo_jdbc_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/nuo_jdbc_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    95071 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/nuo_jdbc_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)     9833 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/nuo_jdbc_handler/nuo_jdbc_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/nuo_jdbc_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:54:03.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/nuo_jdbc_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/nuo_jdbc_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/nuo_jdbc_handler/tests/test_nuo_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:54:03.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/oceanbase_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/oceanbase_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/oceanbase_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37289 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/oceanbase_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/oceanbase_handler/oceanbase_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/oceanbase_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:54:03.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/oceanbase_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/oceanbase_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1741 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/oceanbase_handler/tests/test_oceanbase_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:54:03.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/openai_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/openai_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/openai_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5126 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/openai_handler/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29025 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/openai_handler/openai_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/openai_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/openai_handler/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:54:03.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/opengauss_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/opengauss_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/opengauss_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1362 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/opengauss_handler/opengauss_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/opengauss_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:54:03.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/opengauss_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/opengauss_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/opengauss_handler/tests/test_opengauss_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:54:03.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/oracle_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/oracle_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/oracle_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1820 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/oracle_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     6257 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/oracle_handler/oracle_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/oracle_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:54:03.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/oracle_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/oracle_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/oracle_handler/tests/test_oracle_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:54:03.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/orioledb_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/orioledb_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/orioledb_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8388 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/orioledb_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/orioledb_handler/orioledb_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/orioledb_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:54:03.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/orioledb_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/orioledb_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/orioledb_handler/tests/test_orioledb_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:54:03.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/paypal_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/paypal_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/paypal_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11776 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/paypal_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2527 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/paypal_handler/paypal_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/paypal_handler/paypal_tables.py
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/paypal_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:54:03.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/phoenix_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/phoenix_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/phoenix_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4286 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/phoenix_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)     8767 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/phoenix_handler/phoenix_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/phoenix_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:54:03.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/phoenix_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/phoenix_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/phoenix_handler/tests/test_phoenix_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:54:03.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/pinot_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/pinot_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/pinot_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18645 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/pinot_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)     8577 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/pinot_handler/pinot_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/pinot_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:54:03.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/pinot_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/pinot_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/pinot_handler/tests/test_pinot_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:54:03.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/plaid_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/plaid_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/plaid_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/plaid_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     8076 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/plaid_handler/plaid_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5151 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/plaid_handler/plaid_tables.py
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/plaid_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/plaid_handler/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:54:03.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/planetscale_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/planetscale_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      621 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/planetscale_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    97032 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/planetscale_handler/create-db.png
+-rw-r--r--   0 runner    (1001) docker     (123)    98334 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/planetscale_handler/create-predictor.png
+-rw-r--r--   0 runner    (1001) docker     (123)    63619 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/planetscale_handler/drop-db.png
+-rw-r--r--   0 runner    (1001) docker     (123)      555 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/planetscale_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/planetscale_handler/planetscale_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)   112840 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/planetscale_handler/predict-target.png
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/planetscale_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:54:03.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/postgres_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/postgres_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/postgres_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15261 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/postgres_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     5725 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/postgres_handler/postgres_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/postgres_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:54:03.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/questdb_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/questdb_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/questdb_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5301 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/questdb_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/questdb_handler/questdb_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/questdb_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:54:03.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/questdb_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/questdb_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/questdb_handler/tests/test_questdb_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:54:03.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/quickbooks_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/quickbooks_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      512 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/quickbooks_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/quickbooks_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     3370 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/quickbooks_handler/quickbooks_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13384 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/quickbooks_handler/quickbooks_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/quickbooks_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:54:03.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/ray_serve_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/ray_serve_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/ray_serve_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2661 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/ray_serve_handler/ray_serve_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/ray_serve_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/ray_serve_handler/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:54:03.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/reddit_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/reddit_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/reddit_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2434 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/reddit_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     3234 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/reddit_handler/reddit_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6558 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/reddit_handler/reddit_tables.py
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/reddit_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:54:03.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/redshift_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/redshift_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/redshift_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17615 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/redshift_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7319 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/redshift_handler/redshift_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/redshift_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:54:03.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/redshift_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/redshift_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/redshift_handler/tests/test_redshift_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:54:03.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/rocket_chat_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/rocket_chat_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/rocket_chat_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1923 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/rocket_chat_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/rocket_chat_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5225 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/rocket_chat_handler/rocket_chat_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6187 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/rocket_chat_handler/rocket_chat_tables.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:54:03.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/rockset_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)    22361 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/rockset_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/rockset_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:54:03.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/rockset_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)   194064 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/rockset_handler/tests/test.png
+-rw-r--r--   0 runner    (1001) docker     (123)   108141 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/rockset_handler/tests/test2.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:54:03.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/s3_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/s3_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/s3_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24332 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/s3_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/s3_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7191 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/s3_handler/s3_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:54:03.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/s3_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/s3_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/s3_handler/tests/test_s3_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:54:03.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/scylla_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/scylla_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/scylla_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40148 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/scylla_handler/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/scylla_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6429 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/scylla_handler/scylla_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:54:03.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/scylla_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/scylla_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/scylla_handler/tests/test_scylla_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:54:03.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/sendinblue_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/sendinblue_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/sendinblue_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3458 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/sendinblue_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/sendinblue_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2572 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/sendinblue_handler/sendinblue_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1921 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/sendinblue_handler/sendinblue_tables.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:54:03.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/sheets_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/sheets_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/sheets_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27211 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/sheets_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/sheets_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5770 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/sheets_handler/sheets_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:54:03.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/sheets_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/sheets_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/sheets_handler/tests/test_sheets_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:54:03.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/shopify_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/shopify_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/shopify_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26694 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/shopify_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/shopify_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2701 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/shopify_handler/shopify_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4865 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/shopify_handler/shopify_tables.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:54:03.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/singlestore_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/singlestore_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/singlestore_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/singlestore_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/singlestore_handler/singlestore_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:54:03.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/singlestore_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/singlestore_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/singlestore_handler/tests/test_singlestore_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:54:03.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/slack_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/slack_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      518 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/slack_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/slack_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/slack_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    13091 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/slack_handler/slack_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:54:03.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/slack_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/slack_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/slack_handler/tests/test_slack.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:54:03.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/snowflake_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/snowflake_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/snowflake_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/snowflake_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4721 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/snowflake_handler/snowflake_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:54:03.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/snowflake_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/snowflake_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/snowflake_handler/tests/test_snowflake_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:54:03.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/solr_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/solr_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/solr_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/solr_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     8302 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/solr_handler/solr.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     6903 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/solr_handler/solr_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:54:03.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/solr_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/solr_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/solr_handler/tests/test_solr_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:54:03.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/sqlany_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/sqlany_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/sqlany_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      715 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/sqlany_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/sqlany_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7009 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/sqlany_handler/sqlany_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:54:03.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/sqlite_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/sqlite_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/sqlite_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   521282 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/sqlite_handler/db_connection.png
+-rw-r--r--   0 runner    (1001) docker     (123)   369371 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/sqlite_handler/error.png
+-rw-r--r--   0 runner    (1001) docker     (123)    11559 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/sqlite_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)   479779 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/sqlite_handler/model_drop.png
+-rw-r--r--   0 runner    (1001) docker     (123)   477242 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/sqlite_handler/prediction_result.png
+-rw-r--r--   0 runner    (1001) docker     (123)   552154 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/sqlite_handler/predictor_model.png
+-rw-r--r--   0 runner    (1001) docker     (123)     5974 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/sqlite_handler/sqlite_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:54:03.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/sqlite_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/sqlite_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/sqlite_handler/tests/test_sqlite_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:54:03.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/sqreamdb_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/sqreamdb_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/sqreamdb_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2843 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/sqreamdb_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/sqreamdb_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6273 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/sqreamdb_handler/sqreamdb_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:54:03.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/sqreamdb_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/sqreamdb_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/sqreamdb_handler/tests/test_sqreamdb_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:54:03.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/starrocks_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/starrocks_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/starrocks_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    72778 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/starrocks_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/starrocks_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/starrocks_handler/starrocks_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:54:03.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/starrocks_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/starrocks_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/starrocks_handler/tests/test_starrocks_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:54:03.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/statsforecast_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/statsforecast_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/statsforecast_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/statsforecast_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/statsforecast_handler/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7584 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/statsforecast_handler/statsforecast_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:54:03.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/strava_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/strava_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/strava_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3662 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/strava_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/strava_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3456 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/strava_handler/strava_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8211 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/strava_handler/strava_tables.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:54:03.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/stripe_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/stripe_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/stripe_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58244 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/stripe_handler/icon.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:54:03.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/stripe_handler/query_handlers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/stripe_handler/query_handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5687 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/stripe_handler/query_handlers/select_query_handlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/stripe_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2599 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/stripe_handler/stripe_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4781 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/stripe_handler/stripe_tables.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:54:03.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/supabase_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/supabase_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/supabase_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/supabase_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/supabase_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/supabase_handler/supabase_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:54:03.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/supabase_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/supabase_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/supabase_handler/tests/test_supabase_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:54:03.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/surrealdb_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/surrealdb_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/surrealdb_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25475 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/surrealdb_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/surrealdb_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7116 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/surrealdb_handler/surrealdb_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:54:03.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/surrealdb_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/surrealdb_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1904 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/surrealdb_handler/tests/test_surrealdb_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:54:03.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/surrealdb_handler/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/surrealdb_handler/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      512 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/surrealdb_handler/utils/surreal_get_info.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:54:03.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/tdengine_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/tdengine_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/tdengine_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3770 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/tdengine_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/tdengine_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5356 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/tdengine_handler/tdengine_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:54:03.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/tdengine_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/tdengine_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1577 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/tdengine_handler/tests/test_tdengine_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:54:03.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/teradata_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/teradata_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/teradata_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3924 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/teradata_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/teradata_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     8261 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/teradata_handler/teradata_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:54:03.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/tidb_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/tidb_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      570 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/tidb_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/tidb_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:54:03.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/tidb_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/tidb_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1334 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/tidb_handler/tests/test_tidb_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/tidb_handler/tidb_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:54:03.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/timescaledb_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/timescaledb_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/timescaledb_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11184 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/timescaledb_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/timescaledb_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:54:03.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/timescaledb_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/timescaledb_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1565 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/timescaledb_handler/tests/test_timescaledb_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/timescaledb_handler/timescaledb_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:54:03.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/tpot_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/tpot_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/tpot_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/tpot_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/tpot_handler/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3341 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/tpot_handler/tpot_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:54:03.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/trino_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/trino_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/trino_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13752 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/trino_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/trino_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:54:03.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/trino_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/trino_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1630 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/trino_handler/tests/test_trino_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/trino_handler/trino_config_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6788 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/trino_handler/trino_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:54:03.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/twitter_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/twitter_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/twitter_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      732 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/twitter_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/twitter_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    16126 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/twitter_handler/twitter_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:54:03.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/utilities/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:54:03.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/utilities/query_utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/utilities/query_utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5687 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/utilities/query_utilities/select_query_utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:54:03.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/vertica_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/vertica_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/vertica_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/vertica_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/vertica_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:54:03.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/vertica_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/vertica_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1676 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/vertica_handler/tests/test_vertica_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6014 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/vertica_handler/vertica_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:54:03.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/vitess_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/vitess_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/vitess_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4744 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/vitess_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/vitess_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:54:03.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/vitess_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/vitess_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1727 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/vitess_handler/tests/test_vitess_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/vitess_handler/vitess_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:54:03.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/youtube_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/youtube_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/youtube_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6833 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/youtube_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/youtube_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2962 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/youtube_handler/youtube_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5433 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/youtube_handler/youtube_tables.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:54:03.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/yugabyte_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/yugabyte_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/yugabyte_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16563 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/yugabyte_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/yugabyte_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:54:03.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/yugabyte_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/yugabyte_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/yugabyte_handler/tests/test_yugabyte_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1994 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers/yugabyte_handler/yugabyte_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:54:03.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers_client/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers_client/db_client_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5264 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers_client/db_grpc_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2338 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers_client/ml_client_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4043 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers_client/ml_grpc_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:54:03.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers_wrapper/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers_wrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7894 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers_wrapper/db_grpc_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers_wrapper/db_handler_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6071 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers_wrapper/ml_grpc_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/handlers_wrapper/ml_handler_service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:54:03.000000 MindsDB-23.6.1.1/mindsdb/integrations/libs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/libs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6861 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/libs/api_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7147 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/libs/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/libs/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2328 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/libs/handler_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18616 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/libs/ml_exec_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6468 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/libs/ml_handler_proc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/libs/net_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2792 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/libs/response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3512 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/libs/storage_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:54:03.000000 MindsDB-23.6.1.1/mindsdb/integrations/utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2032 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/utilities/date_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      929 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/utilities/install.py
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/utilities/processes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2461 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/utilities/sql_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/utilities/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6300 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/utilities/time_series_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/integrations/utilities/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:54:03.000000 MindsDB-23.6.1.1/mindsdb/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/interfaces/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:54:03.000000 MindsDB-23.6.1.1/mindsdb/interfaces/database/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/interfaces/database/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2901 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/interfaces/database/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23139 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/interfaces/database/integrations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10054 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/interfaces/database/projects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3370 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/interfaces/database/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:54:03.000000 MindsDB-23.6.1.1/mindsdb/interfaces/file/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/interfaces/file/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4417 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/interfaces/file/file_controller.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:54:03.000000 MindsDB-23.6.1.1/mindsdb/interfaces/jobs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/interfaces/jobs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13212 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/interfaces/jobs/jobs_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3446 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/interfaces/jobs/scheduler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:54:03.000000 MindsDB-23.6.1.1/mindsdb/interfaces/model/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/interfaces/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4422 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/interfaces/model/functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22442 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/interfaces/model/model_controller.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:54:03.000000 MindsDB-23.6.1.1/mindsdb/interfaces/storage/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/interfaces/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9164 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/interfaces/storage/db.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10434 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/interfaces/storage/fs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2353 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/interfaces/storage/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4446 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/interfaces/storage/model_fs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:54:03.000000 MindsDB-23.6.1.1/mindsdb/interfaces/stream/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/interfaces/stream/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:54:03.000000 MindsDB-23.6.1.1/mindsdb/interfaces/stream/base/
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/interfaces/stream/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6057 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/interfaces/stream/base/integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/interfaces/stream/stream.py
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/interfaces/stream/utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:54:03.000000 MindsDB-23.6.1.1/mindsdb/microservices_grpc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/microservices_grpc/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:54:03.000000 MindsDB-23.6.1.1/mindsdb/microservices_grpc/db/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/microservices_grpc/db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/microservices_grpc/db/common_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/microservices_grpc/db/common_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/microservices_grpc/db/db_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12845 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/microservices_grpc/db/db_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:54:03.000000 MindsDB-23.6.1.1/mindsdb/microservices_grpc/executor/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/microservices_grpc/executor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3565 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/microservices_grpc/executor/executor_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14810 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/microservices_grpc/executor/executor_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:54:03.000000 MindsDB-23.6.1.1/mindsdb/microservices_grpc/ml/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/microservices_grpc/ml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/microservices_grpc/ml/common_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/microservices_grpc/ml/common_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2170 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/microservices_grpc/ml/ml_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5430 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/microservices_grpc/ml/ml_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:54:03.000000 MindsDB-23.6.1.1/mindsdb/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2695 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/migrations/alembic.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     2427 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/migrations/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/migrations/migrate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:54:03.000000 MindsDB-23.6.1.1/mindsdb/migrations/versions/
+-rw-r--r--   0 runner    (1001) docker     (123)     5750 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/migrations/versions/2021-11-30_17c3d2384711_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/migrations/versions/2022-01-26_47f97b83cee4_views.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10808 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/migrations/versions/2022-02-09_27c5aca9e47e_db_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6163 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/migrations/versions/2022-05-25_d74c189b87e6_predictor_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2773 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/migrations/versions/2022-07-08_999bceb904df_integration_args.py
+-rw-r--r--   0 runner    (1001) docker     (123)      849 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/migrations/versions/2022-07-15_b5b53e0ea7f8_training_data_rows_columns_count.py
+-rw-r--r--   0 runner    (1001) docker     (123)      998 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/migrations/versions/2022-07-22_6e834843e7e9_training_time.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/migrations/versions/2022-08-19_976f15a37e6a_predictors_versioning.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/migrations/versions/2022-08-25_6a54ba55872e_view_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/migrations/versions/2022-08-29_473e8f239481_straighten.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/migrations/versions/2022-09-06_96d5fef10caa_data_integration_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/migrations/versions/2022-09-08_87b2df2b83e1_predictor_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1789 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/migrations/versions/2022-09-19_3d5e70105df7_content_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2366 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/migrations/versions/2022-09-29_cada7d2be947_json_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3467 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/migrations/versions/2022-10-14_43c52d23845a_projects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/migrations/versions/2022-11-07_1e60096fc817_predictor_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3463 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/migrations/versions/2022-11-11_d429095b570f_data_integration_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)      799 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/migrations/versions/2022-12-26_459218b0844c_fix_unique_constraint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/migrations/versions/2023-02-02_b6d0a47294ac_jobs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/migrations/versions/2023-02-17_ee63d868fa84_predictor_integration_null.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/migrations/versions/2023-02-25_3154382dab17_training_progress.py
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/migrations/versions/2023-02-27_ef04cdbe51ed_jobs_user_class.py
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/migrations/versions/2023-04-11_b8be148dbc85_jobs_history_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/migrations/versions/2023-05-24_6d748f2c7b0b_remove_streams.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/migrations/versions/2023-05-31_aaecd7012a78_chatbot.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/migrations/versions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:54:03.000000 MindsDB-23.6.1.1/mindsdb/utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2336 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/utilities/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6805 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/utilities/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5775 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/utilities/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/utilities/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4064 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/utilities/fs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5046 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/utilities/functions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:54:03.000000 MindsDB-23.6.1.1/mindsdb/utilities/hooks/
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/utilities/hooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/utilities/hooks/profiling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/utilities/json_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5197 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/utilities/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/utilities/log_controller.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:54:03.000000 MindsDB-23.6.1.1/mindsdb/utilities/profiler/
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/utilities/profiler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3665 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/utilities/profiler/profiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2339 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/utilities/ps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/utilities/telemetry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1708 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/mindsdb/utilities/wizards.py
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-08 22:54:03.000000 MindsDB-23.6.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3655 2023-06-08 22:53:35.000000 MindsDB-23.6.1.1/setup.py
```

### Comparing `MindsDB-23.5.4.1/MindsDB.egg-info/PKG-INFO` & `MindsDB-23.6.1.1/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,209 +1,194 @@
-Metadata-Version: 2.1
-Name: MindsDB
-Version: 23.5.4.1
-Summary: MindsDB server, provides server capabilities to mindsdb native python library
-Home-page: https://github.com/mindsdb/mindsdb
-Author: MindsDB Inc
-Author-email: jorge@mindsdb.com
-License: GPL-3.0
-Download-URL: https://pypi.org/project/mindsdb/
-Description: <h1 align="center">
-        	<img width="300" src="https://github.com/mindsdb/mindsdb_native/blob/stable/assets/MindsDBColorPurp@3x.png?raw=true" alt="MindsDB">
-        	<br>
-        </h1>
-        
-        <div align="center">
-        
-        <a
-             href="https://runacap.com/ross-index/annual-2022/"
-             target="_blank"
-             rel="noopener"
-        />
-            <img
-                style="width: 260px; height: 56px"
-                src="https://runacap.com/wp-content/uploads/2023/02/Annual_ROSS_badge_white_2022.svg"
-                alt="ROSS Index - Fastest Growing Open-Source Startups | Runa Capital"
-                width="260"
-                height="56"
-            />
-        </a>
-        
-        <p>
-        	<a href="https://github.com/mindsdb/mindsdb/actions"><img src="https://github.com/mindsdb/mindsdb/workflows/MindsDB%20workflow/badge.svg" alt="MindsDB workflow"></a>
-        	<a href="https://www.python.org/downloads/" target="_blank"><img src="https://img.shields.io/badge/python-3.7.x%20|%203.8.x|%203.9.x-brightgreen.svg" alt="Python supported"></a>
-        	<a href="https://pypi.org/project/MindsDB/" target="_blank"><img src="https://badge.fury.io/py/MindsDB.svg" alt="PyPi Version"></a>
-        	<br />
-        	<img alt="PyPI - Downloads" src="https://img.shields.io/pypi/dm/Mindsdb">  <a href="https://hub.docker.com/u/mindsdb" target="_blank"><img src="https://img.shields.io/docker/pulls/mindsdb/mindsdb" alt="Docker pulls"></a>
-        	<a href="https://ossrank.com/p/630"><img src="https://shields.io/endpoint?url=https://ossrank.com/shield/630"></a>
-        	<a href="https://www.mindsdb.com/"><img src="https://img.shields.io/website?url=https%3A%2F%2Fwww.mindsdb.com%2F" alt="MindsDB Website"></a>
-        	<a href="https://join.slack.com/t/mindsdbcommunity/shared_invite/zt-o8mrmx3l-5ai~5H66s6wlxFfBMVI6wQ" target="_blank"><img src="https://img.shields.io/badge/slack-@mindsdbcommunity-brightgreen.svg?logo=slack " alt="MindsDB Community"></a>
-        	<br />
-        	<a href="https://deepnote.com/project/Machine-Learning-With-SQL-8GDF7bc7SzKlhBLorqoIcw/%2Fmindsdb_demo.ipynb" target="_blank"><img src="https://deepnote.com/buttons/launch-in-deepnote-white.svg" alt="Launch in Deepnote"></a>
-        	<br />
-        	<a href="https://gitpod.io/#https://github.com/mindsdb/mindsdb" target="_blank"><img src="https://gitpod.io/button/open-in-gitpod.svg" alt="Open in Gitpod"></a>
-        </p>
-        
-        <h3 align="center">
-        	<a href="https://www.mindsdb.com?utm_medium=community&utm_source=github&utm_campaign=mindsdb%20repo">Website</a>
-        	<span> | </span>
-        	<a href="https://docs.mindsdb.com?utm_medium=community&utm_source=github&utm_campaign=mindsdb%20repo">Docs</a>
-        	<span> | </span>
-        	<a href="https://mindsdb.com/joincommunity">Community Slack</a>
-        	<span> | </span>
-        	<a href="https://github.com/mindsdb/mindsdb/projects?type=classic">Contribute</a>
-        	<span> | </span>
-        	<a href="https://cloud.mindsdb.com?utm_medium=community&utm_source=github&utm_campaign=mindsdb%20repo">Demo</a>
-        	<span> | </span>
-        	<a href="https://hashnode.com/hackathons/mindsdb?source=hncounter-feed">Hackathon</a>
-        </h3>
-        
-        </div>
-        
-        ----------------------------------------
-        
-        [MindsDB](https://mindsdb.com?utm_medium=community&utm_source=github&utm_campaign=mindsdb%20repo) is an emerging low-code machine learning platform to help developers easily build #AI-powered solutions [![Tweet](https://img.shields.io/twitter/url/http/shields.io.svg?style=social)](https://twitter.com/intent/tweet?text=Build%20AI-Powered%20Applications%20&url=https://www.mindsdb.com&via=mindsdb&hashtags=ai,ml,nlp,machine_learning,neural_networks,databases,gpt3)
-        
-        
-        **NEW!** Check-out the [rewards and community programs.](https://mindsdb.com/community?utm_medium=community&utm_source=github&utm_campaign=mindsdb%20repo)
-        
-        ----------------------------------------
-        
-        [Installation](https://github.com/mindsdb/mindsdb#installation) - [Overview](https://github.com/mindsdb/mindsdb#overview) - [Features](https://github.com/mindsdb/mindsdb#features) - [Database Integrations](https://github.com/mindsdb/mindsdb#database-integrations) - [Quickstart](https://github.com/mindsdb/mindsdb#quickstart) - [Documentation](https://github.com/mindsdb/mindsdb#documentation) - [Support](https://github.com/mindsdb/mindsdb#support) - [Contributing](https://github.com/mindsdb/mindsdb#contributing) - [Mailing lists](https://github.com/mindsdb/mindsdb#mailing-lists) - [License](https://github.com/mindsdb/mindsdb#license)
-        
-        ----------------------------
-        
-        MindsDB automates and integrates top machine learning frameworks (including GPT-4) into the data stack as "AI Tables" to streamline the integration of AI into applications, making it accessible to developers of all skill levels.
-        "[AI tables](https://www.youtube.com/watch?v=tnB4Y9T1E2k)" allow you to get predictions via SQL queries and continuously learn from your data.
-        
-        <h2 align="center">
-           <br/>
-           <br/>
-          <img width="450" src="https://docs.google.com/drawings/d/e/2PACX-1vQ1KImK0cqvZ_KpPm3SKDZF6peuM-d1lZwOkrZNpT1_PO5UVyveEIyeJGbDZFBF124LmWbHSB2HFQ97/pub?w=691&h=728" alt="MindsDB">
-        
-        </h2>
-        
-        ## Use cases
-        
-        Here are some popular use cases you can build with MindsDB:
-        
-        * Conversational AI: Leverage MindsDB native integrations with data platforms and pre-trained large language models, like OpenAI's GPT, to quickly build conversational AI solutions without the overhead of managing complex data pipelines.
-        * Fraud Detection: MindsDB can help developers build models to detect fraudulent activity in financial transactions, eCommerce platforms etc.
-        * Sales Forecasting: MindsDB can be used to develop models to predict future sales based on historical sales data, allowing businesses to make better-informed decisions.
-        * Customer Segmentation: MindsDB can help developers segment customers based on their behavior, preferences, and other factors, allowing businesses to tailor their marketing efforts.
-        * Sentiment analysis: MindsDB native integration with pre-trained models like OpenAI GPT or Hugging Face can be used to analyze the sentiment of a text data, such as a customer reviews - in a single command, instead of individual API calls and ETL-ing data.
-        * Predictive Maintenance: MindsDB can be used to build models to predict when equipment or machinery is likely to fail, allowing for proactive maintenance and minimizing downtime.
-        
-        See more examples and community tutorials [here](https://docs.mindsdb.com/tutorials)
-        
-        ## Demo
-        
-        You can try MindsDB using our [demo environment](https://cloud.mindsdb.com/?utm_medium=community&utm_source=github&utm_campaign=mindsdb%20repo) with sample data for most popular use cases.
-        
-        ## Installation
-        
-        The prefered way is to use MindsDB Cloud [free demo instance](https://cloud.mindsdb.com/home) or use a [dedicated instance](https://cloud.mindsdb.com/home). If you want to move to production use [the AWS AMI image](https://aws.amazon.com/marketplace/seller-profile?id=03a65520-86ca-4ab8-a394-c11eb54573a9)/
-        
-        To install locally or on-premise pull the latest Docker image:
-        
-        ```
-        docker pull mindsdb/mindsdb
-        ```
-        
-        ## How it works
-        
-        1. First, CONNECT MindsDB to your data platform. We support 70+ data platforms and this list is constantly growing. If you can’t find the integration you need, please [let us know](https://mindsdb.com/joincommunity).
-        2. Run the CREATE MODEL query pointing to your data table or a view, that will automatically create and deploy a machine learning model as an [AI Table](https://www.youtube.com/watch?v=tnB4Y9T1E2k).
-            1. If you have an NLP use case, CREATE MODEL will integrate the [AI Table](https://www.youtube.com/watch?v=tnB4Y9T1E2k) with already pre-trained model you choose (like OpenAI’s GPT-3 or Hugging Face models).
-            2. Please check the [docs](https://docs.mindsdb.com/sql/create/predictor?utm_medium=community&utm_source=github&utm_campaign=mindsdb%20repo) if you want to have manual control over model engineering.
-        3. JOIN the model with your database tables to make predictions for thousands or even millions of data points at once, or run SELECT statements or API calls to make one time predictions.
-        4. Set up a JOB to automate your model re-training cycle and predictions pipelines for the new incoming data.
-        
-        Follow the [quickstart guide](https://docs.mindsdb.com/quickstart?utm_medium=community&utm_source=github&utm_campaign=mindsdb%20repo) with sample data to get on-boarded as fast as possible.
-        
-        
-        ## Database Integrations
-        
-        MindsDB works with most of the SQL and NoSQL databases, data lakes, data Streams and popular applications.
-        
-        | Connect your Data | Connect your Data | Connect your Data
-        |-|-|-|
-        | <a href="https://docs.mindsdb.com/connect/kafka"><img src="https://img.shields.io/badge/Apache Kafka-808080?style=for-the-badge&logo=apache-kafka&logoColor=white" alt="Connect Apache Kafka"></a> | <a href="https://docs.mindsdb.com/data-integrations/microsoft-access"><img src="https://img.shields.io/badge/Microsoft%20Access-A4373A?logo=microsoftaccess&logoColor=fff&style=for-the-badge" alt="Connect Microsoft Access"></a> | <a href="https://docs.mindsdb.com/data-integrations/oracle"><img src="https://img.shields.io/badge/Oracle-F80000?logo=oracle&logoColor=fff&style=for-the-badge" alt="Oracle Badge"></a> |
-        | <a href="https://docs.mindsdb.com/data-integrations/amazon-redshift"><img src="https://img.shields.io/badge/Amazon%20Redshift-0466C8?style=for-the-badge&logo=amazon-aws&logoColor=white" alt="Connect Amazon Redshift"></a> | <a href="https://docs.mindsdb.com/data-integrations/airtable"><img src="https://img.shields.io/badge/Airtable-18BFFF?logo=airtable&logoColor=fff&style=for-the-badge" alt="Airtable Badge"></a> | <a href="https://docs.mindsdb.com/data-integrations/apache-pinot"><img src="https://img.shields.io/badge/Pinot-000?logo=pinot&logoColor=fff&style=for-the-badge" alt="Pinot Badge"></a> |
-        | <a href="https://docs.mindsdb.com/data-integrations/apache-cassandra"><img src="https://img.shields.io/badge/Cassandra-1287B1?style=for-the-badge&logo=apache%20cassandra&logoColor=white" alt="Connect Cassandra"></a> | <a href="https://docs.mindsdb.com/data-integrations/datastax"><img src="https://img.shields.io/badge/DataStax-3A3A42?logo=datastax&logoColor=fff&style=for-the-badge" alt="DataStax Badge"></a> | <a href="https://docs.mindsdb.com/data-integrations/amazon-s3"><img src="https://img.shields.io/badge/Amazon%20S3-569A31?logo=amazons3&logoColor=fff&style=for-the-badge" alt="Amazon S3 Badge"></a> |
-        | <a href="https://docs.mindsdb.com/data-integrations/cockroachdb"><img src="https://img.shields.io/badge/CockroachDB-426EDF?style=for-the-badge&logo=cockroach-labs&logoColor=white" alt="Connect CockroachDB"></a> | <a href="https://docs.mindsdb.com/data-integrations/ckan"><img src="https://img.shields.io/badge/ckan-7D929E?logo=ckan&logoColor=fff&style=for-the-badge" alt="ckan Badge"></a> | <a href="https://docs.mindsdb.com/data-integrations/supabase"><img src="https://img.shields.io/badge/Supabase-3ECF8E?logo=supabase&logoColor=fff&style=for-the-badge" alt="Supabase Badge"></a> |
-        | <a href="https://docs.mindsdb.com/data-integrations/clickhouse"><img src="https://img.shields.io/badge/Clickhouse-e6e600?style=for-the-badge&logo=clickhouse&logoColor=white" alt="Connect Clickhouse"></a> | <a href="https://docs.mindsdb.com/data-integrations/google-bigquery"><img src="https://img.shields.io/badge/Google Big Query-0466C8?logo=Big Query&logoColor=fff&style=for-the-badge" alt="Google Big Query Badge"></a> | <a href="https://docs.mindsdb.com/data-integrations/sqlite"><img src="https://img.shields.io/badge/SQLite-003B57?logo=sqlite&logoColor=fff&style=for-the-badge" alt="SQLite Badge"></a> |
-        | <a href="https://docs.mindsdb.com/data-integrations/mariadb"><img src="https://img.shields.io/badge/MariaDB-003545?style=for-the-badge&logo=mariadb&logoColor=white" alt="Connect MariaDB"></a> | <a href="https://docs.mindsdb.com/data-integrations/couchbase"><img src="https://img.shields.io/badge/Couchbase-EA2328?logo=couchbase&logoColor=fff&style=for-the-badge" alt="Couchbase Badge"></a> | <a href="https://docs.mindsdb.com/data-integrations/tidb#tidb-handler"><img src="https://img.shields.io/badge/TiDB-DD0031?logo=tidb&logoColor=fff&style=for-the-badge" alt="TiDB Badge"></a> |
-        | <a href="https://docs.mindsdb.com/data-integrations/microsoft-sql-server"><img src="https://img.shields.io/badge/Microsoft%20SQL%20Sever-CC2927?style=for-the-badge&logo=microsoft%20sql%20server&logoColor=white" alt="Connect SQL Server"></a> | <a href="https://docs.mindsdb.com/data-integrations/cratedb"><img src="https://img.shields.io/badge/CrateDB-009DC7?logo=cratedb&logoColor=fff&style=for-the-badge" alt="CrateDB Badge"></a> | <a href=" https://docs.mindsdb.com/data-integrations/timescaledb"><img src="https://img.shields.io/badge/Timescale-FDB515?logo=timescale&logoColor=fff&style=for-the-badge" alt="Timescale Badge"></a> |
-        | <a href="https://docs.mindsdb.com/data-integrations/mongodb"><img src="https://img.shields.io/badge/MongoDB-4EA94B?style=for-the-badge&logo=mongodb&logoColor=white" alt="Connect MongoDB"></a> | <a href="https://docs.mindsdb.com/data-integrations/d0lt"><img src="https://img.shields.io/badge/DoIt-00B388?logo=DoIt&logoColor=fff&style=for-the-badge" alt="DoIt Badge"></a> | <a href="https://docs.mindsdb.com/data-integrations/amazon-dynamodb"><img src="https://img.shields.io/badge/Amazon%20DynamoDB-4053D6?logo=amazondynamodb&logoColor=fff&style=for-the-badge" alt="Amazon DynamoDB Badge"></a> |
-        | <a href="https://docs.mindsdb.com/data-integrations/postgresql"><img src="https://img.shields.io/badge/PostgreSQL-316192?style=for-the-badge&logo=postgresql&logoColor=white" alt="Connect PostgreSQL"></a> | <a href="https://docs.mindsdb.com/data-integrations/ibm-db2"><img src="https://img.shields.io/badge/IBMDB2-008000?logo=IBMDB2&logoColor=fff&style=for-the-badge" alt="IBMDB2 Badge"></a> | <a href="https://docs.mindsdb.com/data-integrations/opengauss"><img src="https://img.shields.io/badge/openGauss-02458D?logo=opengauss&logoColor=fff&style=for-the-badge" alt="openGauss Badge"></a> |
-        | <a href="https://docs.mindsdb.com/data-integrations/mysql"><img src="https://img.shields.io/badge/MySQL-00758F?style=for-the-badge&logo=mysql&logoColor=white" alt="Connect MySQL"></a> | <a href=" https://docs.mindsdb.com/data-integrations/databricks"><img src="https://img.shields.io/badge/Databricks-FF3621?logo=databricks&logoColor=fff&style=for-the-badge" alt="Databricks Badge"></a> | <a href="https://docs.mindsdb.com/data-integrations/yugabytedb"><img src="https://img.shields.io/badge/YugabyteDB-02458D?logo=yugabytedb&logoColor=fff&style=for-the-badge" alt="YugabyteDB Badge"></a>
-        | <a href="https://docs.mindsdb.com/data-integrations/questdb"><img src="https://img.shields.io/badge/QuestDB-d14671?style=for-the-badge&logo=questdb&logoColor=white" alt="Connect QuestDB"></a> | <a href="https://docs.mindsdb.com/data-integrations/apache-druid"><img src="https://img.shields.io/badge/Apache%20Druid-29F1FB?logo=apachedruid&logoColor=000&style=for-the-badge" alt="Apache Druid Badge"></a> |
-        | <a href="https://docs.mindsdb.com/data-integrations/starrocks"><img src="https://img.shields.io/badge/starrocks-000000?style=for-the-badge&logo=starrocks&logoColor=white" alt="StarRocks Badge"></a> | <a href="https://docs.mindsdb.com/data-integrations/vertica"><img src="https://img.shields.io/badge/Vertica-000?logo=vertica&logoColor=fff&style=for-the-badge" alt="Vertica Badge"></a> | <a href="https://docs.mindsdb.com/data-integrations/duckdb"><img src="https://img.shields.io/badge/duckdb-fff?logo=duckdb&logoColor=000&style=for-the-badge" alt="DuckDB Badge"></a> |
-        | <a href="https://docs.mindsdb.com/data-integrations/sap-hana"><img src="https://img.shields.io/badge/SAP%20HANA-1661BE?style=for-the-badge&logo=sap&logoColor=white" alt="Connect SAP HANA"></a> | <a href="https://docs.mindsdb.com/data-integrations/elasticsearch"><img src="https://img.shields.io/badge/Elastic-005571?logo=elastic&logoColor=fff&style=for-the-badge" alt="Elastic Badge"></a> | <a href="https://docs.mindsdb.com/data-integrations/cloud-spanner"><img src="https://img.shields.io/badge/Cloud%20Spanner-4285F4?style=for-the-badge" alt="Cloud Spanner Badge"></a> |
-        | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#scylla"><img src="https://img.shields.io/badge/ScyllaDB-53CADD?style=for-the-badge&logo=scylladbb&logoColor=white" alt="Connect ScyllaDB"></a> | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#firebird"><img src="https://img.shields.io/badge/Firebird-F40D12?logo=Firebird&logoColor=fff&style=for-the-badge" alt="Firebird Badge"></a> |
-        | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#singlestore"><img src="https://img.shields.io/badge/Singlestore-5f07b4?style=for-the-badge&logo=singlestore&logoColor=white" alt="Connect Singlestore"></a> | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#hive"><img src="https://img.shields.io/badge/Apache%20Hive-FDEE21?logo=apachehive&logoColor=000&style=for-the-badge" alt="Apache Hive Badge"></a> |
-        | <a href="https://docs.mindsdb.com/data-integrations/teradata"><img src="https://img.shields.io/badge/Teradata-e36c42?style=for-the-badge&logo=teradata&logoColor=white" alt="Connect Teradata"></a> | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#matrix-one"><img src="https://img.shields.io/badge/Matrixone-02458D?logo=Matrixone&logoColor=fff&style=for-the-badge" alt="Matrixone Badge"></a> |
-        | <a href=" https://docs.mindsdb.com/data-integrations/snowflake"><img src="https://img.shields.io/badge/Snowflake-35aedd?style=for-the-badge&logo=snowflake&logoColor=blue" alt="Connect Snowflake"></a> | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#informix"><img src="https://img.shields.io/badge/Informix-191A1B?logo=informix&logoColor=fff&style=for-the-badge" alt="Informix Badge"></a> |
-        | <a href="https://docs.mindsdb.com/data-integrations/trino"><img src="https://img.shields.io/badge/Trino-dd00a1?style=for-the-badge&logo=trino&logoColor=white" alt="Connect Trino"></a> | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#monetdb"><img src="https://img.shields.io/badge/Monetdb-0099E5?logo=Monetdb&logoColor=fff&style=for-the-badge" alt="Monetdb Badge"></a> |
-        
-        
-        
-        [:question: :wave: Missing integration?](https://github.com/mindsdb/mindsdb/issues/new?assignees=&labels=&template=feature-mindsdb-request.yaml)
-        
-        
-        ## Documentation
-        
-        You can find the complete documentation of MindsDB at [docs.mindsdb.com](https://docs.mindsdb.com?utm_medium=community&utm_source=github&utm_campaign=mindsdb%20repo).
-        
-        ## Support
-        
-        If you found a bug, please submit an [issue on GitHub](https://github.com/mindsdb/mindsdb/issues/new/choose).
-        
-        To get community support, you can:
-        
-        * Post at MindsDB [Slack community](https://mindsdb.com/joincommunity).
-        * Ask for help at our [GitHub Discussions](https://github.com/mindsdb/mindsdb/discussions).
-        * Ask a question at [Stackoverflow](https://stackoverflow.com/questions/tagged/mindsdb) with a MindsDB tag.
-        
-        If you need commercial support, please [contact](https://mindsdb.com/contact/?utm_medium=community&utm_source=github&utm_campaign=mindsdb%20repo) MindsDB team.
-        
-        ## Contributing
-        
-        A great place to start contributing to MindsDB is to check our GitHub projects :checkered_flag:
-        
-        * Tutorials & documentation [dashboard tasks](https://github.com/mindsdb/mindsdb/projects/7).
-        * Code contributor's [dashboard tasks](https://github.com/mindsdb/mindsdb/projects/8).
-        * [First timers only issues](https://github.com/mindsdb/mindsdb/issues?q=is%3Aissue+is%3Aopen+label%3Afirst-timers-only), if this is your first time contributing to an open source project.
-        
-        We are always open to suggestions so feel free to open new issues with your ideas and we can guide you!
-        
-        Being part of the core team is accessible to anyone who is motivated and wants to be part of that journey!
-        If you'd like to contribute to the project, refer to the [contributing documentation](https://docs.mindsdb.com/contribute/?utm_medium=community&utm_source=github&utm_campaign=mindsdb%20repo).
-        
-        Please note that this project is released with a [Contributor Code of Conduct](https://github.com/mindsdb/mindsdb/blob/stable/CODE_OF_CONDUCT.md). By participating in this project, you agree to abide by its terms.
-        
-        Also, check out the [rewards and community programs](https://mindsdb.com/community?utm_medium=community&utm_source=github&utm_campaign=mindsdb%20repo).
-        
-        
-        ### Current contributors
-        
-        <a href="https://github.com/mindsdb/mindsdb/graphs/contributors">
-          <img src="https://contributors-img.web.app/image?repo=mindsdb/mindsdb" />
-        </a>
-        
-        Made with [contributors-img](https://contributors-img.web.app).
-        
-        ## Subscribe to updates
-        
-        Join our [Slack community](https://mindsdb.com/joincommunity) and subscribe to the monthly [Developer Newsletter](https://mindsdb.com/newsletter/?utm_medium=community&utm_source=github&utm_campaign=mindsdb%20repo) to get product updates, information about MindsDB events and contests, and useful content, like tutorials.
-        
-        
-        ## License
-        
-        MindsDB is licensed under [GNU General Public License v3.0](https://github.com/mindsdb/mindsdb/blob/master/LICENSE)
-        
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
+<h1 align="center">
+	<img width="300" src="https://github.com/mindsdb/mindsdb_native/blob/stable/assets/MindsDBColorPurp@3x.png?raw=true" alt="MindsDB">
+	<br>
+</h1>
+
+<div align="center">
+
+<a
+     href="https://runacap.com/ross-index/annual-2022/"
+     target="_blank"
+     rel="noopener"
+/>
+    <img
+        style="width: 260px; height: 56px"
+        src="https://runacap.com/wp-content/uploads/2023/02/Annual_ROSS_badge_white_2022.svg"
+        alt="ROSS Index - Fastest Growing Open-Source Startups | Runa Capital"
+        width="260"
+        height="56"
+    />
+</a>
+
+<p>
+	<a href="https://github.com/mindsdb/mindsdb/actions"><img src="https://github.com/mindsdb/mindsdb/workflows/MindsDB%20workflow/badge.svg" alt="MindsDB workflow"></a>
+	<a href="https://www.python.org/downloads/" target="_blank"><img src="https://img.shields.io/badge/python-3.7.x%20|%203.8.x|%203.9.x-brightgreen.svg" alt="Python supported"></a>
+	<a href="https://pypi.org/project/MindsDB/" target="_blank"><img src="https://badge.fury.io/py/MindsDB.svg" alt="PyPi Version"></a>
+	<br />
+	<img alt="PyPI - Downloads" src="https://img.shields.io/pypi/dm/Mindsdb">  <a href="https://hub.docker.com/u/mindsdb" target="_blank"><img src="https://img.shields.io/docker/pulls/mindsdb/mindsdb" alt="Docker pulls"></a>
+	<a href="https://ossrank.com/p/630"><img src="https://shields.io/endpoint?url=https://ossrank.com/shield/630"></a>
+	<a href="https://www.mindsdb.com/"><img src="https://img.shields.io/website?url=https%3A%2F%2Fwww.mindsdb.com%2F" alt="MindsDB Website"></a>
+	<a href="https://mindsdb.com/joincommunity" target="_blank"><img src="https://img.shields.io/badge/slack-@mindsdbcommunity-brightgreen.svg?logo=slack " alt="MindsDB Community"></a>
+	<br />
+	<a href="https://deepnote.com/project/Machine-Learning-With-SQL-8GDF7bc7SzKlhBLorqoIcw/%2Fmindsdb_demo.ipynb" target="_blank"><img src="https://deepnote.com/buttons/launch-in-deepnote-white.svg" alt="Launch in Deepnote"></a>
+	<br />
+	<a href="https://gitpod.io/#https://github.com/mindsdb/mindsdb" target="_blank"><img src="https://gitpod.io/button/open-in-gitpod.svg" alt="Open in Gitpod"></a>
+</p>
+
+<h3 align="center">
+	<a href="https://www.mindsdb.com?utm_medium=community&utm_source=github&utm_campaign=mindsdb%20repo">Website</a>
+	<span> | </span>
+	<a href="https://docs.mindsdb.com?utm_medium=community&utm_source=github&utm_campaign=mindsdb%20repo">Docs</a>
+	<span> | </span>
+	<a href="https://mindsdb.com/joincommunity">Community Slack</a>
+	<span> | </span>
+	<a href="https://github.com/mindsdb/mindsdb/projects?type=classic">Contribute</a>
+	<span> | </span>
+	<a href="https://cloud.mindsdb.com?utm_medium=community&utm_source=github&utm_campaign=mindsdb%20repo">Demo</a>
+	<span> | </span>
+	<a href="https://hashnode.com/hackathons/mindsdb?source=hncounter-feed">Hackathon</a>
+</h3>
+
+</div>
+
+----------------------------------------
+
+[MindsDB](https://mindsdb.com?utm_medium=community&utm_source=github&utm_campaign=mindsdb%20repo) is a Server for Artificial Intelligence Logic, enabling developers to ship AI powered projects from prototyping & experimentation to production in a fast & scalable way. [![Tweet](https://img.shields.io/twitter/url/http/shields.io.svg?style=social)](https://twitter.com/intent/tweet?text=Build%20AI-Centered%20Applications%20&url=https://www.mindsdb.com&via=mindsdb&hashtags=ai,ml,nlp,machine_learning,neural_networks,databases,gpt3)
+
+We do this by abstracting Generative AI, Large Language and other Models as a virtual tables ([AI Tables](https://www.youtube.com/watch?v=tnB4Y9T1E2k)) on top of enterprise databases. This increases accessibility with organizations and enables development teams to use their existing skills to build applications powered by AI.
+
+By taking a data-centric approach to AI MindsDB brings the process closer to the source of the data minimizing the need to build and maintain data pipelines and ETL’ing, speeding up the time to deployment and reducing complexity.
+
+**P.S. If you like our open-source project we'd appreciate if you star it on GitHub ⭐!**
+
+<h2 align="center">
+   <br/>
+   <br/>
+  <img width="100%" src="https://github.com/mindsdb/mindsdb/assets/12409467/8418fec3-8c8b-4414-b1dc-7943041047b4" alt="MindsDB">
+
+</h2>
+
+----------------------------------------
+MindsDB has an active and helpful community. Feel free to join our [Slack](https://mindsdb.com/joincommunity) and check-out the [rewards and community programs](https://mindsdb.com/community?utm_medium=community&utm_source=github&utm_campaign=mindsdb%20repo).
+
+----------------------------------------
+
+[Installation](https://github.com/mindsdb/mindsdb#installation) - [Overview](https://github.com/mindsdb/mindsdb#overview) - [Features](https://github.com/mindsdb/mindsdb#features) - [Database Integrations](https://github.com/mindsdb/mindsdb#database-integrations) - [Quickstart](https://github.com/mindsdb/mindsdb#quickstart) - [Documentation](https://github.com/mindsdb/mindsdb#documentation) - [Support](https://github.com/mindsdb/mindsdb#support) - [Contributing](https://github.com/mindsdb/mindsdb#contributing) - [Mailing lists](https://github.com/mindsdb/mindsdb#mailing-lists) - [License](https://github.com/mindsdb/mindsdb#license)
+
+----------------------------------------
+
+## Use cases
+
+Here are some popular use cases you can build with MindsDB:
+
+* Conversational AI: Leverage MindsDB native integrations with data platforms and pre-trained large language models, like OpenAI's GPT, to quickly build conversational AI solutions without the overhead of managing complex data pipelines.
+* Fraud Detection: MindsDB can help developers build models to detect fraudulent activity in financial transactions, eCommerce platforms etc.
+* Sales Forecasting: MindsDB can be used to develop models to predict future sales based on historical sales data, allowing businesses to make better-informed decisions.
+* Customer Segmentation: MindsDB can help developers segment customers based on their behavior, preferences, and other factors, allowing businesses to tailor their marketing efforts.
+* Sentiment analysis: MindsDB native integration with pre-trained models like OpenAI GPT or Hugging Face can be used to analyze the sentiment of a text data, such as a customer reviews - in a single command, instead of individual API calls and ETL-ing data.
+* Predictive Maintenance: MindsDB can be used to build models to predict when equipment or machinery is likely to fail, allowing for proactive maintenance and minimizing downtime.
+
+See more examples and community tutorials [here](https://docs.mindsdb.com/tutorials).
+
+## Demo
+
+You can try MindsDB using our [demo environment](https://cloud.mindsdb.com/?utm_medium=community&utm_source=github&utm_campaign=mindsdb%20repo) with sample data for most popular use cases.
+
+## Installation
+
+The prefered way is to use MindsDB Cloud [free demo instance](https://cloud.mindsdb.com/home) or use a [dedicated instance](https://cloud.mindsdb.com/home). If you want to move to production use [the AWS AMI image](https://aws.amazon.com/marketplace/seller-profile?id=03a65520-86ca-4ab8-a394-c11eb54573a9).
+
+To install locally or on-premise pull the latest Docker image:
+
+```
+docker pull mindsdb/mindsdb
+```
+
+## How it works
+
+1. CONNECT MindsDB to your data platform. We support 100+ data platforms and this list is constantly growing. If you can’t find the integration you need, please [let us know](https://mindsdb.com/joincommunity).
+2. CREATE MODEL to connect the AI Engine you pick that will learn from your data and serve it as [AI Table](https://www.youtube.com/watch?v=tnB4Y9T1E2k).
+    1. If you have an NLP use case, CREATE MODEL will integrate the [AI Table](https://www.youtube.com/watch?v=tnB4Y9T1E2k) with already pre-trained model you choose (like OpenAI’s GPT or Hugging Face models).
+    2. Please check the [docs](https://docs.mindsdb.com/sql/create/model?utm_medium=community&utm_source=github&utm_campaign=mindsdb%20repo) if you want to have manual control over model engineering.
+3. JOIN such model with your database tables to make predictions for thousands or even millions of data points at once, or run SELECT statements or API calls to make one time predictions.
+4. Set up a JOB to automate your re-training cycle and predictions pipelines for the new incoming data.
+5. Alternatively, use REST API to query the models
+
+Follow the [quickstart guide](https://docs.mindsdb.com/quickstart?utm_medium=community&utm_source=github&utm_campaign=mindsdb%20repo) with sample data to get on-boarded as fast as possible.
+
+
+## Database Integrations
+
+MindsDB works with most of the SQL and NoSQL databases, data lakes and popular applications.
+
+| Connect your Data | Connect your Data | Connect your Data
+|-|-|-|
+| <a href="https://docs.mindsdb.com/data-integrations/amazon-redshift"><img src="https://img.shields.io/badge/Amazon%20Redshift-0466C8?style=for-the-badge&logo=amazon-aws&logoColor=white" alt="Connect Amazon Redshift"></a> | <a href="https://docs.mindsdb.com/data-integrations/airtable"><img src="https://img.shields.io/badge/Airtable-18BFFF?logo=airtable&logoColor=fff&style=for-the-badge" alt="Airtable Badge"></a> | <a href="https://docs.mindsdb.com/data-integrations/apache-pinot"><img src="https://img.shields.io/badge/Pinot-000?logo=pinot&logoColor=fff&style=for-the-badge" alt="Pinot Badge"></a> |
+| <a href="https://docs.mindsdb.com/data-integrations/apache-cassandra"><img src="https://img.shields.io/badge/Cassandra-1287B1?style=for-the-badge&logo=apache%20cassandra&logoColor=white" alt="Connect Cassandra"></a> | <a href="https://docs.mindsdb.com/data-integrations/datastax"><img src="https://img.shields.io/badge/DataStax-3A3A42?logo=datastax&logoColor=fff&style=for-the-badge" alt="DataStax Badge"></a> | <a href="https://docs.mindsdb.com/data-integrations/amazon-s3"><img src="https://img.shields.io/badge/Amazon%20S3-569A31?logo=amazons3&logoColor=fff&style=for-the-badge" alt="Amazon S3 Badge"></a> |
+| <a href="https://docs.mindsdb.com/data-integrations/cockroachdb"><img src="https://img.shields.io/badge/CockroachDB-426EDF?style=for-the-badge&logo=cockroach-labs&logoColor=white" alt="Connect CockroachDB"></a> | <a href="https://docs.mindsdb.com/data-integrations/ckan"><img src="https://img.shields.io/badge/ckan-7D929E?logo=ckan&logoColor=fff&style=for-the-badge" alt="ckan Badge"></a> | <a href="https://docs.mindsdb.com/data-integrations/supabase"><img src="https://img.shields.io/badge/Supabase-3ECF8E?logo=supabase&logoColor=fff&style=for-the-badge" alt="Supabase Badge"></a> |
+| <a href="https://docs.mindsdb.com/data-integrations/clickhouse"><img src="https://img.shields.io/badge/Clickhouse-e6e600?style=for-the-badge&logo=clickhouse&logoColor=white" alt="Connect Clickhouse"></a> | <a href="https://docs.mindsdb.com/data-integrations/google-bigquery"><img src="https://img.shields.io/badge/Google Big Query-0466C8?logo=Big Query&logoColor=fff&style=for-the-badge" alt="Google Big Query Badge"></a> | <a href="https://docs.mindsdb.com/data-integrations/sqlite"><img src="https://img.shields.io/badge/SQLite-003B57?logo=sqlite&logoColor=fff&style=for-the-badge" alt="SQLite Badge"></a> |
+| <a href="https://docs.mindsdb.com/data-integrations/mariadb"><img src="https://img.shields.io/badge/MariaDB-003545?style=for-the-badge&logo=mariadb&logoColor=white" alt="Connect MariaDB"></a> | <a href="https://docs.mindsdb.com/data-integrations/couchbase"><img src="https://img.shields.io/badge/Couchbase-EA2328?logo=couchbase&logoColor=fff&style=for-the-badge" alt="Couchbase Badge"></a> | <a href="https://docs.mindsdb.com/data-integrations/tidb#tidb-handler"><img src="https://img.shields.io/badge/TiDB-DD0031?logo=tidb&logoColor=fff&style=for-the-badge" alt="TiDB Badge"></a> |
+| <a href="https://docs.mindsdb.com/data-integrations/microsoft-sql-server"><img src="https://img.shields.io/badge/Microsoft%20SQL%20Sever-CC2927?style=for-the-badge&logo=microsoft%20sql%20server&logoColor=white" alt="Connect SQL Server"></a> | <a href="https://docs.mindsdb.com/data-integrations/cratedb"><img src="https://img.shields.io/badge/CrateDB-009DC7?logo=cratedb&logoColor=fff&style=for-the-badge" alt="CrateDB Badge"></a> | <a href=" https://docs.mindsdb.com/data-integrations/timescaledb"><img src="https://img.shields.io/badge/Timescale-FDB515?logo=timescale&logoColor=fff&style=for-the-badge" alt="Timescale Badge"></a> |
+| <a href="https://docs.mindsdb.com/data-integrations/mongodb"><img src="https://img.shields.io/badge/MongoDB-4EA94B?style=for-the-badge&logo=mongodb&logoColor=white" alt="Connect MongoDB"></a> | <a href="https://docs.mindsdb.com/data-integrations/d0lt"><img src="https://img.shields.io/badge/DoIt-00B388?logo=DoIt&logoColor=fff&style=for-the-badge" alt="DoIt Badge"></a> | <a href="https://docs.mindsdb.com/data-integrations/amazon-dynamodb"><img src="https://img.shields.io/badge/Amazon%20DynamoDB-4053D6?logo=amazondynamodb&logoColor=fff&style=for-the-badge" alt="Amazon DynamoDB Badge"></a> |
+| <a href="https://docs.mindsdb.com/data-integrations/postgresql"><img src="https://img.shields.io/badge/PostgreSQL-316192?style=for-the-badge&logo=postgresql&logoColor=white" alt="Connect PostgreSQL"></a> | <a href="https://docs.mindsdb.com/data-integrations/ibm-db2"><img src="https://img.shields.io/badge/IBMDB2-008000?logo=IBMDB2&logoColor=fff&style=for-the-badge" alt="IBMDB2 Badge"></a> | <a href="https://docs.mindsdb.com/data-integrations/opengauss"><img src="https://img.shields.io/badge/openGauss-02458D?logo=opengauss&logoColor=fff&style=for-the-badge" alt="openGauss Badge"></a> |
+| <a href="https://docs.mindsdb.com/data-integrations/mysql"><img src="https://img.shields.io/badge/MySQL-00758F?style=for-the-badge&logo=mysql&logoColor=white" alt="Connect MySQL"></a> | <a href=" https://docs.mindsdb.com/data-integrations/databricks"><img src="https://img.shields.io/badge/Databricks-FF3621?logo=databricks&logoColor=fff&style=for-the-badge" alt="Databricks Badge"></a> | <a href="https://docs.mindsdb.com/data-integrations/yugabytedb"><img src="https://img.shields.io/badge/YugabyteDB-02458D?logo=yugabytedb&logoColor=fff&style=for-the-badge" alt="YugabyteDB Badge"></a>
+| <a href="https://docs.mindsdb.com/data-integrations/questdb"><img src="https://img.shields.io/badge/QuestDB-d14671?style=for-the-badge&logo=questdb&logoColor=white" alt="Connect QuestDB"></a> | <a href="https://docs.mindsdb.com/data-integrations/apache-druid"><img src="https://img.shields.io/badge/Apache%20Druid-29F1FB?logo=apachedruid&logoColor=000&style=for-the-badge" alt="Apache Druid Badge"></a> |
+| <a href="https://docs.mindsdb.com/data-integrations/starrocks"><img src="https://img.shields.io/badge/starrocks-000000?style=for-the-badge&logo=starrocks&logoColor=white" alt="StarRocks Badge"></a> | <a href="https://docs.mindsdb.com/data-integrations/vertica"><img src="https://img.shields.io/badge/Vertica-000?logo=vertica&logoColor=fff&style=for-the-badge" alt="Vertica Badge"></a> | <a href="https://docs.mindsdb.com/data-integrations/duckdb"><img src="https://img.shields.io/badge/duckdb-fff?logo=duckdb&logoColor=000&style=for-the-badge" alt="DuckDB Badge"></a> |
+| <a href="https://docs.mindsdb.com/data-integrations/sap-hana"><img src="https://img.shields.io/badge/SAP%20HANA-1661BE?style=for-the-badge&logo=sap&logoColor=white" alt="Connect SAP HANA"></a> | <a href="https://docs.mindsdb.com/data-integrations/elasticsearch"><img src="https://img.shields.io/badge/Elastic-005571?logo=elastic&logoColor=fff&style=for-the-badge" alt="Elastic Badge"></a> | <a href="https://docs.mindsdb.com/data-integrations/cloud-spanner"><img src="https://img.shields.io/badge/Cloud%20Spanner-4285F4?style=for-the-badge" alt="Cloud Spanner Badge"></a> |
+| <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#scylla"><img src="https://img.shields.io/badge/ScyllaDB-53CADD?style=for-the-badge&logo=scylladbb&logoColor=white" alt="Connect ScyllaDB"></a> | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#firebird"><img src="https://img.shields.io/badge/Firebird-F40D12?logo=Firebird&logoColor=fff&style=for-the-badge" alt="Firebird Badge"></a> |
+| <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#singlestore"><img src="https://img.shields.io/badge/Singlestore-5f07b4?style=for-the-badge&logo=singlestore&logoColor=white" alt="Connect Singlestore"></a> | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#hive"><img src="https://img.shields.io/badge/Apache%20Hive-FDEE21?logo=apachehive&logoColor=000&style=for-the-badge" alt="Apache Hive Badge"></a> |
+| <a href="https://docs.mindsdb.com/data-integrations/teradata"><img src="https://img.shields.io/badge/Teradata-e36c42?style=for-the-badge&logo=teradata&logoColor=white" alt="Connect Teradata"></a> | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#matrix-one"><img src="https://img.shields.io/badge/Matrixone-02458D?logo=Matrixone&logoColor=fff&style=for-the-badge" alt="Matrixone Badge"></a> |
+| <a href=" https://docs.mindsdb.com/data-integrations/snowflake"><img src="https://img.shields.io/badge/Snowflake-35aedd?style=for-the-badge&logo=snowflake&logoColor=blue" alt="Connect Snowflake"></a> | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#informix"><img src="https://img.shields.io/badge/Informix-191A1B?logo=informix&logoColor=fff&style=for-the-badge" alt="Informix Badge"></a> |
+| <a href="https://docs.mindsdb.com/data-integrations/trino"><img src="https://img.shields.io/badge/Trino-dd00a1?style=for-the-badge&logo=trino&logoColor=white" alt="Connect Trino"></a> | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#monetdb"><img src="https://img.shields.io/badge/Monetdb-0099E5?logo=Monetdb&logoColor=fff&style=for-the-badge" alt="Monetdb Badge"></a> |
+
+[:question: :wave: Missing integration?](https://github.com/mindsdb/mindsdb/issues/new?assignees=&labels=&template=feature-mindsdb-request.yaml)
+
+
+## Documentation
+
+You can find the complete documentation of MindsDB at [docs.mindsdb.com](https://docs.mindsdb.com?utm_medium=community&utm_source=github&utm_campaign=mindsdb%20repo).
+
+## Support
+
+If you found a bug, please submit an [issue on GitHub](https://github.com/mindsdb/mindsdb/issues/new/choose).
+
+To get community support, you can:
+
+* Post a question at MindsDB [Slack community](https://mindsdb.com/joincommunity).
+* Ask for help at our [GitHub Discussions](https://github.com/mindsdb/mindsdb/discussions).
+* Ask a question at [Stackoverflow](https://stackoverflow.com/questions/tagged/mindsdb) with a MindsDB tag.
+
+If you need commercial support, please [contact](https://mindsdb.com/contact/?utm_medium=community&utm_source=github&utm_campaign=mindsdb%20repo) MindsDB team.
+
+## Contributing
+
+A great place to start contributing to MindsDB is to check our GitHub projects :checkered_flag:
+
+* Community contributor's [dashboard tasks](https://github.com/mindsdb/mindsdb/projects/8).
+* [First timers only issues](https://github.com/mindsdb/mindsdb/issues?q=is%3Aissue+is%3Aopen+label%3Afirst-timers-only), if this is your first time contributing to an open source project.
+
+We are always open to suggestions so feel free to open new issues with your ideas and we can guide you!
+
+Being part of the core team is accessible to anyone who is motivated and wants to be part of that journey!
+If you'd like to contribute to the project, refer to the [contributing documentation](https://docs.mindsdb.com/contribute/?utm_medium=community&utm_source=github&utm_campaign=mindsdb%20repo).
+
+Please note that this project is released with a [Contributor Code of Conduct](https://github.com/mindsdb/mindsdb/blob/stable/CODE_OF_CONDUCT.md). By participating in this project, you agree to abide by its terms.
+
+Also, check out the [rewards and community programs](https://mindsdb.com/community?utm_medium=community&utm_source=github&utm_campaign=mindsdb%20repo).
+
+
+### Current contributors
+
+<a href="https://github.com/mindsdb/mindsdb/graphs/contributors">
+  <img src="https://contributors-img.web.app/image?repo=mindsdb/mindsdb" />
+</a>
+
+Made with [contributors-img](https://contributors-img.web.app).
+
+## Subscribe to updates
+
+Join our [Slack community](https://mindsdb.com/joincommunity) and subscribe to the monthly [Developer Newsletter](https://mindsdb.com/newsletter/?utm_medium=community&utm_source=github&utm_campaign=mindsdb%20repo) to get product updates, information about MindsDB events and contests, and useful content, like tutorials.
+
+
+## License
+
+MindsDB is licensed under [GNU General Public License v3.0](https://github.com/mindsdb/mindsdb/blob/master/LICENSE)
```

#### html2text {}

```diff
@@ -1,100 +1,100 @@
-Metadata-Version: 2.1 Name: MindsDB Version: 23.5.4.1 Summary: MindsDB server,
-provides server capabilities to mindsdb native python library Home-page: https:
-//github.com/mindsdb/mindsdb Author: MindsDB Inc Author-email:
-jorge@mindsdb.com License: GPL-3.0 Download-URL: https://pypi.org/project/
-mindsdb/ Description:
                                ****** [MindsDB]
                                      ******
       [ROSS_Index_-_Fastest_Growing_Open-Source_Startups_|_Runa_Capital]
              [MindsDB_workflow] [Python_supported] [PyPi_Version]
   [PyPI - Downloads] [Docker_pulls] [https://shields.io/endpoint?url=https://
         ossrank.com/shield/630] [MindsDB_Website] [MindsDB_Community]
                              [Launch_in_Deepnote]
                                [Open_in_Gitpod]
 **** Website  |  Docs  |  Community_Slack  |  Contribute  |  Demo  |  Hackathon
                                      ****
 ---------------------------------------- [MindsDB](https://
 mindsdb.com?utm_medium=community&utm_source=github&utm_campaign=mindsdb%20repo)
-is an emerging low-code machine learning platform to help developers easily
-build #AI-powered solutions [![Tweet](https://img.shields.io/twitter/url/http/
+is a Server for Artificial Intelligence Logic, enabling developers to ship AI
+powered projects from prototyping & experimentation to production in a fast &
+scalable way. [![Tweet](https://img.shields.io/twitter/url/http/
 shields.io.svg?style=social)](https://twitter.com/intent/tweet?text=Build%20AI-
-Powered%20Applications%20&url=https://
+Centered%20Applications%20&url=https://
 www.mindsdb.com&via=mindsdb&hashtags=ai,ml,nlp,machine_learning,neural_networks,databases,gpt3)
-**NEW!** Check-out the [rewards and community programs.](https://mindsdb.com/
-community?utm_medium=community&utm_source=github&utm_campaign=mindsdb%20repo) -
---------------------------------------- [Installation](https://github.com/
+We do this by abstracting Generative AI, Large Language and other Models as a
+virtual tables ([AI Tables](https://www.youtube.com/watch?v=tnB4Y9T1E2k)) on
+top of enterprise databases. This increases accessibility with organizations
+and enables development teams to use their existing skills to build
+applications powered by AI. By taking a data-centric approach to AI MindsDB
+brings the process closer to the source of the data minimizing the need to
+build and maintain data pipelines and ETLâing, speeding up the time to
+deployment and reducing complexity. **P.S. If you like our open-source project
+we'd appreciate if you star it on GitHub â­!**
+                                    *****
+
+                                [MindsDB] *****
+---------------------------------------- MindsDB has an active and helpful
+community. Feel free to join our [Slack](https://mindsdb.com/joincommunity) and
+check-out the [rewards and community programs](https://mindsdb.com/
+community?utm_medium=community&utm_source=github&utm_campaign=mindsdb%20repo).
+---------------------------------------- [Installation](https://github.com/
 mindsdb/mindsdb#installation) - [Overview](https://github.com/mindsdb/
 mindsdb#overview) - [Features](https://github.com/mindsdb/mindsdb#features) -
 [Database Integrations](https://github.com/mindsdb/mindsdb#database-
 integrations) - [Quickstart](https://github.com/mindsdb/mindsdb#quickstart) -
 [Documentation](https://github.com/mindsdb/mindsdb#documentation) - [Support]
 (https://github.com/mindsdb/mindsdb#support) - [Contributing](https://
 github.com/mindsdb/mindsdb#contributing) - [Mailing lists](https://github.com/
 mindsdb/mindsdb#mailing-lists) - [License](https://github.com/mindsdb/
-mindsdb#license) ---------------------------- MindsDB automates and integrates
-top machine learning frameworks (including GPT-4) into the data stack as "AI
-Tables" to streamline the integration of AI into applications, making it
-accessible to developers of all skill levels. "[AI tables](https://
-www.youtube.com/watch?v=tnB4Y9T1E2k)" allow you to get predictions via SQL
-queries and continuously learn from your data.
-                                    *****
-
-                                [MindsDB] *****
-## Use cases Here are some popular use cases you can build with MindsDB: *
-Conversational AI: Leverage MindsDB native integrations with data platforms and
-pre-trained large language models, like OpenAI's GPT, to quickly build
-conversational AI solutions without the overhead of managing complex data
-pipelines. * Fraud Detection: MindsDB can help developers build models to
-detect fraudulent activity in financial transactions, eCommerce platforms etc.
-* Sales Forecasting: MindsDB can be used to develop models to predict future
-sales based on historical sales data, allowing businesses to make better-
-informed decisions. * Customer Segmentation: MindsDB can help developers
-segment customers based on their behavior, preferences, and other factors,
-allowing businesses to tailor their marketing efforts. * Sentiment analysis:
-MindsDB native integration with pre-trained models like OpenAI GPT or Hugging
-Face can be used to analyze the sentiment of a text data, such as a customer
-reviews - in a single command, instead of individual API calls and ETL-ing
-data. * Predictive Maintenance: MindsDB can be used to build models to predict
-when equipment or machinery is likely to fail, allowing for proactive
-maintenance and minimizing downtime. See more examples and community tutorials
-[here](https://docs.mindsdb.com/tutorials) ## Demo You can try MindsDB using
-our [demo environment](https://cloud.mindsdb.com/
+mindsdb#license) ---------------------------------------- ## Use cases Here are
+some popular use cases you can build with MindsDB: * Conversational AI:
+Leverage MindsDB native integrations with data platforms and pre-trained large
+language models, like OpenAI's GPT, to quickly build conversational AI
+solutions without the overhead of managing complex data pipelines. * Fraud
+Detection: MindsDB can help developers build models to detect fraudulent
+activity in financial transactions, eCommerce platforms etc. * Sales
+Forecasting: MindsDB can be used to develop models to predict future sales
+based on historical sales data, allowing businesses to make better-informed
+decisions. * Customer Segmentation: MindsDB can help developers segment
+customers based on their behavior, preferences, and other factors, allowing
+businesses to tailor their marketing efforts. * Sentiment analysis: MindsDB
+native integration with pre-trained models like OpenAI GPT or Hugging Face can
+be used to analyze the sentiment of a text data, such as a customer reviews -
+in a single command, instead of individual API calls and ETL-ing data. *
+Predictive Maintenance: MindsDB can be used to build models to predict when
+equipment or machinery is likely to fail, allowing for proactive maintenance
+and minimizing downtime. See more examples and community tutorials [here]
+(https://docs.mindsdb.com/tutorials). ## Demo You can try MindsDB using our
+[demo environment](https://cloud.mindsdb.com/
 ?utm_medium=community&utm_source=github&utm_campaign=mindsdb%20repo) with
 sample data for most popular use cases. ## Installation The prefered way is to
 use MindsDB Cloud [free demo instance](https://cloud.mindsdb.com/home) or use a
 [dedicated instance](https://cloud.mindsdb.com/home). If you want to move to
 production use [the AWS AMI image](https://aws.amazon.com/marketplace/seller-
-profile?id=03a65520-86ca-4ab8-a394-c11eb54573a9)/ To install locally or on-
+profile?id=03a65520-86ca-4ab8-a394-c11eb54573a9). To install locally or on-
 premise pull the latest Docker image: ``` docker pull mindsdb/mindsdb ``` ##
-How it works 1. First, CONNECT MindsDB to your data platform. We support 70+
-data platforms and this list is constantly growing. If you canât find the
+How it works 1. CONNECT MindsDB to your data platform. We support 100+ data
+platforms and this list is constantly growing. If you canât find the
 integration you need, please [let us know](https://mindsdb.com/joincommunity).
-2. Run the CREATE MODEL query pointing to your data table or a view, that will
-automatically create and deploy a machine learning model as an [AI Table]
-(https://www.youtube.com/watch?v=tnB4Y9T1E2k). 1. If you have an NLP use case,
-CREATE MODEL will integrate the [AI Table](https://www.youtube.com/
-watch?v=tnB4Y9T1E2k) with already pre-trained model you choose (like OpenAIâs
-GPT-3 or Hugging Face models). 2. Please check the [docs](https://
-docs.mindsdb.com/sql/create/
-predictor?utm_medium=community&utm_source=github&utm_campaign=mindsdb%20repo)
-if you want to have manual control over model engineering. 3. JOIN the model
-with your database tables to make predictions for thousands or even millions of
-data points at once, or run SELECT statements or API calls to make one time
-predictions. 4. Set up a JOB to automate your model re-training cycle and
-predictions pipelines for the new incoming data. Follow the [quickstart guide]
-(https://docs.mindsdb.com/
+2. CREATE MODEL to connect the AI Engine you pick that will learn from your
+data and serve it as [AI Table](https://www.youtube.com/watch?v=tnB4Y9T1E2k).
+1. If you have an NLP use case, CREATE MODEL will integrate the [AI Table]
+(https://www.youtube.com/watch?v=tnB4Y9T1E2k) with already pre-trained model
+you choose (like OpenAIâs GPT or Hugging Face models). 2. Please check the
+[docs](https://docs.mindsdb.com/sql/create/
+model?utm_medium=community&utm_source=github&utm_campaign=mindsdb%20repo) if
+you want to have manual control over model engineering. 3. JOIN such model with
+your database tables to make predictions for thousands or even millions of data
+points at once, or run SELECT statements or API calls to make one time
+predictions. 4. Set up a JOB to automate your re-training cycle and predictions
+pipelines for the new incoming data. 5. Alternatively, use REST API to query
+the models Follow the [quickstart guide](https://docs.mindsdb.com/
 quickstart?utm_medium=community&utm_source=github&utm_campaign=mindsdb%20repo)
 with sample data to get on-boarded as fast as possible. ## Database
-Integrations MindsDB works with most of the SQL and NoSQL databases, data
-lakes, data Streams and popular applications. | Connect your Data | Connect
-your Data | Connect your Data |-|-|-| | [Connect_Apache_Kafka] | [Connect
-Microsoft_Access] | [Oracle_Badge] | | [Connect_Amazon_Redshift] | [Airtable
-Badge] | [Pinot_Badge] | | [Connect_Cassandra] | [DataStax_Badge] | [Amazon_S3
-Badge] | | [Connect_CockroachDB] | [ckan_Badge] | [Supabase_Badge] | | [Connect
+Integrations MindsDB works with most of the SQL and NoSQL databases, data lakes
+and popular applications. | Connect your Data | Connect your Data | Connect
+your Data |-|-|-| | [Connect_Amazon_Redshift] | [Airtable_Badge] | [Pinot
+Badge] | | [Connect_Cassandra] | [DataStax_Badge] | [Amazon_S3_Badge] | |
+[Connect_CockroachDB] | [ckan_Badge] | [Supabase_Badge] | | [Connect
 Clickhouse] | [Google_Big_Query_Badge] | [SQLite_Badge] | | [Connect_MariaDB] |
 [Couchbase_Badge] | [TiDB_Badge] | | [Connect_SQL_Server] | [CrateDB_Badge] |
 [Timescale_Badge] | | [Connect_MongoDB] | [DoIt_Badge] | [Amazon_DynamoDB
 Badge] | | [Connect_PostgreSQL] | [IBMDB2_Badge] | [openGauss_Badge] | |
 [Connect_MySQL] | [Databricks_Badge] | [YugabyteDB_Badge] | [Connect_QuestDB] |
 [Apache_Druid_Badge] | | [StarRocks_Badge] | [Vertica_Badge] | [DuckDB_Badge] |
 | [Connect_SAP_HANA] | [Elastic_Badge] | [Cloud_Spanner_Badge] | | [Connect
@@ -104,25 +104,24 @@
 integration?](https://github.com/mindsdb/mindsdb/issues/
 new?assignees=&labels=&template=feature-mindsdb-request.yaml) ## Documentation
 You can find the complete documentation of MindsDB at [docs.mindsdb.com](https:
 //
 docs.mindsdb.com?utm_medium=community&utm_source=github&utm_campaign=mindsdb%20repo).
 ## Support If you found a bug, please submit an [issue on GitHub](https://
 github.com/mindsdb/mindsdb/issues/new/choose). To get community support, you
-can: * Post at MindsDB [Slack community](https://mindsdb.com/joincommunity). *
-Ask for help at our [GitHub Discussions](https://github.com/mindsdb/mindsdb/
-discussions). * Ask a question at [Stackoverflow](https://stackoverflow.com/
-questions/tagged/mindsdb) with a MindsDB tag. If you need commercial support,
-please [contact](https://mindsdb.com/contact/
+can: * Post a question at MindsDB [Slack community](https://mindsdb.com/
+joincommunity). * Ask for help at our [GitHub Discussions](https://github.com/
+mindsdb/mindsdb/discussions). * Ask a question at [Stackoverflow](https://
+stackoverflow.com/questions/tagged/mindsdb) with a MindsDB tag. If you need
+commercial support, please [contact](https://mindsdb.com/contact/
 ?utm_medium=community&utm_source=github&utm_campaign=mindsdb%20repo) MindsDB
 team. ## Contributing A great place to start contributing to MindsDB is to
-check our GitHub projects :checkered_flag: * Tutorials & documentation
-[dashboard tasks](https://github.com/mindsdb/mindsdb/projects/7). * Code
-contributor's [dashboard tasks](https://github.com/mindsdb/mindsdb/projects/8).
-* [First timers only issues](https://github.com/mindsdb/mindsdb/
+check our GitHub projects :checkered_flag: * Community contributor's [dashboard
+tasks](https://github.com/mindsdb/mindsdb/projects/8). * [First timers only
+issues](https://github.com/mindsdb/mindsdb/
 issues?q=is%3Aissue+is%3Aopen+label%3Afirst-timers-only), if this is your first
 time contributing to an open source project. We are always open to suggestions
 so feel free to open new issues with your ideas and we can guide you! Being
 part of the core team is accessible to anyone who is motivated and wants to be
 part of that journey! If you'd like to contribute to the project, refer to the
 [contributing documentation](https://docs.mindsdb.com/contribute/
 ?utm_medium=community&utm_source=github&utm_campaign=mindsdb%20repo). Please
@@ -136,10 +135,7 @@
 Subscribe to updates Join our [Slack community](https://mindsdb.com/
 joincommunity) and subscribe to the monthly [Developer Newsletter](https://
 mindsdb.com/newsletter/
 ?utm_medium=community&utm_source=github&utm_campaign=mindsdb%20repo) to get
 product updates, information about MindsDB events and contests, and useful
 content, like tutorials. ## License MindsDB is licensed under [GNU General
 Public License v3.0](https://github.com/mindsdb/mindsdb/blob/master/LICENSE)
-Platform: UNKNOWN Classifier: Programming Language :: Python :: 3 Classifier:
-Operating System :: OS Independent Requires-Python: >=3.8 Description-Content-
-Type: text/markdown
```

### Comparing `MindsDB-23.5.4.1/MindsDB.egg-info/SOURCES.txt` & `MindsDB-23.6.1.1/MindsDB.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -27,30 +27,28 @@
 mindsdb/api/http/namespaces/databases.py
 mindsdb/api/http/namespaces/default.py
 mindsdb/api/http/namespaces/file.py
 mindsdb/api/http/namespaces/handlers.py
 mindsdb/api/http/namespaces/models.py
 mindsdb/api/http/namespaces/projects.py
 mindsdb/api/http/namespaces/sql.py
-mindsdb/api/http/namespaces/stream.py
 mindsdb/api/http/namespaces/tab.py
 mindsdb/api/http/namespaces/tree.py
 mindsdb/api/http/namespaces/util.py
 mindsdb/api/http/namespaces/views.py
 mindsdb/api/http/namespaces/configs/__init__.py
 mindsdb/api/http/namespaces/configs/analysis.py
 mindsdb/api/http/namespaces/configs/auth.py
 mindsdb/api/http/namespaces/configs/config.py
 mindsdb/api/http/namespaces/configs/databases.py
 mindsdb/api/http/namespaces/configs/default.py
 mindsdb/api/http/namespaces/configs/files.py
 mindsdb/api/http/namespaces/configs/handlers.py
 mindsdb/api/http/namespaces/configs/projects.py
 mindsdb/api/http/namespaces/configs/sql.py
-mindsdb/api/http/namespaces/configs/streams.py
 mindsdb/api/http/namespaces/configs/tabs.py
 mindsdb/api/http/namespaces/configs/tree.py
 mindsdb/api/http/namespaces/configs/util.py
 mindsdb/api/mongo/__init__.py
 mindsdb/api/mongo/server.py
 mindsdb/api/mongo/start.py
 mindsdb/api/mongo/classes/__init__.py
@@ -269,14 +267,19 @@
 mindsdb/integrations/handlers/cloud_sql_handler/tests/test_cloud_sql_mysql_handler.py
 mindsdb/integrations/handlers/cockroach_handler/__about__.py
 mindsdb/integrations/handlers/cockroach_handler/__init__.py
 mindsdb/integrations/handlers/cockroach_handler/cockroach_handler.py
 mindsdb/integrations/handlers/cockroach_handler/requirements.txt
 mindsdb/integrations/handlers/cockroach_handler/tests/__init__.py
 mindsdb/integrations/handlers/cockroach_handler/tests/test_cockroachdb_handler.py
+mindsdb/integrations/handlers/cohere_handler/__about__.py
+mindsdb/integrations/handlers/cohere_handler/__init__.py
+mindsdb/integrations/handlers/cohere_handler/cohere_handler.py
+mindsdb/integrations/handlers/cohere_handler/requirements.txt
+mindsdb/integrations/handlers/cohere_handler/setup.py
 mindsdb/integrations/handlers/confluence_handler/__about__.py
 mindsdb/integrations/handlers/confluence_handler/__init__.py
 mindsdb/integrations/handlers/confluence_handler/confluence_handler.py
 mindsdb/integrations/handlers/confluence_handler/confluence_table.py
 mindsdb/integrations/handlers/confluence_handler/icon.png
 mindsdb/integrations/handlers/confluence_handler/requirements.txt
 mindsdb/integrations/handlers/couchbase_handler/__about__.py
@@ -402,14 +405,19 @@
 mindsdb/integrations/handlers/firebird_handler/__about__.py
 mindsdb/integrations/handlers/firebird_handler/__init__.py
 mindsdb/integrations/handlers/firebird_handler/firebird_handler.py
 mindsdb/integrations/handlers/firebird_handler/icon.png
 mindsdb/integrations/handlers/firebird_handler/requirements.txt
 mindsdb/integrations/handlers/firebird_handler/tests/__init__.py
 mindsdb/integrations/handlers/firebird_handler/tests/test_firebird_handler.py
+mindsdb/integrations/handlers/flaml_handler/__about__.py
+mindsdb/integrations/handlers/flaml_handler/__init__.py
+mindsdb/integrations/handlers/flaml_handler/flaml_handler.py
+mindsdb/integrations/handlers/flaml_handler/requirements.txt
+mindsdb/integrations/handlers/flaml_handler/setup.py
 mindsdb/integrations/handlers/frappe_handler/__about__.py
 mindsdb/integrations/handlers/frappe_handler/__init__.py
 mindsdb/integrations/handlers/frappe_handler/frappe_client.py
 mindsdb/integrations/handlers/frappe_handler/frappe_handler.py
 mindsdb/integrations/handlers/frappe_handler/frappe_tables.py
 mindsdb/integrations/handlers/frappe_handler/icon.svg
 mindsdb/integrations/handlers/frappe_handler/requirements.txt
@@ -556,32 +564,30 @@
 mindsdb/integrations/handlers/lightwood_handler/lightwood_handler/__about__.py
 mindsdb/integrations/handlers/lightwood_handler/lightwood_handler/__init__.py
 mindsdb/integrations/handlers/lightwood_handler/lightwood_handler/functions.py
 mindsdb/integrations/handlers/lightwood_handler/lightwood_handler/lightwood_handler.py
 mindsdb/integrations/handlers/lightwood_handler/lightwood_handler/utils.py
 mindsdb/integrations/handlers/lightwood_handler/tests/__init__.py
 mindsdb/integrations/handlers/lightwood_handler/tests/test_lightwood_handler.py
+mindsdb/integrations/handlers/llama_index_handler/__about__.py
+mindsdb/integrations/handlers/llama_index_handler/__init__.py
+mindsdb/integrations/handlers/llama_index_handler/llama_index_handler.py
+mindsdb/integrations/handlers/llama_index_handler/requirements.txt
+mindsdb/integrations/handlers/llama_index_handler/setup.py
 mindsdb/integrations/handlers/ludwig_handler/__about__.py
 mindsdb/integrations/handlers/ludwig_handler/__init__.py
 mindsdb/integrations/handlers/ludwig_handler/functions.py
 mindsdb/integrations/handlers/ludwig_handler/ludwig_handler.py
 mindsdb/integrations/handlers/ludwig_handler/requirements.txt
 mindsdb/integrations/handlers/ludwig_handler/setup.py
 mindsdb/integrations/handlers/ludwig_handler/utils.py
-mindsdb/integrations/handlers/mariadb_handler/1-create_db.png
-mindsdb/integrations/handlers/mariadb_handler/2-create_predictor.png
-mindsdb/integrations/handlers/mariadb_handler/3-predict_target.png
-mindsdb/integrations/handlers/mariadb_handler/4-drop_db.png
 mindsdb/integrations/handlers/mariadb_handler/__about__.py
 mindsdb/integrations/handlers/mariadb_handler/__init__.py
-mindsdb/integrations/handlers/mariadb_handler/create-db.png
 mindsdb/integrations/handlers/mariadb_handler/icon.svg
 mindsdb/integrations/handlers/mariadb_handler/mariadb_handler.py
-mindsdb/integrations/handlers/mariadb_handler/predict-db.png
-mindsdb/integrations/handlers/mariadb_handler/predictor.png
 mindsdb/integrations/handlers/mariadb_handler/requirements.txt
 mindsdb/integrations/handlers/materialize_handler/__about__.py
 mindsdb/integrations/handlers/materialize_handler/__init__.py
 mindsdb/integrations/handlers/materialize_handler/icon.png
 mindsdb/integrations/handlers/materialize_handler/materialize_handler.py
 mindsdb/integrations/handlers/materialize_handler/requirements.txt
 mindsdb/integrations/handlers/materialize_handler/tests/__init__.py
@@ -626,14 +632,19 @@
 mindsdb/integrations/handlers/mongodb_handler/__about__.py
 mindsdb/integrations/handlers/mongodb_handler/__init__.py
 mindsdb/integrations/handlers/mongodb_handler/icon.svg
 mindsdb/integrations/handlers/mongodb_handler/mongodb_handler.py
 mindsdb/integrations/handlers/mongodb_handler/requirements.txt
 mindsdb/integrations/handlers/mongodb_handler/utils/__init__.py
 mindsdb/integrations/handlers/mongodb_handler/utils/mongodb_render.py
+mindsdb/integrations/handlers/monkeylearn_handler/__about__.py
+mindsdb/integrations/handlers/monkeylearn_handler/__init__.py
+mindsdb/integrations/handlers/monkeylearn_handler/monkeylearn_handler.py
+mindsdb/integrations/handlers/monkeylearn_handler/requirements.txt
+mindsdb/integrations/handlers/monkeylearn_handler/setup.py
 mindsdb/integrations/handlers/mssql_handler/__about__.py
 mindsdb/integrations/handlers/mssql_handler/__init__.py
 mindsdb/integrations/handlers/mssql_handler/icon.png
 mindsdb/integrations/handlers/mssql_handler/mssql_handler.py
 mindsdb/integrations/handlers/mssql_handler/requirements.txt
 mindsdb/integrations/handlers/mssql_handler/tests/__init__.py
 mindsdb/integrations/handlers/mssql_handler/tests/test_mssql_handler.py
@@ -690,14 +701,20 @@
 mindsdb/integrations/handlers/orioledb_handler/__about__.py
 mindsdb/integrations/handlers/orioledb_handler/__init__.py
 mindsdb/integrations/handlers/orioledb_handler/icon.svg
 mindsdb/integrations/handlers/orioledb_handler/orioledb_handler.py
 mindsdb/integrations/handlers/orioledb_handler/requirements.txt
 mindsdb/integrations/handlers/orioledb_handler/tests/__init__.py
 mindsdb/integrations/handlers/orioledb_handler/tests/test_orioledb_handler.py
+mindsdb/integrations/handlers/paypal_handler/__about__.py
+mindsdb/integrations/handlers/paypal_handler/__init__.py
+mindsdb/integrations/handlers/paypal_handler/icon.png
+mindsdb/integrations/handlers/paypal_handler/paypal_handler.py
+mindsdb/integrations/handlers/paypal_handler/paypal_tables.py
+mindsdb/integrations/handlers/paypal_handler/requirements.txt
 mindsdb/integrations/handlers/phoenix_handler/__about__.py
 mindsdb/integrations/handlers/phoenix_handler/__init__.py
 mindsdb/integrations/handlers/phoenix_handler/icon.png
 mindsdb/integrations/handlers/phoenix_handler/phoenix_handler.py
 mindsdb/integrations/handlers/phoenix_handler/requirements.txt
 mindsdb/integrations/handlers/phoenix_handler/tests/__init__.py
 mindsdb/integrations/handlers/phoenix_handler/tests/test_phoenix_handler.py
@@ -760,15 +777,14 @@
 mindsdb/integrations/handlers/redshift_handler/requirements.txt
 mindsdb/integrations/handlers/redshift_handler/tests/__init__.py
 mindsdb/integrations/handlers/redshift_handler/tests/test_redshift_handler.py
 mindsdb/integrations/handlers/rocket_chat_handler/__about__.py
 mindsdb/integrations/handlers/rocket_chat_handler/__init__.py
 mindsdb/integrations/handlers/rocket_chat_handler/icon.svg
 mindsdb/integrations/handlers/rocket_chat_handler/requirements.txt
-mindsdb/integrations/handlers/rocket_chat_handler/rocket_chat_client.py
 mindsdb/integrations/handlers/rocket_chat_handler/rocket_chat_handler.py
 mindsdb/integrations/handlers/rocket_chat_handler/rocket_chat_tables.py
 mindsdb/integrations/handlers/rockset_handler/icon.png
 mindsdb/integrations/handlers/rockset_handler/requirements.txt
 mindsdb/integrations/handlers/rockset_handler/tests/test.png
 mindsdb/integrations/handlers/rockset_handler/tests/test2.png
 mindsdb/integrations/handlers/s3_handler/__about__.py
@@ -800,15 +816,14 @@
 mindsdb/integrations/handlers/sheets_handler/tests/test_sheets_handler.py
 mindsdb/integrations/handlers/shopify_handler/__about__.py
 mindsdb/integrations/handlers/shopify_handler/__init__.py
 mindsdb/integrations/handlers/shopify_handler/icon.png
 mindsdb/integrations/handlers/shopify_handler/requirements.txt
 mindsdb/integrations/handlers/shopify_handler/shopify_handler.py
 mindsdb/integrations/handlers/shopify_handler/shopify_tables.py
-mindsdb/integrations/handlers/shopify_handler/utils.py
 mindsdb/integrations/handlers/singlestore_handler/__about__.py
 mindsdb/integrations/handlers/singlestore_handler/__init__.py
 mindsdb/integrations/handlers/singlestore_handler/requirements.txt
 mindsdb/integrations/handlers/singlestore_handler/singlestore_handler.py
 mindsdb/integrations/handlers/singlestore_handler/tests/__init__.py
 mindsdb/integrations/handlers/singlestore_handler/tests/test_singlestore_handler.py
 mindsdb/integrations/handlers/slack_handler/__about__.py
@@ -868,14 +883,22 @@
 mindsdb/integrations/handlers/statsforecast_handler/statsforecast_handler.py
 mindsdb/integrations/handlers/strava_handler/__about__.py
 mindsdb/integrations/handlers/strava_handler/__init__.py
 mindsdb/integrations/handlers/strava_handler/icon.png
 mindsdb/integrations/handlers/strava_handler/requirements.txt
 mindsdb/integrations/handlers/strava_handler/strava_handler.py
 mindsdb/integrations/handlers/strava_handler/strava_tables.py
+mindsdb/integrations/handlers/stripe_handler/__about__.py
+mindsdb/integrations/handlers/stripe_handler/__init__.py
+mindsdb/integrations/handlers/stripe_handler/icon.png
+mindsdb/integrations/handlers/stripe_handler/requirements.txt
+mindsdb/integrations/handlers/stripe_handler/stripe_handler.py
+mindsdb/integrations/handlers/stripe_handler/stripe_tables.py
+mindsdb/integrations/handlers/stripe_handler/query_handlers/__init__.py
+mindsdb/integrations/handlers/stripe_handler/query_handlers/select_query_handlers.py
 mindsdb/integrations/handlers/supabase_handler/__about__.py
 mindsdb/integrations/handlers/supabase_handler/__init__.py
 mindsdb/integrations/handlers/supabase_handler/icon.svg
 mindsdb/integrations/handlers/supabase_handler/requirements.txt
 mindsdb/integrations/handlers/supabase_handler/supabase_handler.py
 mindsdb/integrations/handlers/supabase_handler/tests/__init__.py
 mindsdb/integrations/handlers/supabase_handler/tests/test_supabase_handler.py
@@ -927,14 +950,17 @@
 mindsdb/integrations/handlers/trino_handler/tests/__init__.py
 mindsdb/integrations/handlers/trino_handler/tests/test_trino_handler.py
 mindsdb/integrations/handlers/twitter_handler/__about__.py
 mindsdb/integrations/handlers/twitter_handler/__init__.py
 mindsdb/integrations/handlers/twitter_handler/icon.svg
 mindsdb/integrations/handlers/twitter_handler/requirements.txt
 mindsdb/integrations/handlers/twitter_handler/twitter_handler.py
+mindsdb/integrations/handlers/utilities/__init__.py
+mindsdb/integrations/handlers/utilities/query_utilities/__init__.py
+mindsdb/integrations/handlers/utilities/query_utilities/select_query_utilities.py
 mindsdb/integrations/handlers/vertica_handler/__about__.py
 mindsdb/integrations/handlers/vertica_handler/__init__.py
 mindsdb/integrations/handlers/vertica_handler/icon.svg
 mindsdb/integrations/handlers/vertica_handler/requirements.txt
 mindsdb/integrations/handlers/vertica_handler/vertica_handler.py
 mindsdb/integrations/handlers/vertica_handler/tests/__init__.py
 mindsdb/integrations/handlers/vertica_handler/tests/test_vertica_handler.py
@@ -1006,18 +1032,14 @@
 mindsdb/interfaces/storage/json.py
 mindsdb/interfaces/storage/model_fs.py
 mindsdb/interfaces/stream/__init__.py
 mindsdb/interfaces/stream/stream.py
 mindsdb/interfaces/stream/utilities.py
 mindsdb/interfaces/stream/base/__init__.py
 mindsdb/interfaces/stream/base/integration.py
-mindsdb/interfaces/stream/kafka/__init__.py
-mindsdb/interfaces/stream/kafka/kafkadb.py
-mindsdb/interfaces/stream/redis/__init__.py
-mindsdb/interfaces/stream/redis/redisdb.py
 mindsdb/microservices_grpc/__init__.py
 mindsdb/microservices_grpc/db/__init__.py
 mindsdb/microservices_grpc/db/common_pb2.py
 mindsdb/microservices_grpc/db/common_pb2_grpc.py
 mindsdb/microservices_grpc/db/db_pb2.py
 mindsdb/microservices_grpc/db/db_pb2_grpc.py
 mindsdb/microservices_grpc/executor/__init__.py
@@ -1051,14 +1073,16 @@
 mindsdb/migrations/versions/2022-11-11_d429095b570f_data_integration_id.py
 mindsdb/migrations/versions/2022-12-26_459218b0844c_fix_unique_constraint.py
 mindsdb/migrations/versions/2023-02-02_b6d0a47294ac_jobs.py
 mindsdb/migrations/versions/2023-02-17_ee63d868fa84_predictor_integration_null.py
 mindsdb/migrations/versions/2023-02-25_3154382dab17_training_progress.py
 mindsdb/migrations/versions/2023-02-27_ef04cdbe51ed_jobs_user_class.py
 mindsdb/migrations/versions/2023-04-11_b8be148dbc85_jobs_history_query.py
+mindsdb/migrations/versions/2023-05-24_6d748f2c7b0b_remove_streams.py
+mindsdb/migrations/versions/2023-05-31_aaecd7012a78_chatbot.py
 mindsdb/migrations/versions/__init__.py
 mindsdb/utilities/__init__.py
 mindsdb/utilities/auth.py
 mindsdb/utilities/cache.py
 mindsdb/utilities/config.py
 mindsdb/utilities/context.py
 mindsdb/utilities/fs.py
```

### Comparing `MindsDB-23.5.4.1/PKG-INFO` & `MindsDB-23.6.1.1/MindsDB.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MindsDB
-Version: 23.5.4.1
+Version: 23.6.1.1
 Summary: MindsDB server, provides server capabilities to mindsdb native python library
 Home-page: https://github.com/mindsdb/mindsdb
 Author: MindsDB Inc
 Author-email: jorge@mindsdb.com
 License: GPL-3.0
 Download-URL: https://pypi.org/project/mindsdb/
 Description: <h1 align="center">
@@ -32,15 +32,15 @@
         	<a href="https://github.com/mindsdb/mindsdb/actions"><img src="https://github.com/mindsdb/mindsdb/workflows/MindsDB%20workflow/badge.svg" alt="MindsDB workflow"></a>
         	<a href="https://www.python.org/downloads/" target="_blank"><img src="https://img.shields.io/badge/python-3.7.x%20|%203.8.x|%203.9.x-brightgreen.svg" alt="Python supported"></a>
         	<a href="https://pypi.org/project/MindsDB/" target="_blank"><img src="https://badge.fury.io/py/MindsDB.svg" alt="PyPi Version"></a>
         	<br />
         	<img alt="PyPI - Downloads" src="https://img.shields.io/pypi/dm/Mindsdb">  <a href="https://hub.docker.com/u/mindsdb" target="_blank"><img src="https://img.shields.io/docker/pulls/mindsdb/mindsdb" alt="Docker pulls"></a>
         	<a href="https://ossrank.com/p/630"><img src="https://shields.io/endpoint?url=https://ossrank.com/shield/630"></a>
         	<a href="https://www.mindsdb.com/"><img src="https://img.shields.io/website?url=https%3A%2F%2Fwww.mindsdb.com%2F" alt="MindsDB Website"></a>
-        	<a href="https://join.slack.com/t/mindsdbcommunity/shared_invite/zt-o8mrmx3l-5ai~5H66s6wlxFfBMVI6wQ" target="_blank"><img src="https://img.shields.io/badge/slack-@mindsdbcommunity-brightgreen.svg?logo=slack " alt="MindsDB Community"></a>
+        	<a href="https://mindsdb.com/joincommunity" target="_blank"><img src="https://img.shields.io/badge/slack-@mindsdbcommunity-brightgreen.svg?logo=slack " alt="MindsDB Community"></a>
         	<br />
         	<a href="https://deepnote.com/project/Machine-Learning-With-SQL-8GDF7bc7SzKlhBLorqoIcw/%2Fmindsdb_demo.ipynb" target="_blank"><img src="https://deepnote.com/buttons/launch-in-deepnote-white.svg" alt="Launch in Deepnote"></a>
         	<br />
         	<a href="https://gitpod.io/#https://github.com/mindsdb/mindsdb" target="_blank"><img src="https://gitpod.io/button/open-in-gitpod.svg" alt="Open in Gitpod"></a>
         </p>
         
         <h3 align="center">
@@ -57,81 +57,84 @@
         	<a href="https://hashnode.com/hackathons/mindsdb?source=hncounter-feed">Hackathon</a>
         </h3>
         
         </div>
         
         ----------------------------------------
         
-        [MindsDB](https://mindsdb.com?utm_medium=community&utm_source=github&utm_campaign=mindsdb%20repo) is an emerging low-code machine learning platform to help developers easily build #AI-powered solutions [![Tweet](https://img.shields.io/twitter/url/http/shields.io.svg?style=social)](https://twitter.com/intent/tweet?text=Build%20AI-Powered%20Applications%20&url=https://www.mindsdb.com&via=mindsdb&hashtags=ai,ml,nlp,machine_learning,neural_networks,databases,gpt3)
+        [MindsDB](https://mindsdb.com?utm_medium=community&utm_source=github&utm_campaign=mindsdb%20repo) is a Server for Artificial Intelligence Logic, enabling developers to ship AI powered projects from prototyping & experimentation to production in a fast & scalable way. [![Tweet](https://img.shields.io/twitter/url/http/shields.io.svg?style=social)](https://twitter.com/intent/tweet?text=Build%20AI-Centered%20Applications%20&url=https://www.mindsdb.com&via=mindsdb&hashtags=ai,ml,nlp,machine_learning,neural_networks,databases,gpt3)
         
+        We do this by abstracting Generative AI, Large Language and other Models as a virtual tables ([AI Tables](https://www.youtube.com/watch?v=tnB4Y9T1E2k)) on top of enterprise databases. This increases accessibility with organizations and enables development teams to use their existing skills to build applications powered by AI.
         
-        **NEW!** Check-out the [rewards and community programs.](https://mindsdb.com/community?utm_medium=community&utm_source=github&utm_campaign=mindsdb%20repo)
+        By taking a data-centric approach to AI MindsDB brings the process closer to the source of the data minimizing the need to build and maintain data pipelines and ETL’ing, speeding up the time to deployment and reducing complexity.
         
-        ----------------------------------------
-        
-        [Installation](https://github.com/mindsdb/mindsdb#installation) - [Overview](https://github.com/mindsdb/mindsdb#overview) - [Features](https://github.com/mindsdb/mindsdb#features) - [Database Integrations](https://github.com/mindsdb/mindsdb#database-integrations) - [Quickstart](https://github.com/mindsdb/mindsdb#quickstart) - [Documentation](https://github.com/mindsdb/mindsdb#documentation) - [Support](https://github.com/mindsdb/mindsdb#support) - [Contributing](https://github.com/mindsdb/mindsdb#contributing) - [Mailing lists](https://github.com/mindsdb/mindsdb#mailing-lists) - [License](https://github.com/mindsdb/mindsdb#license)
-        
-        ----------------------------
-        
-        MindsDB automates and integrates top machine learning frameworks (including GPT-4) into the data stack as "AI Tables" to streamline the integration of AI into applications, making it accessible to developers of all skill levels.
-        "[AI tables](https://www.youtube.com/watch?v=tnB4Y9T1E2k)" allow you to get predictions via SQL queries and continuously learn from your data.
+        **P.S. If you like our open-source project we'd appreciate if you star it on GitHub ⭐!**
         
         <h2 align="center">
            <br/>
            <br/>
-          <img width="450" src="https://docs.google.com/drawings/d/e/2PACX-1vQ1KImK0cqvZ_KpPm3SKDZF6peuM-d1lZwOkrZNpT1_PO5UVyveEIyeJGbDZFBF124LmWbHSB2HFQ97/pub?w=691&h=728" alt="MindsDB">
+          <img width="100%" src="https://github.com/mindsdb/mindsdb/assets/12409467/8418fec3-8c8b-4414-b1dc-7943041047b4" alt="MindsDB">
         
         </h2>
         
+        ----------------------------------------
+        MindsDB has an active and helpful community. Feel free to join our [Slack](https://mindsdb.com/joincommunity) and check-out the [rewards and community programs](https://mindsdb.com/community?utm_medium=community&utm_source=github&utm_campaign=mindsdb%20repo).
+        
+        ----------------------------------------
+        
+        [Installation](https://github.com/mindsdb/mindsdb#installation) - [Overview](https://github.com/mindsdb/mindsdb#overview) - [Features](https://github.com/mindsdb/mindsdb#features) - [Database Integrations](https://github.com/mindsdb/mindsdb#database-integrations) - [Quickstart](https://github.com/mindsdb/mindsdb#quickstart) - [Documentation](https://github.com/mindsdb/mindsdb#documentation) - [Support](https://github.com/mindsdb/mindsdb#support) - [Contributing](https://github.com/mindsdb/mindsdb#contributing) - [Mailing lists](https://github.com/mindsdb/mindsdb#mailing-lists) - [License](https://github.com/mindsdb/mindsdb#license)
+        
+        ----------------------------------------
+        
         ## Use cases
         
         Here are some popular use cases you can build with MindsDB:
         
         * Conversational AI: Leverage MindsDB native integrations with data platforms and pre-trained large language models, like OpenAI's GPT, to quickly build conversational AI solutions without the overhead of managing complex data pipelines.
         * Fraud Detection: MindsDB can help developers build models to detect fraudulent activity in financial transactions, eCommerce platforms etc.
         * Sales Forecasting: MindsDB can be used to develop models to predict future sales based on historical sales data, allowing businesses to make better-informed decisions.
         * Customer Segmentation: MindsDB can help developers segment customers based on their behavior, preferences, and other factors, allowing businesses to tailor their marketing efforts.
         * Sentiment analysis: MindsDB native integration with pre-trained models like OpenAI GPT or Hugging Face can be used to analyze the sentiment of a text data, such as a customer reviews - in a single command, instead of individual API calls and ETL-ing data.
         * Predictive Maintenance: MindsDB can be used to build models to predict when equipment or machinery is likely to fail, allowing for proactive maintenance and minimizing downtime.
         
-        See more examples and community tutorials [here](https://docs.mindsdb.com/tutorials)
+        See more examples and community tutorials [here](https://docs.mindsdb.com/tutorials).
         
         ## Demo
         
         You can try MindsDB using our [demo environment](https://cloud.mindsdb.com/?utm_medium=community&utm_source=github&utm_campaign=mindsdb%20repo) with sample data for most popular use cases.
         
         ## Installation
         
-        The prefered way is to use MindsDB Cloud [free demo instance](https://cloud.mindsdb.com/home) or use a [dedicated instance](https://cloud.mindsdb.com/home). If you want to move to production use [the AWS AMI image](https://aws.amazon.com/marketplace/seller-profile?id=03a65520-86ca-4ab8-a394-c11eb54573a9)/
+        The prefered way is to use MindsDB Cloud [free demo instance](https://cloud.mindsdb.com/home) or use a [dedicated instance](https://cloud.mindsdb.com/home). If you want to move to production use [the AWS AMI image](https://aws.amazon.com/marketplace/seller-profile?id=03a65520-86ca-4ab8-a394-c11eb54573a9).
         
         To install locally or on-premise pull the latest Docker image:
         
         ```
         docker pull mindsdb/mindsdb
         ```
         
         ## How it works
         
-        1. First, CONNECT MindsDB to your data platform. We support 70+ data platforms and this list is constantly growing. If you can’t find the integration you need, please [let us know](https://mindsdb.com/joincommunity).
-        2. Run the CREATE MODEL query pointing to your data table or a view, that will automatically create and deploy a machine learning model as an [AI Table](https://www.youtube.com/watch?v=tnB4Y9T1E2k).
-            1. If you have an NLP use case, CREATE MODEL will integrate the [AI Table](https://www.youtube.com/watch?v=tnB4Y9T1E2k) with already pre-trained model you choose (like OpenAI’s GPT-3 or Hugging Face models).
-            2. Please check the [docs](https://docs.mindsdb.com/sql/create/predictor?utm_medium=community&utm_source=github&utm_campaign=mindsdb%20repo) if you want to have manual control over model engineering.
-        3. JOIN the model with your database tables to make predictions for thousands or even millions of data points at once, or run SELECT statements or API calls to make one time predictions.
-        4. Set up a JOB to automate your model re-training cycle and predictions pipelines for the new incoming data.
+        1. CONNECT MindsDB to your data platform. We support 100+ data platforms and this list is constantly growing. If you can’t find the integration you need, please [let us know](https://mindsdb.com/joincommunity).
+        2. CREATE MODEL to connect the AI Engine you pick that will learn from your data and serve it as [AI Table](https://www.youtube.com/watch?v=tnB4Y9T1E2k).
+            1. If you have an NLP use case, CREATE MODEL will integrate the [AI Table](https://www.youtube.com/watch?v=tnB4Y9T1E2k) with already pre-trained model you choose (like OpenAI’s GPT or Hugging Face models).
+            2. Please check the [docs](https://docs.mindsdb.com/sql/create/model?utm_medium=community&utm_source=github&utm_campaign=mindsdb%20repo) if you want to have manual control over model engineering.
+        3. JOIN such model with your database tables to make predictions for thousands or even millions of data points at once, or run SELECT statements or API calls to make one time predictions.
+        4. Set up a JOB to automate your re-training cycle and predictions pipelines for the new incoming data.
+        5. Alternatively, use REST API to query the models
         
         Follow the [quickstart guide](https://docs.mindsdb.com/quickstart?utm_medium=community&utm_source=github&utm_campaign=mindsdb%20repo) with sample data to get on-boarded as fast as possible.
         
         
         ## Database Integrations
         
-        MindsDB works with most of the SQL and NoSQL databases, data lakes, data Streams and popular applications.
+        MindsDB works with most of the SQL and NoSQL databases, data lakes and popular applications.
         
         | Connect your Data | Connect your Data | Connect your Data
         |-|-|-|
-        | <a href="https://docs.mindsdb.com/connect/kafka"><img src="https://img.shields.io/badge/Apache Kafka-808080?style=for-the-badge&logo=apache-kafka&logoColor=white" alt="Connect Apache Kafka"></a> | <a href="https://docs.mindsdb.com/data-integrations/microsoft-access"><img src="https://img.shields.io/badge/Microsoft%20Access-A4373A?logo=microsoftaccess&logoColor=fff&style=for-the-badge" alt="Connect Microsoft Access"></a> | <a href="https://docs.mindsdb.com/data-integrations/oracle"><img src="https://img.shields.io/badge/Oracle-F80000?logo=oracle&logoColor=fff&style=for-the-badge" alt="Oracle Badge"></a> |
         | <a href="https://docs.mindsdb.com/data-integrations/amazon-redshift"><img src="https://img.shields.io/badge/Amazon%20Redshift-0466C8?style=for-the-badge&logo=amazon-aws&logoColor=white" alt="Connect Amazon Redshift"></a> | <a href="https://docs.mindsdb.com/data-integrations/airtable"><img src="https://img.shields.io/badge/Airtable-18BFFF?logo=airtable&logoColor=fff&style=for-the-badge" alt="Airtable Badge"></a> | <a href="https://docs.mindsdb.com/data-integrations/apache-pinot"><img src="https://img.shields.io/badge/Pinot-000?logo=pinot&logoColor=fff&style=for-the-badge" alt="Pinot Badge"></a> |
         | <a href="https://docs.mindsdb.com/data-integrations/apache-cassandra"><img src="https://img.shields.io/badge/Cassandra-1287B1?style=for-the-badge&logo=apache%20cassandra&logoColor=white" alt="Connect Cassandra"></a> | <a href="https://docs.mindsdb.com/data-integrations/datastax"><img src="https://img.shields.io/badge/DataStax-3A3A42?logo=datastax&logoColor=fff&style=for-the-badge" alt="DataStax Badge"></a> | <a href="https://docs.mindsdb.com/data-integrations/amazon-s3"><img src="https://img.shields.io/badge/Amazon%20S3-569A31?logo=amazons3&logoColor=fff&style=for-the-badge" alt="Amazon S3 Badge"></a> |
         | <a href="https://docs.mindsdb.com/data-integrations/cockroachdb"><img src="https://img.shields.io/badge/CockroachDB-426EDF?style=for-the-badge&logo=cockroach-labs&logoColor=white" alt="Connect CockroachDB"></a> | <a href="https://docs.mindsdb.com/data-integrations/ckan"><img src="https://img.shields.io/badge/ckan-7D929E?logo=ckan&logoColor=fff&style=for-the-badge" alt="ckan Badge"></a> | <a href="https://docs.mindsdb.com/data-integrations/supabase"><img src="https://img.shields.io/badge/Supabase-3ECF8E?logo=supabase&logoColor=fff&style=for-the-badge" alt="Supabase Badge"></a> |
         | <a href="https://docs.mindsdb.com/data-integrations/clickhouse"><img src="https://img.shields.io/badge/Clickhouse-e6e600?style=for-the-badge&logo=clickhouse&logoColor=white" alt="Connect Clickhouse"></a> | <a href="https://docs.mindsdb.com/data-integrations/google-bigquery"><img src="https://img.shields.io/badge/Google Big Query-0466C8?logo=Big Query&logoColor=fff&style=for-the-badge" alt="Google Big Query Badge"></a> | <a href="https://docs.mindsdb.com/data-integrations/sqlite"><img src="https://img.shields.io/badge/SQLite-003B57?logo=sqlite&logoColor=fff&style=for-the-badge" alt="SQLite Badge"></a> |
         | <a href="https://docs.mindsdb.com/data-integrations/mariadb"><img src="https://img.shields.io/badge/MariaDB-003545?style=for-the-badge&logo=mariadb&logoColor=white" alt="Connect MariaDB"></a> | <a href="https://docs.mindsdb.com/data-integrations/couchbase"><img src="https://img.shields.io/badge/Couchbase-EA2328?logo=couchbase&logoColor=fff&style=for-the-badge" alt="Couchbase Badge"></a> | <a href="https://docs.mindsdb.com/data-integrations/tidb#tidb-handler"><img src="https://img.shields.io/badge/TiDB-DD0031?logo=tidb&logoColor=fff&style=for-the-badge" alt="TiDB Badge"></a> |
         | <a href="https://docs.mindsdb.com/data-integrations/microsoft-sql-server"><img src="https://img.shields.io/badge/Microsoft%20SQL%20Sever-CC2927?style=for-the-badge&logo=microsoft%20sql%20server&logoColor=white" alt="Connect SQL Server"></a> | <a href="https://docs.mindsdb.com/data-integrations/cratedb"><img src="https://img.shields.io/badge/CrateDB-009DC7?logo=cratedb&logoColor=fff&style=for-the-badge" alt="CrateDB Badge"></a> | <a href=" https://docs.mindsdb.com/data-integrations/timescaledb"><img src="https://img.shields.io/badge/Timescale-FDB515?logo=timescale&logoColor=fff&style=for-the-badge" alt="Timescale Badge"></a> |
         | <a href="https://docs.mindsdb.com/data-integrations/mongodb"><img src="https://img.shields.io/badge/MongoDB-4EA94B?style=for-the-badge&logo=mongodb&logoColor=white" alt="Connect MongoDB"></a> | <a href="https://docs.mindsdb.com/data-integrations/d0lt"><img src="https://img.shields.io/badge/DoIt-00B388?logo=DoIt&logoColor=fff&style=for-the-badge" alt="DoIt Badge"></a> | <a href="https://docs.mindsdb.com/data-integrations/amazon-dynamodb"><img src="https://img.shields.io/badge/Amazon%20DynamoDB-4053D6?logo=amazondynamodb&logoColor=fff&style=for-the-badge" alt="Amazon DynamoDB Badge"></a> |
@@ -142,41 +145,38 @@
         | <a href="https://docs.mindsdb.com/data-integrations/sap-hana"><img src="https://img.shields.io/badge/SAP%20HANA-1661BE?style=for-the-badge&logo=sap&logoColor=white" alt="Connect SAP HANA"></a> | <a href="https://docs.mindsdb.com/data-integrations/elasticsearch"><img src="https://img.shields.io/badge/Elastic-005571?logo=elastic&logoColor=fff&style=for-the-badge" alt="Elastic Badge"></a> | <a href="https://docs.mindsdb.com/data-integrations/cloud-spanner"><img src="https://img.shields.io/badge/Cloud%20Spanner-4285F4?style=for-the-badge" alt="Cloud Spanner Badge"></a> |
         | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#scylla"><img src="https://img.shields.io/badge/ScyllaDB-53CADD?style=for-the-badge&logo=scylladbb&logoColor=white" alt="Connect ScyllaDB"></a> | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#firebird"><img src="https://img.shields.io/badge/Firebird-F40D12?logo=Firebird&logoColor=fff&style=for-the-badge" alt="Firebird Badge"></a> |
         | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#singlestore"><img src="https://img.shields.io/badge/Singlestore-5f07b4?style=for-the-badge&logo=singlestore&logoColor=white" alt="Connect Singlestore"></a> | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#hive"><img src="https://img.shields.io/badge/Apache%20Hive-FDEE21?logo=apachehive&logoColor=000&style=for-the-badge" alt="Apache Hive Badge"></a> |
         | <a href="https://docs.mindsdb.com/data-integrations/teradata"><img src="https://img.shields.io/badge/Teradata-e36c42?style=for-the-badge&logo=teradata&logoColor=white" alt="Connect Teradata"></a> | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#matrix-one"><img src="https://img.shields.io/badge/Matrixone-02458D?logo=Matrixone&logoColor=fff&style=for-the-badge" alt="Matrixone Badge"></a> |
         | <a href=" https://docs.mindsdb.com/data-integrations/snowflake"><img src="https://img.shields.io/badge/Snowflake-35aedd?style=for-the-badge&logo=snowflake&logoColor=blue" alt="Connect Snowflake"></a> | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#informix"><img src="https://img.shields.io/badge/Informix-191A1B?logo=informix&logoColor=fff&style=for-the-badge" alt="Informix Badge"></a> |
         | <a href="https://docs.mindsdb.com/data-integrations/trino"><img src="https://img.shields.io/badge/Trino-dd00a1?style=for-the-badge&logo=trino&logoColor=white" alt="Connect Trino"></a> | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#monetdb"><img src="https://img.shields.io/badge/Monetdb-0099E5?logo=Monetdb&logoColor=fff&style=for-the-badge" alt="Monetdb Badge"></a> |
         
-        
-        
         [:question: :wave: Missing integration?](https://github.com/mindsdb/mindsdb/issues/new?assignees=&labels=&template=feature-mindsdb-request.yaml)
         
         
         ## Documentation
         
         You can find the complete documentation of MindsDB at [docs.mindsdb.com](https://docs.mindsdb.com?utm_medium=community&utm_source=github&utm_campaign=mindsdb%20repo).
         
         ## Support
         
         If you found a bug, please submit an [issue on GitHub](https://github.com/mindsdb/mindsdb/issues/new/choose).
         
         To get community support, you can:
         
-        * Post at MindsDB [Slack community](https://mindsdb.com/joincommunity).
+        * Post a question at MindsDB [Slack community](https://mindsdb.com/joincommunity).
         * Ask for help at our [GitHub Discussions](https://github.com/mindsdb/mindsdb/discussions).
         * Ask a question at [Stackoverflow](https://stackoverflow.com/questions/tagged/mindsdb) with a MindsDB tag.
         
         If you need commercial support, please [contact](https://mindsdb.com/contact/?utm_medium=community&utm_source=github&utm_campaign=mindsdb%20repo) MindsDB team.
         
         ## Contributing
         
         A great place to start contributing to MindsDB is to check our GitHub projects :checkered_flag:
         
-        * Tutorials & documentation [dashboard tasks](https://github.com/mindsdb/mindsdb/projects/7).
-        * Code contributor's [dashboard tasks](https://github.com/mindsdb/mindsdb/projects/8).
+        * Community contributor's [dashboard tasks](https://github.com/mindsdb/mindsdb/projects/8).
         * [First timers only issues](https://github.com/mindsdb/mindsdb/issues?q=is%3Aissue+is%3Aopen+label%3Afirst-timers-only), if this is your first time contributing to an open source project.
         
         We are always open to suggestions so feel free to open new issues with your ideas and we can guide you!
         
         Being part of the core team is accessible to anyone who is motivated and wants to be part of that journey!
         If you'd like to contribute to the project, refer to the [contributing documentation](https://docs.mindsdb.com/contribute/?utm_medium=community&utm_source=github&utm_campaign=mindsdb%20repo).
         
@@ -203,7 +203,127 @@
         MindsDB is licensed under [GNU General Public License v3.0](https://github.com/mindsdb/mindsdb/blob/master/LICENSE)
         
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+Provides-Extra: grpc
+Provides-Extra: telemetry
+Provides-Extra: all_extras
+Provides-Extra: edgelessdb
+Provides-Extra: mlflow
+Provides-Extra: derby
+Provides-Extra: d0lt
+Provides-Extra: vitess
+Provides-Extra: newsapi
+Provides-Extra: databend
+Provides-Extra: scylla
+Provides-Extra: huggingface
+Provides-Extra: flaml
+Provides-Extra: aurora
+Provides-Extra: orioledb
+Provides-Extra: vertica
+Provides-Extra: trino
+Provides-Extra: cloud_sql
+Provides-Extra: questdb
+Provides-Extra: dynamodb
+Provides-Extra: cohere
+Provides-Extra: crate
+Provides-Extra: sqreamdb
+Provides-Extra: oceanbase
+Provides-Extra: statsforecast
+Provides-Extra: shopify
+Provides-Extra: huggingface_api
+Provides-Extra: github
+Provides-Extra: datastax
+Provides-Extra: postgres
+Provides-Extra: solr
+Provides-Extra: lightwood
+Provides-Extra: stripe
+Provides-Extra: tidb
+Provides-Extra: redshift
+Provides-Extra: impala
+Provides-Extra: ingres
+Provides-Extra: google_fit
+Provides-Extra: access
+Provides-Extra: s3
+Provides-Extra: twitter
+Provides-Extra: neuralforecast
+Provides-Extra: gmail
+Provides-Extra: mysql
+Provides-Extra: plaid
+Provides-Extra: databricks
+Provides-Extra: supabase
+Provides-Extra: confluence
+Provides-Extra: sheets
+Provides-Extra: materialize
+Provides-Extra: firebird
+Provides-Extra: youtube
+Provides-Extra: mariadb
+Provides-Extra: monetdb
+Provides-Extra: pinot
+Provides-Extra: surrealdb
+Provides-Extra: informix
+Provides-Extra: influxdb
+Provides-Extra: merlion
+Provides-Extra: google_books
+Provides-Extra: binance
+Provides-Extra: db2
+Provides-Extra: paypal
+Provides-Extra: strava
+Provides-Extra: bigquery
+Provides-Extra: cockroach
+Provides-Extra: starrocks
+Provides-Extra: clickhouse
+Provides-Extra: maxdb
+Provides-Extra: hsqldb
+Provides-Extra: cloud_spanner
+Provides-Extra: phoenix
+Provides-Extra: ludwig
+Provides-Extra: slack
+Provides-Extra: duckdb
+Provides-Extra: mongodb
+Provides-Extra: quickbooks
+Provides-Extra: sendinblue
+Provides-Extra: yugabyte
+Provides-Extra: matrixone
+Provides-Extra: openai
+Provides-Extra: reddit
+Provides-Extra: elasticsearch
+Provides-Extra: singlestore
+Provides-Extra: google_content_shopping
+Provides-Extra: langchain
+Provides-Extra: rocket_chat
+Provides-Extra: frappe
+Provides-Extra: ray_serve
+Provides-Extra: nuo_jdbc
+Provides-Extra: dremio
+Provides-Extra: timescaledb
+Provides-Extra: rockset
+Provides-Extra: druid
+Provides-Extra: ckan
+Provides-Extra: tdengine
+Provides-Extra: mssql
+Provides-Extra: oracle
+Provides-Extra: google_calendar
+Provides-Extra: sqlany
+Provides-Extra: jira
+Provides-Extra: planetscale
+Provides-Extra: autosklearn
+Provides-Extra: hive
+Provides-Extra: opengauss
+Provides-Extra: hana
+Provides-Extra: empress
+Provides-Extra: google_search
+Provides-Extra: gitlab
+Provides-Extra: airtable
+Provides-Extra: llama_index
+Provides-Extra: couchbase
+Provides-Extra: ignite
+Provides-Extra: cassandra
+Provides-Extra: monkeylearn
+Provides-Extra: tpot
+Provides-Extra: altibase
+Provides-Extra: snowflake
+Provides-Extra: teradata
+Provides-Extra: all_handlers_extras
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: MindsDB Version: 23.5.4.1 Summary: MindsDB server,
+Metadata-Version: 2.1 Name: MindsDB Version: 23.6.1.1 Summary: MindsDB server,
 provides server capabilities to mindsdb native python library Home-page: https:
 //github.com/mindsdb/mindsdb Author: MindsDB Inc Author-email:
 jorge@mindsdb.com License: GPL-3.0 Download-URL: https://pypi.org/project/
 mindsdb/ Description:
                                ****** [MindsDB]
                                      ******
       [ROSS_Index_-_Fastest_Growing_Open-Source_Startups_|_Runa_Capital]
@@ -11,90 +11,95 @@
         ossrank.com/shield/630] [MindsDB_Website] [MindsDB_Community]
                              [Launch_in_Deepnote]
                                [Open_in_Gitpod]
 **** Website  |  Docs  |  Community_Slack  |  Contribute  |  Demo  |  Hackathon
                                      ****
 ---------------------------------------- [MindsDB](https://
 mindsdb.com?utm_medium=community&utm_source=github&utm_campaign=mindsdb%20repo)
-is an emerging low-code machine learning platform to help developers easily
-build #AI-powered solutions [![Tweet](https://img.shields.io/twitter/url/http/
+is a Server for Artificial Intelligence Logic, enabling developers to ship AI
+powered projects from prototyping & experimentation to production in a fast &
+scalable way. [![Tweet](https://img.shields.io/twitter/url/http/
 shields.io.svg?style=social)](https://twitter.com/intent/tweet?text=Build%20AI-
-Powered%20Applications%20&url=https://
+Centered%20Applications%20&url=https://
 www.mindsdb.com&via=mindsdb&hashtags=ai,ml,nlp,machine_learning,neural_networks,databases,gpt3)
-**NEW!** Check-out the [rewards and community programs.](https://mindsdb.com/
-community?utm_medium=community&utm_source=github&utm_campaign=mindsdb%20repo) -
---------------------------------------- [Installation](https://github.com/
+We do this by abstracting Generative AI, Large Language and other Models as a
+virtual tables ([AI Tables](https://www.youtube.com/watch?v=tnB4Y9T1E2k)) on
+top of enterprise databases. This increases accessibility with organizations
+and enables development teams to use their existing skills to build
+applications powered by AI. By taking a data-centric approach to AI MindsDB
+brings the process closer to the source of the data minimizing the need to
+build and maintain data pipelines and ETLâing, speeding up the time to
+deployment and reducing complexity. **P.S. If you like our open-source project
+we'd appreciate if you star it on GitHub â­!**
+                                    *****
+
+                                [MindsDB] *****
+---------------------------------------- MindsDB has an active and helpful
+community. Feel free to join our [Slack](https://mindsdb.com/joincommunity) and
+check-out the [rewards and community programs](https://mindsdb.com/
+community?utm_medium=community&utm_source=github&utm_campaign=mindsdb%20repo).
+---------------------------------------- [Installation](https://github.com/
 mindsdb/mindsdb#installation) - [Overview](https://github.com/mindsdb/
 mindsdb#overview) - [Features](https://github.com/mindsdb/mindsdb#features) -
 [Database Integrations](https://github.com/mindsdb/mindsdb#database-
 integrations) - [Quickstart](https://github.com/mindsdb/mindsdb#quickstart) -
 [Documentation](https://github.com/mindsdb/mindsdb#documentation) - [Support]
 (https://github.com/mindsdb/mindsdb#support) - [Contributing](https://
 github.com/mindsdb/mindsdb#contributing) - [Mailing lists](https://github.com/
 mindsdb/mindsdb#mailing-lists) - [License](https://github.com/mindsdb/
-mindsdb#license) ---------------------------- MindsDB automates and integrates
-top machine learning frameworks (including GPT-4) into the data stack as "AI
-Tables" to streamline the integration of AI into applications, making it
-accessible to developers of all skill levels. "[AI tables](https://
-www.youtube.com/watch?v=tnB4Y9T1E2k)" allow you to get predictions via SQL
-queries and continuously learn from your data.
-                                    *****
-
-                                [MindsDB] *****
-## Use cases Here are some popular use cases you can build with MindsDB: *
-Conversational AI: Leverage MindsDB native integrations with data platforms and
-pre-trained large language models, like OpenAI's GPT, to quickly build
-conversational AI solutions without the overhead of managing complex data
-pipelines. * Fraud Detection: MindsDB can help developers build models to
-detect fraudulent activity in financial transactions, eCommerce platforms etc.
-* Sales Forecasting: MindsDB can be used to develop models to predict future
-sales based on historical sales data, allowing businesses to make better-
-informed decisions. * Customer Segmentation: MindsDB can help developers
-segment customers based on their behavior, preferences, and other factors,
-allowing businesses to tailor their marketing efforts. * Sentiment analysis:
-MindsDB native integration with pre-trained models like OpenAI GPT or Hugging
-Face can be used to analyze the sentiment of a text data, such as a customer
-reviews - in a single command, instead of individual API calls and ETL-ing
-data. * Predictive Maintenance: MindsDB can be used to build models to predict
-when equipment or machinery is likely to fail, allowing for proactive
-maintenance and minimizing downtime. See more examples and community tutorials
-[here](https://docs.mindsdb.com/tutorials) ## Demo You can try MindsDB using
-our [demo environment](https://cloud.mindsdb.com/
+mindsdb#license) ---------------------------------------- ## Use cases Here are
+some popular use cases you can build with MindsDB: * Conversational AI:
+Leverage MindsDB native integrations with data platforms and pre-trained large
+language models, like OpenAI's GPT, to quickly build conversational AI
+solutions without the overhead of managing complex data pipelines. * Fraud
+Detection: MindsDB can help developers build models to detect fraudulent
+activity in financial transactions, eCommerce platforms etc. * Sales
+Forecasting: MindsDB can be used to develop models to predict future sales
+based on historical sales data, allowing businesses to make better-informed
+decisions. * Customer Segmentation: MindsDB can help developers segment
+customers based on their behavior, preferences, and other factors, allowing
+businesses to tailor their marketing efforts. * Sentiment analysis: MindsDB
+native integration with pre-trained models like OpenAI GPT or Hugging Face can
+be used to analyze the sentiment of a text data, such as a customer reviews -
+in a single command, instead of individual API calls and ETL-ing data. *
+Predictive Maintenance: MindsDB can be used to build models to predict when
+equipment or machinery is likely to fail, allowing for proactive maintenance
+and minimizing downtime. See more examples and community tutorials [here]
+(https://docs.mindsdb.com/tutorials). ## Demo You can try MindsDB using our
+[demo environment](https://cloud.mindsdb.com/
 ?utm_medium=community&utm_source=github&utm_campaign=mindsdb%20repo) with
 sample data for most popular use cases. ## Installation The prefered way is to
 use MindsDB Cloud [free demo instance](https://cloud.mindsdb.com/home) or use a
 [dedicated instance](https://cloud.mindsdb.com/home). If you want to move to
 production use [the AWS AMI image](https://aws.amazon.com/marketplace/seller-
-profile?id=03a65520-86ca-4ab8-a394-c11eb54573a9)/ To install locally or on-
+profile?id=03a65520-86ca-4ab8-a394-c11eb54573a9). To install locally or on-
 premise pull the latest Docker image: ``` docker pull mindsdb/mindsdb ``` ##
-How it works 1. First, CONNECT MindsDB to your data platform. We support 70+
-data platforms and this list is constantly growing. If you canât find the
+How it works 1. CONNECT MindsDB to your data platform. We support 100+ data
+platforms and this list is constantly growing. If you canât find the
 integration you need, please [let us know](https://mindsdb.com/joincommunity).
-2. Run the CREATE MODEL query pointing to your data table or a view, that will
-automatically create and deploy a machine learning model as an [AI Table]
-(https://www.youtube.com/watch?v=tnB4Y9T1E2k). 1. If you have an NLP use case,
-CREATE MODEL will integrate the [AI Table](https://www.youtube.com/
-watch?v=tnB4Y9T1E2k) with already pre-trained model you choose (like OpenAIâs
-GPT-3 or Hugging Face models). 2. Please check the [docs](https://
-docs.mindsdb.com/sql/create/
-predictor?utm_medium=community&utm_source=github&utm_campaign=mindsdb%20repo)
-if you want to have manual control over model engineering. 3. JOIN the model
-with your database tables to make predictions for thousands or even millions of
-data points at once, or run SELECT statements or API calls to make one time
-predictions. 4. Set up a JOB to automate your model re-training cycle and
-predictions pipelines for the new incoming data. Follow the [quickstart guide]
-(https://docs.mindsdb.com/
+2. CREATE MODEL to connect the AI Engine you pick that will learn from your
+data and serve it as [AI Table](https://www.youtube.com/watch?v=tnB4Y9T1E2k).
+1. If you have an NLP use case, CREATE MODEL will integrate the [AI Table]
+(https://www.youtube.com/watch?v=tnB4Y9T1E2k) with already pre-trained model
+you choose (like OpenAIâs GPT or Hugging Face models). 2. Please check the
+[docs](https://docs.mindsdb.com/sql/create/
+model?utm_medium=community&utm_source=github&utm_campaign=mindsdb%20repo) if
+you want to have manual control over model engineering. 3. JOIN such model with
+your database tables to make predictions for thousands or even millions of data
+points at once, or run SELECT statements or API calls to make one time
+predictions. 4. Set up a JOB to automate your re-training cycle and predictions
+pipelines for the new incoming data. 5. Alternatively, use REST API to query
+the models Follow the [quickstart guide](https://docs.mindsdb.com/
 quickstart?utm_medium=community&utm_source=github&utm_campaign=mindsdb%20repo)
 with sample data to get on-boarded as fast as possible. ## Database
-Integrations MindsDB works with most of the SQL and NoSQL databases, data
-lakes, data Streams and popular applications. | Connect your Data | Connect
-your Data | Connect your Data |-|-|-| | [Connect_Apache_Kafka] | [Connect
-Microsoft_Access] | [Oracle_Badge] | | [Connect_Amazon_Redshift] | [Airtable
-Badge] | [Pinot_Badge] | | [Connect_Cassandra] | [DataStax_Badge] | [Amazon_S3
-Badge] | | [Connect_CockroachDB] | [ckan_Badge] | [Supabase_Badge] | | [Connect
+Integrations MindsDB works with most of the SQL and NoSQL databases, data lakes
+and popular applications. | Connect your Data | Connect your Data | Connect
+your Data |-|-|-| | [Connect_Amazon_Redshift] | [Airtable_Badge] | [Pinot
+Badge] | | [Connect_Cassandra] | [DataStax_Badge] | [Amazon_S3_Badge] | |
+[Connect_CockroachDB] | [ckan_Badge] | [Supabase_Badge] | | [Connect
 Clickhouse] | [Google_Big_Query_Badge] | [SQLite_Badge] | | [Connect_MariaDB] |
 [Couchbase_Badge] | [TiDB_Badge] | | [Connect_SQL_Server] | [CrateDB_Badge] |
 [Timescale_Badge] | | [Connect_MongoDB] | [DoIt_Badge] | [Amazon_DynamoDB
 Badge] | | [Connect_PostgreSQL] | [IBMDB2_Badge] | [openGauss_Badge] | |
 [Connect_MySQL] | [Databricks_Badge] | [YugabyteDB_Badge] | [Connect_QuestDB] |
 [Apache_Druid_Badge] | | [StarRocks_Badge] | [Vertica_Badge] | [DuckDB_Badge] |
 | [Connect_SAP_HANA] | [Elastic_Badge] | [Cloud_Spanner_Badge] | | [Connect
@@ -104,25 +109,24 @@
 integration?](https://github.com/mindsdb/mindsdb/issues/
 new?assignees=&labels=&template=feature-mindsdb-request.yaml) ## Documentation
 You can find the complete documentation of MindsDB at [docs.mindsdb.com](https:
 //
 docs.mindsdb.com?utm_medium=community&utm_source=github&utm_campaign=mindsdb%20repo).
 ## Support If you found a bug, please submit an [issue on GitHub](https://
 github.com/mindsdb/mindsdb/issues/new/choose). To get community support, you
-can: * Post at MindsDB [Slack community](https://mindsdb.com/joincommunity). *
-Ask for help at our [GitHub Discussions](https://github.com/mindsdb/mindsdb/
-discussions). * Ask a question at [Stackoverflow](https://stackoverflow.com/
-questions/tagged/mindsdb) with a MindsDB tag. If you need commercial support,
-please [contact](https://mindsdb.com/contact/
+can: * Post a question at MindsDB [Slack community](https://mindsdb.com/
+joincommunity). * Ask for help at our [GitHub Discussions](https://github.com/
+mindsdb/mindsdb/discussions). * Ask a question at [Stackoverflow](https://
+stackoverflow.com/questions/tagged/mindsdb) with a MindsDB tag. If you need
+commercial support, please [contact](https://mindsdb.com/contact/
 ?utm_medium=community&utm_source=github&utm_campaign=mindsdb%20repo) MindsDB
 team. ## Contributing A great place to start contributing to MindsDB is to
-check our GitHub projects :checkered_flag: * Tutorials & documentation
-[dashboard tasks](https://github.com/mindsdb/mindsdb/projects/7). * Code
-contributor's [dashboard tasks](https://github.com/mindsdb/mindsdb/projects/8).
-* [First timers only issues](https://github.com/mindsdb/mindsdb/
+check our GitHub projects :checkered_flag: * Community contributor's [dashboard
+tasks](https://github.com/mindsdb/mindsdb/projects/8). * [First timers only
+issues](https://github.com/mindsdb/mindsdb/
 issues?q=is%3Aissue+is%3Aopen+label%3Afirst-timers-only), if this is your first
 time contributing to an open source project. We are always open to suggestions
 so feel free to open new issues with your ideas and we can guide you! Being
 part of the core team is accessible to anyone who is motivated and wants to be
 part of that journey! If you'd like to contribute to the project, refer to the
 [contributing documentation](https://docs.mindsdb.com/contribute/
 ?utm_medium=community&utm_source=github&utm_campaign=mindsdb%20repo). Please
@@ -138,8 +142,47 @@
 mindsdb.com/newsletter/
 ?utm_medium=community&utm_source=github&utm_campaign=mindsdb%20repo) to get
 product updates, information about MindsDB events and contests, and useful
 content, like tutorials. ## License MindsDB is licensed under [GNU General
 Public License v3.0](https://github.com/mindsdb/mindsdb/blob/master/LICENSE)
 Platform: UNKNOWN Classifier: Programming Language :: Python :: 3 Classifier:
 Operating System :: OS Independent Requires-Python: >=3.8 Description-Content-
-Type: text/markdown
+Type: text/markdown Provides-Extra: grpc Provides-Extra: telemetry Provides-
+Extra: all_extras Provides-Extra: edgelessdb Provides-Extra: mlflow Provides-
+Extra: derby Provides-Extra: d0lt Provides-Extra: vitess Provides-Extra:
+newsapi Provides-Extra: databend Provides-Extra: scylla Provides-Extra:
+huggingface Provides-Extra: flaml Provides-Extra: aurora Provides-Extra:
+orioledb Provides-Extra: vertica Provides-Extra: trino Provides-Extra:
+cloud_sql Provides-Extra: questdb Provides-Extra: dynamodb Provides-Extra:
+cohere Provides-Extra: crate Provides-Extra: sqreamdb Provides-Extra: oceanbase
+Provides-Extra: statsforecast Provides-Extra: shopify Provides-Extra:
+huggingface_api Provides-Extra: github Provides-Extra: datastax Provides-Extra:
+postgres Provides-Extra: solr Provides-Extra: lightwood Provides-Extra: stripe
+Provides-Extra: tidb Provides-Extra: redshift Provides-Extra: impala Provides-
+Extra: ingres Provides-Extra: google_fit Provides-Extra: access Provides-Extra:
+s3 Provides-Extra: twitter Provides-Extra: neuralforecast Provides-Extra: gmail
+Provides-Extra: mysql Provides-Extra: plaid Provides-Extra: databricks
+Provides-Extra: supabase Provides-Extra: confluence Provides-Extra: sheets
+Provides-Extra: materialize Provides-Extra: firebird Provides-Extra: youtube
+Provides-Extra: mariadb Provides-Extra: monetdb Provides-Extra: pinot Provides-
+Extra: surrealdb Provides-Extra: informix Provides-Extra: influxdb Provides-
+Extra: merlion Provides-Extra: google_books Provides-Extra: binance Provides-
+Extra: db2 Provides-Extra: paypal Provides-Extra: strava Provides-Extra:
+bigquery Provides-Extra: cockroach Provides-Extra: starrocks Provides-Extra:
+clickhouse Provides-Extra: maxdb Provides-Extra: hsqldb Provides-Extra:
+cloud_spanner Provides-Extra: phoenix Provides-Extra: ludwig Provides-Extra:
+slack Provides-Extra: duckdb Provides-Extra: mongodb Provides-Extra: quickbooks
+Provides-Extra: sendinblue Provides-Extra: yugabyte Provides-Extra: matrixone
+Provides-Extra: openai Provides-Extra: reddit Provides-Extra: elasticsearch
+Provides-Extra: singlestore Provides-Extra: google_content_shopping Provides-
+Extra: langchain Provides-Extra: rocket_chat Provides-Extra: frappe Provides-
+Extra: ray_serve Provides-Extra: nuo_jdbc Provides-Extra: dremio Provides-
+Extra: timescaledb Provides-Extra: rockset Provides-Extra: druid Provides-
+Extra: ckan Provides-Extra: tdengine Provides-Extra: mssql Provides-Extra:
+oracle Provides-Extra: google_calendar Provides-Extra: sqlany Provides-Extra:
+jira Provides-Extra: planetscale Provides-Extra: autosklearn Provides-Extra:
+hive Provides-Extra: opengauss Provides-Extra: hana Provides-Extra: empress
+Provides-Extra: google_search Provides-Extra: gitlab Provides-Extra: airtable
+Provides-Extra: llama_index Provides-Extra: couchbase Provides-Extra: ignite
+Provides-Extra: cassandra Provides-Extra: monkeylearn Provides-Extra: tpot
+Provides-Extra: altibase Provides-Extra: snowflake Provides-Extra: teradata
+Provides-Extra: all_handlers_extras
```

### Comparing `MindsDB-23.5.4.1/README.md` & `MindsDB-23.6.1.1/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,194 +1,329 @@
-<h1 align="center">
-	<img width="300" src="https://github.com/mindsdb/mindsdb_native/blob/stable/assets/MindsDBColorPurp@3x.png?raw=true" alt="MindsDB">
-	<br>
-</h1>
-
-<div align="center">
-
-<a
-     href="https://runacap.com/ross-index/annual-2022/"
-     target="_blank"
-     rel="noopener"
-/>
-    <img
-        style="width: 260px; height: 56px"
-        src="https://runacap.com/wp-content/uploads/2023/02/Annual_ROSS_badge_white_2022.svg"
-        alt="ROSS Index - Fastest Growing Open-Source Startups | Runa Capital"
-        width="260"
-        height="56"
-    />
-</a>
-
-<p>
-	<a href="https://github.com/mindsdb/mindsdb/actions"><img src="https://github.com/mindsdb/mindsdb/workflows/MindsDB%20workflow/badge.svg" alt="MindsDB workflow"></a>
-	<a href="https://www.python.org/downloads/" target="_blank"><img src="https://img.shields.io/badge/python-3.7.x%20|%203.8.x|%203.9.x-brightgreen.svg" alt="Python supported"></a>
-	<a href="https://pypi.org/project/MindsDB/" target="_blank"><img src="https://badge.fury.io/py/MindsDB.svg" alt="PyPi Version"></a>
-	<br />
-	<img alt="PyPI - Downloads" src="https://img.shields.io/pypi/dm/Mindsdb">  <a href="https://hub.docker.com/u/mindsdb" target="_blank"><img src="https://img.shields.io/docker/pulls/mindsdb/mindsdb" alt="Docker pulls"></a>
-	<a href="https://ossrank.com/p/630"><img src="https://shields.io/endpoint?url=https://ossrank.com/shield/630"></a>
-	<a href="https://www.mindsdb.com/"><img src="https://img.shields.io/website?url=https%3A%2F%2Fwww.mindsdb.com%2F" alt="MindsDB Website"></a>
-	<a href="https://join.slack.com/t/mindsdbcommunity/shared_invite/zt-o8mrmx3l-5ai~5H66s6wlxFfBMVI6wQ" target="_blank"><img src="https://img.shields.io/badge/slack-@mindsdbcommunity-brightgreen.svg?logo=slack " alt="MindsDB Community"></a>
-	<br />
-	<a href="https://deepnote.com/project/Machine-Learning-With-SQL-8GDF7bc7SzKlhBLorqoIcw/%2Fmindsdb_demo.ipynb" target="_blank"><img src="https://deepnote.com/buttons/launch-in-deepnote-white.svg" alt="Launch in Deepnote"></a>
-	<br />
-	<a href="https://gitpod.io/#https://github.com/mindsdb/mindsdb" target="_blank"><img src="https://gitpod.io/button/open-in-gitpod.svg" alt="Open in Gitpod"></a>
-</p>
-
-<h3 align="center">
-	<a href="https://www.mindsdb.com?utm_medium=community&utm_source=github&utm_campaign=mindsdb%20repo">Website</a>
-	<span> | </span>
-	<a href="https://docs.mindsdb.com?utm_medium=community&utm_source=github&utm_campaign=mindsdb%20repo">Docs</a>
-	<span> | </span>
-	<a href="https://mindsdb.com/joincommunity">Community Slack</a>
-	<span> | </span>
-	<a href="https://github.com/mindsdb/mindsdb/projects?type=classic">Contribute</a>
-	<span> | </span>
-	<a href="https://cloud.mindsdb.com?utm_medium=community&utm_source=github&utm_campaign=mindsdb%20repo">Demo</a>
-	<span> | </span>
-	<a href="https://hashnode.com/hackathons/mindsdb?source=hncounter-feed">Hackathon</a>
-</h3>
-
-</div>
-
-----------------------------------------
-
-[MindsDB](https://mindsdb.com?utm_medium=community&utm_source=github&utm_campaign=mindsdb%20repo) is an emerging low-code machine learning platform to help developers easily build #AI-powered solutions [![Tweet](https://img.shields.io/twitter/url/http/shields.io.svg?style=social)](https://twitter.com/intent/tweet?text=Build%20AI-Powered%20Applications%20&url=https://www.mindsdb.com&via=mindsdb&hashtags=ai,ml,nlp,machine_learning,neural_networks,databases,gpt3)
-
-
-**NEW!** Check-out the [rewards and community programs.](https://mindsdb.com/community?utm_medium=community&utm_source=github&utm_campaign=mindsdb%20repo)
-
-----------------------------------------
-
-[Installation](https://github.com/mindsdb/mindsdb#installation) - [Overview](https://github.com/mindsdb/mindsdb#overview) - [Features](https://github.com/mindsdb/mindsdb#features) - [Database Integrations](https://github.com/mindsdb/mindsdb#database-integrations) - [Quickstart](https://github.com/mindsdb/mindsdb#quickstart) - [Documentation](https://github.com/mindsdb/mindsdb#documentation) - [Support](https://github.com/mindsdb/mindsdb#support) - [Contributing](https://github.com/mindsdb/mindsdb#contributing) - [Mailing lists](https://github.com/mindsdb/mindsdb#mailing-lists) - [License](https://github.com/mindsdb/mindsdb#license)
-
-----------------------------
-
-MindsDB automates and integrates top machine learning frameworks (including GPT-4) into the data stack as "AI Tables" to streamline the integration of AI into applications, making it accessible to developers of all skill levels.
-"[AI tables](https://www.youtube.com/watch?v=tnB4Y9T1E2k)" allow you to get predictions via SQL queries and continuously learn from your data.
-
-<h2 align="center">
-   <br/>
-   <br/>
-  <img width="450" src="https://docs.google.com/drawings/d/e/2PACX-1vQ1KImK0cqvZ_KpPm3SKDZF6peuM-d1lZwOkrZNpT1_PO5UVyveEIyeJGbDZFBF124LmWbHSB2HFQ97/pub?w=691&h=728" alt="MindsDB">
-
-</h2>
-
-## Use cases
-
-Here are some popular use cases you can build with MindsDB:
-
-* Conversational AI: Leverage MindsDB native integrations with data platforms and pre-trained large language models, like OpenAI's GPT, to quickly build conversational AI solutions without the overhead of managing complex data pipelines.
-* Fraud Detection: MindsDB can help developers build models to detect fraudulent activity in financial transactions, eCommerce platforms etc.
-* Sales Forecasting: MindsDB can be used to develop models to predict future sales based on historical sales data, allowing businesses to make better-informed decisions.
-* Customer Segmentation: MindsDB can help developers segment customers based on their behavior, preferences, and other factors, allowing businesses to tailor their marketing efforts.
-* Sentiment analysis: MindsDB native integration with pre-trained models like OpenAI GPT or Hugging Face can be used to analyze the sentiment of a text data, such as a customer reviews - in a single command, instead of individual API calls and ETL-ing data.
-* Predictive Maintenance: MindsDB can be used to build models to predict when equipment or machinery is likely to fail, allowing for proactive maintenance and minimizing downtime.
-
-See more examples and community tutorials [here](https://docs.mindsdb.com/tutorials)
-
-## Demo
-
-You can try MindsDB using our [demo environment](https://cloud.mindsdb.com/?utm_medium=community&utm_source=github&utm_campaign=mindsdb%20repo) with sample data for most popular use cases.
-
-## Installation
-
-The prefered way is to use MindsDB Cloud [free demo instance](https://cloud.mindsdb.com/home) or use a [dedicated instance](https://cloud.mindsdb.com/home). If you want to move to production use [the AWS AMI image](https://aws.amazon.com/marketplace/seller-profile?id=03a65520-86ca-4ab8-a394-c11eb54573a9)/
-
-To install locally or on-premise pull the latest Docker image:
-
-```
-docker pull mindsdb/mindsdb
-```
-
-## How it works
-
-1. First, CONNECT MindsDB to your data platform. We support 70+ data platforms and this list is constantly growing. If you can’t find the integration you need, please [let us know](https://mindsdb.com/joincommunity).
-2. Run the CREATE MODEL query pointing to your data table or a view, that will automatically create and deploy a machine learning model as an [AI Table](https://www.youtube.com/watch?v=tnB4Y9T1E2k).
-    1. If you have an NLP use case, CREATE MODEL will integrate the [AI Table](https://www.youtube.com/watch?v=tnB4Y9T1E2k) with already pre-trained model you choose (like OpenAI’s GPT-3 or Hugging Face models).
-    2. Please check the [docs](https://docs.mindsdb.com/sql/create/predictor?utm_medium=community&utm_source=github&utm_campaign=mindsdb%20repo) if you want to have manual control over model engineering.
-3. JOIN the model with your database tables to make predictions for thousands or even millions of data points at once, or run SELECT statements or API calls to make one time predictions.
-4. Set up a JOB to automate your model re-training cycle and predictions pipelines for the new incoming data.
-
-Follow the [quickstart guide](https://docs.mindsdb.com/quickstart?utm_medium=community&utm_source=github&utm_campaign=mindsdb%20repo) with sample data to get on-boarded as fast as possible.
-
-
-## Database Integrations
-
-MindsDB works with most of the SQL and NoSQL databases, data lakes, data Streams and popular applications.
-
-| Connect your Data | Connect your Data | Connect your Data
-|-|-|-|
-| <a href="https://docs.mindsdb.com/connect/kafka"><img src="https://img.shields.io/badge/Apache Kafka-808080?style=for-the-badge&logo=apache-kafka&logoColor=white" alt="Connect Apache Kafka"></a> | <a href="https://docs.mindsdb.com/data-integrations/microsoft-access"><img src="https://img.shields.io/badge/Microsoft%20Access-A4373A?logo=microsoftaccess&logoColor=fff&style=for-the-badge" alt="Connect Microsoft Access"></a> | <a href="https://docs.mindsdb.com/data-integrations/oracle"><img src="https://img.shields.io/badge/Oracle-F80000?logo=oracle&logoColor=fff&style=for-the-badge" alt="Oracle Badge"></a> |
-| <a href="https://docs.mindsdb.com/data-integrations/amazon-redshift"><img src="https://img.shields.io/badge/Amazon%20Redshift-0466C8?style=for-the-badge&logo=amazon-aws&logoColor=white" alt="Connect Amazon Redshift"></a> | <a href="https://docs.mindsdb.com/data-integrations/airtable"><img src="https://img.shields.io/badge/Airtable-18BFFF?logo=airtable&logoColor=fff&style=for-the-badge" alt="Airtable Badge"></a> | <a href="https://docs.mindsdb.com/data-integrations/apache-pinot"><img src="https://img.shields.io/badge/Pinot-000?logo=pinot&logoColor=fff&style=for-the-badge" alt="Pinot Badge"></a> |
-| <a href="https://docs.mindsdb.com/data-integrations/apache-cassandra"><img src="https://img.shields.io/badge/Cassandra-1287B1?style=for-the-badge&logo=apache%20cassandra&logoColor=white" alt="Connect Cassandra"></a> | <a href="https://docs.mindsdb.com/data-integrations/datastax"><img src="https://img.shields.io/badge/DataStax-3A3A42?logo=datastax&logoColor=fff&style=for-the-badge" alt="DataStax Badge"></a> | <a href="https://docs.mindsdb.com/data-integrations/amazon-s3"><img src="https://img.shields.io/badge/Amazon%20S3-569A31?logo=amazons3&logoColor=fff&style=for-the-badge" alt="Amazon S3 Badge"></a> |
-| <a href="https://docs.mindsdb.com/data-integrations/cockroachdb"><img src="https://img.shields.io/badge/CockroachDB-426EDF?style=for-the-badge&logo=cockroach-labs&logoColor=white" alt="Connect CockroachDB"></a> | <a href="https://docs.mindsdb.com/data-integrations/ckan"><img src="https://img.shields.io/badge/ckan-7D929E?logo=ckan&logoColor=fff&style=for-the-badge" alt="ckan Badge"></a> | <a href="https://docs.mindsdb.com/data-integrations/supabase"><img src="https://img.shields.io/badge/Supabase-3ECF8E?logo=supabase&logoColor=fff&style=for-the-badge" alt="Supabase Badge"></a> |
-| <a href="https://docs.mindsdb.com/data-integrations/clickhouse"><img src="https://img.shields.io/badge/Clickhouse-e6e600?style=for-the-badge&logo=clickhouse&logoColor=white" alt="Connect Clickhouse"></a> | <a href="https://docs.mindsdb.com/data-integrations/google-bigquery"><img src="https://img.shields.io/badge/Google Big Query-0466C8?logo=Big Query&logoColor=fff&style=for-the-badge" alt="Google Big Query Badge"></a> | <a href="https://docs.mindsdb.com/data-integrations/sqlite"><img src="https://img.shields.io/badge/SQLite-003B57?logo=sqlite&logoColor=fff&style=for-the-badge" alt="SQLite Badge"></a> |
-| <a href="https://docs.mindsdb.com/data-integrations/mariadb"><img src="https://img.shields.io/badge/MariaDB-003545?style=for-the-badge&logo=mariadb&logoColor=white" alt="Connect MariaDB"></a> | <a href="https://docs.mindsdb.com/data-integrations/couchbase"><img src="https://img.shields.io/badge/Couchbase-EA2328?logo=couchbase&logoColor=fff&style=for-the-badge" alt="Couchbase Badge"></a> | <a href="https://docs.mindsdb.com/data-integrations/tidb#tidb-handler"><img src="https://img.shields.io/badge/TiDB-DD0031?logo=tidb&logoColor=fff&style=for-the-badge" alt="TiDB Badge"></a> |
-| <a href="https://docs.mindsdb.com/data-integrations/microsoft-sql-server"><img src="https://img.shields.io/badge/Microsoft%20SQL%20Sever-CC2927?style=for-the-badge&logo=microsoft%20sql%20server&logoColor=white" alt="Connect SQL Server"></a> | <a href="https://docs.mindsdb.com/data-integrations/cratedb"><img src="https://img.shields.io/badge/CrateDB-009DC7?logo=cratedb&logoColor=fff&style=for-the-badge" alt="CrateDB Badge"></a> | <a href=" https://docs.mindsdb.com/data-integrations/timescaledb"><img src="https://img.shields.io/badge/Timescale-FDB515?logo=timescale&logoColor=fff&style=for-the-badge" alt="Timescale Badge"></a> |
-| <a href="https://docs.mindsdb.com/data-integrations/mongodb"><img src="https://img.shields.io/badge/MongoDB-4EA94B?style=for-the-badge&logo=mongodb&logoColor=white" alt="Connect MongoDB"></a> | <a href="https://docs.mindsdb.com/data-integrations/d0lt"><img src="https://img.shields.io/badge/DoIt-00B388?logo=DoIt&logoColor=fff&style=for-the-badge" alt="DoIt Badge"></a> | <a href="https://docs.mindsdb.com/data-integrations/amazon-dynamodb"><img src="https://img.shields.io/badge/Amazon%20DynamoDB-4053D6?logo=amazondynamodb&logoColor=fff&style=for-the-badge" alt="Amazon DynamoDB Badge"></a> |
-| <a href="https://docs.mindsdb.com/data-integrations/postgresql"><img src="https://img.shields.io/badge/PostgreSQL-316192?style=for-the-badge&logo=postgresql&logoColor=white" alt="Connect PostgreSQL"></a> | <a href="https://docs.mindsdb.com/data-integrations/ibm-db2"><img src="https://img.shields.io/badge/IBMDB2-008000?logo=IBMDB2&logoColor=fff&style=for-the-badge" alt="IBMDB2 Badge"></a> | <a href="https://docs.mindsdb.com/data-integrations/opengauss"><img src="https://img.shields.io/badge/openGauss-02458D?logo=opengauss&logoColor=fff&style=for-the-badge" alt="openGauss Badge"></a> |
-| <a href="https://docs.mindsdb.com/data-integrations/mysql"><img src="https://img.shields.io/badge/MySQL-00758F?style=for-the-badge&logo=mysql&logoColor=white" alt="Connect MySQL"></a> | <a href=" https://docs.mindsdb.com/data-integrations/databricks"><img src="https://img.shields.io/badge/Databricks-FF3621?logo=databricks&logoColor=fff&style=for-the-badge" alt="Databricks Badge"></a> | <a href="https://docs.mindsdb.com/data-integrations/yugabytedb"><img src="https://img.shields.io/badge/YugabyteDB-02458D?logo=yugabytedb&logoColor=fff&style=for-the-badge" alt="YugabyteDB Badge"></a>
-| <a href="https://docs.mindsdb.com/data-integrations/questdb"><img src="https://img.shields.io/badge/QuestDB-d14671?style=for-the-badge&logo=questdb&logoColor=white" alt="Connect QuestDB"></a> | <a href="https://docs.mindsdb.com/data-integrations/apache-druid"><img src="https://img.shields.io/badge/Apache%20Druid-29F1FB?logo=apachedruid&logoColor=000&style=for-the-badge" alt="Apache Druid Badge"></a> |
-| <a href="https://docs.mindsdb.com/data-integrations/starrocks"><img src="https://img.shields.io/badge/starrocks-000000?style=for-the-badge&logo=starrocks&logoColor=white" alt="StarRocks Badge"></a> | <a href="https://docs.mindsdb.com/data-integrations/vertica"><img src="https://img.shields.io/badge/Vertica-000?logo=vertica&logoColor=fff&style=for-the-badge" alt="Vertica Badge"></a> | <a href="https://docs.mindsdb.com/data-integrations/duckdb"><img src="https://img.shields.io/badge/duckdb-fff?logo=duckdb&logoColor=000&style=for-the-badge" alt="DuckDB Badge"></a> |
-| <a href="https://docs.mindsdb.com/data-integrations/sap-hana"><img src="https://img.shields.io/badge/SAP%20HANA-1661BE?style=for-the-badge&logo=sap&logoColor=white" alt="Connect SAP HANA"></a> | <a href="https://docs.mindsdb.com/data-integrations/elasticsearch"><img src="https://img.shields.io/badge/Elastic-005571?logo=elastic&logoColor=fff&style=for-the-badge" alt="Elastic Badge"></a> | <a href="https://docs.mindsdb.com/data-integrations/cloud-spanner"><img src="https://img.shields.io/badge/Cloud%20Spanner-4285F4?style=for-the-badge" alt="Cloud Spanner Badge"></a> |
-| <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#scylla"><img src="https://img.shields.io/badge/ScyllaDB-53CADD?style=for-the-badge&logo=scylladbb&logoColor=white" alt="Connect ScyllaDB"></a> | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#firebird"><img src="https://img.shields.io/badge/Firebird-F40D12?logo=Firebird&logoColor=fff&style=for-the-badge" alt="Firebird Badge"></a> |
-| <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#singlestore"><img src="https://img.shields.io/badge/Singlestore-5f07b4?style=for-the-badge&logo=singlestore&logoColor=white" alt="Connect Singlestore"></a> | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#hive"><img src="https://img.shields.io/badge/Apache%20Hive-FDEE21?logo=apachehive&logoColor=000&style=for-the-badge" alt="Apache Hive Badge"></a> |
-| <a href="https://docs.mindsdb.com/data-integrations/teradata"><img src="https://img.shields.io/badge/Teradata-e36c42?style=for-the-badge&logo=teradata&logoColor=white" alt="Connect Teradata"></a> | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#matrix-one"><img src="https://img.shields.io/badge/Matrixone-02458D?logo=Matrixone&logoColor=fff&style=for-the-badge" alt="Matrixone Badge"></a> |
-| <a href=" https://docs.mindsdb.com/data-integrations/snowflake"><img src="https://img.shields.io/badge/Snowflake-35aedd?style=for-the-badge&logo=snowflake&logoColor=blue" alt="Connect Snowflake"></a> | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#informix"><img src="https://img.shields.io/badge/Informix-191A1B?logo=informix&logoColor=fff&style=for-the-badge" alt="Informix Badge"></a> |
-| <a href="https://docs.mindsdb.com/data-integrations/trino"><img src="https://img.shields.io/badge/Trino-dd00a1?style=for-the-badge&logo=trino&logoColor=white" alt="Connect Trino"></a> | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#monetdb"><img src="https://img.shields.io/badge/Monetdb-0099E5?logo=Monetdb&logoColor=fff&style=for-the-badge" alt="Monetdb Badge"></a> |
-
-
-
-[:question: :wave: Missing integration?](https://github.com/mindsdb/mindsdb/issues/new?assignees=&labels=&template=feature-mindsdb-request.yaml)
-
-
-## Documentation
-
-You can find the complete documentation of MindsDB at [docs.mindsdb.com](https://docs.mindsdb.com?utm_medium=community&utm_source=github&utm_campaign=mindsdb%20repo).
-
-## Support
-
-If you found a bug, please submit an [issue on GitHub](https://github.com/mindsdb/mindsdb/issues/new/choose).
-
-To get community support, you can:
-
-* Post at MindsDB [Slack community](https://mindsdb.com/joincommunity).
-* Ask for help at our [GitHub Discussions](https://github.com/mindsdb/mindsdb/discussions).
-* Ask a question at [Stackoverflow](https://stackoverflow.com/questions/tagged/mindsdb) with a MindsDB tag.
-
-If you need commercial support, please [contact](https://mindsdb.com/contact/?utm_medium=community&utm_source=github&utm_campaign=mindsdb%20repo) MindsDB team.
-
-## Contributing
-
-A great place to start contributing to MindsDB is to check our GitHub projects :checkered_flag:
-
-* Tutorials & documentation [dashboard tasks](https://github.com/mindsdb/mindsdb/projects/7).
-* Code contributor's [dashboard tasks](https://github.com/mindsdb/mindsdb/projects/8).
-* [First timers only issues](https://github.com/mindsdb/mindsdb/issues?q=is%3Aissue+is%3Aopen+label%3Afirst-timers-only), if this is your first time contributing to an open source project.
-
-We are always open to suggestions so feel free to open new issues with your ideas and we can guide you!
-
-Being part of the core team is accessible to anyone who is motivated and wants to be part of that journey!
-If you'd like to contribute to the project, refer to the [contributing documentation](https://docs.mindsdb.com/contribute/?utm_medium=community&utm_source=github&utm_campaign=mindsdb%20repo).
-
-Please note that this project is released with a [Contributor Code of Conduct](https://github.com/mindsdb/mindsdb/blob/stable/CODE_OF_CONDUCT.md). By participating in this project, you agree to abide by its terms.
-
-Also, check out the [rewards and community programs](https://mindsdb.com/community?utm_medium=community&utm_source=github&utm_campaign=mindsdb%20repo).
-
-
-### Current contributors
-
-<a href="https://github.com/mindsdb/mindsdb/graphs/contributors">
-  <img src="https://contributors-img.web.app/image?repo=mindsdb/mindsdb" />
-</a>
-
-Made with [contributors-img](https://contributors-img.web.app).
-
-## Subscribe to updates
-
-Join our [Slack community](https://mindsdb.com/joincommunity) and subscribe to the monthly [Developer Newsletter](https://mindsdb.com/newsletter/?utm_medium=community&utm_source=github&utm_campaign=mindsdb%20repo) to get product updates, information about MindsDB events and contests, and useful content, like tutorials.
-
-
-## License
-
-MindsDB is licensed under [GNU General Public License v3.0](https://github.com/mindsdb/mindsdb/blob/master/LICENSE)
+Metadata-Version: 2.1
+Name: MindsDB
+Version: 23.6.1.1
+Summary: MindsDB server, provides server capabilities to mindsdb native python library
+Home-page: https://github.com/mindsdb/mindsdb
+Author: MindsDB Inc
+Author-email: jorge@mindsdb.com
+License: GPL-3.0
+Download-URL: https://pypi.org/project/mindsdb/
+Description: <h1 align="center">
+        	<img width="300" src="https://github.com/mindsdb/mindsdb_native/blob/stable/assets/MindsDBColorPurp@3x.png?raw=true" alt="MindsDB">
+        	<br>
+        </h1>
+        
+        <div align="center">
+        
+        <a
+             href="https://runacap.com/ross-index/annual-2022/"
+             target="_blank"
+             rel="noopener"
+        />
+            <img
+                style="width: 260px; height: 56px"
+                src="https://runacap.com/wp-content/uploads/2023/02/Annual_ROSS_badge_white_2022.svg"
+                alt="ROSS Index - Fastest Growing Open-Source Startups | Runa Capital"
+                width="260"
+                height="56"
+            />
+        </a>
+        
+        <p>
+        	<a href="https://github.com/mindsdb/mindsdb/actions"><img src="https://github.com/mindsdb/mindsdb/workflows/MindsDB%20workflow/badge.svg" alt="MindsDB workflow"></a>
+        	<a href="https://www.python.org/downloads/" target="_blank"><img src="https://img.shields.io/badge/python-3.7.x%20|%203.8.x|%203.9.x-brightgreen.svg" alt="Python supported"></a>
+        	<a href="https://pypi.org/project/MindsDB/" target="_blank"><img src="https://badge.fury.io/py/MindsDB.svg" alt="PyPi Version"></a>
+        	<br />
+        	<img alt="PyPI - Downloads" src="https://img.shields.io/pypi/dm/Mindsdb">  <a href="https://hub.docker.com/u/mindsdb" target="_blank"><img src="https://img.shields.io/docker/pulls/mindsdb/mindsdb" alt="Docker pulls"></a>
+        	<a href="https://ossrank.com/p/630"><img src="https://shields.io/endpoint?url=https://ossrank.com/shield/630"></a>
+        	<a href="https://www.mindsdb.com/"><img src="https://img.shields.io/website?url=https%3A%2F%2Fwww.mindsdb.com%2F" alt="MindsDB Website"></a>
+        	<a href="https://mindsdb.com/joincommunity" target="_blank"><img src="https://img.shields.io/badge/slack-@mindsdbcommunity-brightgreen.svg?logo=slack " alt="MindsDB Community"></a>
+        	<br />
+        	<a href="https://deepnote.com/project/Machine-Learning-With-SQL-8GDF7bc7SzKlhBLorqoIcw/%2Fmindsdb_demo.ipynb" target="_blank"><img src="https://deepnote.com/buttons/launch-in-deepnote-white.svg" alt="Launch in Deepnote"></a>
+        	<br />
+        	<a href="https://gitpod.io/#https://github.com/mindsdb/mindsdb" target="_blank"><img src="https://gitpod.io/button/open-in-gitpod.svg" alt="Open in Gitpod"></a>
+        </p>
+        
+        <h3 align="center">
+        	<a href="https://www.mindsdb.com?utm_medium=community&utm_source=github&utm_campaign=mindsdb%20repo">Website</a>
+        	<span> | </span>
+        	<a href="https://docs.mindsdb.com?utm_medium=community&utm_source=github&utm_campaign=mindsdb%20repo">Docs</a>
+        	<span> | </span>
+        	<a href="https://mindsdb.com/joincommunity">Community Slack</a>
+        	<span> | </span>
+        	<a href="https://github.com/mindsdb/mindsdb/projects?type=classic">Contribute</a>
+        	<span> | </span>
+        	<a href="https://cloud.mindsdb.com?utm_medium=community&utm_source=github&utm_campaign=mindsdb%20repo">Demo</a>
+        	<span> | </span>
+        	<a href="https://hashnode.com/hackathons/mindsdb?source=hncounter-feed">Hackathon</a>
+        </h3>
+        
+        </div>
+        
+        ----------------------------------------
+        
+        [MindsDB](https://mindsdb.com?utm_medium=community&utm_source=github&utm_campaign=mindsdb%20repo) is a Server for Artificial Intelligence Logic, enabling developers to ship AI powered projects from prototyping & experimentation to production in a fast & scalable way. [![Tweet](https://img.shields.io/twitter/url/http/shields.io.svg?style=social)](https://twitter.com/intent/tweet?text=Build%20AI-Centered%20Applications%20&url=https://www.mindsdb.com&via=mindsdb&hashtags=ai,ml,nlp,machine_learning,neural_networks,databases,gpt3)
+        
+        We do this by abstracting Generative AI, Large Language and other Models as a virtual tables ([AI Tables](https://www.youtube.com/watch?v=tnB4Y9T1E2k)) on top of enterprise databases. This increases accessibility with organizations and enables development teams to use their existing skills to build applications powered by AI.
+        
+        By taking a data-centric approach to AI MindsDB brings the process closer to the source of the data minimizing the need to build and maintain data pipelines and ETL’ing, speeding up the time to deployment and reducing complexity.
+        
+        **P.S. If you like our open-source project we'd appreciate if you star it on GitHub ⭐!**
+        
+        <h2 align="center">
+           <br/>
+           <br/>
+          <img width="100%" src="https://github.com/mindsdb/mindsdb/assets/12409467/8418fec3-8c8b-4414-b1dc-7943041047b4" alt="MindsDB">
+        
+        </h2>
+        
+        ----------------------------------------
+        MindsDB has an active and helpful community. Feel free to join our [Slack](https://mindsdb.com/joincommunity) and check-out the [rewards and community programs](https://mindsdb.com/community?utm_medium=community&utm_source=github&utm_campaign=mindsdb%20repo).
+        
+        ----------------------------------------
+        
+        [Installation](https://github.com/mindsdb/mindsdb#installation) - [Overview](https://github.com/mindsdb/mindsdb#overview) - [Features](https://github.com/mindsdb/mindsdb#features) - [Database Integrations](https://github.com/mindsdb/mindsdb#database-integrations) - [Quickstart](https://github.com/mindsdb/mindsdb#quickstart) - [Documentation](https://github.com/mindsdb/mindsdb#documentation) - [Support](https://github.com/mindsdb/mindsdb#support) - [Contributing](https://github.com/mindsdb/mindsdb#contributing) - [Mailing lists](https://github.com/mindsdb/mindsdb#mailing-lists) - [License](https://github.com/mindsdb/mindsdb#license)
+        
+        ----------------------------------------
+        
+        ## Use cases
+        
+        Here are some popular use cases you can build with MindsDB:
+        
+        * Conversational AI: Leverage MindsDB native integrations with data platforms and pre-trained large language models, like OpenAI's GPT, to quickly build conversational AI solutions without the overhead of managing complex data pipelines.
+        * Fraud Detection: MindsDB can help developers build models to detect fraudulent activity in financial transactions, eCommerce platforms etc.
+        * Sales Forecasting: MindsDB can be used to develop models to predict future sales based on historical sales data, allowing businesses to make better-informed decisions.
+        * Customer Segmentation: MindsDB can help developers segment customers based on their behavior, preferences, and other factors, allowing businesses to tailor their marketing efforts.
+        * Sentiment analysis: MindsDB native integration with pre-trained models like OpenAI GPT or Hugging Face can be used to analyze the sentiment of a text data, such as a customer reviews - in a single command, instead of individual API calls and ETL-ing data.
+        * Predictive Maintenance: MindsDB can be used to build models to predict when equipment or machinery is likely to fail, allowing for proactive maintenance and minimizing downtime.
+        
+        See more examples and community tutorials [here](https://docs.mindsdb.com/tutorials).
+        
+        ## Demo
+        
+        You can try MindsDB using our [demo environment](https://cloud.mindsdb.com/?utm_medium=community&utm_source=github&utm_campaign=mindsdb%20repo) with sample data for most popular use cases.
+        
+        ## Installation
+        
+        The prefered way is to use MindsDB Cloud [free demo instance](https://cloud.mindsdb.com/home) or use a [dedicated instance](https://cloud.mindsdb.com/home). If you want to move to production use [the AWS AMI image](https://aws.amazon.com/marketplace/seller-profile?id=03a65520-86ca-4ab8-a394-c11eb54573a9).
+        
+        To install locally or on-premise pull the latest Docker image:
+        
+        ```
+        docker pull mindsdb/mindsdb
+        ```
+        
+        ## How it works
+        
+        1. CONNECT MindsDB to your data platform. We support 100+ data platforms and this list is constantly growing. If you can’t find the integration you need, please [let us know](https://mindsdb.com/joincommunity).
+        2. CREATE MODEL to connect the AI Engine you pick that will learn from your data and serve it as [AI Table](https://www.youtube.com/watch?v=tnB4Y9T1E2k).
+            1. If you have an NLP use case, CREATE MODEL will integrate the [AI Table](https://www.youtube.com/watch?v=tnB4Y9T1E2k) with already pre-trained model you choose (like OpenAI’s GPT or Hugging Face models).
+            2. Please check the [docs](https://docs.mindsdb.com/sql/create/model?utm_medium=community&utm_source=github&utm_campaign=mindsdb%20repo) if you want to have manual control over model engineering.
+        3. JOIN such model with your database tables to make predictions for thousands or even millions of data points at once, or run SELECT statements or API calls to make one time predictions.
+        4. Set up a JOB to automate your re-training cycle and predictions pipelines for the new incoming data.
+        5. Alternatively, use REST API to query the models
+        
+        Follow the [quickstart guide](https://docs.mindsdb.com/quickstart?utm_medium=community&utm_source=github&utm_campaign=mindsdb%20repo) with sample data to get on-boarded as fast as possible.
+        
+        
+        ## Database Integrations
+        
+        MindsDB works with most of the SQL and NoSQL databases, data lakes and popular applications.
+        
+        | Connect your Data | Connect your Data | Connect your Data
+        |-|-|-|
+        | <a href="https://docs.mindsdb.com/data-integrations/amazon-redshift"><img src="https://img.shields.io/badge/Amazon%20Redshift-0466C8?style=for-the-badge&logo=amazon-aws&logoColor=white" alt="Connect Amazon Redshift"></a> | <a href="https://docs.mindsdb.com/data-integrations/airtable"><img src="https://img.shields.io/badge/Airtable-18BFFF?logo=airtable&logoColor=fff&style=for-the-badge" alt="Airtable Badge"></a> | <a href="https://docs.mindsdb.com/data-integrations/apache-pinot"><img src="https://img.shields.io/badge/Pinot-000?logo=pinot&logoColor=fff&style=for-the-badge" alt="Pinot Badge"></a> |
+        | <a href="https://docs.mindsdb.com/data-integrations/apache-cassandra"><img src="https://img.shields.io/badge/Cassandra-1287B1?style=for-the-badge&logo=apache%20cassandra&logoColor=white" alt="Connect Cassandra"></a> | <a href="https://docs.mindsdb.com/data-integrations/datastax"><img src="https://img.shields.io/badge/DataStax-3A3A42?logo=datastax&logoColor=fff&style=for-the-badge" alt="DataStax Badge"></a> | <a href="https://docs.mindsdb.com/data-integrations/amazon-s3"><img src="https://img.shields.io/badge/Amazon%20S3-569A31?logo=amazons3&logoColor=fff&style=for-the-badge" alt="Amazon S3 Badge"></a> |
+        | <a href="https://docs.mindsdb.com/data-integrations/cockroachdb"><img src="https://img.shields.io/badge/CockroachDB-426EDF?style=for-the-badge&logo=cockroach-labs&logoColor=white" alt="Connect CockroachDB"></a> | <a href="https://docs.mindsdb.com/data-integrations/ckan"><img src="https://img.shields.io/badge/ckan-7D929E?logo=ckan&logoColor=fff&style=for-the-badge" alt="ckan Badge"></a> | <a href="https://docs.mindsdb.com/data-integrations/supabase"><img src="https://img.shields.io/badge/Supabase-3ECF8E?logo=supabase&logoColor=fff&style=for-the-badge" alt="Supabase Badge"></a> |
+        | <a href="https://docs.mindsdb.com/data-integrations/clickhouse"><img src="https://img.shields.io/badge/Clickhouse-e6e600?style=for-the-badge&logo=clickhouse&logoColor=white" alt="Connect Clickhouse"></a> | <a href="https://docs.mindsdb.com/data-integrations/google-bigquery"><img src="https://img.shields.io/badge/Google Big Query-0466C8?logo=Big Query&logoColor=fff&style=for-the-badge" alt="Google Big Query Badge"></a> | <a href="https://docs.mindsdb.com/data-integrations/sqlite"><img src="https://img.shields.io/badge/SQLite-003B57?logo=sqlite&logoColor=fff&style=for-the-badge" alt="SQLite Badge"></a> |
+        | <a href="https://docs.mindsdb.com/data-integrations/mariadb"><img src="https://img.shields.io/badge/MariaDB-003545?style=for-the-badge&logo=mariadb&logoColor=white" alt="Connect MariaDB"></a> | <a href="https://docs.mindsdb.com/data-integrations/couchbase"><img src="https://img.shields.io/badge/Couchbase-EA2328?logo=couchbase&logoColor=fff&style=for-the-badge" alt="Couchbase Badge"></a> | <a href="https://docs.mindsdb.com/data-integrations/tidb#tidb-handler"><img src="https://img.shields.io/badge/TiDB-DD0031?logo=tidb&logoColor=fff&style=for-the-badge" alt="TiDB Badge"></a> |
+        | <a href="https://docs.mindsdb.com/data-integrations/microsoft-sql-server"><img src="https://img.shields.io/badge/Microsoft%20SQL%20Sever-CC2927?style=for-the-badge&logo=microsoft%20sql%20server&logoColor=white" alt="Connect SQL Server"></a> | <a href="https://docs.mindsdb.com/data-integrations/cratedb"><img src="https://img.shields.io/badge/CrateDB-009DC7?logo=cratedb&logoColor=fff&style=for-the-badge" alt="CrateDB Badge"></a> | <a href=" https://docs.mindsdb.com/data-integrations/timescaledb"><img src="https://img.shields.io/badge/Timescale-FDB515?logo=timescale&logoColor=fff&style=for-the-badge" alt="Timescale Badge"></a> |
+        | <a href="https://docs.mindsdb.com/data-integrations/mongodb"><img src="https://img.shields.io/badge/MongoDB-4EA94B?style=for-the-badge&logo=mongodb&logoColor=white" alt="Connect MongoDB"></a> | <a href="https://docs.mindsdb.com/data-integrations/d0lt"><img src="https://img.shields.io/badge/DoIt-00B388?logo=DoIt&logoColor=fff&style=for-the-badge" alt="DoIt Badge"></a> | <a href="https://docs.mindsdb.com/data-integrations/amazon-dynamodb"><img src="https://img.shields.io/badge/Amazon%20DynamoDB-4053D6?logo=amazondynamodb&logoColor=fff&style=for-the-badge" alt="Amazon DynamoDB Badge"></a> |
+        | <a href="https://docs.mindsdb.com/data-integrations/postgresql"><img src="https://img.shields.io/badge/PostgreSQL-316192?style=for-the-badge&logo=postgresql&logoColor=white" alt="Connect PostgreSQL"></a> | <a href="https://docs.mindsdb.com/data-integrations/ibm-db2"><img src="https://img.shields.io/badge/IBMDB2-008000?logo=IBMDB2&logoColor=fff&style=for-the-badge" alt="IBMDB2 Badge"></a> | <a href="https://docs.mindsdb.com/data-integrations/opengauss"><img src="https://img.shields.io/badge/openGauss-02458D?logo=opengauss&logoColor=fff&style=for-the-badge" alt="openGauss Badge"></a> |
+        | <a href="https://docs.mindsdb.com/data-integrations/mysql"><img src="https://img.shields.io/badge/MySQL-00758F?style=for-the-badge&logo=mysql&logoColor=white" alt="Connect MySQL"></a> | <a href=" https://docs.mindsdb.com/data-integrations/databricks"><img src="https://img.shields.io/badge/Databricks-FF3621?logo=databricks&logoColor=fff&style=for-the-badge" alt="Databricks Badge"></a> | <a href="https://docs.mindsdb.com/data-integrations/yugabytedb"><img src="https://img.shields.io/badge/YugabyteDB-02458D?logo=yugabytedb&logoColor=fff&style=for-the-badge" alt="YugabyteDB Badge"></a>
+        | <a href="https://docs.mindsdb.com/data-integrations/questdb"><img src="https://img.shields.io/badge/QuestDB-d14671?style=for-the-badge&logo=questdb&logoColor=white" alt="Connect QuestDB"></a> | <a href="https://docs.mindsdb.com/data-integrations/apache-druid"><img src="https://img.shields.io/badge/Apache%20Druid-29F1FB?logo=apachedruid&logoColor=000&style=for-the-badge" alt="Apache Druid Badge"></a> |
+        | <a href="https://docs.mindsdb.com/data-integrations/starrocks"><img src="https://img.shields.io/badge/starrocks-000000?style=for-the-badge&logo=starrocks&logoColor=white" alt="StarRocks Badge"></a> | <a href="https://docs.mindsdb.com/data-integrations/vertica"><img src="https://img.shields.io/badge/Vertica-000?logo=vertica&logoColor=fff&style=for-the-badge" alt="Vertica Badge"></a> | <a href="https://docs.mindsdb.com/data-integrations/duckdb"><img src="https://img.shields.io/badge/duckdb-fff?logo=duckdb&logoColor=000&style=for-the-badge" alt="DuckDB Badge"></a> |
+        | <a href="https://docs.mindsdb.com/data-integrations/sap-hana"><img src="https://img.shields.io/badge/SAP%20HANA-1661BE?style=for-the-badge&logo=sap&logoColor=white" alt="Connect SAP HANA"></a> | <a href="https://docs.mindsdb.com/data-integrations/elasticsearch"><img src="https://img.shields.io/badge/Elastic-005571?logo=elastic&logoColor=fff&style=for-the-badge" alt="Elastic Badge"></a> | <a href="https://docs.mindsdb.com/data-integrations/cloud-spanner"><img src="https://img.shields.io/badge/Cloud%20Spanner-4285F4?style=for-the-badge" alt="Cloud Spanner Badge"></a> |
+        | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#scylla"><img src="https://img.shields.io/badge/ScyllaDB-53CADD?style=for-the-badge&logo=scylladbb&logoColor=white" alt="Connect ScyllaDB"></a> | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#firebird"><img src="https://img.shields.io/badge/Firebird-F40D12?logo=Firebird&logoColor=fff&style=for-the-badge" alt="Firebird Badge"></a> |
+        | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#singlestore"><img src="https://img.shields.io/badge/Singlestore-5f07b4?style=for-the-badge&logo=singlestore&logoColor=white" alt="Connect Singlestore"></a> | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#hive"><img src="https://img.shields.io/badge/Apache%20Hive-FDEE21?logo=apachehive&logoColor=000&style=for-the-badge" alt="Apache Hive Badge"></a> |
+        | <a href="https://docs.mindsdb.com/data-integrations/teradata"><img src="https://img.shields.io/badge/Teradata-e36c42?style=for-the-badge&logo=teradata&logoColor=white" alt="Connect Teradata"></a> | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#matrix-one"><img src="https://img.shields.io/badge/Matrixone-02458D?logo=Matrixone&logoColor=fff&style=for-the-badge" alt="Matrixone Badge"></a> |
+        | <a href=" https://docs.mindsdb.com/data-integrations/snowflake"><img src="https://img.shields.io/badge/Snowflake-35aedd?style=for-the-badge&logo=snowflake&logoColor=blue" alt="Connect Snowflake"></a> | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#informix"><img src="https://img.shields.io/badge/Informix-191A1B?logo=informix&logoColor=fff&style=for-the-badge" alt="Informix Badge"></a> |
+        | <a href="https://docs.mindsdb.com/data-integrations/trino"><img src="https://img.shields.io/badge/Trino-dd00a1?style=for-the-badge&logo=trino&logoColor=white" alt="Connect Trino"></a> | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#monetdb"><img src="https://img.shields.io/badge/Monetdb-0099E5?logo=Monetdb&logoColor=fff&style=for-the-badge" alt="Monetdb Badge"></a> |
+        
+        [:question: :wave: Missing integration?](https://github.com/mindsdb/mindsdb/issues/new?assignees=&labels=&template=feature-mindsdb-request.yaml)
+        
+        
+        ## Documentation
+        
+        You can find the complete documentation of MindsDB at [docs.mindsdb.com](https://docs.mindsdb.com?utm_medium=community&utm_source=github&utm_campaign=mindsdb%20repo).
+        
+        ## Support
+        
+        If you found a bug, please submit an [issue on GitHub](https://github.com/mindsdb/mindsdb/issues/new/choose).
+        
+        To get community support, you can:
+        
+        * Post a question at MindsDB [Slack community](https://mindsdb.com/joincommunity).
+        * Ask for help at our [GitHub Discussions](https://github.com/mindsdb/mindsdb/discussions).
+        * Ask a question at [Stackoverflow](https://stackoverflow.com/questions/tagged/mindsdb) with a MindsDB tag.
+        
+        If you need commercial support, please [contact](https://mindsdb.com/contact/?utm_medium=community&utm_source=github&utm_campaign=mindsdb%20repo) MindsDB team.
+        
+        ## Contributing
+        
+        A great place to start contributing to MindsDB is to check our GitHub projects :checkered_flag:
+        
+        * Community contributor's [dashboard tasks](https://github.com/mindsdb/mindsdb/projects/8).
+        * [First timers only issues](https://github.com/mindsdb/mindsdb/issues?q=is%3Aissue+is%3Aopen+label%3Afirst-timers-only), if this is your first time contributing to an open source project.
+        
+        We are always open to suggestions so feel free to open new issues with your ideas and we can guide you!
+        
+        Being part of the core team is accessible to anyone who is motivated and wants to be part of that journey!
+        If you'd like to contribute to the project, refer to the [contributing documentation](https://docs.mindsdb.com/contribute/?utm_medium=community&utm_source=github&utm_campaign=mindsdb%20repo).
+        
+        Please note that this project is released with a [Contributor Code of Conduct](https://github.com/mindsdb/mindsdb/blob/stable/CODE_OF_CONDUCT.md). By participating in this project, you agree to abide by its terms.
+        
+        Also, check out the [rewards and community programs](https://mindsdb.com/community?utm_medium=community&utm_source=github&utm_campaign=mindsdb%20repo).
+        
+        
+        ### Current contributors
+        
+        <a href="https://github.com/mindsdb/mindsdb/graphs/contributors">
+          <img src="https://contributors-img.web.app/image?repo=mindsdb/mindsdb" />
+        </a>
+        
+        Made with [contributors-img](https://contributors-img.web.app).
+        
+        ## Subscribe to updates
+        
+        Join our [Slack community](https://mindsdb.com/joincommunity) and subscribe to the monthly [Developer Newsletter](https://mindsdb.com/newsletter/?utm_medium=community&utm_source=github&utm_campaign=mindsdb%20repo) to get product updates, information about MindsDB events and contests, and useful content, like tutorials.
+        
+        
+        ## License
+        
+        MindsDB is licensed under [GNU General Public License v3.0](https://github.com/mindsdb/mindsdb/blob/master/LICENSE)
+        
+Platform: UNKNOWN
+Classifier: Programming Language :: Python :: 3
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+Provides-Extra: grpc
+Provides-Extra: telemetry
+Provides-Extra: all_extras
+Provides-Extra: edgelessdb
+Provides-Extra: mlflow
+Provides-Extra: derby
+Provides-Extra: d0lt
+Provides-Extra: vitess
+Provides-Extra: newsapi
+Provides-Extra: databend
+Provides-Extra: scylla
+Provides-Extra: huggingface
+Provides-Extra: flaml
+Provides-Extra: aurora
+Provides-Extra: orioledb
+Provides-Extra: vertica
+Provides-Extra: trino
+Provides-Extra: cloud_sql
+Provides-Extra: questdb
+Provides-Extra: dynamodb
+Provides-Extra: cohere
+Provides-Extra: crate
+Provides-Extra: sqreamdb
+Provides-Extra: oceanbase
+Provides-Extra: statsforecast
+Provides-Extra: shopify
+Provides-Extra: huggingface_api
+Provides-Extra: github
+Provides-Extra: datastax
+Provides-Extra: postgres
+Provides-Extra: solr
+Provides-Extra: lightwood
+Provides-Extra: stripe
+Provides-Extra: tidb
+Provides-Extra: redshift
+Provides-Extra: impala
+Provides-Extra: ingres
+Provides-Extra: google_fit
+Provides-Extra: access
+Provides-Extra: s3
+Provides-Extra: twitter
+Provides-Extra: neuralforecast
+Provides-Extra: gmail
+Provides-Extra: mysql
+Provides-Extra: plaid
+Provides-Extra: databricks
+Provides-Extra: supabase
+Provides-Extra: confluence
+Provides-Extra: sheets
+Provides-Extra: materialize
+Provides-Extra: firebird
+Provides-Extra: youtube
+Provides-Extra: mariadb
+Provides-Extra: monetdb
+Provides-Extra: pinot
+Provides-Extra: surrealdb
+Provides-Extra: informix
+Provides-Extra: influxdb
+Provides-Extra: merlion
+Provides-Extra: google_books
+Provides-Extra: binance
+Provides-Extra: db2
+Provides-Extra: paypal
+Provides-Extra: strava
+Provides-Extra: bigquery
+Provides-Extra: cockroach
+Provides-Extra: starrocks
+Provides-Extra: clickhouse
+Provides-Extra: maxdb
+Provides-Extra: hsqldb
+Provides-Extra: cloud_spanner
+Provides-Extra: phoenix
+Provides-Extra: ludwig
+Provides-Extra: slack
+Provides-Extra: duckdb
+Provides-Extra: mongodb
+Provides-Extra: quickbooks
+Provides-Extra: sendinblue
+Provides-Extra: yugabyte
+Provides-Extra: matrixone
+Provides-Extra: openai
+Provides-Extra: reddit
+Provides-Extra: elasticsearch
+Provides-Extra: singlestore
+Provides-Extra: google_content_shopping
+Provides-Extra: langchain
+Provides-Extra: rocket_chat
+Provides-Extra: frappe
+Provides-Extra: ray_serve
+Provides-Extra: nuo_jdbc
+Provides-Extra: dremio
+Provides-Extra: timescaledb
+Provides-Extra: rockset
+Provides-Extra: druid
+Provides-Extra: ckan
+Provides-Extra: tdengine
+Provides-Extra: mssql
+Provides-Extra: oracle
+Provides-Extra: google_calendar
+Provides-Extra: sqlany
+Provides-Extra: jira
+Provides-Extra: planetscale
+Provides-Extra: autosklearn
+Provides-Extra: hive
+Provides-Extra: opengauss
+Provides-Extra: hana
+Provides-Extra: empress
+Provides-Extra: google_search
+Provides-Extra: gitlab
+Provides-Extra: airtable
+Provides-Extra: llama_index
+Provides-Extra: couchbase
+Provides-Extra: ignite
+Provides-Extra: cassandra
+Provides-Extra: monkeylearn
+Provides-Extra: tpot
+Provides-Extra: altibase
+Provides-Extra: snowflake
+Provides-Extra: teradata
+Provides-Extra: all_handlers_extras
```

#### html2text {}

```diff
@@ -1,95 +1,105 @@
+Metadata-Version: 2.1 Name: MindsDB Version: 23.6.1.1 Summary: MindsDB server,
+provides server capabilities to mindsdb native python library Home-page: https:
+//github.com/mindsdb/mindsdb Author: MindsDB Inc Author-email:
+jorge@mindsdb.com License: GPL-3.0 Download-URL: https://pypi.org/project/
+mindsdb/ Description:
                                ****** [MindsDB]
                                      ******
       [ROSS_Index_-_Fastest_Growing_Open-Source_Startups_|_Runa_Capital]
              [MindsDB_workflow] [Python_supported] [PyPi_Version]
   [PyPI - Downloads] [Docker_pulls] [https://shields.io/endpoint?url=https://
         ossrank.com/shield/630] [MindsDB_Website] [MindsDB_Community]
                              [Launch_in_Deepnote]
                                [Open_in_Gitpod]
 **** Website  |  Docs  |  Community_Slack  |  Contribute  |  Demo  |  Hackathon
                                      ****
 ---------------------------------------- [MindsDB](https://
 mindsdb.com?utm_medium=community&utm_source=github&utm_campaign=mindsdb%20repo)
-is an emerging low-code machine learning platform to help developers easily
-build #AI-powered solutions [![Tweet](https://img.shields.io/twitter/url/http/
+is a Server for Artificial Intelligence Logic, enabling developers to ship AI
+powered projects from prototyping & experimentation to production in a fast &
+scalable way. [![Tweet](https://img.shields.io/twitter/url/http/
 shields.io.svg?style=social)](https://twitter.com/intent/tweet?text=Build%20AI-
-Powered%20Applications%20&url=https://
+Centered%20Applications%20&url=https://
 www.mindsdb.com&via=mindsdb&hashtags=ai,ml,nlp,machine_learning,neural_networks,databases,gpt3)
-**NEW!** Check-out the [rewards and community programs.](https://mindsdb.com/
-community?utm_medium=community&utm_source=github&utm_campaign=mindsdb%20repo) -
---------------------------------------- [Installation](https://github.com/
+We do this by abstracting Generative AI, Large Language and other Models as a
+virtual tables ([AI Tables](https://www.youtube.com/watch?v=tnB4Y9T1E2k)) on
+top of enterprise databases. This increases accessibility with organizations
+and enables development teams to use their existing skills to build
+applications powered by AI. By taking a data-centric approach to AI MindsDB
+brings the process closer to the source of the data minimizing the need to
+build and maintain data pipelines and ETLâing, speeding up the time to
+deployment and reducing complexity. **P.S. If you like our open-source project
+we'd appreciate if you star it on GitHub â­!**
+                                    *****
+
+                                [MindsDB] *****
+---------------------------------------- MindsDB has an active and helpful
+community. Feel free to join our [Slack](https://mindsdb.com/joincommunity) and
+check-out the [rewards and community programs](https://mindsdb.com/
+community?utm_medium=community&utm_source=github&utm_campaign=mindsdb%20repo).
+---------------------------------------- [Installation](https://github.com/
 mindsdb/mindsdb#installation) - [Overview](https://github.com/mindsdb/
 mindsdb#overview) - [Features](https://github.com/mindsdb/mindsdb#features) -
 [Database Integrations](https://github.com/mindsdb/mindsdb#database-
 integrations) - [Quickstart](https://github.com/mindsdb/mindsdb#quickstart) -
 [Documentation](https://github.com/mindsdb/mindsdb#documentation) - [Support]
 (https://github.com/mindsdb/mindsdb#support) - [Contributing](https://
 github.com/mindsdb/mindsdb#contributing) - [Mailing lists](https://github.com/
 mindsdb/mindsdb#mailing-lists) - [License](https://github.com/mindsdb/
-mindsdb#license) ---------------------------- MindsDB automates and integrates
-top machine learning frameworks (including GPT-4) into the data stack as "AI
-Tables" to streamline the integration of AI into applications, making it
-accessible to developers of all skill levels. "[AI tables](https://
-www.youtube.com/watch?v=tnB4Y9T1E2k)" allow you to get predictions via SQL
-queries and continuously learn from your data.
-                                    *****
-
-                                [MindsDB] *****
-## Use cases Here are some popular use cases you can build with MindsDB: *
-Conversational AI: Leverage MindsDB native integrations with data platforms and
-pre-trained large language models, like OpenAI's GPT, to quickly build
-conversational AI solutions without the overhead of managing complex data
-pipelines. * Fraud Detection: MindsDB can help developers build models to
-detect fraudulent activity in financial transactions, eCommerce platforms etc.
-* Sales Forecasting: MindsDB can be used to develop models to predict future
-sales based on historical sales data, allowing businesses to make better-
-informed decisions. * Customer Segmentation: MindsDB can help developers
-segment customers based on their behavior, preferences, and other factors,
-allowing businesses to tailor their marketing efforts. * Sentiment analysis:
-MindsDB native integration with pre-trained models like OpenAI GPT or Hugging
-Face can be used to analyze the sentiment of a text data, such as a customer
-reviews - in a single command, instead of individual API calls and ETL-ing
-data. * Predictive Maintenance: MindsDB can be used to build models to predict
-when equipment or machinery is likely to fail, allowing for proactive
-maintenance and minimizing downtime. See more examples and community tutorials
-[here](https://docs.mindsdb.com/tutorials) ## Demo You can try MindsDB using
-our [demo environment](https://cloud.mindsdb.com/
+mindsdb#license) ---------------------------------------- ## Use cases Here are
+some popular use cases you can build with MindsDB: * Conversational AI:
+Leverage MindsDB native integrations with data platforms and pre-trained large
+language models, like OpenAI's GPT, to quickly build conversational AI
+solutions without the overhead of managing complex data pipelines. * Fraud
+Detection: MindsDB can help developers build models to detect fraudulent
+activity in financial transactions, eCommerce platforms etc. * Sales
+Forecasting: MindsDB can be used to develop models to predict future sales
+based on historical sales data, allowing businesses to make better-informed
+decisions. * Customer Segmentation: MindsDB can help developers segment
+customers based on their behavior, preferences, and other factors, allowing
+businesses to tailor their marketing efforts. * Sentiment analysis: MindsDB
+native integration with pre-trained models like OpenAI GPT or Hugging Face can
+be used to analyze the sentiment of a text data, such as a customer reviews -
+in a single command, instead of individual API calls and ETL-ing data. *
+Predictive Maintenance: MindsDB can be used to build models to predict when
+equipment or machinery is likely to fail, allowing for proactive maintenance
+and minimizing downtime. See more examples and community tutorials [here]
+(https://docs.mindsdb.com/tutorials). ## Demo You can try MindsDB using our
+[demo environment](https://cloud.mindsdb.com/
 ?utm_medium=community&utm_source=github&utm_campaign=mindsdb%20repo) with
 sample data for most popular use cases. ## Installation The prefered way is to
 use MindsDB Cloud [free demo instance](https://cloud.mindsdb.com/home) or use a
 [dedicated instance](https://cloud.mindsdb.com/home). If you want to move to
 production use [the AWS AMI image](https://aws.amazon.com/marketplace/seller-
-profile?id=03a65520-86ca-4ab8-a394-c11eb54573a9)/ To install locally or on-
+profile?id=03a65520-86ca-4ab8-a394-c11eb54573a9). To install locally or on-
 premise pull the latest Docker image: ``` docker pull mindsdb/mindsdb ``` ##
-How it works 1. First, CONNECT MindsDB to your data platform. We support 70+
-data platforms and this list is constantly growing. If you canât find the
+How it works 1. CONNECT MindsDB to your data platform. We support 100+ data
+platforms and this list is constantly growing. If you canât find the
 integration you need, please [let us know](https://mindsdb.com/joincommunity).
-2. Run the CREATE MODEL query pointing to your data table or a view, that will
-automatically create and deploy a machine learning model as an [AI Table]
-(https://www.youtube.com/watch?v=tnB4Y9T1E2k). 1. If you have an NLP use case,
-CREATE MODEL will integrate the [AI Table](https://www.youtube.com/
-watch?v=tnB4Y9T1E2k) with already pre-trained model you choose (like OpenAIâs
-GPT-3 or Hugging Face models). 2. Please check the [docs](https://
-docs.mindsdb.com/sql/create/
-predictor?utm_medium=community&utm_source=github&utm_campaign=mindsdb%20repo)
-if you want to have manual control over model engineering. 3. JOIN the model
-with your database tables to make predictions for thousands or even millions of
-data points at once, or run SELECT statements or API calls to make one time
-predictions. 4. Set up a JOB to automate your model re-training cycle and
-predictions pipelines for the new incoming data. Follow the [quickstart guide]
-(https://docs.mindsdb.com/
+2. CREATE MODEL to connect the AI Engine you pick that will learn from your
+data and serve it as [AI Table](https://www.youtube.com/watch?v=tnB4Y9T1E2k).
+1. If you have an NLP use case, CREATE MODEL will integrate the [AI Table]
+(https://www.youtube.com/watch?v=tnB4Y9T1E2k) with already pre-trained model
+you choose (like OpenAIâs GPT or Hugging Face models). 2. Please check the
+[docs](https://docs.mindsdb.com/sql/create/
+model?utm_medium=community&utm_source=github&utm_campaign=mindsdb%20repo) if
+you want to have manual control over model engineering. 3. JOIN such model with
+your database tables to make predictions for thousands or even millions of data
+points at once, or run SELECT statements or API calls to make one time
+predictions. 4. Set up a JOB to automate your re-training cycle and predictions
+pipelines for the new incoming data. 5. Alternatively, use REST API to query
+the models Follow the [quickstart guide](https://docs.mindsdb.com/
 quickstart?utm_medium=community&utm_source=github&utm_campaign=mindsdb%20repo)
 with sample data to get on-boarded as fast as possible. ## Database
-Integrations MindsDB works with most of the SQL and NoSQL databases, data
-lakes, data Streams and popular applications. | Connect your Data | Connect
-your Data | Connect your Data |-|-|-| | [Connect_Apache_Kafka] | [Connect
-Microsoft_Access] | [Oracle_Badge] | | [Connect_Amazon_Redshift] | [Airtable
-Badge] | [Pinot_Badge] | | [Connect_Cassandra] | [DataStax_Badge] | [Amazon_S3
-Badge] | | [Connect_CockroachDB] | [ckan_Badge] | [Supabase_Badge] | | [Connect
+Integrations MindsDB works with most of the SQL and NoSQL databases, data lakes
+and popular applications. | Connect your Data | Connect your Data | Connect
+your Data |-|-|-| | [Connect_Amazon_Redshift] | [Airtable_Badge] | [Pinot
+Badge] | | [Connect_Cassandra] | [DataStax_Badge] | [Amazon_S3_Badge] | |
+[Connect_CockroachDB] | [ckan_Badge] | [Supabase_Badge] | | [Connect
 Clickhouse] | [Google_Big_Query_Badge] | [SQLite_Badge] | | [Connect_MariaDB] |
 [Couchbase_Badge] | [TiDB_Badge] | | [Connect_SQL_Server] | [CrateDB_Badge] |
 [Timescale_Badge] | | [Connect_MongoDB] | [DoIt_Badge] | [Amazon_DynamoDB
 Badge] | | [Connect_PostgreSQL] | [IBMDB2_Badge] | [openGauss_Badge] | |
 [Connect_MySQL] | [Databricks_Badge] | [YugabyteDB_Badge] | [Connect_QuestDB] |
 [Apache_Druid_Badge] | | [StarRocks_Badge] | [Vertica_Badge] | [DuckDB_Badge] |
 | [Connect_SAP_HANA] | [Elastic_Badge] | [Cloud_Spanner_Badge] | | [Connect
@@ -99,25 +109,24 @@
 integration?](https://github.com/mindsdb/mindsdb/issues/
 new?assignees=&labels=&template=feature-mindsdb-request.yaml) ## Documentation
 You can find the complete documentation of MindsDB at [docs.mindsdb.com](https:
 //
 docs.mindsdb.com?utm_medium=community&utm_source=github&utm_campaign=mindsdb%20repo).
 ## Support If you found a bug, please submit an [issue on GitHub](https://
 github.com/mindsdb/mindsdb/issues/new/choose). To get community support, you
-can: * Post at MindsDB [Slack community](https://mindsdb.com/joincommunity). *
-Ask for help at our [GitHub Discussions](https://github.com/mindsdb/mindsdb/
-discussions). * Ask a question at [Stackoverflow](https://stackoverflow.com/
-questions/tagged/mindsdb) with a MindsDB tag. If you need commercial support,
-please [contact](https://mindsdb.com/contact/
+can: * Post a question at MindsDB [Slack community](https://mindsdb.com/
+joincommunity). * Ask for help at our [GitHub Discussions](https://github.com/
+mindsdb/mindsdb/discussions). * Ask a question at [Stackoverflow](https://
+stackoverflow.com/questions/tagged/mindsdb) with a MindsDB tag. If you need
+commercial support, please [contact](https://mindsdb.com/contact/
 ?utm_medium=community&utm_source=github&utm_campaign=mindsdb%20repo) MindsDB
 team. ## Contributing A great place to start contributing to MindsDB is to
-check our GitHub projects :checkered_flag: * Tutorials & documentation
-[dashboard tasks](https://github.com/mindsdb/mindsdb/projects/7). * Code
-contributor's [dashboard tasks](https://github.com/mindsdb/mindsdb/projects/8).
-* [First timers only issues](https://github.com/mindsdb/mindsdb/
+check our GitHub projects :checkered_flag: * Community contributor's [dashboard
+tasks](https://github.com/mindsdb/mindsdb/projects/8). * [First timers only
+issues](https://github.com/mindsdb/mindsdb/
 issues?q=is%3Aissue+is%3Aopen+label%3Afirst-timers-only), if this is your first
 time contributing to an open source project. We are always open to suggestions
 so feel free to open new issues with your ideas and we can guide you! Being
 part of the core team is accessible to anyone who is motivated and wants to be
 part of that journey! If you'd like to contribute to the project, refer to the
 [contributing documentation](https://docs.mindsdb.com/contribute/
 ?utm_medium=community&utm_source=github&utm_campaign=mindsdb%20repo). Please
@@ -131,7 +140,49 @@
 Subscribe to updates Join our [Slack community](https://mindsdb.com/
 joincommunity) and subscribe to the monthly [Developer Newsletter](https://
 mindsdb.com/newsletter/
 ?utm_medium=community&utm_source=github&utm_campaign=mindsdb%20repo) to get
 product updates, information about MindsDB events and contests, and useful
 content, like tutorials. ## License MindsDB is licensed under [GNU General
 Public License v3.0](https://github.com/mindsdb/mindsdb/blob/master/LICENSE)
+Platform: UNKNOWN Classifier: Programming Language :: Python :: 3 Classifier:
+Operating System :: OS Independent Requires-Python: >=3.8 Description-Content-
+Type: text/markdown Provides-Extra: grpc Provides-Extra: telemetry Provides-
+Extra: all_extras Provides-Extra: edgelessdb Provides-Extra: mlflow Provides-
+Extra: derby Provides-Extra: d0lt Provides-Extra: vitess Provides-Extra:
+newsapi Provides-Extra: databend Provides-Extra: scylla Provides-Extra:
+huggingface Provides-Extra: flaml Provides-Extra: aurora Provides-Extra:
+orioledb Provides-Extra: vertica Provides-Extra: trino Provides-Extra:
+cloud_sql Provides-Extra: questdb Provides-Extra: dynamodb Provides-Extra:
+cohere Provides-Extra: crate Provides-Extra: sqreamdb Provides-Extra: oceanbase
+Provides-Extra: statsforecast Provides-Extra: shopify Provides-Extra:
+huggingface_api Provides-Extra: github Provides-Extra: datastax Provides-Extra:
+postgres Provides-Extra: solr Provides-Extra: lightwood Provides-Extra: stripe
+Provides-Extra: tidb Provides-Extra: redshift Provides-Extra: impala Provides-
+Extra: ingres Provides-Extra: google_fit Provides-Extra: access Provides-Extra:
+s3 Provides-Extra: twitter Provides-Extra: neuralforecast Provides-Extra: gmail
+Provides-Extra: mysql Provides-Extra: plaid Provides-Extra: databricks
+Provides-Extra: supabase Provides-Extra: confluence Provides-Extra: sheets
+Provides-Extra: materialize Provides-Extra: firebird Provides-Extra: youtube
+Provides-Extra: mariadb Provides-Extra: monetdb Provides-Extra: pinot Provides-
+Extra: surrealdb Provides-Extra: informix Provides-Extra: influxdb Provides-
+Extra: merlion Provides-Extra: google_books Provides-Extra: binance Provides-
+Extra: db2 Provides-Extra: paypal Provides-Extra: strava Provides-Extra:
+bigquery Provides-Extra: cockroach Provides-Extra: starrocks Provides-Extra:
+clickhouse Provides-Extra: maxdb Provides-Extra: hsqldb Provides-Extra:
+cloud_spanner Provides-Extra: phoenix Provides-Extra: ludwig Provides-Extra:
+slack Provides-Extra: duckdb Provides-Extra: mongodb Provides-Extra: quickbooks
+Provides-Extra: sendinblue Provides-Extra: yugabyte Provides-Extra: matrixone
+Provides-Extra: openai Provides-Extra: reddit Provides-Extra: elasticsearch
+Provides-Extra: singlestore Provides-Extra: google_content_shopping Provides-
+Extra: langchain Provides-Extra: rocket_chat Provides-Extra: frappe Provides-
+Extra: ray_serve Provides-Extra: nuo_jdbc Provides-Extra: dremio Provides-
+Extra: timescaledb Provides-Extra: rockset Provides-Extra: druid Provides-
+Extra: ckan Provides-Extra: tdengine Provides-Extra: mssql Provides-Extra:
+oracle Provides-Extra: google_calendar Provides-Extra: sqlany Provides-Extra:
+jira Provides-Extra: planetscale Provides-Extra: autosklearn Provides-Extra:
+hive Provides-Extra: opengauss Provides-Extra: hana Provides-Extra: empress
+Provides-Extra: google_search Provides-Extra: gitlab Provides-Extra: airtable
+Provides-Extra: llama_index Provides-Extra: couchbase Provides-Extra: ignite
+Provides-Extra: cassandra Provides-Extra: monkeylearn Provides-Extra: tpot
+Provides-Extra: altibase Provides-Extra: snowflake Provides-Extra: teradata
+Provides-Extra: all_handlers_extras
```

### Comparing `MindsDB-23.5.4.1/mindsdb/__main__.py` & `MindsDB-23.6.1.1/mindsdb/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,43 +12,40 @@
 from packaging import version
 
 from mindsdb.__about__ import __version__ as mindsdb_version
 from mindsdb.api.http.start import start as start_http
 from mindsdb.api.mysql.start import start as start_mysql
 from mindsdb.api.mongo.start import start as start_mongo
 from mindsdb.api.postgres.start import start as start_postgres
+from mindsdb.interfaces.chatbot.chatbot_monitor import start as start_chatbot
 from mindsdb.interfaces.jobs.scheduler import start as start_scheduler
 from mindsdb.utilities.config import Config
 from mindsdb.utilities.ps import is_pid_listen_port, get_child_pids
 from mindsdb.utilities.functions import args_parse, get_versions_where_predictors_become_obsolete
 from mindsdb.utilities import log
-from mindsdb.interfaces.stream.stream import StreamController
-from mindsdb.interfaces.stream.utilities import STOP_THREADS_EVENT
 from mindsdb.interfaces.database.integrations import integration_controller
 import mindsdb.interfaces.storage.db as db
 from mindsdb.integrations.utilities.install import install_dependencies
 from mindsdb.utilities.fs import create_dirs_recursive, clean_process_marks, clean_unlinked_process_marks
 from mindsdb.utilities.telemetry import telemetry_file_exists, disable_telemetry
 from mindsdb.utilities.context import context as ctx
 from mindsdb.utilities.auth import register_oauth_client, get_aws_meta_data
 
-
 import torch.multiprocessing as mp
 try:
     mp.set_start_method('spawn')
 except RuntimeError:
     log.logger.info('Torch multiprocessing context already set, ignoring...')
 
 
 _stop_event = threading.Event()
 
 
 def close_api_gracefully(apis):
     _stop_event.set()
-    STOP_THREADS_EVENT.set()
     try:
         for api in apis.values():
             process = api['process']
             childs = get_child_pids(process.pid)
             for p in childs:
                 try:
                     os.kill(p, signal.SIGTERM)
@@ -251,23 +248,14 @@
                 engine = integration_data.get('type')
                 if engine is not None:
                     del integration_data['type']
                 integration_controller.add(integration_name, engine, integration_data)
             except Exception as e:
                 log.logger.error(f'\n\nError: {e} adding database integration {integration_name}\n\n')
 
-        stream_controller = StreamController()
-        for integration_name, integration_meta in integration_controller.get_all(sensitive_info=True).items():
-            if (
-                integration_meta.get('type') in stream_controller.known_dbs
-                and integration_meta.get('publish', False) is True
-            ):
-                print(f"Setting up stream: {integration_name}")
-                stream_controller.setup(integration_name)
-        del stream_controller
     # @TODO Backwards compatibility for tests, remove later
 
     if args.api is None:
         api_arr = ['http', 'mysql']
     else:
         api_arr = args.api.split(',')
 
@@ -286,22 +274,30 @@
 
     start_functions = {
         'http': start_http,
         'mysql': start_mysql,
         'mongodb': start_mongo,
         'postgres': start_postgres,
         'jobs': start_scheduler,
+        'chatbot': start_chatbot
     }
 
     if config.get('jobs', {}).get('disable') is not True:
         apis['jobs'] = {
             'process': None,
             'started': False
         }
 
+    # disabled on cloud
+    if config.get('chatbot', {}).get('disable') is not True and not is_cloud:
+        apis['chatbot'] = {
+            'process': None,
+            'started': False
+        }
+
     ctx = mp.get_context('spawn')
     for api_name, api_data in apis.items():
         if api_data['started']:
             continue
         print(f'{api_name} API: starting...')
         try:
             if api_name == 'http':
```

### Comparing `MindsDB-23.5.4.1/mindsdb/api/common/check_auth.py` & `MindsDB-23.6.1.1/mindsdb/api/common/check_auth.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/api/http/gui.py` & `MindsDB-23.6.1.1/mindsdb/api/http/gui.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/api/http/gunicorn_wrapper.py` & `MindsDB-23.6.1.1/mindsdb/api/http/gunicorn_wrapper.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/api/http/initialize.py` & `MindsDB-23.6.1.1/mindsdb/api/http/initialize.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,14 @@
 from mindsdb.api.http.namespaces.databases import ns_conf as databases_ns
 from mindsdb.api.http.namespaces.default import ns_conf as default_ns, check_auth
 from mindsdb.api.http.namespaces.file import ns_conf as file_ns
 from mindsdb.api.http.namespaces.handlers import ns_conf as handlers_ns
 from mindsdb.api.http.namespaces.models import ns_conf as models_ns
 from mindsdb.api.http.namespaces.projects import ns_conf as projects_ns
 from mindsdb.api.http.namespaces.sql import ns_conf as sql_ns
-from mindsdb.api.http.namespaces.stream import ns_conf as stream_ns
 from mindsdb.api.http.namespaces.tab import ns_conf as tab_ns
 from mindsdb.api.http.namespaces.tree import ns_conf as tree_ns
 from mindsdb.api.http.namespaces.views import ns_conf as views_ns
 from mindsdb.api.http.namespaces.util import ns_conf as utils_ns
 from mindsdb.api.nlp.nlp import ns_conf as nlp_ns
 from mindsdb.interfaces.database.integrations import integration_controller
 from mindsdb.interfaces.database.database import DatabaseController
@@ -197,15 +196,14 @@
         if static_root.joinpath(path).is_file():
             return send_from_directory(static_root, path)
         else:
             return send_from_directory(static_root, 'index.html')
 
     protected_namespaces = [
         tab_ns,
-        stream_ns,
         utils_ns,
         conf_ns,
         file_ns,
         sql_ns,
         analysis_ns,
         handlers_ns,
         tree_ns,
```

### Comparing `MindsDB-23.5.4.1/mindsdb/api/http/namespaces/analysis.py` & `MindsDB-23.6.1.1/mindsdb/api/http/namespaces/analysis.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/api/http/namespaces/auth.py` & `MindsDB-23.6.1.1/mindsdb/api/http/namespaces/auth.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/api/http/namespaces/config.py` & `MindsDB-23.6.1.1/mindsdb/api/http/namespaces/config.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 from flask_restx import Resource, abort
 from flask import current_app as ca
 from dateutil.tz import tzlocal
 
 from mindsdb.utilities import log
 from mindsdb.api.http.namespaces.configs.config import ns_conf
 from mindsdb.utilities.log_controller import get_logs
-from mindsdb.interfaces.stream.stream import StreamController
 from mindsdb.utilities.config import Config
 from mindsdb.api.http.utils import http_error
 
 
 @ns_conf.route('/logs')
 @ns_conf.param('name', 'Get logs')
 class GetLogs(Resource):
@@ -145,21 +144,17 @@
         if integration is not None:
             abort(400, f"Integration with name '{name}' already exists")
 
         try:
             engine = params['type']
             if engine is not None:
                 del params['type']
-            publish = params.pop('publish', False)
+            params.pop('publish', False)
             ca.integration_controller.add(name, engine, params)
 
-            if is_test is False and publish is True:
-                stream_controller = StreamController()
-                if engine in stream_controller.known_dbs and publish is True:
-                    stream_controller.setup(name)
         except Exception as e:
             log.logger.error(str(e))
             if temp_dir is not None:
                 shutil.rmtree(temp_dir)
             abort(500, f'Error during config update: {str(e)}')
 
         if temp_dir is not None:
@@ -191,17 +186,14 @@
             abort(400, f"Nothin to modify. '{name}' not exists.")
         try:
             if 'enabled' in params:
                 params['publish'] = params['enabled']
                 del params['enabled']
             ca.integration_controller.modify(name, params)
 
-            stream_controller = StreamController()
-            if params.get('type') in stream_controller.known_dbs and params.get('publish', False) is True:
-                stream_controller.setup(name)
         except Exception as e:
             log.logger.error(str(e))
             abort(500, f'Error during integration modifycation: {str(e)}')
         return '', 200
 
 
 @ns_conf.route('/integrations/<name>/check')
```

### Comparing `MindsDB-23.5.4.1/mindsdb/api/http/namespaces/databases.py` & `MindsDB-23.6.1.1/mindsdb/api/http/namespaces/databases.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/api/http/namespaces/default.py` & `MindsDB-23.6.1.1/mindsdb/api/http/namespaces/default.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/api/http/namespaces/file.py` & `MindsDB-23.6.1.1/mindsdb/api/http/namespaces/file.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/api/http/namespaces/handlers.py` & `MindsDB-23.6.1.1/mindsdb/api/http/namespaces/handlers.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/api/http/namespaces/models.py` & `MindsDB-23.6.1.1/mindsdb/api/http/namespaces/models.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/api/http/namespaces/projects.py` & `MindsDB-23.6.1.1/mindsdb/api/http/namespaces/projects.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/api/http/namespaces/sql.py` & `MindsDB-23.6.1.1/mindsdb/api/http/namespaces/sql.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/api/http/namespaces/tab.py` & `MindsDB-23.6.1.1/mindsdb/api/http/namespaces/tab.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/api/http/namespaces/tree.py` & `MindsDB-23.6.1.1/mindsdb/api/http/namespaces/tree.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/api/http/namespaces/util.py` & `MindsDB-23.6.1.1/mindsdb/api/http/namespaces/util.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/api/http/namespaces/views.py` & `MindsDB-23.6.1.1/mindsdb/api/http/namespaces/views.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/api/http/start.py` & `MindsDB-23.6.1.1/mindsdb/api/http/start.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,18 +22,22 @@
 
     app = initialize_app(config, no_studio, with_nlp)
 
     port = config['api']['http']['port']
     host = config['api']['http']['host']
 
     if server.lower() == 'waitress':
-        if host in ('', '0.0.0.0'):
-            serve(app, port=port, host='*', max_request_body_size=1073741824 * 10, inbuf_overflow=1073741824 * 10)
-        else:
-            serve(app, port=port, host=host, max_request_body_size=1073741824 * 10, inbuf_overflow=1073741824 * 10)
+        serve(
+            app,
+            host='*' if host in ('', '0.0.0.0') else host,
+            port=port,
+            threads=16,
+            max_request_body_size=1073741824 * 10,
+            inbuf_overflow=1073741824 * 10
+        )
     elif server.lower() == 'flask':
         # that will 'disable access' log in console
         logger = logging.getLogger('werkzeug')
         logger.setLevel(logging.WARNING)
 
         app.run(debug=False, port=port, host=host)
     elif server.lower() == 'gunicorn':
```

### Comparing `MindsDB-23.5.4.1/mindsdb/api/http/utils.py` & `MindsDB-23.6.1.1/mindsdb/api/http/utils.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/api/mongo/classes/query_sql.py` & `MindsDB-23.6.1.1/mindsdb/api/mongo/classes/query_sql.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/api/mongo/classes/responder.py` & `MindsDB-23.6.1.1/mindsdb/api/mongo/classes/responder.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/api/mongo/classes/responder_collection.py` & `MindsDB-23.6.1.1/mindsdb/api/mongo/classes/responder_collection.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/api/mongo/classes/scram.py` & `MindsDB-23.6.1.1/mindsdb/api/mongo/classes/scram.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/api/mongo/classes/session.py` & `MindsDB-23.6.1.1/mindsdb/api/mongo/classes/session.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/api/mongo/responders/__init__.py` & `MindsDB-23.6.1.1/mindsdb/api/mongo/responders/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/api/mongo/responders/aggregate.py` & `MindsDB-23.6.1.1/mindsdb/api/mongo/responders/aggregate.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/api/mongo/responders/coll_stats.py` & `MindsDB-23.6.1.1/mindsdb/api/mongo/responders/coll_stats.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/api/mongo/responders/company_id.py` & `MindsDB-23.6.1.1/mindsdb/api/mongo/responders/company_id.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/api/mongo/responders/connection_status.py` & `MindsDB-23.6.1.1/mindsdb/api/mongo/responders/connection_status.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/api/mongo/responders/db_stats.py` & `MindsDB-23.6.1.1/mindsdb/api/mongo/responders/db_stats.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/api/mongo/responders/delete.py` & `MindsDB-23.6.1.1/mindsdb/api/mongo/responders/delete.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/api/mongo/responders/find.py` & `MindsDB-23.6.1.1/mindsdb/api/mongo/responders/find.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/api/mongo/responders/get_parameter.py` & `MindsDB-23.6.1.1/mindsdb/api/mongo/responders/get_parameter.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/api/mongo/responders/host_info.py` & `MindsDB-23.6.1.1/mindsdb/api/mongo/responders/host_info.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/api/mongo/responders/insert.py` & `MindsDB-23.6.1.1/mindsdb/api/mongo/responders/insert.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/api/mongo/responders/list_collections.py` & `MindsDB-23.6.1.1/mindsdb/api/mongo/responders/list_collections.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/api/mongo/responders/list_databases.py` & `MindsDB-23.6.1.1/mindsdb/api/mongo/responders/list_databases.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/api/mongo/responders/list_indexes.py` & `MindsDB-23.6.1.1/mindsdb/api/mongo/responders/list_indexes.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/api/mongo/responders/sasl_continue.py` & `MindsDB-23.6.1.1/mindsdb/api/mongo/responders/sasl_continue.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/api/mongo/responders/sasl_start.py` & `MindsDB-23.6.1.1/mindsdb/api/mongo/responders/sasl_start.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/api/mongo/server.py` & `MindsDB-23.6.1.1/mindsdb/api/mongo/server.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/api/mongo/utilities/mongodb_ast.py` & `MindsDB-23.6.1.1/mindsdb/api/mongo/utilities/mongodb_ast.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/api/mongo/utilities/mongodb_parser.py` & `MindsDB-23.6.1.1/mindsdb/api/mongo/utilities/mongodb_parser.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/api/mongo/utilities/mongodb_query.py` & `MindsDB-23.6.1.1/mindsdb/api/mongo/utilities/mongodb_query.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/api/mysql/mysql_proxy/classes/client_capabilities.py` & `MindsDB-23.6.1.1/mindsdb/api/mysql/mysql_proxy/classes/client_capabilities.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/api/mysql/mysql_proxy/classes/com_operators.py` & `MindsDB-23.6.1.1/mindsdb/api/mysql/mysql_proxy/classes/com_operators.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/api/mysql/mysql_proxy/classes/fake_mysql_proxy/fake_mysql_proxy.py` & `MindsDB-23.6.1.1/mindsdb/api/mysql/mysql_proxy/classes/fake_mysql_proxy/fake_mysql_proxy.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/api/mysql/mysql_proxy/classes/server_capabilities.py` & `MindsDB-23.6.1.1/mindsdb/api/mysql/mysql_proxy/classes/server_capabilities.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/api/mysql/mysql_proxy/classes/sql_query.py` & `MindsDB-23.6.1.1/mindsdb/api/mysql/mysql_proxy/classes/sql_query.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/api/mysql/mysql_proxy/classes/sql_statement_parser.py` & `MindsDB-23.6.1.1/mindsdb/api/mysql/mysql_proxy/classes/sql_statement_parser.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/api/mysql/mysql_proxy/controllers/session_controller.py` & `MindsDB-23.6.1.1/mindsdb/api/mysql/mysql_proxy/controllers/session_controller.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/api/mysql/mysql_proxy/data_types/mysql_datum.py` & `MindsDB-23.6.1.1/mindsdb/api/mysql/mysql_proxy/data_types/mysql_datum.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packet.py` & `MindsDB-23.6.1.1/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packet.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/__init__.py` & `MindsDB-23.6.1.1/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/binary_resultset_row_package.py` & `MindsDB-23.6.1.1/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/binary_resultset_row_package.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/column_count_packet.py` & `MindsDB-23.6.1.1/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/column_count_packet.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/column_definition_packet.py` & `MindsDB-23.6.1.1/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/column_definition_packet.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/command_packet.py` & `MindsDB-23.6.1.1/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/command_packet.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/eof_packet.py` & `MindsDB-23.6.1.1/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/eof_packet.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/err_packet.py` & `MindsDB-23.6.1.1/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/err_packet.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/handshake_packet.py` & `MindsDB-23.6.1.1/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/handshake_packet.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/handshake_response_packet.py` & `MindsDB-23.6.1.1/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/handshake_response_packet.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/ok_packet.py` & `MindsDB-23.6.1.1/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/ok_packet.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/resultset_row_package.py` & `MindsDB-23.6.1.1/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/resultset_row_package.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/stmt_prepare_header.py` & `MindsDB-23.6.1.1/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/stmt_prepare_header.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/switch_auth_packet.py` & `MindsDB-23.6.1.1/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/switch_auth_packet.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/switch_auth_response_packet.py` & `MindsDB-23.6.1.1/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/switch_auth_response_packet.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/api/mysql/mysql_proxy/datahub/classes/tables_row.py` & `MindsDB-23.6.1.1/mindsdb/api/mysql/mysql_proxy/datahub/classes/tables_row.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/api/mysql/mysql_proxy/datahub/datanodes/information_schema_datanode.py` & `MindsDB-23.6.1.1/mindsdb/api/mysql/mysql_proxy/datahub/datanodes/information_schema_datanode.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/api/mysql/mysql_proxy/datahub/datanodes/integration_datanode.py` & `MindsDB-23.6.1.1/mindsdb/api/mysql/mysql_proxy/datahub/datanodes/integration_datanode.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/api/mysql/mysql_proxy/datahub/datanodes/project_datanode.py` & `MindsDB-23.6.1.1/mindsdb/api/mysql/mysql_proxy/datahub/datanodes/project_datanode.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/api/mysql/mysql_proxy/executor/data_types.py` & `MindsDB-23.6.1.1/mindsdb/api/mysql/mysql_proxy/executor/data_types.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/api/mysql/mysql_proxy/executor/executor.py` & `MindsDB-23.6.1.1/mindsdb/api/mysql/mysql_proxy/executor/executor.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/api/mysql/mysql_proxy/executor/executor_client_factory.py` & `MindsDB-23.6.1.1/mindsdb/api/mysql/mysql_proxy/executor/executor_client_factory.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,28 @@
 import os
 
 from mindsdb.api.mysql.mysql_proxy.executor.executor import Executor
-from mindsdb.api.mysql.mysql_proxy.executor.executor_grpc_client import ExecutorClientGRPC
 from mindsdb.utilities.log import get_log
 
 
 logger = get_log(logger_name="main")
 
 
 class ExecutorClientFactory:
     def __init__(self):
-        self.client_class = ExecutorClientGRPC
-
         self.host = os.environ.get("MINDSDB_EXECUTOR_SERVICE_HOST")
         self.port = os.environ.get("MINDSDB_EXECUTOR_SERVICE_PORT")
+        if self.host is not None and self.port is not None:
+            try:
+                from mindsdb.api.mysql.mysql_proxy.executor.executor_grpc_client import ExecutorClientGRPC
+                self.client_class = ExecutorClientGRPC
+            except (ImportError, ModuleNotFoundError):
+                logger.error("to use microservice mode please install 'pip install mindsdb[grpc]'")
+                self.host = None
+                self.port = None
 
     def __call__(self, session, sqlserver):
         if self.host is None or self.port is None:
             logger.info(
                 "%s.__call__: no post/port to ExecutorService have provided. Local Executor instance will use",
                 self.__class__.__name__,
             )
```

### Comparing `MindsDB-23.5.4.1/mindsdb/api/mysql/mysql_proxy/executor/executor_commands.py` & `MindsDB-23.6.1.1/mindsdb/api/mysql/mysql_proxy/executor/executor_commands.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,17 @@
     CreateMLEngine,
     DropMLEngine,
     DropDatasource,
     DropPredictor,
     CreateView,
     CreateJob,
     DropJob,
-    Evaluate
+    Evaluate,
+    CreateChatBot,
+    DropChatBot,
 )
 from mindsdb_sql import parse_sql
 from mindsdb_sql.parser.dialects.mysql import Variable
 from mindsdb_sql.parser.ast import (
     RollbackTransaction,
     CommitTransaction,
     StartTransaction,
@@ -77,14 +79,15 @@
     get_model_record,
     get_model_records,
     get_predictor_integration,
 )
 from mindsdb.integrations.libs.const import PREDICTOR_STATUS
 from mindsdb.interfaces.database.projects import ProjectController
 from mindsdb.interfaces.jobs.jobs_controller import JobsController
+from mindsdb.interfaces.chatbot.chatbot_controller import ChatBotController
 from mindsdb.interfaces.storage.model_fs import HandlerStorage
 from mindsdb.utilities.context import context as ctx
 from mindsdb.utilities.functions import resolve_model_identifier
 import mindsdb.utilities.profiler as profiler
 
 
 def _get_show_where(
@@ -595,14 +598,19 @@
             # TODO
             return self.answer_apply_predictor(statement)
         # -- jobs --
         elif type(statement) == CreateJob:
             return self.answer_create_job(statement)
         elif type(statement) == DropJob:
             return self.answer_drop_job(statement)
+        # -- chatbots --
+        elif type(statement) == CreateChatBot:
+            return self.answer_create_chatbot(statement)
+        elif type(statement) == DropChatBot:
+            return self.answer_drop_chatbot(statement)
         elif type(statement) == Evaluate:
             statement.data = parse_sql(statement.query_str, dialect='mindsdb')
             return self.answer_evaluate_metric(statement)
         else:
             log.logger.warning(f"Unknown SQL statement: {sql}")
             raise ErNotSupportedYet(f"Unknown SQL statement: {sql}")
 
@@ -624,14 +632,45 @@
         name = statement.name
         job_name = name.parts[-1]
         project_name = name.parts[-2] if len(name.parts) > 1 else self.session.database
         jobs_controller.delete(job_name, project_name)
 
         return ExecuteAnswer(ANSWER_TYPE.OK)
 
+    def answer_create_chatbot(self, statement):
+        chatbot_controller = ChatBotController()
+
+        name = statement.name
+        project_name = name.parts[-2] if len(name.parts) > 1 else self.session.database
+
+        database = self.session.integration_controller.get(statement.database.parts[-1])
+        if database is None:
+            raise SqlApiException(f'Database not found: {statement.database}')
+
+        chatbot_controller.add_chatbot(
+            name.parts[-1],
+            project_name=project_name,
+            model_name=statement.model.parts[-1],
+            database_id=database['id'],
+            params=statement.params
+        )
+        return ExecuteAnswer(ANSWER_TYPE.OK)
+
+    def answer_drop_chatbot(self, statement):
+        chatbot_controller = ChatBotController()
+
+        name = statement.name
+        project_name = name.parts[-2] if len(name.parts) > 1 else self.session.database
+
+        chatbot_controller.delete_chatbot(
+            name.parts[-1],
+            project_name=project_name
+        )
+        return ExecuteAnswer(ANSWER_TYPE.OK)
+
     def answer_evaluate_metric(self, statement):
         try:
             sqlquery = SQLQuery(statement.data, session=self.session)
         except Exception as e:
             raise Exception(f'Nested query failed to execute with error: "{e}", please check and try again.')
         result = sqlquery.fetch(self.session.datahub)
         df = pd.DataFrame.from_dict(result["result"])
@@ -723,24 +762,23 @@
                     f"Can't start {phase_name} process while predictor is in status 'training' or 'generating'"
                 )
 
     def answer_retrain_predictor(self, statement):
         model_record = self._get_model_info(statement.name)['model_record']
 
         if statement.integration_name is None:
-            if model_record.data_integration_ref is None:
-                raise Exception("The model does not have an associated dataset")
-            if model_record.data_integration_ref["type"] == "integration":
-                integration = self.session.integration_controller.get_by_id(
-                    model_record.data_integration_ref["id"]
-                )
-                if integration is None:
-                    raise Exception(
-                        "The database from which the model was trained no longer exists"
+            if model_record.data_integration_ref is not None:
+                if model_record.data_integration_ref["type"] == "integration":
+                    integration = self.session.integration_controller.get_by_id(
+                        model_record.data_integration_ref["id"]
                     )
+                    if integration is None:
+                        raise Exception(
+                            "The database from which the model was trained no longer exists"
+                        )
 
         ml_handler = None
         if statement.using is not None:
             # repack using with lower names
             statement.using = {k.lower(): v for k, v in statement.using.items()}
 
             if "engine" in statement.using:
@@ -872,15 +910,16 @@
             self.session.integration_controller.get_handlers_import_status().get(
                 statement.handler
             )
         )
         if handler_module_meta is None:
             raise SqlApiException(f"There is no engine '{statement.handler}'")
         if handler_module_meta.get("import", {}).get("success") is not True:
-            raise SqlApiException(f"Can't import engine '{statement.handler}'")
+            log.logger.info(f"to use {statement.handler} please install it 'pip install mindsdb[{statement.handler}]'")
+            raise SqlApiException(f"Can't import engine '{statement.handler}'. to use it please install it 'pip install mindsdb[{statement.handler}]'")
 
         integration_id = self.session.integration_controller.add(
             name=name,
             engine=statement.handler,
             connection_args=statement.params
         )
```

### Comparing `MindsDB-23.5.4.1/mindsdb/api/mysql/mysql_proxy/executor/executor_grpc_client.py` & `MindsDB-23.6.1.1/mindsdb/api/mysql/mysql_proxy/executor/executor_grpc_client.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 import os
 import json
 import pickle
 from uuid import uuid4
 
-import grpc
-from mindsdb.microservices_grpc.executor import executor_pb2_grpc
-from mindsdb.microservices_grpc.executor import executor_pb2
-
 from mindsdb.utilities.log import get_log
 from mindsdb.utilities.context import context as ctx
 from mindsdb.integrations.libs.handler_helpers import action_logger
+logger = get_log("main")
 
 
-logger = get_log("main")
+try:
+    import grpc
+    from mindsdb.microservices_grpc.executor import executor_pb2_grpc
+    from mindsdb.microservices_grpc.executor import executor_pb2
+except ImportError:
+    logger.error("to user microservice mode please install 'pip install mindsdb[grpc]'")
 
 
 class ExecutorClientGRPC:
 
     def __init__(self, session, sqlserver):
         self.id = f"executor_{uuid4()}"
```

### Comparing `MindsDB-23.5.4.1/mindsdb/api/mysql/mysql_proxy/executor/executor_grpc_wrapper.py` & `MindsDB-23.6.1.1/mindsdb/api/mysql/mysql_proxy/executor/executor_grpc_wrapper.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/api/mysql/mysql_proxy/executor/executor_service.py` & `MindsDB-23.6.1.1/mindsdb/api/mysql/mysql_proxy/executor/executor_service.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/api/mysql/mysql_proxy/external_libs/mysql_scramble.py` & `MindsDB-23.6.1.1/mindsdb/api/mysql/mysql_proxy/external_libs/mysql_scramble.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/api/mysql/mysql_proxy/libs/constants/mysql.py` & `MindsDB-23.6.1.1/mindsdb/api/mysql/mysql_proxy/libs/constants/mysql.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/api/mysql/mysql_proxy/mysql_proxy.py` & `MindsDB-23.6.1.1/mindsdb/api/mysql/mysql_proxy/mysql_proxy.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/api/mysql/mysql_proxy/utilities/exceptions.py` & `MindsDB-23.6.1.1/mindsdb/api/mysql/mysql_proxy/utilities/exceptions.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/api/mysql/mysql_proxy/utilities/functions.py` & `MindsDB-23.6.1.1/mindsdb/api/mysql/mysql_proxy/utilities/functions.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/api/mysql/mysql_proxy/utilities/lightwood_dtype.py` & `MindsDB-23.6.1.1/mindsdb/api/mysql/mysql_proxy/utilities/lightwood_dtype.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/api/mysql/mysql_proxy/utilities/sql.py` & `MindsDB-23.6.1.1/mindsdb/api/mysql/mysql_proxy/utilities/sql.py`

 * *Files 5% similar despite different names*

```diff
@@ -32,14 +32,15 @@
 
     if isinstance(query_ast, Select) is False \
        or isinstance(query_ast.from_table, Identifier) is False:
         raise Exception(
             "Only 'SELECT from TABLE' statements supported for internal query"
         )
 
+    table_name = query_ast.from_table.parts[0]
     query_ast.from_table.parts = ['df_table']
 
     def adapt_query(node, is_table, **kwargs):
         if is_table:
             return
         if isinstance(node, Identifier):
             if len(node.parts) > 1:
@@ -65,14 +66,19 @@
         query_str = render.get_string(query_ast, with_failback=False)
     except Exception as e:
         log.logger.error(
             f"Exception during query casting to 'postgres' dialect. Query: {str(query)}. Error: {e}"
         )
         query_str = render.get_string(query_ast, with_failback=True)
 
+    # workaround to prevent duckdb.TypeMismatchException
+    if len(df) > 0 and table_name.lower() in ('models', 'predictors'):
+        if 'TRAINING_OPTIONS' in df.columns:
+            df = df.astype({'TRAINING_OPTIONS': 'string'})
+
     con = duckdb.connect(database=':memory:')
     con.register('df_table', df)
     result_df = con.execute(query_str).fetchdf()
     result_df = result_df.replace({np.nan: None})
     description = con.description
     con.unregister('df_table')
     con.close()
```

### Comparing `MindsDB-23.5.4.1/mindsdb/api/nlp/nlp.py` & `MindsDB-23.6.1.1/mindsdb/api/nlp/nlp.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/api/postgres/postgres_proxy/executor/executor.py` & `MindsDB-23.6.1.1/mindsdb/api/postgres/postgres_proxy/executor/executor.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/api/postgres/postgres_proxy/postgres_packets/errors.py` & `MindsDB-23.6.1.1/mindsdb/api/postgres/postgres_proxy/postgres_packets/errors.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/api/postgres/postgres_proxy/postgres_packets/postgres_fields.py` & `MindsDB-23.6.1.1/mindsdb/api/postgres/postgres_proxy/postgres_packets/postgres_fields.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/api/postgres/postgres_proxy/postgres_packets/postgres_message.py` & `MindsDB-23.6.1.1/mindsdb/api/postgres/postgres_proxy/postgres_packets/postgres_message.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/api/postgres/postgres_proxy/postgres_packets/postgres_message_formats.py` & `MindsDB-23.6.1.1/mindsdb/api/postgres/postgres_proxy/postgres_packets/postgres_message_formats.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/api/postgres/postgres_proxy/postgres_packets/postgres_message_identifiers.py` & `MindsDB-23.6.1.1/mindsdb/api/postgres/postgres_proxy/postgres_packets/postgres_message_identifiers.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/api/postgres/postgres_proxy/postgres_packets/postgres_packets.py` & `MindsDB-23.6.1.1/mindsdb/api/postgres/postgres_proxy/postgres_packets/postgres_packets.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/api/postgres/postgres_proxy/postgres_proxy.py` & `MindsDB-23.6.1.1/mindsdb/api/postgres/postgres_proxy/postgres_proxy.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/access_handler/__init__.py` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/access_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/access_handler/access_handler.py` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/access_handler/access_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/access_handler/icon.png` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/access_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/access_handler/tests/test_access_handler.py` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/access_handler/tests/test_access_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/airtable_handler/__init__.py` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/airtable_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/airtable_handler/airtable_handler.py` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/airtable_handler/airtable_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/airtable_handler/icon.png` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/airtable_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/airtable_handler/tests/test_airtable_handler.py` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/airtable_handler/tests/test_airtable_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/altibase_handler/__init__.py` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/altibase_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/altibase_handler/altibase_handler.py` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/altibase_handler/altibase_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/altibase_handler/icon.png` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/altibase_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/altibase_handler/tests/test_altibase_handler.py` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/altibase_handler/tests/test_altibase_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/aurora_handler/__init__.py` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/aurora_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/aurora_handler/aurora_handler.py` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/aurora_handler/aurora_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/aurora_handler/icon.png` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/aurora_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/aurora_handler/tests/test_aurora_mysql_handler.py` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/aurora_handler/tests/test_aurora_mysql_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/aurora_handler/tests/test_aurora_postgres_handler.py` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/aurora_handler/tests/test_aurora_postgres_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/autokeras_handler/__init__.py` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/autokeras_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/autokeras_handler/autokeras_handler.py` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/autokeras_handler/autokeras_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/autokeras_handler/setup.py` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/autokeras_handler/setup.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/autosklearn_handler/__init__.py` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/autosklearn_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/autosklearn_handler/autosklearn_handler.py` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/autosklearn_handler/autosklearn_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/autosklearn_handler/config.py` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/autosklearn_handler/config.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/autosklearn_handler/setup.py` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/autosklearn_handler/setup.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/bigquery_handler/__init__.py` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/bigquery_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/bigquery_handler/bigquery_handler.py` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/bigquery_handler/bigquery_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/bigquery_handler/logo.svg` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/bigquery_handler/logo.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/bigquery_handler/tests/test_bigquery_handler.py` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/bigquery_handler/tests/test_bigquery_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/binance_handler/binance_handler.py` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/binance_handler/binance_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/binance_handler/binance_tables.py` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/binance_handler/binance_tables.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/binance_handler/icon.svg` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/binance_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/byom_handler/byom_handler.py` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/byom_handler/byom_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/byom_handler/proc_wrapper.py` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/byom_handler/proc_wrapper.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/cassandra_handler/__init__.py` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/cassandra_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/cassandra_handler/cassandra_handler.py` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/cassandra_handler/cassandra_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/cassandra_handler/logo.png` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/cassandra_handler/logo.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/cassandra_handler/tests/test_cassandra_handler.py` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/cassandra_handler/tests/test_cassandra_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/ckan_handler/ckan_handler.py` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/ckan_handler/ckan_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/ckan_handler/logo.png` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/ckan_handler/logo.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/ckan_handler/tests/test_ckan_handler.py` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/ckan_handler/tests/test_ckan_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/clickhouse_handler/__init__.py` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/clickhouse_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/clickhouse_handler/clickhouse_handler.py` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/clickhouse_handler/clickhouse_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/clickhouse_handler/tests/test_clickhouse_handler.py` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/clickhouse_handler/tests/test_clickhouse_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/cloud_spanner_handler/__init__.py` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/cloud_spanner_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/cloud_spanner_handler/cloud_spanner_handler.py` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/cloud_spanner_handler/cloud_spanner_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/cloud_spanner_handler/icon.png` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/cloud_spanner_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/cloud_spanner_handler/tests/test_cloud_spanner_handler.py` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/cloud_spanner_handler/tests/test_cloud_spanner_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/cloud_sql_handler/__init__.py` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/cloud_sql_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/cloud_sql_handler/cloud_sql_handler.py` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/cloud_sql_handler/cloud_sql_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/cloud_sql_handler/icon.png` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/cloud_sql_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/cloud_sql_handler/tests/test_cloud_sql_mssql_handler.py` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/cloud_sql_handler/tests/test_cloud_sql_mssql_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/cloud_sql_handler/tests/test_cloud_sql_mysql_handler.py` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/cloud_sql_handler/tests/test_cloud_sql_mysql_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/cockroach_handler/tests/test_cockroachdb_handler.py` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/cockroach_handler/tests/test_cockroachdb_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/confluence_handler/__init__.py` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/confluence_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/confluence_handler/confluence_handler.py` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/confluence_handler/confluence_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/confluence_handler/confluence_table.py` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/confluence_handler/confluence_table.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/confluence_handler/icon.png` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/confluence_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/couchbase_handler/__init__.py` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/couchbase_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/couchbase_handler/couchbase_handler.py` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/couchbase_handler/couchbase_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/couchbase_handler/icon.svg` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/couchbase_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/couchbase_handler/tests/test_couchbase_handler.py` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/couchbase_handler/tests/test_couchbase_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/crate_handler/crate_handler.py` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/crate_handler/crate_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/crate_handler/icon.svg` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/crate_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/crate_handler/tests/test_crate_handler.py` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/crate_handler/tests/test_crate_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/d0lt_handler/create-db.png` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/d0lt_handler/create-db.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/d0lt_handler/create-predictor.png` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/d0lt_handler/create-predictor.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/d0lt_handler/icon.svg` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/d0lt_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/d0lt_handler/predict-target.png` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/d0lt_handler/predict-target.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/d0lt_handler/tests/test_d0lt_handler.py` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/d0lt_handler/tests/test_d0lt_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/databend_handler/__init__.py` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/databend_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/databend_handler/databend_handler.py` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/databend_handler/databend_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/databend_handler/icon.png` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/databend_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/databend_handler/tests/test_databend_handler.py` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/databend_handler/tests/test_databend_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/databricks_handler/__init__.py` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/databricks_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/databricks_handler/databricks/createdb.jpg` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/databricks_handler/databricks/createdb.jpg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/databricks_handler/databricks/createpred.jpg` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/databricks_handler/databricks/createpred.jpg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/databricks_handler/databricks/hivmetastore.jpg` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/databricks_handler/databricks/hivmetastore.jpg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/databricks_handler/databricks/mindsdbdatabricks.jpg` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/databricks_handler/databricks/mindsdbdatabricks.jpg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/databricks_handler/databricks/selectfrom.jpg` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/databricks_handler/databricks/selectfrom.jpg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/databricks_handler/databricks_handler.py` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/databricks_handler/databricks_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/databricks_handler/icon.png` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/databricks_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/databricks_handler/tests/test_databricks_handler.py` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/databricks_handler/tests/test_databricks_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/datastax_handler/__init__.py` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/datastax_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/datastax_handler/logo.png` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/datastax_handler/logo.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/datastax_handler/tests/test_cassandra_handler.py` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/datastax_handler/tests/test_cassandra_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/db2_handler/__init__.py` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/db2_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/db2_handler/db2_handler.py` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/db2_handler/db2_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/db2_handler/icon.png` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/db2_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/db2_handler/tests/test_db2_handler.py` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/db2_handler/tests/test_db2_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/derby_handler/__init__.py` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/derby_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/derby_handler/derby_handler.py` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/derby_handler/derby_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/derby_handler/icon.png` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/derby_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/derby_handler/tests/test_derby_handler.py` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/derby_handler/tests/test_derby_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/dremio_handler/__init__.py` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/dremio_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/dremio_handler/dremio_handler.py` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/dremio_handler/dremio_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/dremio_handler/icon.png` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/dremio_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/dremio_handler/tests/test_dremio_handler.py` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/dremio_handler/tests/test_dremio_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/druid_handler/__init__.py` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/druid_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/druid_handler/druid_handler.py` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/druid_handler/druid_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/druid_handler/icon.png` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/druid_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/druid_handler/tests/test_druid_handler.py` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/druid_handler/tests/test_druid_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/duckdb_handler/__init__.py` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/duckdb_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/duckdb_handler/duckdb_handler.py` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/duckdb_handler/duckdb_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/duckdb_handler/icon.png` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/duckdb_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/duckdb_handler/tests/test_duckdb_handler.py` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/duckdb_handler/tests/test_duckdb_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/dynamodb_handler/__init__.py` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/dynamodb_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/dynamodb_handler/dynamodb_handler.py` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/dynamodb_handler/dynamodb_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/dynamodb_handler/icon.png` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/dynamodb_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/dynamodb_handler/tests/test_dynamodb_handler.py` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/dynamodb_handler/tests/test_dynamodb_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/edgelessdb_handler/__init__.py` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/edgelessdb_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/edgelessdb_handler/edgelessdb_handler.py` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/edgelessdb_handler/edgelessdb_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/edgelessdb_handler/icon.svg` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/edgelessdb_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/edgelessdb_handler/tests/test_edgelessdb_handler.py` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/edgelessdb_handler/tests/test_edgelessdb_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/elasticsearch_handler/__init__.py` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/elasticsearch_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/elasticsearch_handler/elasticsearch_handler.py` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/elasticsearch_handler/elasticsearch_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/elasticsearch_handler/icon.png` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/elasticsearch_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/elasticsearch_handler/tests/test_elasticsearch_handler.py` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/elasticsearch_handler/tests/test_elasticsearch_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/empress_handler/__init__.py` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/empress_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/empress_handler/empress_handler.py` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/empress_handler/empress_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/empress_handler/icon.svg` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/empress_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/empress_handler/tests/test_empress_handler.py` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/empress_handler/tests/test_empress_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/eventstoredb_handler/eventstoredb_handler.py` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/eventstoredb_handler/eventstoredb_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/eventstoredb_handler/icon.svg` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/eventstoredb_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/file_handler/file_handler.py` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/file_handler/file_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/firebird_handler/__init__.py` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/firebird_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/firebird_handler/firebird_handler.py` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/firebird_handler/firebird_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/firebird_handler/icon.png` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/firebird_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/firebird_handler/tests/test_firebird_handler.py` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/firebird_handler/tests/test_firebird_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/frappe_handler/frappe_client.py` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/frappe_handler/frappe_client.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import json
 import requests
 from typing import Dict, List
 
 
 class FrappeClient(object):
     """Client to interact with the Frappe API.
     
@@ -33,32 +34,49 @@
         document_response = requests.get(
             f'{self.base_url}/resource/{doctype}/{name}',
             headers=self.headers)
         if not document_response.ok:
             document_response.raise_for_status()
         return document_response.json()['data']
 
-    def get_documents(self, doctype: str, limit: int = None, filters: List[List] = None) -> List[Dict]:
+    def get_documents(self, doctype: str, limit: int = None, fields: List[str] = None, filters: List[List] = None) -> List[Dict]:
         """Gets all documents matching the given doctype from Frappe.
         
         See https://frappeframework.com/docs/v14/user/en/api/rest#listing-documents
         Args:
             doctype (str): The document type to retrieve.
             limit (int): At most, how many messages to return.
             filters (List[List]): List of filters in the form [field, operator, value] e.g. ["amount", ">", 50]
         """
-        params = {}
+        params = {
+            'fields': json.dumps(["*"])
+        }
         if limit is not None:
-            params['limit'] = limit
+            params['limit_page_length'] = limit
         if filters is not None:
-            params['filters'] = filters
+            params['filters'] = json.dumps(filters)
+        if fields is not None:
+            params['fields'] = json.dumps(fields)
         documents_response = requests.get(
-            f'{self.base_url}/resource/{doctype}',
+            f'{self.base_url}/resource/{doctype}/',
             params=params,
-            headers=self.headers)
+            headers=self.headers,
+            allow_redirects=False)
+        if documents_response.is_redirect:
+            # We have to manually redirect to preserve the 'Authorization' header.
+            # See https://github.com/request/request/pull/1184/commits/210b326fd8625f358e06c59dc11e74468b1de515.
+            redirect_url = documents_response.headers.get('location', None)
+            if redirect_url is None:
+                raise requests.HTTPError('Could not find redirect URL')
+            documents_response = requests.get(
+                redirect_url,
+                params=params,
+                headers=self.headers,
+                allow_redirects=False)
+
         if not documents_response.ok:
             documents_response.raise_for_status()
         return documents_response.json()['data']
 
     def post_document(
             self,
             doctype: str,
```

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/frappe_handler/frappe_tables.py` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/frappe_handler/frappe_tables.py`

 * *Files 3% similar despite different names*

```diff
@@ -31,14 +31,16 @@
                 filters.append([arg1, op, arg2])
 
         if not 'doctype' in params:
             raise ValueError('"doctype" parameter required')
 
         if query.limit:
             params['limit'] = query.limit.value
+        if filters:
+            params['filters'] = filters
 
         if 'name' in params:
             document_data = self.handler.call_frappe_api(
                 method_name='get_document',
                 params=params
             )
         else:
```

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/frappe_handler/icon.svg` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/frappe_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/github_handler/github_handler.py` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/github_handler/github_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/github_handler/github_tables.py` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/github_handler/github_tables.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/github_handler/icon.svg` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/github_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/gitlab_handler/gitlab_handler.py` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/gitlab_handler/gitlab_handler.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import gitlab
 
-from mindsdb.integrations.handlers.gitlab_handler.gitlab_tables import GitlabIssuesTable
+from mindsdb.integrations.handlers.gitlab_handler.gitlab_tables import GitlabIssuesTable, GitlabMergeRequestsTable
 from mindsdb.integrations.libs.api_handler import APIHandler
 from mindsdb.integrations.libs.response import (
     HandlerStatusResponse as StatusResponse,
 )
 
 from mindsdb.utilities.log import get_log
 from mindsdb_sql import parse_sql
@@ -27,15 +27,17 @@
         self.repository = connection_data["repository"]
         self.kwargs = kwargs
 
         self.connection = None
         self.is_connected = False
 
         gitlab_issues_data = GitlabIssuesTable(self)
+        gitlab_merge_requests_data = GitlabMergeRequestsTable(self)
         self._register_table("issues", gitlab_issues_data)
+        self._register_table("merge_requests", gitlab_merge_requests_data)
 
     def connect(self) -> StatusResponse:
         """ Set up the connections required by the handler
         Returns:
             HandlerStatusResponse
         """
```

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/gitlab_handler/icon.svg` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/gitlab_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/gmail_handler/gmail_handler.py` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/gmail_handler/gmail_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/gmail_handler/tests/test_gmail_handler.py` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/gmail_handler/tests/test_gmail_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/google_books_handler/google_books_handler.py` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/google_books_handler/google_books_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/google_books_handler/google_books_tables.py` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/google_books_handler/google_books_tables.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/google_books_handler/icon.svg` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/google_books_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/google_books_handler/tests/test_google_books_handler.py` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/google_books_handler/tests/test_google_books_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/google_calendar_handler/__init__.py` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/google_calendar_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/google_calendar_handler/google_calendar_handler.py` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/google_calendar_handler/google_calendar_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/google_calendar_handler/google_calendar_tables.py` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/google_calendar_handler/google_calendar_tables.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/google_calendar_handler/icon.svg` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/google_calendar_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/google_calendar_handler/tests/test_google_calendar_handler.py` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/google_calendar_handler/tests/test_google_calendar_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/google_content_shopping_handler/__init__.py` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/google_content_shopping_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/google_content_shopping_handler/google_content_shopping_handler.py` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/google_content_shopping_handler/google_content_shopping_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/google_content_shopping_handler/google_content_shopping_tables.py` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/google_content_shopping_handler/google_content_shopping_tables.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/google_content_shopping_handler/icon.png` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/google_content_shopping_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/google_content_shopping_handler/tests/test_google_content_shopping_handler.py` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/google_content_shopping_handler/tests/test_google_content_shopping_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/google_fit_handler/google_fit_handler.py` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/google_fit_handler/google_fit_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/google_fit_handler/google_fit_tables.py` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/google_fit_handler/google_fit_tables.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/google_fit_handler/icon.png` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/google_fit_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/google_search_handler/__init__.py` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/google_search_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/google_search_handler/google_search_handler.py` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/google_search_handler/google_search_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/google_search_handler/google_search_tables.py` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/google_search_handler/google_search_tables.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/google_search_handler/icon.svg` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/google_search_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/google_search_handler/tests/test_google_search_handler.py` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/google_search_handler/tests/test_google_search_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/hackernews_handler/hn_handler.py` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/hackernews_handler/hn_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/hackernews_handler/hn_table.py` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/hackernews_handler/hn_table.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/hackernews_handler/icon.svg` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/hackernews_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/hana_handler/__init__.py` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/hana_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/hana_handler/hana_handler.py` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/hana_handler/hana_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/hana_handler/icon.svg` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/hana_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/hive_handler/__init__.py` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/hive_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/hive_handler/hive_handler.py` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/hive_handler/hive_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/hive_handler/icon.svg` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/hive_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/hive_handler/tests/test_hive_handler.py` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/hive_handler/tests/test_hive_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/hsqldb_handler/__init__.py` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/hsqldb_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/hsqldb_handler/hsqldb_handler.py` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/hsqldb_handler/hsqldb_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/hsqldb_handler/icon.png` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/hsqldb_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/huggingface_api_handler/__init__.py` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/huggingface_api_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/huggingface_api_handler/huggingface_api_handler.py` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/huggingface_api_handler/huggingface_api_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/huggingface_api_handler/setup.py` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/huggingface_api_handler/setup.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/huggingface_handler/__init__.py` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/huggingface_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/huggingface_handler/huggingface_handler.py` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/huggingface_handler/huggingface_handler.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
             args = args['using']
 
         hf_api = HfApi()
 
         # check model is pytorch based
         metadata = hf_api.model_info(args['model_name'])
         if 'pytorch' not in metadata.tags:
-            raise Exception('Currently only PyTorch models are supported (https://huggingface.co/models?library=pytorch&sort=downloads). To request another library, please contact us on our community slack (https://mindsdbcommunity.slack.com/join/shared_invite/zt-1e2cxo4ts-dUuoryp8n2hhyymPlzjD0A#/shared-invite/email).')
+            raise Exception('Currently only PyTorch models are supported (https://huggingface.co/models?library=pytorch&sort=downloads). To request another library, please contact us on our community slack (https://mindsdb.com/joincommunity).')
 
         # check model task
         supported_tasks = ['text-classification',
                            'zero-shot-classification',
                            'translation',
                            'summarization',
                            'text2text-generation',
```

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/huggingface_handler/setup.py` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/huggingface_handler/setup.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/ignite_handler/__init__.py` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/ignite_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/ignite_handler/icon.png` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/ignite_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/ignite_handler/ignite_handler.py` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/ignite_handler/ignite_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/ignite_handler/tests/test_ignite_handler.py` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/ignite_handler/tests/test_ignite_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/impala_handler/__init__.py` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/impala_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/impala_handler/icon.svg` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/impala_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/impala_handler/impala_handler.py` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/impala_handler/impala_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/impala_handler/tests/test_impala_handler.py` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/impala_handler/tests/test_impala_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/influxdb_handler/__init__.py` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/influxdb_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/influxdb_handler/icon.png` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/influxdb_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/influxdb_handler/influxdb_handler.py` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/influxdb_handler/influxdb_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/influxdb_handler/influxdb_tables.py` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/influxdb_handler/influxdb_tables.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/informix_handler/icon.png` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/informix_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/informix_handler/informix_handler.py` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/informix_handler/informix_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/informix_handler/tests/test_informix_handler.py` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/informix_handler/tests/test_informix_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/ingres_handler/__init__.py` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/ingres_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/ingres_handler/icon.svg` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/ingres_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/ingres_handler/ingres_handler.py` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/ingres_handler/ingres_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/ingres_handler/tests/test_ingres_handler.py` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/ingres_handler/tests/test_ingres_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/jira_handler/__init__.py` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/jira_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/jira_handler/icon.png` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/jira_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/jira_handler/jira_handler.py` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/jira_handler/jira_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/jira_handler/jira_table.py` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/jira_handler/jira_table.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/langchain_handler/langchain_handler.py` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/langchain_handler/langchain_handler.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 import re
 import os
 from typing import Optional, Dict
 
 import numpy as np
 import pandas as pd
 
+from langchain.schema import SystemMessage
+from langchain.agents import AgentType
 from langchain.llms import OpenAI
 from langchain.chat_models import ChatOpenAI  # GPT-4 fails to follow the output langchain requires, avoid using for now
 from langchain.agents import initialize_agent, load_tools, Tool, create_sql_agent
 from langchain.prompts import PromptTemplate
 from langchain.utilities import GoogleSerperAPIWrapper
 from langchain.agents.agent_toolkits import SQLDatabaseToolkit
-from langchain.chains.conversation.memory import ConversationSummaryMemory
+from langchain.chains.conversation.memory import ConversationSummaryBufferMemory
 
 from mindsdb.integrations.handlers.openai_handler.openai_handler import OpenAIHandler, CHAT_MODELS
 from mindsdb.integrations.handlers.langchain_handler.mindsdb_database_agent import MindsDBSQL
 from mindsdb_sql import parse_sql, Insert
 
 
 _DEFAULT_MODEL = 'gpt-3.5-turbo'  # TODO: enable other LLM backends (AI21, Anthropic, etc.)
@@ -46,14 +48,15 @@
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.stops = []
         self.default_model = _DEFAULT_MODEL
         self.default_max_tokens = _DEFAULT_MAX_TOKENS
         self.default_agent_model = _DEFAULT_AGENT_MODEL
         self.default_agent_tools = _DEFAULT_AGENT_TOOLS
+        self.write_privileges = False  # if True, this agent is able to write into other active mindsdb integrations
 
     def _get_serper_api_key(self, args, strict=True):
         if 'serper_api_key' in args:
             return args['serper_api_key']
         # 2
         connection_args = self.engine_storage.get_connection_args()
         if 'serper_api_key' in connection_args:
@@ -63,121 +66,217 @@
         if api_key is not None:
             return api_key
 
         if strict:
             raise Exception(f'Missing API key serper_api_key. Either re-create this ML_ENGINE specifying the `serper_api_key` parameter,\
                  or re-create this model and pass the API key with `USING` syntax.')  # noqa
 
+    def create(self, target, args=None, **kwargs):
+        self.write_privileges = args.get('using', {}).get('writer', self.write_privileges)
+        self.default_agent_tools = args.get('tools', self.default_agent_tools)
+        super().create(target, args, **kwargs)
+
     @staticmethod
     def create_validation(target, args=None, **kwargs):
         if 'using' not in args:
             raise Exception("LangChain engine requires a USING clause! Refer to its documentation for more details.")
         else:
             args = args['using']
 
-        if len(set(args.keys()) & {'prompt_template'}) == 0:
-            raise Exception('Please provide a `prompt_template` for this engine.')
+        if args.get('mode') != 'conversational':
+            if len(set(args.keys()) & {'prompt_template'}) == 0:
+                raise Exception('Please provide a `prompt_template` for this engine.')
 
     def predict(self, df, args=None):
         """
         Dispatch is performed depending on the underlying model type. Currently, only the default text completion
         is supported.
         """
         executor = args['executor']  # used as tool in custom tool for the agent to have mindsdb-wide access
         pred_args = args['predict_params'] if args else {}
         args = self.model_storage.json_get('args')
         args['executor'] = executor
 
         df = df.reset_index(drop=True)
 
-        if 'prompt_template' not in args and 'prompt_template' not in pred_args:
-            raise Exception(f"This model expects a prompt template, please provide one.")
+        if args.get('mode') != 'conversational':
+            if 'prompt_template' not in args and 'prompt_template' not in pred_args:
+                raise Exception(f"This model expects a prompt template, please provide one.")
 
         if 'stops' in pred_args:
             self.stops = pred_args['stops']
 
         # TODO: offload creation to the `create` method instead for faster inference?
+
         modal_dispatch = {
             'default': 'default_completion',
             'sql_agent': 'sql_agent_completion',
         }
 
         agent_creation_method = modal_dispatch.get(args.get('modal_dispatch', 'default'), 'default_completion')
-        agent = getattr(self, agent_creation_method)(df, args, pred_args)
+
+        if args.get('mode') == 'conversational':
+            agent_creation_method = 'conversational_completion'
+
+        # input dataframe can be modified
+        agent, df = getattr(self, agent_creation_method)(df, args, pred_args)
         return self.run_agent(df, agent, args, pred_args)
 
+    def conversational_completion(self, df, args=None, pred_args=None):
+        pred_args = pred_args if pred_args else {}
+
+        # api argument validation
+        model_name = args.get('model_name', self.default_model)
+
+        model_kwargs = {
+            'model_name': model_name,
+            'temperature': min(1.0, max(0.0, args.get('temperature', 0.0))),
+            'max_tokens': pred_args.get('max_tokens', args.get('max_tokens', self.default_max_tokens)),
+            'top_p': pred_args.get('top_p', None),
+            'frequency_penalty': pred_args.get('frequency_penalty', None),
+            'presence_penalty': pred_args.get('presence_penalty', None),
+            'n': pred_args.get('n', None),
+            'best_of': pred_args.get('best_of', None),
+            'request_timeout': pred_args.get('request_timeout', None),
+            'logit_bias': pred_args.get('logit_bias', None),
+            'openai_api_key': self._get_openai_api_key(args, strict=True),
+            'serper_api_key': self._get_serper_api_key(args, strict=False),
+        }
+        model_kwargs = {k: v for k, v in model_kwargs.items() if v is not None}  # filter out None values
+
+        # langchain tool setup
+        tools = self._setup_tools(model_kwargs, pred_args, args['executor'])
+
+        llm = ChatOpenAI(**model_kwargs)
+
+        memory = ConversationSummaryBufferMemory(llm=llm,
+                                                 max_token_limit=model_kwargs.get('max_tokens', None),
+                                                 memory_key="chat_history")
+
+        # fill memory
+
+        # system prompt
+        prompt = args['prompt']
+        if 'prompt' in pred_args:
+            prompt = pred_args['prompt']
+        if 'context' in pred_args:
+            prompt += '\n\n' + 'Useful information:\n' + pred_args['context'] + '\n'
+        memory.chat_memory.messages.insert(0, SystemMessage(content=prompt))
+
+        # user - assistant conversation. get all except the last message
+        for row in df[:-1].to_dict('records'):
+            question = row[args['user_column']]
+            answer = row[args['assistant_column']]
+
+            if question:
+                memory.chat_memory.add_user_message(question)
+            if answer:
+                memory.chat_memory.add_ai_message(answer)
+
+        # use last message as prompt, remove other questions
+        df.iloc[:-1, df.columns.get_loc('question')] = ''
+
+        agent_name = AgentType.CONVERSATIONAL_REACT_DESCRIPTION
+        agent = initialize_agent(
+            tools,
+            llm,
+            memory=memory,
+            agent=agent_name,
+            max_iterations=pred_args.get('max_iterations', 3),
+            verbose=pred_args.get('verbose', args.get('verbose', False)),
+            handle_parsing_errors=True,
+        )
+
+        # setup model description
+        description = {
+            'allowed_tools': [agent.agent.allowed_tools],  # packed as list to avoid additional rows
+            'agent_type': agent_name,
+            'max_iterations': agent.max_iterations,
+            'memory_type': memory.__class__.__name__,
+        }
+
+        description = {**description, **model_kwargs}
+        description.pop('openai_api_key', None)
+        self.model_storage.json_set('description', description)
+
+        return agent, df
+
     def default_completion(self, df, args=None, pred_args=None):
         """
         Mostly follows the logic of the OpenAI handler, but with a few additions:
             - setup the langchain toolkit
             - setup the langchain agent (memory included)
             - setup information to be published when describing the model
 
         Ref link from the LangChain documentation on how to accomplish the first two items:
             - python.langchain.com/en/latest/modules/agents/agents/custom_agent.html
         """
         pred_args = pred_args if pred_args else {}
 
         # api argument validation
-        model_name = args.get('model_name', self.default_model)
-        agent_name = args.get('agent_name', self.default_agent_model)
+        model_name = pred_args.get('model_name', args.get('model_name', self.default_model))
+        agent_name = pred_args.get('agent_name', args.get('agent_name', self.default_agent_model))
 
         model_kwargs = {
             'model_name': model_name,
-            'temperature': min(1.0, max(0.0, args.get('temperature', 0.0))),
+            'temperature': min(1.0, max(0.0, pred_args.get('temperature', args.get('temperature', 0.0)))),
             'max_tokens': pred_args.get('max_tokens', args.get('max_tokens', self.default_max_tokens)),
             'top_p': pred_args.get('top_p', None),
             'frequency_penalty': pred_args.get('frequency_penalty', None),
             'presence_penalty': pred_args.get('presence_penalty', None),
             'n': pred_args.get('n', None),
             'best_of': pred_args.get('best_of', None),
             'request_timeout': pred_args.get('request_timeout', None),
             'logit_bias': pred_args.get('logit_bias', None),
             'openai_api_key': self._get_openai_api_key(args, strict=True),
             'serper_api_key': self._get_serper_api_key(args, strict=False),
         }
         model_kwargs = {k: v for k, v in model_kwargs.items() if v is not None}  # filter out None values
 
         # langchain tool setup
+        pred_args['tools'] = args.get('tools') if 'tools' not in pred_args else pred_args.get('tools', [])
         tools = self._setup_tools(model_kwargs, pred_args, args['executor'])
 
         # langchain agent setup
         if model_kwargs['model_name'] in CHAT_MODELS:
             llm = ChatOpenAI(**model_kwargs)
         else:
             llm = OpenAI(**model_kwargs)
-        memory = ConversationSummaryMemory(llm=llm)
+        memory = ConversationSummaryBufferMemory(llm=llm, max_token_limit=model_kwargs.get('max_tokens', None))
         agent = initialize_agent(
             tools,
             llm,
             memory=memory,
             agent=agent_name,
             max_iterations=pred_args.get('max_iterations', 3),
             verbose=pred_args.get('verbose', args.get('verbose', False)),
+            handle_parsing_errors=True,
         )
 
         # setup model description
         description = {
             'allowed_tools': [agent.agent.allowed_tools],   # packed as list to avoid additional rows
             'agent_type': agent_name,
             'max_iterations': agent.max_iterations,
             'memory_type': memory.__class__.__name__,
         }
         description = {**description, **model_kwargs}
         description.pop('openai_api_key', None)
         self.model_storage.json_set('description', description)
 
-        return agent
+        return agent, df
 
-    def run_agent(self, df, agent, pred_args, args):
+    def run_agent(self, df, agent, args, pred_args):
         # TODO abstract prompt templating into a common utility method, this is also used in vanilla OpenAI
-        if pred_args.get('prompt_template', False):
-            base_template = pred_args['prompt_template']  # override with predict-time template if available
+        if args.get('prompt_template', False):
+            base_template = args['prompt_template']  # override with predict-time template if available
+        elif 'prompt_template' in pred_args:
+            base_template = pred_args['prompt_template']
         else:
-            base_template = args['prompt_template']
+            base_template = '{{question}}'
 
         input_variables = []
         matches = list(re.finditer("{{(.*?)}}", base_template))
 
         for m in matches:
             input_variables.append(m[0].replace('{', '').replace('}', ''))
 
@@ -195,27 +294,31 @@
                 prompts.append(prompt.format(**kwargs))
 
         def _completion(agent, prompts):
             # TODO: ensure that agent completion plus prompt match the maximum allowed by the user
             # TODO: use async API if possible for parallelized completion
             completions = []
             for prompt in prompts:
+                if not prompt:
+                    # skip empty values
+                    completions.append('')
+                    continue
                 try:
                     completions.append(agent.run(prompt))
                 except Exception as e:
                     completions.append(f'agent failed with error:\n{str(e)[:50]}...')
             return [c for c in completions]
 
         completion = _completion(agent, prompts)
 
         # add null completion for empty prompts
         for i in sorted(empty_prompt_ids):
             completion.insert(i, None)
 
-        pred_df = pd.DataFrame(completion, columns=[pred_args['target']])
+        pred_df = pd.DataFrame(completion, columns=[args['target']])
 
         return pred_df
 
     def _setup_tools(self, model_kwargs, pred_args, executor):
         def _mdb_exec_call(query: str) -> str:
             """ We define it like this to pass the executor through the closure, as custom classes don't allow custom field assignment. """  # noqa
             try:
@@ -293,28 +396,47 @@
 
         mdb_write_tool = Tool(
             name="MDB-Write",
             func=_mdb_write_call,
             description="useful to write into data sources connected to mindsdb. command must be a valid SQL query with syntax: `INSERT INTO data_source_name.table_name (column_name_1, column_name_2, [...]) VALUES (column_1_value_row_1, column_2_value_row_1, [...]), (column_1_value_row_2, column_2_value_row_2, [...]), [...];`. note the command always ends with a semicolon. order of column names and values for each row must be a perfect match. If write fails, try casting value with a function, passing the value without quotes, or truncating string as needed.`."  # noqa
         )
 
-        toolkit = pred_args.get('tools', self.default_agent_tools)
-        tools = load_tools(toolkit)
+        toolkit = pred_args['tools'] if pred_args['tools'] is not None else self.default_agent_tools
+
+        standard_tools = []
+        custom_tools = []
+        # possible to pass standart tool name or custom function
+        for tool in toolkit:
+            if isinstance(tool, str):
+                standard_tools.append(tool)
+            else:
+                custom_tools.append(tool)
+
+        tools = load_tools(standard_tools)
         if model_kwargs.get('serper_api_key', False):
             search = GoogleSerperAPIWrapper(serper_api_key=model_kwargs.pop('serper_api_key'))
             tools.append(Tool(
                 name="Intermediate Answer (serper.dev)",
                 func=search.run,
-                description="useful for when you need to ask with search"
+                description="useful for when you need to search the internet (note: in general, use this as a last resort)"  # noqa
             ))
 
         # add connection to mindsdb
         tools.append(mdb_tool)
         tools.append(mdb_meta_tool)
-        tools.append(mdb_write_tool)
+
+        if self.write_privileges:
+            tools.append(mdb_write_tool)
+
+        for tool in custom_tools:
+            tools.append(Tool(
+                name=tool['name'],
+                func=tool['func'],
+                description=tool['description'],
+            ))
 
         return tools
 
     def describe(self, attribute: Optional[str] = None) -> pd.DataFrame:
         info = self.model_storage.json_get('description')
 
         if attribute == 'info':
@@ -340,8 +462,8 @@
         model_name = args.get('model_name', self.default_model)
         llm = OpenAI(temperature=0) if model_name not in CHAT_MODELS else ChatOpenAI(temperature=0)
         agent = create_sql_agent(
             llm=llm,
             toolkit=toolkit,
             verbose=True
         )
-        return agent
+        return agent, df
```

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/langchain_handler/mindsdb_database_agent.py` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/langchain_handler/mindsdb_database_agent.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/langchain_handler/setup.py` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/langchain_handler/setup.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/lightwood_handler/lightwood_handler/functions.py` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/lightwood_handler/lightwood_handler/functions.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/lightwood_handler/lightwood_handler/lightwood_handler.py` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/lightwood_handler/lightwood_handler/lightwood_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/lightwood_handler/lightwood_handler/utils.py` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/lightwood_handler/lightwood_handler/utils.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/lightwood_handler/setup.py` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/lightwood_handler/setup.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/lightwood_handler/tests/test_lightwood_handler.py` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/lightwood_handler/tests/test_lightwood_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/ludwig_handler/ludwig_handler.py` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/ludwig_handler/ludwig_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/ludwig_handler/setup.py` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/ludwig_handler/setup.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/mariadb_handler/icon.svg` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/mariadb_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/materialize_handler/icon.png` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/materialize_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/materialize_handler/materialize_handler.py` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/materialize_handler/materialize_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/materialize_handler/tests/test_materialize_handler.py` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/materialize_handler/tests/test_materialize_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/matrixone_handler/__init__.py` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/matrixone_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/matrixone_handler/icon.png` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/matrixone_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/matrixone_handler/matrixone_handler.py` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/matrixone_handler/matrixone_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/matrixone_handler/tests/test_matrixone_handler.py` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/matrixone_handler/tests/test_matrixone_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/maxdb_handler/__init__.py` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/maxdb_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/maxdb_handler/icon.png` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/maxdb_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/maxdb_handler/maxdb_handler.py` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/maxdb_handler/maxdb_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/maxdb_handler/tests/test_maxdb_handler.py` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/maxdb_handler/tests/test_maxdb_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/merlion_handler/adapters.py` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/merlion_handler/adapters.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/merlion_handler/merlion_handler.py` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/merlion_handler/merlion_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/merlion_handler/setup.py` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/merlion_handler/setup.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/mlflow_handler/__init__.py` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/mlflow_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/mlflow_handler/mlflow_handler.py` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/mlflow_handler/mlflow_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/mlflow_handler/setup.py` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/mlflow_handler/setup.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/monetdb_handler/__init__.py` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/monetdb_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/monetdb_handler/create-database.png` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/monetdb_handler/create-database.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/monetdb_handler/create-predictor.png` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/monetdb_handler/create-predictor.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/monetdb_handler/icon.png` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/monetdb_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/monetdb_handler/monetdb_handler.py` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/monetdb_handler/monetdb_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/monetdb_handler/select-predictor.png` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/monetdb_handler/select-predictor.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/monetdb_handler/tests/test_monetdb_handler.py` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/monetdb_handler/tests/test_monetdb_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/monetdb_handler/utils/monet_get_id.py` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/monetdb_handler/utils/monet_get_id.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/mongodb_handler/icon.svg` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/mongodb_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/mongodb_handler/mongodb_handler.py` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/mongodb_handler/mongodb_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/mongodb_handler/utils/mongodb_render.py` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/mongodb_handler/utils/mongodb_render.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/mssql_handler/icon.png` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/mssql_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/mssql_handler/mssql_handler.py` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/mssql_handler/mssql_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/mssql_handler/tests/test_mssql_handler.py` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/mssql_handler/tests/test_mssql_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/mysql_handler/__init__.py` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/mysql_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/mysql_handler/icon.svg` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/mysql_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/mysql_handler/mysql_handler.py` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/mysql_handler/mysql_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/neuralforecast_handler/neuralforecast_handler.py` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/neuralforecast_handler/neuralforecast_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/neuralforecast_handler/setup.py` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/neuralforecast_handler/setup.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/newsapi_handler/__init__.py` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/newsapi_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/newsapi_handler/icon.png` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/newsapi_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/newsapi_handler/newsapi_handler.py` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/newsapi_handler/newsapi_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/newsapi_handler/tests/test_newsapi_handler.py` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/newsapi_handler/tests/test_newsapi_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/nuo_jdbc_handler/__init__.py` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/nuo_jdbc_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/nuo_jdbc_handler/icon.png` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/nuo_jdbc_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/nuo_jdbc_handler/nuo_jdbc_handler.py` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/nuo_jdbc_handler/nuo_jdbc_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/nuo_jdbc_handler/tests/test_nuo_handler.py` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/nuo_jdbc_handler/tests/test_nuo_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/oceanbase_handler/icon.png` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/oceanbase_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/oceanbase_handler/oceanbase_handler.py` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/oceanbase_handler/oceanbase_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/oceanbase_handler/tests/test_oceanbase_handler.py` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/oceanbase_handler/tests/test_oceanbase_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/openai_handler/helpers.py` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/openai_handler/helpers.py`

 * *Files 1% similar despite different names*

```diff
@@ -90,15 +90,15 @@
     Note: first message for chat completion models are general directives with the system role, which will ideally be kept at all times. 
     """  # noqa
     encoder = tiktoken.encoding_for_model(model_name)
     sys_priming = messages[0:1]
     n_tokens = count_tokens(messages, encoder, model_name)
     while n_tokens > max_tokens:
         if len(messages) == 2:
-            return messages[-1]  # edge case: if limit is surpassed by just one input, we remove initial instruction
+            return messages[:-1]  # edge case: if limit is surpassed by just one input, we remove initial instruction
         elif len(messages) == 1:
             return messages
 
         if truncate == 'first':
             messages = sys_priming + messages[2:]
         else:
             messages = sys_priming + messages[1:-1]
```

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/openai_handler/openai_handler.py` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/openai_handler/openai_handler.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,29 +39,31 @@
     @staticmethod
     def create_validation(target, args=None, **kwargs):
         if 'using' not in args:
             raise Exception("OpenAI engine requires a USING clause! Refer to its documentation for more details.")
         else:
             args = args['using']
 
-        if len(set(args.keys()) & {'question_column', 'prompt_template', 'json_struct'}) == 0:
+        if len(set(args.keys()) & {'question_column', 'prompt_template', 'json_struct', 'prompt'}) == 0:
             raise Exception('One of `question_column`, `prompt_template` or `json_struct` is required for this engine.')
 
         keys_collection = [
             ['prompt_template'],
             ['question_column', 'context_column'],
+            ['prompt', 'user_column', 'assistant_column'],
             ['json_struct']
         ]
         for keys in keys_collection:
             if keys[0] in args and any(x[0] in args for x in keys_collection if x != keys):
                 raise Exception(textwrap.dedent('''\
                     Please provide one of
                         1) a `prompt_template`
                         2) a `question_column` and an optional `context_column`
                         3) a `json_struct`
+                        4) a `prompt' and 'user_column' and 'assistant_column`
                 '''))
 
     def create(self, target, args=None, **kwargs):
         args = args['using']
 
         args['target'] = target
         available_models = [m.openai_id for m in openai.Model.list(api_key=self._get_openai_api_key(args)).data]
@@ -213,15 +215,17 @@
                     ''')
                     p = p.replace('{{json_struct}}', json_struct)
                     for column in df.columns:
                         if column == 'json_struct':
                             continue
                         p = p.replace(f'{{{{{column}}}}}', str(df[column][i]))
                     prompts.append(p)
-
+            elif 'prompt' in args:
+                empty_prompt_ids = []
+                prompts = list(df[args['user_column']])
             else:
                 empty_prompt_ids = np.where(df[[args['question_column']]].isna().all(axis=1).values)[0]
                 prompts = list(df[args['question_column']].apply(lambda x: str(x)))
 
         # remove prompts without signal from completion queue
         prompts = [j for i, j in enumerate(prompts) if i not in empty_prompt_ids]
 
@@ -308,20 +312,33 @@
                 tidy_comps = []
                 for c in comp['choices']:
                     if 'message' in c:
                         tidy_comps.append(c['message']['content'].strip('\n').strip(''))
                 return tidy_comps
 
             completions = []
-            initial_prompt = {"role": "system", "content": "You are a helpful assistant. Your task is to continue the chat."}  # noqa
+            if mode != 'conversational':
+                initial_prompt = {"role": "system", "content": "You are a helpful assistant. Your task is to continue the chat."}  # noqa
+            else:
+                # get prompt from model
+                initial_prompt = {"role": "system",  "content": args['prompt']}  # noqa
+
             kwargs['messages'] = [initial_prompt]
             last_completion_content = None
 
             for pidx in range(len(prompts)):
-                kwargs['messages'].append({'role': 'user', 'content': prompts[pidx]})
+                if mode != 'conversational':
+                    kwargs['messages'].append({'role': 'user', 'content': prompts[pidx]})
+                else:
+                    question = prompts[pidx]
+                    if question:
+                        kwargs['messages'].append({'role': 'user', 'content': question})
+                    answer = df.iloc[pidx][args.get('assistant_column')]
+                    if answer:
+                        kwargs['messages'].append({'role': 'assistant', 'content': answer})
 
                 if mode == 'conversational-full' or (mode == 'conversational' and pidx == len(prompts) - 1):
                     kwargs['messages'] = truncate_msgs_for_token_limit(kwargs['messages'],
                                                                        kwargs['model'],
                                                                        api_args['max_tokens'])
                     pkwargs = {**kwargs, **api_args}
                     resp = _tidy(openai.ChatCompletion.create(**pkwargs))
```

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/openai_handler/setup.py` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/openai_handler/setup.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/opengauss_handler/__init__.py` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/opengauss_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/opengauss_handler/opengauss_handler.py` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/opengauss_handler/opengauss_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/opengauss_handler/tests/test_opengauss_handler.py` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/opengauss_handler/tests/test_opengauss_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/oracle_handler/__init__.py` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/oracle_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/oracle_handler/icon.svg` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/oracle_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/oracle_handler/oracle_handler.py` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/oracle_handler/oracle_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/oracle_handler/tests/test_oracle_handler.py` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/oracle_handler/tests/test_oracle_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/orioledb_handler/icon.svg` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/orioledb_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/orioledb_handler/orioledb_handler.py` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/orioledb_handler/orioledb_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/orioledb_handler/tests/test_orioledb_handler.py` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/orioledb_handler/tests/test_orioledb_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/phoenix_handler/__init__.py` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/phoenix_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/phoenix_handler/icon.png` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/phoenix_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/phoenix_handler/phoenix_handler.py` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/phoenix_handler/phoenix_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/phoenix_handler/tests/test_phoenix_handler.py` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/phoenix_handler/tests/test_phoenix_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/pinot_handler/__init__.py` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/pinot_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/pinot_handler/icon.png` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/pinot_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/pinot_handler/pinot_handler.py` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/pinot_handler/pinot_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/pinot_handler/tests/test_pinot_handler.py` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/pinot_handler/tests/test_pinot_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/plaid_handler/icon.svg` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/plaid_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/plaid_handler/plaid_handler.py` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/plaid_handler/plaid_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/plaid_handler/plaid_tables.py` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/plaid_handler/plaid_tables.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/planetscale_handler/__init__.py` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/planetscale_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/planetscale_handler/create-db.png` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/planetscale_handler/create-db.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/planetscale_handler/create-predictor.png` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/planetscale_handler/create-predictor.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/planetscale_handler/drop-db.png` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/planetscale_handler/drop-db.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/planetscale_handler/icon.svg` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/planetscale_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/planetscale_handler/predict-target.png` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/planetscale_handler/predict-target.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/postgres_handler/icon.svg` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/postgres_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/postgres_handler/postgres_handler.py` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/postgres_handler/postgres_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/questdb_handler/icon.svg` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/questdb_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/questdb_handler/questdb_handler.py` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/questdb_handler/questdb_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/questdb_handler/tests/test_questdb_handler.py` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/questdb_handler/tests/test_questdb_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/quickbooks_handler/__init__.py` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/quickbooks_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/quickbooks_handler/icon.svg` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/quickbooks_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/quickbooks_handler/quickbooks_handler.py` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/quickbooks_handler/quickbooks_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/quickbooks_handler/quickbooks_table.py` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/quickbooks_handler/quickbooks_table.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/ray_serve_handler/__init__.py` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/ray_serve_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/ray_serve_handler/ray_serve_handler.py` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/ray_serve_handler/ray_serve_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/ray_serve_handler/setup.py` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/ray_serve_handler/setup.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/reddit_handler/icon.svg` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/reddit_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/reddit_handler/reddit_handler.py` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/reddit_handler/reddit_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/reddit_handler/reddit_tables.py` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/reddit_handler/reddit_tables.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/redshift_handler/__init__.py` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/redshift_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/redshift_handler/icon.png` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/redshift_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/redshift_handler/redshift_handler.py` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/redshift_handler/redshift_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/redshift_handler/tests/test_redshift_handler.py` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/redshift_handler/tests/test_redshift_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/rocket_chat_handler/icon.svg` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/rocket_chat_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/rockset_handler/icon.png` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/rockset_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/rockset_handler/tests/test.png` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/rockset_handler/tests/test.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/rockset_handler/tests/test2.png` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/rockset_handler/tests/test2.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/s3_handler/__init__.py` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/s3_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/s3_handler/icon.png` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/s3_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/s3_handler/s3_handler.py` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/s3_handler/s3_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/s3_handler/tests/test_s3_handler.py` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/s3_handler/tests/test_s3_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/scylla_handler/__init__.py` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/scylla_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/scylla_handler/logo.png` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/scylla_handler/logo.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/scylla_handler/scylla_handler.py` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/scylla_handler/scylla_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/scylla_handler/tests/test_scylla_handler.py` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/scylla_handler/tests/test_scylla_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/sendinblue_handler/__init__.py` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/sendinblue_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/sendinblue_handler/icon.png` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/sendinblue_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/sendinblue_handler/sendinblue_handler.py` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/sendinblue_handler/sendinblue_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/sheets_handler/__init__.py` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/sheets_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/sheets_handler/icon.png` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/sheets_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/sheets_handler/sheets_handler.py` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/sheets_handler/sheets_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/sheets_handler/tests/test_sheets_handler.py` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/sheets_handler/tests/test_sheets_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/shopify_handler/icon.png` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/shopify_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/shopify_handler/shopify_handler.py` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/shopify_handler/shopify_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/shopify_handler/shopify_tables.py` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/shopify_handler/shopify_tables.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import shopify
 import pandas as pd
 from typing import Text, List, Dict
 
 from mindsdb_sql.parser import ast
 from mindsdb.integrations.libs.api_handler import APITable
 
-from .utils import parse_statement, get_results
+from mindsdb.integrations.handlers.utilities.query_utilities import SELECTQueryParser, SELECTQueryExecutor
 
 
 class ProductsTable(APITable):
     """The Shopify Products Table implementation"""
 
     def select(self, query: ast.Select) -> pd.DataFrame:
         """Pulls data from the Shopify "GET /products" API endpoint.
@@ -26,23 +26,30 @@
 
         Raises
         ------
         ValueError
             If the query contains an unsupported condition
         """
 
-        selected_columns, where_conditions, order_by_conditions, result_limit = parse_statement(
+        select_statement_parser = SELECTQueryParser(
             query,
             'products',
             self.get_columns()
         )
+        selected_columns, where_conditions, order_by_conditions, result_limit = select_statement_parser.parse_query()
 
         products_df = pd.json_normalize(self.get_products(limit=result_limit))
 
-        products_df = get_results(products_df, selected_columns, where_conditions, order_by_conditions)
+        select_statement_executor = SELECTQueryExecutor(
+            products_df,
+            selected_columns,
+            where_conditions,
+            order_by_conditions
+        )
+        products_df = select_statement_executor.execute_query()
 
         return products_df
 
     def get_columns(self) -> List[Text]:
         return pd.json_normalize(self.get_products(limit=1)).columns.tolist()
 
     def get_products(self, **kwargs) -> List[Dict]:
@@ -69,23 +76,30 @@
             Shopify Customers matching the query
 
         Raises
         ------
         ValueError
             If the query contains an unsupported condition
         """
-        selected_columns, where_conditions, order_by_conditions, total_results = parse_statement(
+        select_statement_parser = SELECTQueryParser(
             query,
             'customers',
             self.get_columns()
         )
+        selected_columns, where_conditions, order_by_conditions, result_limit = select_statement_parser.parse_query()
 
-        customers_df = pd.json_normalize(self.get_customers(limit=total_results))
+        customers_df = pd.json_normalize(self.get_customers(limit=result_limit))
 
-        customers_df = get_results(customers_df, selected_columns, where_conditions, order_by_conditions)
+        select_statement_executor = SELECTQueryExecutor(
+            customers_df,
+            selected_columns,
+            where_conditions,
+            order_by_conditions
+        )
+        customers_df = select_statement_executor.execute_query()
 
         return customers_df
 
     def get_columns(self) -> List[Text]:
         return pd.json_normalize(self.get_customers(limit=1)).columns.tolist()
 
     def get_customers(self, **kwargs) -> List[Dict]:
@@ -112,23 +126,30 @@
             Shopify Orders matching the query
 
         Raises
         ------
         ValueError
             If the query contains an unsupported condition
         """
-        selected_columns, where_conditions, order_by_conditions, total_results = parse_statement(
+        select_statement_parser = SELECTQueryParser(
             query,
             'orders',
             self.get_columns()
         )
+        selected_columns, where_conditions, order_by_conditions, result_limit = select_statement_parser.parse_query()
 
-        orders_df = pd.json_normalize(self.get_orders(limit=total_results))
+        orders_df = pd.json_normalize(self.get_orders(limit=result_limit))
 
-        orders_df = get_results(orders_df, selected_columns, where_conditions, order_by_conditions)
+        select_statement_executor = SELECTQueryExecutor(
+            orders_df,
+            selected_columns,
+            where_conditions,
+            order_by_conditions
+        )
+        orders_df = select_statement_executor.execute_query()
 
         return orders_df
 
     def get_columns(self) -> List[Text]:
         return pd.json_normalize(self.get_orders(limit=1)).columns.tolist()
 
     def get_orders(self, **kwargs) -> List[Dict]:
```

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/singlestore_handler/tests/test_singlestore_handler.py` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/singlestore_handler/tests/test_singlestore_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/slack_handler/__init__.py` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/slack_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/slack_handler/icon.svg` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/slack_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/slack_handler/slack_handler.py` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/slack_handler/slack_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/slack_handler/tests/test_slack.py` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/slack_handler/tests/test_slack.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/snowflake_handler/snowflake_handler.py` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/snowflake_handler/snowflake_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/snowflake_handler/tests/test_snowflake_handler.py` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/snowflake_handler/tests/test_snowflake_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/solr_handler/__init__.py` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/solr_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/solr_handler/solr.svg` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/solr_handler/solr.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/solr_handler/solr_handler.py` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/solr_handler/solr_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/solr_handler/tests/test_solr_handler.py` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/solr_handler/tests/test_solr_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/sqlany_handler/__init__.py` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/sqlany_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/sqlany_handler/icon.svg` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/sqlany_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/sqlany_handler/sqlany_handler.py` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/sqlany_handler/sqlany_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/sqlite_handler/__init__.py` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/sqlite_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/sqlite_handler/db_connection.png` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/sqlite_handler/db_connection.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/sqlite_handler/error.png` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/sqlite_handler/error.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/sqlite_handler/icon.png` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/sqlite_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/sqlite_handler/model_drop.png` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/sqlite_handler/model_drop.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/sqlite_handler/prediction_result.png` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/sqlite_handler/prediction_result.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/sqlite_handler/predictor_model.png` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/sqlite_handler/predictor_model.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/sqlite_handler/sqlite_handler.py` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/sqlite_handler/sqlite_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/sqlite_handler/tests/test_sqlite_handler.py` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/sqlite_handler/tests/test_sqlite_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/sqreamdb_handler/__init__.py` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/sqreamdb_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/sqreamdb_handler/icon.png` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/sqreamdb_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/sqreamdb_handler/sqreamdb_handler.py` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/sqreamdb_handler/sqreamdb_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/sqreamdb_handler/tests/test_sqreamdb_handler.py` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/sqreamdb_handler/tests/test_sqreamdb_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/starrocks_handler/icon.png` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/starrocks_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/starrocks_handler/starrocks_handler.py` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/starrocks_handler/starrocks_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/starrocks_handler/tests/test_starrocks_handler.py` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/starrocks_handler/tests/test_starrocks_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/statsforecast_handler/setup.py` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/statsforecast_handler/setup.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/statsforecast_handler/statsforecast_handler.py` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/statsforecast_handler/statsforecast_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/strava_handler/__init__.py` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/strava_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/strava_handler/icon.png` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/strava_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/strava_handler/strava_handler.py` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/strava_handler/strava_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/strava_handler/strava_tables.py` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/strava_handler/strava_tables.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/supabase_handler/icon.svg` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/supabase_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/supabase_handler/tests/test_supabase_handler.py` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/supabase_handler/tests/test_supabase_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/surrealdb_handler/__init__.py` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/surrealdb_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/surrealdb_handler/icon.png` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/surrealdb_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/surrealdb_handler/surrealdb_handler.py` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/surrealdb_handler/surrealdb_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/surrealdb_handler/tests/test_surrealdb_handler.py` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/surrealdb_handler/tests/test_surrealdb_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/surrealdb_handler/utils/surreal_get_info.py` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/surrealdb_handler/utils/surreal_get_info.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/tdengine_handler/__init__.py` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/tdengine_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/tdengine_handler/icon.svg` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/tdengine_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/tdengine_handler/tdengine_handler.py` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/tdengine_handler/tdengine_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/tdengine_handler/tests/test_tdengine_handler.py` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/tdengine_handler/tests/test_tdengine_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/teradata_handler/__init__.py` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/teradata_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/teradata_handler/icon.svg` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/teradata_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/teradata_handler/teradata_handler.py` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/teradata_handler/teradata_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/tidb_handler/__init__.py` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/tidb_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/tidb_handler/tests/test_tidb_handler.py` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/tidb_handler/tests/test_tidb_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/tidb_handler/tidb_handler.py` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/tidb_handler/tidb_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/timescaledb_handler/icon.svg` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/timescaledb_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/timescaledb_handler/tests/test_timescaledb_handler.py` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/timescaledb_handler/tests/test_timescaledb_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/timescaledb_handler/timescaledb_handler.py` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/timescaledb_handler/timescaledb_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/tpot_handler/setup.py` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/tpot_handler/setup.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/tpot_handler/tpot_handler.py` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/flaml_handler/flaml_handler.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,52 +1,47 @@
-from typing import Optional
 import dill
 import pandas as pd
 from mindsdb.integrations.libs.base import BaseMLEngine
 from typing import Dict, Optional
 from type_infer.infer import infer_types
-from tpot import TPOTClassifier, TPOTRegressor
+from flaml import AutoML
 
 
-class TPOTHandler(BaseMLEngine):
-    name = "TPOT"
+class FLAMLHandler(BaseMLEngine):
+    name = "FLAML"
+
     def create(self, target: str, df: Optional[pd.DataFrame] = None, args: Optional[Dict] = None) -> None:
         if args is None:
             args = {}
-        
-        target_dtype=infer_types(df,0).to_dict()["dtypes"][target]
-
-
-        if target_dtype in ['binary','categorical','tags']:
-            model = TPOTClassifier(generations=args.get('generations', 10),
-                                       population_size=args.get('population_size', 100),
-                                       verbosity=0,
-                                       max_time_mins=args.get('max_time_mins', None),
-                                       n_jobs=args.get('n_jobs', -1))
             
-
-        elif target_dtype in ['integer','float','quantity'] :
-            model = TPOTRegressor(generations=args.get('generations', 10),
-                                      population_size=args.get('population_size', 100),
-                                      verbosity=0,
-                                      max_time_mins=args.get('max_time_mins', None),
-                                      n_jobs=args.get('n_jobs', -1))
-        
-
         if df is not None:
-            model.fit(df.drop(columns=[target]), df[target])
+            target_dtype = infer_types(df, 0).to_dict()["dtypes"][target]
+            model = AutoML(verbose=0)
+
+            if target_dtype in ['binary', 'categorical', 'tags']:
+                model.fit(X_train=df.drop(columns=[target]),
+                      y_train=df[target],
+                      task='classification',
+                      **args.get('using'))
+
+            elif target_dtype in ['integer', 'float', 'quantity']:
+                model.fit(X_train=df.drop(columns=[target]),
+                      y_train=df[target],
+                      task='regression',
+                      **args.get('using'))
+                
             self.model_storage.json_set('args', args)
-            self.model_storage.file_set('model', dill.dumps(model.fitted_pipeline_))
-        else :
+            self.model_storage.file_set('model', dill.dumps(model))
+            
+        else:
             raise Exception(
                 "Data is empty!!"
             )
-        
 
     def predict(self, df: pd.DataFrame, args: Optional[Dict] = None) -> pd.DataFrame:
 
-        model=dill.loads(self.model_storage.file_get("model"))
-        target=self.model_storage.json_get('args').get("target")
-        
-        results=pd.DataFrame(model.predict(df),columns=[target])
-        
+        model = dill.loads(self.model_storage.file_get("model"))
+        target = self.model_storage.json_get('args').get("target")
+
+        results = pd.DataFrame(model.predict(df), columns=[target])
+
         return results
```

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/trino_handler/icon.png` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/trino_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/trino_handler/tests/test_trino_handler.py` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/trino_handler/tests/test_trino_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/trino_handler/trino_handler.py` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/trino_handler/trino_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/twitter_handler/icon.svg` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/twitter_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/twitter_handler/twitter_handler.py` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/twitter_handler/twitter_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/vertica_handler/__init__.py` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/vertica_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/vertica_handler/icon.svg` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/vertica_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/vertica_handler/tests/test_vertica_handler.py` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/vertica_handler/tests/test_vertica_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/vertica_handler/vertica_handler.py` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/vertica_handler/vertica_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/vitess_handler/icon.svg` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/vitess_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/vitess_handler/tests/test_vitess_handler.py` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/vitess_handler/tests/test_vitess_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/vitess_handler/vitess_handler.py` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/vitess_handler/vitess_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/youtube_handler/__init__.py` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/youtube_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/youtube_handler/icon.png` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/youtube_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/youtube_handler/youtube_handler.py` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/youtube_handler/youtube_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/youtube_handler/youtube_tables.py` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/youtube_handler/youtube_tables.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/yugabyte_handler/icon.svg` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/yugabyte_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers/yugabyte_handler/tests/test_yugabyte_handler.py` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers/yugabyte_handler/tests/test_yugabyte_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers_client/db_grpc_client.py` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers_client/db_grpc_client.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers_client/ml_client_factory.py` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers_client/ml_client_factory.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,33 +1,42 @@
 import os
-from mindsdb.integrations.handlers_client.ml_grpc_client import MLClientGRPC
 from mindsdb.integrations.libs.handler_helpers import discover_services
 from mindsdb.utilities.log import get_log
 
 
 logger = get_log(logger_name="main")
 
 
 class MLClientFactory:
     def __init__(self, handler_class, engine):
         self.engine = engine
-        self.client_class = MLClientGRPC
+        self.client_class = None
+        # self.client_class = MLClientGRPC
         self.handler_class = handler_class
         self.__name__ = self.handler_class.__name__
         self.__module__ = self.handler_class.__module__
 
     def __call__(self, engine_storage, model_storage, **kwargs):
         service_info = self.discover_service(self.engine)
         if service_info:
             host = service_info["host"]
             port = service_info["port"]
         else:
             host = os.environ.get("MINDSDB_ML_SERVICE_HOST", None)
             port = os.environ.get("MINDSDB_ML_SERVICE_PORT", None)
 
+        if host is not None and port is not None:
+            try:
+                from mindsdb.integrations.handlers_client.ml_grpc_client import MLClientGRPC
+                self.client_class = MLClientGRPC
+            except (ImportError, ModuleNotFoundError):
+                logger.error("to use microservice mode please install 'pip install mindsdb[grpc]'")
+                host = None
+                port = None
+
         if host is None or port is None:
             logger.info(
                 "%s.__call__: no post/port to MLService have provided. Handle all ML request locally",
                 self.__class__.__name__,
             )
             return self.handler_class(engine_storage=engine_storage, model_storage=model_storage, **kwargs)
```

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers_client/ml_grpc_client.py` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers_client/ml_grpc_client.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers_wrapper/db_grpc_wrapper.py` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers_wrapper/db_grpc_wrapper.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers_wrapper/db_handler_service.py` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers_wrapper/db_handler_service.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers_wrapper/ml_grpc_wrapper.py` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers_wrapper/ml_grpc_wrapper.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/handlers_wrapper/ml_handler_service.py` & `MindsDB-23.6.1.1/mindsdb/integrations/handlers_wrapper/ml_handler_service.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/libs/api_handler.py` & `MindsDB-23.6.1.1/mindsdb/integrations/libs/api_handler.py`

 * *Files 3% similar despite different names*

```diff
@@ -223,7 +223,26 @@
         """
         result = list(self._tables.keys())
 
         df = pd.DataFrame(result, columns=['table_name'])
         df['table_type'] = 'BASE TABLE'
 
         return Response(RESPONSE_TYPE.TABLE, df)
+
+
+class APIChatHandler(APIHandler):
+
+    def get_chat_config(self):
+        """Return configuration to connect to chatbot
+
+        Returns:
+            Dict
+        """
+        raise NotImplementedError()
+
+    def get_my_user_name(self) -> list:
+        """Return configuration to connect to chatbot
+
+        Returns:
+            Dict
+        """
+        raise NotImplementedError()
```

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/libs/base.py` & `MindsDB-23.6.1.1/mindsdb/integrations/libs/base.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/libs/handler_helpers.py` & `MindsDB-23.6.1.1/mindsdb/integrations/libs/handler_helpers.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/libs/ml_exec_base.py` & `MindsDB-23.6.1.1/mindsdb/integrations/libs/ml_exec_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -344,18 +344,25 @@
 
     def predict(self, model_name: str, data: list, pred_format: str = 'dict',
                 project_name: str = None, version=None, params: dict = None):
         """ Generates predictions with some model and input data. """
         if isinstance(data, dict):
             data = [data]
         df = pd.DataFrame(data)
-        predictor_record = get_model_record(
-            name=model_name, ml_handler_name=self.name, project_name=project_name,
-            version=version
-        )
+        kwargs = {
+            'name': model_name,
+            'ml_handler_name': self.name,
+            'project_name': project_name
+        }
+        if version is None:
+            kwargs['active'] = True
+        else:
+            kwargs['active'] = None
+            kwargs['version'] = version
+        predictor_record = get_model_record(**kwargs)
         if predictor_record is None:
             if version is not None:
                 model_name = f'{model_name}.{version}'
             raise Exception(f"Error: model '{model_name}' does not exists!")
         if predictor_record.status != PREDICTOR_STATUS.COMPLETE:
             raise Exception("Error: model creation not completed")
 
@@ -406,34 +413,37 @@
             columns_in_count=df.shape[1],
             rows_out_count=len(predictions)
         )
         return predictions
 
     def update(
             self, model_name, project_name, version,
+            base_model_version: int,
             data_integration_ref=None,
             fetch_data_query=None,
             join_learn_process=False,
             label=None,
             set_active=True,
             args: Optional[dict] = None
     ):
         # generate new record from latest version as starting point
         project = self.database_controller.get_project(name=project_name)
-        predictor_records = get_model_records(
-            active=None,
-            name=model_name,
-        )
-        predictor_records = [
-            x for x in predictor_records
-            if x.training_stop_at is not None and x.status == 'complete'
-        ]
-        predictor_records.sort(key=lambda x: x.training_stop_at, reverse=True)
 
+        search_args = {
+            'active': None,
+            'name': model_name,
+            'status': PREDICTOR_STATUS.COMPLETE
+        }
+        if base_model_version is not None:
+            search_args['version'] = base_model_version
+        predictor_records = get_model_records(**search_args)
+        predictor_records.sort(key=lambda x: x.training_stop_at, reverse=True)
+        predictor_records = [x for x in predictor_records if x.training_stop_at is not None]
         base_predictor_record = predictor_records[0]
+
         learn_args = base_predictor_record.learn_args
         learn_args['using'] = args if not learn_args.get('using', False) else {**learn_args['using'], **args}
 
         predictor_record = db.Predictor(
             company_id=ctx.company_id,
             name=model_name,
             integration_id=self.integration_id,
```

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/libs/ml_handler_proc.py` & `MindsDB-23.6.1.1/mindsdb/integrations/libs/ml_handler_proc.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/libs/net_helpers.py` & `MindsDB-23.6.1.1/mindsdb/integrations/libs/net_helpers.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/libs/response.py` & `MindsDB-23.6.1.1/mindsdb/integrations/libs/response.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/libs/storage_handler.py` & `MindsDB-23.6.1.1/mindsdb/integrations/libs/storage_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/utilities/date_utils.py` & `MindsDB-23.6.1.1/mindsdb/integrations/utilities/date_utils.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/utilities/install.py` & `MindsDB-23.6.1.1/mindsdb/integrations/utilities/install.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/utilities/sql_utils.py` & `MindsDB-23.6.1.1/mindsdb/integrations/utilities/sql_utils.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,20 +1,33 @@
+import pandas as pd
+
 from mindsdb_sql.parser import ast
 from mindsdb_sql.parser.ast.base import ASTNode
 from mindsdb_sql.planner.utils import query_traversal
 
 
 def make_sql_session():
     from mindsdb.api.mysql.mysql_proxy.controllers.session_controller import SessionController
 
     sql_session = SessionController()
     sql_session.database = 'mindsdb'
     return sql_session
 
 
+def conditions_to_filter(binary_op: ASTNode):
+    conditions = extract_comparison_conditions(binary_op)
+
+    filters = {}
+    for op, arg1, arg2 in conditions:
+        if op != '=':
+            raise NotImplementedError
+        filters[arg1] = arg2
+    return filters
+
+
 def extract_comparison_conditions(binary_op: ASTNode):
     '''Extracts all simple comparison conditions that must be true from an AST node.
     Does NOT support 'or' conditions.
     '''
     conditions = []
 
     def _extract_comparison_conditions(node: ASTNode, **kwargs):
@@ -34,7 +47,30 @@
             else:
                 raise NotImplementedError(f'Not implemented arg2: {node.args[1]}')
 
             conditions.append([op, node.args[0].parts[-1], value])
 
     query_traversal(binary_op, _extract_comparison_conditions)
     return conditions
+
+
+def project_dataframe(df, targets, table_columns):
+    columns = []
+    for target in targets:
+        if isinstance(target, ast.Star):
+            columns = table_columns
+            break
+        elif isinstance(target, ast.Identifier):
+            columns.append(target.parts[-1])
+        else:
+            raise NotImplementedError
+
+    if len(df) == 0:
+        df = pd.DataFrame([], columns=columns)
+    else:
+        # add absent columns
+        for col in set(columns) & set(df.columns) ^ set(columns):
+            df[col] = None
+
+        # filter by columns
+        df = df[columns]
+    return df
```

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/utilities/test_utils.py` & `MindsDB-23.6.1.1/mindsdb/integrations/utilities/test_utils.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/integrations/utilities/time_series_utils.py` & `MindsDB-23.6.1.1/mindsdb/integrations/utilities/time_series_utils.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/interfaces/database/database.py` & `MindsDB-23.6.1.1/mindsdb/interfaces/database/database.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/interfaces/database/integrations.py` & `MindsDB-23.6.1.1/mindsdb/interfaces/database/integrations.py`

 * *Files 5% similar despite different names*

```diff
@@ -54,14 +54,15 @@
         if (
             isinstance(self.cleaner_thread, threading.Thread)
             and self.cleaner_thread.is_alive()
         ):
             return
         self._stop_event.clear()
         self.cleaner_thread = threading.Thread(target=self._clean)
+        self.cleaner_thread.daemon = True
         self.cleaner_thread.start()
 
     def _stop_clean(self) -> None:
         """ stop clean worker
         """
         self._stop_event.set()
 
@@ -158,16 +159,14 @@
             company_id=ctx.company_id
         )
         db.session.add(integration_record)
         db.session.commit()
         return integration_record.id
 
     def add(self, name, engine, connection_args):
-        if engine in ['redis', 'kafka']:
-            return self._add_integration_record(name, engine, connection_args)
 
         logger.debug(
             "%s: add method calling name=%s, engine=%s, connection_args=%s, company_id=%s",
             self.__class__.__name__, name, engine, connection_args, ctx.company_id
         )
         handlers_meta = self.get_handlers_import_status()
         handler_meta = handlers_meta[engine]
@@ -361,14 +360,17 @@
             Args:
                 handler_type (str)
                 connection_data (dict)
 
             Returns:
                 Handler object
         """
+        handler_meta = self.handlers_import_status[handler_type]
+        if not handler_meta["import"]["success"]:
+            logger.info(f"to use {handler_type} please install 'pip install mindsdb[{handler_type}]'")
 
         logger.debug("%s.create_tmp_handler: connection args - %s", self.__class__.__name__, connection_data)
         resource_id = int(time() * 10000)
         fs_store = FileStorage(
             resource_group=RESOURCE_GROUP.INTEGRATION,
             resource_id=resource_id,
             root_dir='tmp',
@@ -379,18 +381,15 @@
         handler_ars = dict(
             name='tmp_handler',
             fs_store=fs_store,
             connection_data=connection_data
         )
 
         logger.debug("%s.create_tmp_handler: create a client to db of %s type", self.__class__.__name__, handler_type)
-        if DBClient.is_local:
-            return self.handler_modules[handler_type].Handler(**handler_ars)
-        else:
-            return DBClient(handler_type, **handler_ars)
+        return DBClient(handler_type, self.handler_modules[handler_type].Handler, **handler_ars)
 
     def get_handler(self, name, case_sensitive=False):
         handler = self.handlers_cache.get(name)
         if handler is not None:
             return handler
 
         if case_sensitive:
@@ -409,14 +408,19 @@
         integration_name = integration_data['name']
         logger.debug("%s.get_handler: connection_data=%s, engine=%s", self.__class__.__name__, connection_data, integration_engine)
 
         if integration_engine not in self.handler_modules:
             raise Exception(f"Can't find handler for '{integration_name}' ({integration_engine})")
 
         integration_meta = self.handlers_import_status[integration_engine]
+        if not integration_meta["import"]["success"]:
+            msg = f"to use {integration_engine} please install 'pip install mindsdb[{integration_engine}]'"
+            logger.debug(msg)
+            raise Exception(msg)
+
         connection_args = integration_meta.get('connection_args')
         logger.debug("%s.get_handler: connection args - %s", self.__class__.__name__, connection_args)
 
         fs_store = FileStorage(
             resource_group=RESOURCE_GROUP.INTEGRATION,
             resource_id=integration_record.id,
             sync=True,
@@ -454,19 +458,15 @@
             handler_ars['integration_engine'] = integration_engine
             logger.info("%s.get_handler: create a ML client, params - %s", self.__class__.__name__, handler_ars)
             handler = BaseMLEngineExec(**handler_ars)
             # handler = MLClient(**handler_ars)
         else:
 
             logger.info("%s.get_handler: create a client to db service of %s type, args - %s", self.__class__.__name__, integration_engine, handler_ars)
-            if DBClient.is_local:
-                handler = HandlerClass(**handler_ars)
-                self.handlers_cache.set(handler)
-            else:
-                handler = DBClient(integration_engine, **handler_ars)
+            handler = DBClient(integration_engine, HandlerClass, **handler_ars)
 
         return handler
 
     def reload_handler_module(self, handler_name):
         importlib.reload(self.handler_modules[handler_name])
         try:
             handler_meta = self._get_handler_meta(self.handler_modules[handler_name])
@@ -493,17 +493,15 @@
 
     def _get_handler_meta(self, module):
         handler_dir = Path(module.__path__[0])
         handler_folder_name = handler_dir.name
         dependencies = self._read_dependencies(handler_dir)
 
         self.handler_modules[module.name] = module
-        import_error = None
-        if hasattr(module, 'import_error'):
-            import_error = module.import_error
+        import_error = getattr(module, 'import_error', None)
         handler_meta = {
             'import': {
                 'success': import_error is None,
                 'folder': handler_folder_name,
                 'dependencies': dependencies
             },
             'version': module.version
```

### Comparing `MindsDB-23.5.4.1/mindsdb/interfaces/database/projects.py` & `MindsDB-23.6.1.1/mindsdb/interfaces/database/projects.py`

 * *Files 3% similar despite different names*

```diff
@@ -238,16 +238,22 @@
         # at the moment it works only for models
         predictor_record = db.Predictor.query.filter_by(
             company_id=ctx.company_id,
             project_id=self.id,
             name=table_name
         ).first()
         columns = []
-        if predictor_record is not None and isinstance(predictor_record.dtype_dict, dict):
-            columns = list(predictor_record.dtype_dict.keys())
+        if predictor_record is not None:
+            if isinstance(predictor_record.dtype_dict, dict):
+                columns = list(predictor_record.dtype_dict.keys())
+            elif predictor_record.to_predict is not None:
+                # no dtype_dict, use target
+                columns = predictor_record.to_predict
+                if not isinstance(columns, list):
+                    columns = [columns]
 
         return columns
 
 
 class ProjectController:
     def __init__(self):
         pass
```

### Comparing `MindsDB-23.5.4.1/mindsdb/interfaces/database/views.py` & `MindsDB-23.6.1.1/mindsdb/interfaces/database/views.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/interfaces/file/file_controller.py` & `MindsDB-23.6.1.1/mindsdb/interfaces/file/file_controller.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/interfaces/jobs/jobs_controller.py` & `MindsDB-23.6.1.1/mindsdb/interfaces/jobs/jobs_controller.py`

 * *Files 2% similar despite different names*

```diff
@@ -344,15 +344,16 @@
                                 db.JobsHistory.id != history_id)\
                         .order_by(db.JobsHistory.id.desc())\
                         .first()
                     if history_prev is None:
                         # start date of the job
                         value = record.created_at
                     else:
-                        value = history_prev.start_at
+                        # fix for twitter: created_at filter must be minimum of 10 seconds prior to the current time
+                        value = history_prev.start_at - dt.timedelta(seconds=60)
                     value = value.strftime("%Y-%m-%d %H:%M:%S")
                     sql = sql.replace('{{PREVIOUS_START_DATETIME}}', value)
 
                 if '{{START_DATE}}' in sql:
                     value = history_record.start_at.strftime("%Y-%m-%d")
                     sql = sql.replace('{{START_DATE}}', value)
                 if '{{START_DATETIME}}' in sql:
```

### Comparing `MindsDB-23.5.4.1/mindsdb/interfaces/jobs/scheduler.py` & `MindsDB-23.6.1.1/mindsdb/interfaces/jobs/scheduler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/interfaces/model/functions.py` & `MindsDB-23.6.1.1/mindsdb/interfaces/model/functions.py`

 * *Files 4% similar despite different names*

```diff
@@ -110,19 +110,17 @@
                      deleted_at=null(), version: Optional[int] = None, **kwargs):
     kwargs['company_id'] = ctx.company_id
     if kwargs['company_id'] is None:
         kwargs['company_id'] = null()
 
     kwargs['deleted_at'] = deleted_at
     if active is not None:
-        # not use active if version was chosen
-        if version is not None:
-            kwargs['version'] = version
-        else:
-            kwargs['active'] = active
+        kwargs['active'] = active
+    if version is not None:
+        kwargs['version'] = version
 
     if project_name is not None:
         project_record = get_project_record(name=project_name)
         if project_record is None:
             return []
         kwargs['project_id'] = project_record.id
```

### Comparing `MindsDB-23.5.4.1/mindsdb/interfaces/model/model_controller.py` & `MindsDB-23.6.1.1/mindsdb/interfaces/model/model_controller.py`

 * *Files 2% similar despite different names*

```diff
@@ -127,15 +127,15 @@
 
             model_info.insert(0, 'tables', [attributes])
             return model_info
         else:
             return df
 
     def get_model(self, name, version=None, ml_handler_name=None, project_name=None):
-        show_active = True if version is None else False
+        show_active = True if version is None else None
         model_record = get_model_record(
             active=show_active,
             version=version,
             name=name,
             ml_handler_name=ml_handler_name,
             project_name=project_name)
         return self.get_reduced_model_data(predictor_record=model_record)
@@ -373,15 +373,15 @@
             active=True
         )
 
         model_name = params['model_name']
         if base_predictor_record is None:
             raise Exception(f"Error: model '{model_name}' does not exist")
 
-        params['version'] = self._get_retrain_finetune_version(model_name, params['project_name'], base_predictor_record)
+        params['version'] = self._get_retrain_finetune_version(params['project_name'], base_predictor_record)
 
         if params['data_integration_ref'] is None:
             params['data_integration_ref'] = base_predictor_record.data_integration_ref
         if params['fetch_data_query'] is None:
             params['fetch_data_query'] = base_predictor_record.fetch_data_query
 
         problem_definition = base_predictor_record.learn_args.copy()
@@ -391,83 +391,77 @@
         params['is_retrain'] = True
         params['set_active'] = set_active
         predictor_record = ml_handler.learn(**params)
 
         return self.get_model_info(predictor_record)
 
     @staticmethod
-    def _get_retrain_finetune_version(model_name, project_name, base_predictor_record):
+    def _get_retrain_finetune_version(project_name, base_predictor_record):
         if base_predictor_record is None:
-            raise Exception(f"Error: model '{model_name}' does not exist")
+            raise Exception(f"Error: model '{base_predictor_record.name}' does not exist")
 
-        # get max current version
         models = get_model_records(
-            name=model_name,
+            name=base_predictor_record.name,
             project_name=project_name,
-            deleted_at=None,
-            active=None,
+            active=None
         )
-        last_version = 1
-        for m in models:
-            if m.version is not None:
-                last_version = max(last_version, m.version)
+        last_version = max([x.version or 1 for x in models])
 
         return last_version + 1
 
     def prepare_finetune_statement(self, statement, database_controller):
         project_name, model_name, model_version, _describe = resolve_model_identifier(statement.name)
         data_integration_ref, fetch_data_query = self._get_data_integration_ref(statement, database_controller)
 
+        set_active = True
+        if statement.using is not None:
+            set_active = statement.using.pop('active', True)
+            if set_active in ('0', 0, None):
+                set_active = False
+
         label = None
         args = {}
         if statement.using is not None:
             label = statement.using.pop('tag', None)
             args = statement.using
 
         join_learn_process = args.pop('join_learn_process', False)
 
         base_predictor_record = get_model_record(
             name=model_name,
             project_name=project_name,
-            version=model_version
+            version=model_version,
+            active=None
         )
-        version = self._get_retrain_finetune_version(model_name, project_name, base_predictor_record)
+        version = self._get_retrain_finetune_version(project_name, base_predictor_record)
 
         if data_integration_ref is None:
             data_integration_ref = base_predictor_record.data_integration_ref
         if fetch_data_query is None:
             fetch_data_query = base_predictor_record.fetch_data_query
 
         return dict(
             model_name=model_name,
             project_name=project_name,
             data_integration_ref=data_integration_ref,
             fetch_data_query=fetch_data_query,
+            base_model_version=model_version,
             version=version,
             args=args,
             join_learn_process=join_learn_process,
-            label=label
+            label=label,
+            set_active=set_active
         )
 
     def finetune_model(self, statement, ml_handler):
-        # active setting
-        set_active = True
-        if statement.using is not None:
-            set_active = statement.using.pop('active', True)
-            if set_active in ('0', 0, None):
-                set_active = False
-
         params = self.prepare_finetune_statement(statement, ml_handler.database_controller)
-
-        params['set_active'] = set_active
         predictor_record = ml_handler.update(**params)
         return self.get_model_info(predictor_record)
 
     def get_model_info(self, predictor_record):
-
         from mindsdb.interfaces.database.projects import ProjectController
         projects_controller = ProjectController()
         project = projects_controller.get(id=predictor_record.project_id)
 
         columns = ['NAME', 'ENGINE', 'PROJECT', 'ACTIVE', 'VERSION', 'STATUS', 'ACCURACY', 'PREDICT', 'UPDATE_STATUS',
                    'MINDSDB_VERSION', 'ERROR', 'SELECT_DATA_QUERY', 'TRAINING_OPTIONS', 'TAG']
 
@@ -501,15 +495,16 @@
 
         # update
         model = models[0]
 
         model_record = get_model_record(
             name=model['NAME'],
             project_name=model['PROJECT'],
-            version=model['VERSION']
+            version=model['VERSION'],
+            active=None
         )
 
         model_record.active = True
 
         # deactivate current active version
         model_records = db.Predictor.query.filter(
             db.Predictor.name == model_record.name,
@@ -527,15 +522,16 @@
         if len(models) == 0:
             raise Exception(f"Version to delete is not found")
 
         for model in models:
             model_record = get_model_record(
                 name=model['NAME'],
                 project_name=model['PROJECT'],
-                version=model['VERSION']
+                version=model['VERSION'],
+                active=None
             )
             if model_record.active:
                 raise Exception(f"Can't remove active version: f{model['PROJECT']}.{model['NAME']}.{model['VERSION']}")
 
             is_cloud = self.config.get('cloud', False)
             if is_cloud:
                 model_record.deleted_at = dt.datetime.now()
```

### Comparing `MindsDB-23.5.4.1/mindsdb/interfaces/storage/db.py` & `MindsDB-23.6.1.1/mindsdb/interfaces/storage/db.py`

 * *Files 2% similar despite different names*

```diff
@@ -170,32 +170,14 @@
     data = Column(Json)
     company_id = Column(Integer)
     __table_args__ = (
         UniqueConstraint('name', 'company_id', name='unique_integration_name_company_id'),
     )
 
 
-class Stream(Base):
-    __tablename__ = 'stream'
-    id = Column(Integer, primary_key=True)
-    name = Column(String, nullable=False)
-    stream_in = Column(String, nullable=False)
-    stream_out = Column(String, nullable=False)
-    anomaly_stream = Column(String)
-    integration = Column(String)
-    predictor = Column(String, nullable=False)
-    company_id = Column(Integer)
-    updated_at = Column(DateTime, default=datetime.datetime.now, onupdate=datetime.datetime.now)
-    created_at = Column(DateTime, default=datetime.datetime.now)
-    type = Column(String, default='unknown')
-    connection_info = Column(Json, default={})
-    learning_params = Column(Json, default={})
-    learning_threshold = Column(Integer, default=0)
-
-
 class File(Base):
     __tablename__ = 'file'
     id = Column(Integer, primary_key=True)
     name = Column(String, nullable=False)
     company_id = Column(Integer)
     source_file_path = Column(String, nullable=False)
     file_path = Column(String, nullable=False)
@@ -263,7 +245,24 @@
     error = Column(String)
     created_at = Column(DateTime, default=datetime.datetime.now)
     updated_at = Column(DateTime, default=datetime.datetime.now)
 
     __table_args__ = (
         UniqueConstraint('job_id', 'start_at', name='uniq_job_history_job_id_start'),
     )
+
+
+class ChatBots(Base):
+    __tablename__ = 'chat_bots'
+    id = Column(Integer, primary_key=True)
+    company_id = Column(Integer)
+    user_class = Column(Integer, nullable=True)
+
+    name = Column(String, nullable=False)
+    project_id = Column(Integer, nullable=False)
+
+    model_name = Column(String, nullable=False)
+    database_id = Column(Integer, nullable=False)
+    params = Column(JSON)
+
+    updated_at = Column(DateTime, default=datetime.datetime.now, onupdate=datetime.datetime.now)
+    created_at = Column(DateTime, default=datetime.datetime.now)
```

### Comparing `MindsDB-23.5.4.1/mindsdb/interfaces/storage/fs.py` & `MindsDB-23.6.1.1/mindsdb/interfaces/storage/fs.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/interfaces/storage/json.py` & `MindsDB-23.6.1.1/mindsdb/interfaces/storage/json.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/interfaces/storage/model_fs.py` & `MindsDB-23.6.1.1/mindsdb/interfaces/storage/model_fs.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/interfaces/stream/base/integration.py` & `MindsDB-23.6.1.1/mindsdb/interfaces/stream/base/integration.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/microservices_grpc/db/common_pb2.py` & `MindsDB-23.6.1.1/mindsdb/microservices_grpc/db/common_pb2.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/microservices_grpc/db/db_pb2.py` & `MindsDB-23.6.1.1/mindsdb/microservices_grpc/db/db_pb2.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/microservices_grpc/db/db_pb2_grpc.py` & `MindsDB-23.6.1.1/mindsdb/microservices_grpc/db/db_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/microservices_grpc/executor/executor_pb2.py` & `MindsDB-23.6.1.1/mindsdb/microservices_grpc/executor/executor_pb2.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/microservices_grpc/executor/executor_pb2_grpc.py` & `MindsDB-23.6.1.1/mindsdb/microservices_grpc/executor/executor_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/microservices_grpc/ml/common_pb2.py` & `MindsDB-23.6.1.1/mindsdb/microservices_grpc/ml/common_pb2.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/microservices_grpc/ml/ml_pb2.py` & `MindsDB-23.6.1.1/mindsdb/microservices_grpc/ml/ml_pb2.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/microservices_grpc/ml/ml_pb2_grpc.py` & `MindsDB-23.6.1.1/mindsdb/microservices_grpc/ml/ml_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/migrations/alembic.ini` & `MindsDB-23.6.1.1/mindsdb/migrations/alembic.ini`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/migrations/env.py` & `MindsDB-23.6.1.1/mindsdb/migrations/env.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/migrations/migrate.py` & `MindsDB-23.6.1.1/mindsdb/migrations/migrate.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/migrations/versions/2021-11-30_17c3d2384711_init.py` & `MindsDB-23.6.1.1/mindsdb/migrations/versions/2021-11-30_17c3d2384711_init.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/migrations/versions/2022-01-26_47f97b83cee4_views.py` & `MindsDB-23.6.1.1/mindsdb/migrations/versions/2022-01-26_47f97b83cee4_views.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/migrations/versions/2022-02-09_27c5aca9e47e_db_files.py` & `MindsDB-23.6.1.1/mindsdb/migrations/versions/2022-02-09_27c5aca9e47e_db_files.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/migrations/versions/2022-05-25_d74c189b87e6_predictor_integration.py` & `MindsDB-23.6.1.1/mindsdb/migrations/versions/2022-05-25_d74c189b87e6_predictor_integration.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/migrations/versions/2022-07-08_999bceb904df_integration_args.py` & `MindsDB-23.6.1.1/mindsdb/migrations/versions/2022-07-08_999bceb904df_integration_args.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/migrations/versions/2022-07-15_b5b53e0ea7f8_training_data_rows_columns_count.py` & `MindsDB-23.6.1.1/mindsdb/migrations/versions/2022-07-15_b5b53e0ea7f8_training_data_rows_columns_count.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/migrations/versions/2022-07-22_6e834843e7e9_training_time.py` & `MindsDB-23.6.1.1/mindsdb/migrations/versions/2022-07-22_6e834843e7e9_training_time.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/migrations/versions/2022-08-19_976f15a37e6a_predictors_versioning.py` & `MindsDB-23.6.1.1/mindsdb/migrations/versions/2022-08-19_976f15a37e6a_predictors_versioning.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/migrations/versions/2022-08-25_6a54ba55872e_view_integration.py` & `MindsDB-23.6.1.1/mindsdb/migrations/versions/2022-08-25_6a54ba55872e_view_integration.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/migrations/versions/2022-08-29_473e8f239481_straighten.py` & `MindsDB-23.6.1.1/mindsdb/migrations/versions/2022-08-29_473e8f239481_straighten.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/migrations/versions/2022-09-06_96d5fef10caa_data_integration_id.py` & `MindsDB-23.6.1.1/mindsdb/migrations/versions/2022-09-06_96d5fef10caa_data_integration_id.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/migrations/versions/2022-09-08_87b2df2b83e1_predictor_status.py` & `MindsDB-23.6.1.1/mindsdb/migrations/versions/2022-09-08_87b2df2b83e1_predictor_status.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/migrations/versions/2022-09-19_3d5e70105df7_content_storage.py` & `MindsDB-23.6.1.1/mindsdb/migrations/versions/2022-09-19_3d5e70105df7_content_storage.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/migrations/versions/2022-09-29_cada7d2be947_json_storage.py` & `MindsDB-23.6.1.1/mindsdb/migrations/versions/2022-09-29_cada7d2be947_json_storage.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/migrations/versions/2022-10-14_43c52d23845a_projects.py` & `MindsDB-23.6.1.1/mindsdb/migrations/versions/2022-10-14_43c52d23845a_projects.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/migrations/versions/2022-11-07_1e60096fc817_predictor_version.py` & `MindsDB-23.6.1.1/mindsdb/migrations/versions/2022-11-07_1e60096fc817_predictor_version.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/migrations/versions/2022-11-11_d429095b570f_data_integration_id.py` & `MindsDB-23.6.1.1/mindsdb/migrations/versions/2022-11-11_d429095b570f_data_integration_id.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/migrations/versions/2022-12-26_459218b0844c_fix_unique_constraint.py` & `MindsDB-23.6.1.1/mindsdb/migrations/versions/2022-12-26_459218b0844c_fix_unique_constraint.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/migrations/versions/2023-02-02_b6d0a47294ac_jobs.py` & `MindsDB-23.6.1.1/mindsdb/migrations/versions/2023-02-02_b6d0a47294ac_jobs.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/migrations/versions/2023-02-17_ee63d868fa84_predictor_integration_null.py` & `MindsDB-23.6.1.1/mindsdb/migrations/versions/2023-02-17_ee63d868fa84_predictor_integration_null.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/migrations/versions/2023-02-25_3154382dab17_training_progress.py` & `MindsDB-23.6.1.1/mindsdb/migrations/versions/2023-02-25_3154382dab17_training_progress.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/migrations/versions/2023-02-27_ef04cdbe51ed_jobs_user_class.py` & `MindsDB-23.6.1.1/mindsdb/migrations/versions/2023-02-27_ef04cdbe51ed_jobs_user_class.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/migrations/versions/2023-04-11_b8be148dbc85_jobs_history_query.py` & `MindsDB-23.6.1.1/mindsdb/migrations/versions/2023-04-11_b8be148dbc85_jobs_history_query.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/utilities/auth.py` & `MindsDB-23.6.1.1/mindsdb/utilities/auth.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/utilities/cache.py` & `MindsDB-23.6.1.1/mindsdb/utilities/cache.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/utilities/config.py` & `MindsDB-23.6.1.1/mindsdb/utilities/config.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/utilities/context.py` & `MindsDB-23.6.1.1/mindsdb/utilities/context.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/utilities/fs.py` & `MindsDB-23.6.1.1/mindsdb/utilities/fs.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/utilities/functions.py` & `MindsDB-23.6.1.1/mindsdb/utilities/functions.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/utilities/hooks/profiling.py` & `MindsDB-23.6.1.1/mindsdb/utilities/hooks/profiling.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/utilities/json_encoder.py` & `MindsDB-23.6.1.1/mindsdb/utilities/json_encoder.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/utilities/log.py` & `MindsDB-23.6.1.1/mindsdb/utilities/log.py`

 * *Files 4% similar despite different names*

```diff
@@ -98,20 +98,23 @@
     global logger
     if config is None:
         config = Config().get_all()
 
     telemtry_enabled = os.getenv('CHECK_FOR_UPDATES', '1').lower() not in ['0', 'false', 'False']
 
     if telemtry_enabled:
-        import sentry_sdk
-        from sentry_sdk import capture_message, add_breadcrumb
-        sentry_sdk.init(
-            "https://29e64dbdf325404ebf95473d5f4a54d3@o404567.ingest.sentry.io/5633566",
-            traces_sample_rate=0  # Set to `1` to experiment with performance metrics
-        )
+        try:
+            import sentry_sdk
+            from sentry_sdk import capture_message, add_breadcrumb
+            sentry_sdk.init(
+                "https://29e64dbdf325404ebf95473d5f4a54d3@o404567.ingest.sentry.io/5633566",
+                traces_sample_rate=0  # Set to `1` to experiment with performance metrics
+            )
+        except (ImportError, ModuleNotFoundError) as e:
+            raise Exception(f"to use telemetry please install 'pip install mindsdb[telemetry]': {e}")
 
     ''' Create new logger
     :param config: object, app config
     :param logger_name: str, name of logger
     :param wrap_print: bool, if true, then print() calls will be wrapped by log.debug() function.
     '''
     log = logging.getLogger(f'mindsdb.{logger_name}')
```

### Comparing `MindsDB-23.5.4.1/mindsdb/utilities/log_controller.py` & `MindsDB-23.6.1.1/mindsdb/utilities/log_controller.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/utilities/profiler/profiler.py` & `MindsDB-23.6.1.1/mindsdb/utilities/profiler/profiler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/utilities/ps.py` & `MindsDB-23.6.1.1/mindsdb/utilities/ps.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/utilities/telemetry.py` & `MindsDB-23.6.1.1/mindsdb/utilities/telemetry.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.5.4.1/mindsdb/utilities/wizards.py` & `MindsDB-23.6.1.1/mindsdb/utilities/wizards.py`

 * *Files identical despite different names*

