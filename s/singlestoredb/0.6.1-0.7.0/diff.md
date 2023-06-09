# Comparing `tmp/singlestoredb-0.6.1.tar.gz` & `tmp/singlestoredb-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "singlestoredb-0.6.1.tar", last modified: Thu May 18 20:51:00 2023, max compression
+gzip compressed data, was "singlestoredb-0.7.0.tar", last modified: Fri Jun  9 20:35:47 2023, max compression
```

## Comparing `singlestoredb-0.6.1.tar` & `singlestoredb-0.7.0.tar`

### file list

```diff
@@ -1,98 +1,98 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-18 20:51:00.592263 singlestoredb-0.6.1/
--rw-r--r--   0 runner    (1001) docker     (122)    11341 2023-05-18 20:50:36.000000 singlestoredb-0.6.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)     7340 2023-05-18 20:51:00.592263 singlestoredb-0.6.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     6299 2023-05-18 20:50:36.000000 singlestoredb-0.6.1/README.md
--rw-r--r--   0 runner    (1001) docker     (122)     2055 2023-05-18 20:51:00.596263 singlestoredb-0.6.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1316 2023-05-18 20:50:36.000000 singlestoredb-0.6.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-18 20:51:00.572262 singlestoredb-0.6.1/singlestoredb/
--rw-r--r--   0 runner    (1001) docker     (122)      842 2023-05-18 20:50:36.000000 singlestoredb-0.6.1/singlestoredb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     7502 2023-05-18 20:50:36.000000 singlestoredb-0.6.1/singlestoredb/auth.py
--rw-r--r--   0 runner    (1001) docker     (122)     5635 2023-05-18 20:50:36.000000 singlestoredb-0.6.1/singlestoredb/config.py
--rw-r--r--   0 runner    (1001) docker     (122)    42815 2023-05-18 20:50:36.000000 singlestoredb-0.6.1/singlestoredb/connection.py
--rw-r--r--   0 runner    (1001) docker     (122)    12165 2023-05-18 20:50:36.000000 singlestoredb-0.6.1/singlestoredb/converters.py
--rw-r--r--   0 runner    (1001) docker     (122)     2459 2023-05-18 20:50:36.000000 singlestoredb-0.6.1/singlestoredb/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-18 20:51:00.572262 singlestoredb-0.6.1/singlestoredb/http/
--rw-r--r--   0 runner    (1001) docker     (122)      912 2023-05-18 20:50:36.000000 singlestoredb-0.6.1/singlestoredb/http/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    27455 2023-05-18 20:50:36.000000 singlestoredb-0.6.1/singlestoredb/http/connection.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-18 20:51:00.576262 singlestoredb-0.6.1/singlestoredb/management/
--rw-r--r--   0 runner    (1001) docker     (122)       99 2023-05-18 20:50:36.000000 singlestoredb-0.6.1/singlestoredb/management/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    14097 2023-05-18 20:50:36.000000 singlestoredb-0.6.1/singlestoredb/management/cluster.py
--rw-r--r--   0 runner    (1001) docker     (122)     6501 2023-05-18 20:50:36.000000 singlestoredb-0.6.1/singlestoredb/management/manager.py
--rw-r--r--   0 runner    (1001) docker     (122)     1611 2023-05-18 20:50:36.000000 singlestoredb-0.6.1/singlestoredb/management/region.py
--rw-r--r--   0 runner    (1001) docker     (122)     1193 2023-05-18 20:50:36.000000 singlestoredb-0.6.1/singlestoredb/management/utils.py
--rw-r--r--   0 runner    (1001) docker     (122)    18491 2023-05-18 20:50:36.000000 singlestoredb-0.6.1/singlestoredb/management/workspace.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-18 20:51:00.580262 singlestoredb-0.6.1/singlestoredb/mysql/
--rw-r--r--   0 runner    (1001) docker     (122)     4363 2023-05-18 20:50:36.000000 singlestoredb-0.6.1/singlestoredb/mysql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     7985 2023-05-18 20:50:36.000000 singlestoredb-0.6.1/singlestoredb/mysql/_auth.py
--rw-r--r--   0 runner    (1001) docker     (122)    57359 2023-05-18 20:50:36.000000 singlestoredb-0.6.1/singlestoredb/mysql/accel.c
--rw-r--r--   0 runner    (1001) docker     (122)    10324 2023-05-18 20:50:36.000000 singlestoredb-0.6.1/singlestoredb/mysql/charset.py
--rw-r--r--   0 runner    (1001) docker     (122)    58505 2023-05-18 20:50:36.000000 singlestoredb-0.6.1/singlestoredb/mysql/connection.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-18 20:51:00.580262 singlestoredb-0.6.1/singlestoredb/mysql/constants/
--rw-r--r--   0 runner    (1001) docker     (122)      893 2023-05-18 20:50:36.000000 singlestoredb-0.6.1/singlestoredb/mysql/constants/CLIENT.py
--rw-r--r--   0 runner    (1001) docker     (122)      694 2023-05-18 20:50:36.000000 singlestoredb-0.6.1/singlestoredb/mysql/constants/COMMAND.py
--rw-r--r--   0 runner    (1001) docker     (122)     2335 2023-05-18 20:50:36.000000 singlestoredb-0.6.1/singlestoredb/mysql/constants/CR.py
--rw-r--r--   0 runner    (1001) docker     (122)    12311 2023-05-18 20:50:36.000000 singlestoredb-0.6.1/singlestoredb/mysql/constants/ER.py
--rw-r--r--   0 runner    (1001) docker     (122)      385 2023-05-18 20:50:36.000000 singlestoredb-0.6.1/singlestoredb/mysql/constants/FIELD_TYPE.py
--rw-r--r--   0 runner    (1001) docker     (122)      229 2023-05-18 20:50:36.000000 singlestoredb-0.6.1/singlestoredb/mysql/constants/FLAG.py
--rw-r--r--   0 runner    (1001) docker     (122)      348 2023-05-18 20:50:36.000000 singlestoredb-0.6.1/singlestoredb/mysql/constants/SERVER_STATUS.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-18 20:50:36.000000 singlestoredb-0.6.1/singlestoredb/mysql/constants/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4548 2023-05-18 20:50:36.000000 singlestoredb-0.6.1/singlestoredb/mysql/converters.py
--rw-r--r--   0 runner    (1001) docker     (122)    21092 2023-05-18 20:50:36.000000 singlestoredb-0.6.1/singlestoredb/mysql/cursors.py
--rw-r--r--   0 runner    (1001) docker     (122)     2342 2023-05-18 20:50:36.000000 singlestoredb-0.6.1/singlestoredb/mysql/err.py
--rw-r--r--   0 runner    (1001) docker     (122)      589 2023-05-18 20:50:36.000000 singlestoredb-0.6.1/singlestoredb/mysql/optionfile.py
--rw-r--r--   0 runner    (1001) docker     (122)    12081 2023-05-18 20:50:36.000000 singlestoredb-0.6.1/singlestoredb/mysql/protocol.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-18 20:51:00.584262 singlestoredb-0.6.1/singlestoredb/mysql/tests/
--rw-r--r--   0 runner    (1001) docker     (122)      997 2023-05-18 20:50:36.000000 singlestoredb-0.6.1/singlestoredb/mysql/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4025 2023-05-18 20:50:36.000000 singlestoredb-0.6.1/singlestoredb/mysql/tests/base.py
--rw-r--r--   0 runner    (1001) docker     (122)     1117 2023-05-18 20:50:36.000000 singlestoredb-0.6.1/singlestoredb/mysql/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (122)     4878 2023-05-18 20:50:36.000000 singlestoredb-0.6.1/singlestoredb/mysql/tests/test_DictCursor.py
--rw-r--r--   0 runner    (1001) docker     (122)     4306 2023-05-18 20:50:36.000000 singlestoredb-0.6.1/singlestoredb/mysql/tests/test_SSCursor.py
--rw-r--r--   0 runner    (1001) docker     (122)    15465 2023-05-18 20:50:36.000000 singlestoredb-0.6.1/singlestoredb/mysql/tests/test_basic.py
--rw-r--r--   0 runner    (1001) docker     (122)    32297 2023-05-18 20:50:36.000000 singlestoredb-0.6.1/singlestoredb/mysql/tests/test_connection.py
--rw-r--r--   0 runner    (1001) docker     (122)     2002 2023-05-18 20:50:36.000000 singlestoredb-0.6.1/singlestoredb/mysql/tests/test_converters.py
--rw-r--r--   0 runner    (1001) docker     (122)     5045 2023-05-18 20:50:36.000000 singlestoredb-0.6.1/singlestoredb/mysql/tests/test_cursor.py
--rw-r--r--   0 runner    (1001) docker     (122)      422 2023-05-18 20:50:36.000000 singlestoredb-0.6.1/singlestoredb/mysql/tests/test_err.py
--rw-r--r--   0 runner    (1001) docker     (122)    18965 2023-05-18 20:50:36.000000 singlestoredb-0.6.1/singlestoredb/mysql/tests/test_issues.py
--rw-r--r--   0 runner    (1001) docker     (122)     2502 2023-05-18 20:50:36.000000 singlestoredb-0.6.1/singlestoredb/mysql/tests/test_load_local.py
--rw-r--r--   0 runner    (1001) docker     (122)     2725 2023-05-18 20:50:36.000000 singlestoredb-0.6.1/singlestoredb/mysql/tests/test_nextset.py
--rw-r--r--   0 runner    (1001) docker     (122)      585 2023-05-18 20:50:36.000000 singlestoredb-0.6.1/singlestoredb/mysql/tests/test_optionfile.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-18 20:51:00.584262 singlestoredb-0.6.1/singlestoredb/mysql/tests/thirdparty/
--rw-r--r--   0 runner    (1001) docker     (122)      117 2023-05-18 20:50:36.000000 singlestoredb-0.6.1/singlestoredb/mysql/tests/thirdparty/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-18 20:51:00.588263 singlestoredb-0.6.1/singlestoredb/mysql/tests/thirdparty/test_MySQLdb/
--rw-r--r--   0 runner    (1001) docker     (122)      307 2023-05-18 20:50:36.000000 singlestoredb-0.6.1/singlestoredb/mysql/tests/thirdparty/test_MySQLdb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    10171 2023-05-18 20:50:36.000000 singlestoredb-0.6.1/singlestoredb/mysql/tests/thirdparty/test_MySQLdb/capabilities.py
--rw-r--r--   0 runner    (1001) docker     (122)    31414 2023-05-18 20:50:36.000000 singlestoredb-0.6.1/singlestoredb/mysql/tests/thirdparty/test_MySQLdb/dbapi20.py
--rw-r--r--   0 runner    (1001) docker     (122)     3090 2023-05-18 20:50:36.000000 singlestoredb-0.6.1/singlestoredb/mysql/tests/thirdparty/test_MySQLdb/test_MySQLdb_capabilities.py
--rw-r--r--   0 runner    (1001) docker     (122)     8022 2023-05-18 20:50:36.000000 singlestoredb-0.6.1/singlestoredb/mysql/tests/thirdparty/test_MySQLdb/test_MySQLdb_dbapi20.py
--rw-r--r--   0 runner    (1001) docker     (122)     2819 2023-05-18 20:50:36.000000 singlestoredb-0.6.1/singlestoredb/mysql/tests/thirdparty/test_MySQLdb/test_MySQLdb_nonstandard.py
--rw-r--r--   0 runner    (1001) docker     (122)      435 2023-05-18 20:50:36.000000 singlestoredb-0.6.1/singlestoredb/mysql/times.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-18 20:51:00.592263 singlestoredb-0.6.1/singlestoredb/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-18 20:50:36.000000 singlestoredb-0.6.1/singlestoredb/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-18 20:50:36.000000 singlestoredb-0.6.1/singlestoredb/tests/empty.sql
--rw-r--r--   0 runner    (1001) docker     (122)       42 2023-05-18 20:50:36.000000 singlestoredb-0.6.1/singlestoredb/tests/local_infile.csv
--rw-r--r--   0 runner    (1001) docker     (122)     8718 2023-05-18 20:50:36.000000 singlestoredb-0.6.1/singlestoredb/tests/test.sql
--rwxr-xr-x   0 runner    (1001) docker     (122)    36300 2023-05-18 20:50:36.000000 singlestoredb-0.6.1/singlestoredb/tests/test_basics.py
--rwxr-xr-x   0 runner    (1001) docker     (122)    11184 2023-05-18 20:50:36.000000 singlestoredb-0.6.1/singlestoredb/tests/test_config.py
--rwxr-xr-x   0 runner    (1001) docker     (122)    49962 2023-05-18 20:50:36.000000 singlestoredb-0.6.1/singlestoredb/tests/test_connection.py
--rw-r--r--   0 runner    (1001) docker     (122)      652 2023-05-18 20:50:36.000000 singlestoredb-0.6.1/singlestoredb/tests/test_dbapi.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     1131 2023-05-18 20:50:36.000000 singlestoredb-0.6.1/singlestoredb/tests/test_exceptions.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     8580 2023-05-18 20:50:36.000000 singlestoredb-0.6.1/singlestoredb/tests/test_http.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     9721 2023-05-18 20:50:36.000000 singlestoredb-0.6.1/singlestoredb/tests/test_management.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     6582 2023-05-18 20:50:36.000000 singlestoredb-0.6.1/singlestoredb/tests/test_results.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     4500 2023-05-18 20:50:36.000000 singlestoredb-0.6.1/singlestoredb/tests/test_types.py
--rwxr-xr-x   0 runner    (1001) docker     (122)    10408 2023-05-18 20:50:36.000000 singlestoredb-0.6.1/singlestoredb/tests/test_xdict.py
--rw-r--r--   0 runner    (1001) docker     (122)     4673 2023-05-18 20:50:36.000000 singlestoredb-0.6.1/singlestoredb/tests/utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     9969 2023-05-18 20:50:36.000000 singlestoredb-0.6.1/singlestoredb/types.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-18 20:51:00.592263 singlestoredb-0.6.1/singlestoredb/utils/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-18 20:50:36.000000 singlestoredb-0.6.1/singlestoredb/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    23746 2023-05-18 20:50:36.000000 singlestoredb-0.6.1/singlestoredb/utils/config.py
--rw-r--r--   0 runner    (1001) docker     (122)     1816 2023-05-18 20:50:36.000000 singlestoredb-0.6.1/singlestoredb/utils/convert_rows.py
--rw-r--r--   0 runner    (1001) docker     (122)      349 2023-05-18 20:50:36.000000 singlestoredb-0.6.1/singlestoredb/utils/debug.py
--rw-r--r--   0 runner    (1001) docker     (122)     5204 2023-05-18 20:50:36.000000 singlestoredb-0.6.1/singlestoredb/utils/results.py
--rw-r--r--   0 runner    (1001) docker     (122)    12896 2023-05-18 20:50:36.000000 singlestoredb-0.6.1/singlestoredb/utils/xdict.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-18 20:51:00.572262 singlestoredb-0.6.1/singlestoredb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     7340 2023-05-18 20:51:00.000000 singlestoredb-0.6.1/singlestoredb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     3095 2023-05-18 20:51:00.000000 singlestoredb-0.6.1/singlestoredb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-18 20:51:00.000000 singlestoredb-0.6.1/singlestoredb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      239 2023-05-18 20:51:00.000000 singlestoredb-0.6.1/singlestoredb.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       35 2023-05-18 20:51:00.000000 singlestoredb-0.6.1/singlestoredb.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 20:35:47.335817 singlestoredb-0.7.0/
+-rw-r--r--   0 runner    (1001) docker     (122)    11341 2023-06-09 20:35:21.000000 singlestoredb-0.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)     7340 2023-06-09 20:35:47.335817 singlestoredb-0.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     6299 2023-06-09 20:35:21.000000 singlestoredb-0.7.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)     2055 2023-06-09 20:35:47.335817 singlestoredb-0.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1316 2023-06-09 20:35:21.000000 singlestoredb-0.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 20:35:47.323817 singlestoredb-0.7.0/singlestoredb/
+-rw-r--r--   0 runner    (1001) docker     (122)      842 2023-06-09 20:35:21.000000 singlestoredb-0.7.0/singlestoredb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7599 2023-06-09 20:35:21.000000 singlestoredb-0.7.0/singlestoredb/auth.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5914 2023-06-09 20:35:21.000000 singlestoredb-0.7.0/singlestoredb/config.py
+-rw-r--r--   0 runner    (1001) docker     (122)    43133 2023-06-09 20:35:21.000000 singlestoredb-0.7.0/singlestoredb/connection.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12515 2023-06-09 20:35:21.000000 singlestoredb-0.7.0/singlestoredb/converters.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2459 2023-06-09 20:35:21.000000 singlestoredb-0.7.0/singlestoredb/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 20:35:47.323817 singlestoredb-0.7.0/singlestoredb/http/
+-rw-r--r--   0 runner    (1001) docker     (122)      912 2023-06-09 20:35:21.000000 singlestoredb-0.7.0/singlestoredb/http/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    29142 2023-06-09 20:35:21.000000 singlestoredb-0.7.0/singlestoredb/http/connection.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 20:35:47.327817 singlestoredb-0.7.0/singlestoredb/management/
+-rw-r--r--   0 runner    (1001) docker     (122)       99 2023-06-09 20:35:21.000000 singlestoredb-0.7.0/singlestoredb/management/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14097 2023-06-09 20:35:21.000000 singlestoredb-0.7.0/singlestoredb/management/cluster.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6501 2023-06-09 20:35:21.000000 singlestoredb-0.7.0/singlestoredb/management/manager.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1611 2023-06-09 20:35:21.000000 singlestoredb-0.7.0/singlestoredb/management/region.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1193 2023-06-09 20:35:21.000000 singlestoredb-0.7.0/singlestoredb/management/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)    18491 2023-06-09 20:35:21.000000 singlestoredb-0.7.0/singlestoredb/management/workspace.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 20:35:47.327817 singlestoredb-0.7.0/singlestoredb/mysql/
+-rw-r--r--   0 runner    (1001) docker     (122)     4363 2023-06-09 20:35:21.000000 singlestoredb-0.7.0/singlestoredb/mysql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7985 2023-06-09 20:35:21.000000 singlestoredb-0.7.0/singlestoredb/mysql/_auth.py
+-rw-r--r--   0 runner    (1001) docker     (122)    57359 2023-06-09 20:35:21.000000 singlestoredb-0.7.0/singlestoredb/mysql/accel.c
+-rw-r--r--   0 runner    (1001) docker     (122)    10324 2023-06-09 20:35:21.000000 singlestoredb-0.7.0/singlestoredb/mysql/charset.py
+-rw-r--r--   0 runner    (1001) docker     (122)    58819 2023-06-09 20:35:21.000000 singlestoredb-0.7.0/singlestoredb/mysql/connection.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 20:35:47.327817 singlestoredb-0.7.0/singlestoredb/mysql/constants/
+-rw-r--r--   0 runner    (1001) docker     (122)      893 2023-06-09 20:35:21.000000 singlestoredb-0.7.0/singlestoredb/mysql/constants/CLIENT.py
+-rw-r--r--   0 runner    (1001) docker     (122)      694 2023-06-09 20:35:21.000000 singlestoredb-0.7.0/singlestoredb/mysql/constants/COMMAND.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2335 2023-06-09 20:35:21.000000 singlestoredb-0.7.0/singlestoredb/mysql/constants/CR.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12311 2023-06-09 20:35:21.000000 singlestoredb-0.7.0/singlestoredb/mysql/constants/ER.py
+-rw-r--r--   0 runner    (1001) docker     (122)      385 2023-06-09 20:35:21.000000 singlestoredb-0.7.0/singlestoredb/mysql/constants/FIELD_TYPE.py
+-rw-r--r--   0 runner    (1001) docker     (122)      229 2023-06-09 20:35:21.000000 singlestoredb-0.7.0/singlestoredb/mysql/constants/FLAG.py
+-rw-r--r--   0 runner    (1001) docker     (122)      348 2023-06-09 20:35:21.000000 singlestoredb-0.7.0/singlestoredb/mysql/constants/SERVER_STATUS.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-09 20:35:21.000000 singlestoredb-0.7.0/singlestoredb/mysql/constants/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5630 2023-06-09 20:35:21.000000 singlestoredb-0.7.0/singlestoredb/mysql/converters.py
+-rw-r--r--   0 runner    (1001) docker     (122)    21092 2023-06-09 20:35:21.000000 singlestoredb-0.7.0/singlestoredb/mysql/cursors.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2342 2023-06-09 20:35:21.000000 singlestoredb-0.7.0/singlestoredb/mysql/err.py
+-rw-r--r--   0 runner    (1001) docker     (122)      589 2023-06-09 20:35:21.000000 singlestoredb-0.7.0/singlestoredb/mysql/optionfile.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12081 2023-06-09 20:35:21.000000 singlestoredb-0.7.0/singlestoredb/mysql/protocol.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 20:35:47.331817 singlestoredb-0.7.0/singlestoredb/mysql/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)      997 2023-06-09 20:35:21.000000 singlestoredb-0.7.0/singlestoredb/mysql/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4025 2023-06-09 20:35:21.000000 singlestoredb-0.7.0/singlestoredb/mysql/tests/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1117 2023-06-09 20:35:21.000000 singlestoredb-0.7.0/singlestoredb/mysql/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4878 2023-06-09 20:35:21.000000 singlestoredb-0.7.0/singlestoredb/mysql/tests/test_DictCursor.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4306 2023-06-09 20:35:21.000000 singlestoredb-0.7.0/singlestoredb/mysql/tests/test_SSCursor.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15465 2023-06-09 20:35:21.000000 singlestoredb-0.7.0/singlestoredb/mysql/tests/test_basic.py
+-rw-r--r--   0 runner    (1001) docker     (122)    32297 2023-06-09 20:35:21.000000 singlestoredb-0.7.0/singlestoredb/mysql/tests/test_connection.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2002 2023-06-09 20:35:21.000000 singlestoredb-0.7.0/singlestoredb/mysql/tests/test_converters.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5045 2023-06-09 20:35:21.000000 singlestoredb-0.7.0/singlestoredb/mysql/tests/test_cursor.py
+-rw-r--r--   0 runner    (1001) docker     (122)      422 2023-06-09 20:35:21.000000 singlestoredb-0.7.0/singlestoredb/mysql/tests/test_err.py
+-rw-r--r--   0 runner    (1001) docker     (122)    18965 2023-06-09 20:35:21.000000 singlestoredb-0.7.0/singlestoredb/mysql/tests/test_issues.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2502 2023-06-09 20:35:21.000000 singlestoredb-0.7.0/singlestoredb/mysql/tests/test_load_local.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2725 2023-06-09 20:35:21.000000 singlestoredb-0.7.0/singlestoredb/mysql/tests/test_nextset.py
+-rw-r--r--   0 runner    (1001) docker     (122)      585 2023-06-09 20:35:21.000000 singlestoredb-0.7.0/singlestoredb/mysql/tests/test_optionfile.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 20:35:47.331817 singlestoredb-0.7.0/singlestoredb/mysql/tests/thirdparty/
+-rw-r--r--   0 runner    (1001) docker     (122)      117 2023-06-09 20:35:21.000000 singlestoredb-0.7.0/singlestoredb/mysql/tests/thirdparty/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 20:35:47.331817 singlestoredb-0.7.0/singlestoredb/mysql/tests/thirdparty/test_MySQLdb/
+-rw-r--r--   0 runner    (1001) docker     (122)      307 2023-06-09 20:35:21.000000 singlestoredb-0.7.0/singlestoredb/mysql/tests/thirdparty/test_MySQLdb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10171 2023-06-09 20:35:21.000000 singlestoredb-0.7.0/singlestoredb/mysql/tests/thirdparty/test_MySQLdb/capabilities.py
+-rw-r--r--   0 runner    (1001) docker     (122)    31414 2023-06-09 20:35:21.000000 singlestoredb-0.7.0/singlestoredb/mysql/tests/thirdparty/test_MySQLdb/dbapi20.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3090 2023-06-09 20:35:21.000000 singlestoredb-0.7.0/singlestoredb/mysql/tests/thirdparty/test_MySQLdb/test_MySQLdb_capabilities.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8022 2023-06-09 20:35:21.000000 singlestoredb-0.7.0/singlestoredb/mysql/tests/thirdparty/test_MySQLdb/test_MySQLdb_dbapi20.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2819 2023-06-09 20:35:21.000000 singlestoredb-0.7.0/singlestoredb/mysql/tests/thirdparty/test_MySQLdb/test_MySQLdb_nonstandard.py
+-rw-r--r--   0 runner    (1001) docker     (122)      435 2023-06-09 20:35:21.000000 singlestoredb-0.7.0/singlestoredb/mysql/times.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 20:35:47.331817 singlestoredb-0.7.0/singlestoredb/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-09 20:35:21.000000 singlestoredb-0.7.0/singlestoredb/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-09 20:35:21.000000 singlestoredb-0.7.0/singlestoredb/tests/empty.sql
+-rw-r--r--   0 runner    (1001) docker     (122)       42 2023-06-09 20:35:21.000000 singlestoredb-0.7.0/singlestoredb/tests/local_infile.csv
+-rw-r--r--   0 runner    (1001) docker     (122)     8968 2023-06-09 20:35:21.000000 singlestoredb-0.7.0/singlestoredb/tests/test.sql
+-rwxr-xr-x   0 runner    (1001) docker     (122)    40220 2023-06-09 20:35:21.000000 singlestoredb-0.7.0/singlestoredb/tests/test_basics.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)    11184 2023-06-09 20:35:21.000000 singlestoredb-0.7.0/singlestoredb/tests/test_config.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)    49962 2023-06-09 20:35:21.000000 singlestoredb-0.7.0/singlestoredb/tests/test_connection.py
+-rw-r--r--   0 runner    (1001) docker     (122)      652 2023-06-09 20:35:21.000000 singlestoredb-0.7.0/singlestoredb/tests/test_dbapi.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     1131 2023-06-09 20:35:21.000000 singlestoredb-0.7.0/singlestoredb/tests/test_exceptions.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     8580 2023-06-09 20:35:21.000000 singlestoredb-0.7.0/singlestoredb/tests/test_http.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     9721 2023-06-09 20:35:21.000000 singlestoredb-0.7.0/singlestoredb/tests/test_management.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     6582 2023-06-09 20:35:21.000000 singlestoredb-0.7.0/singlestoredb/tests/test_results.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     4500 2023-06-09 20:35:21.000000 singlestoredb-0.7.0/singlestoredb/tests/test_types.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)    10408 2023-06-09 20:35:21.000000 singlestoredb-0.7.0/singlestoredb/tests/test_xdict.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4673 2023-06-09 20:35:21.000000 singlestoredb-0.7.0/singlestoredb/tests/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9969 2023-06-09 20:35:21.000000 singlestoredb-0.7.0/singlestoredb/types.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 20:35:47.335817 singlestoredb-0.7.0/singlestoredb/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-09 20:35:21.000000 singlestoredb-0.7.0/singlestoredb/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    24503 2023-06-09 20:35:21.000000 singlestoredb-0.7.0/singlestoredb/utils/config.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1816 2023-06-09 20:35:21.000000 singlestoredb-0.7.0/singlestoredb/utils/convert_rows.py
+-rw-r--r--   0 runner    (1001) docker     (122)      349 2023-06-09 20:35:21.000000 singlestoredb-0.7.0/singlestoredb/utils/debug.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5204 2023-06-09 20:35:21.000000 singlestoredb-0.7.0/singlestoredb/utils/results.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12896 2023-06-09 20:35:21.000000 singlestoredb-0.7.0/singlestoredb/utils/xdict.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 20:35:47.323817 singlestoredb-0.7.0/singlestoredb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     7340 2023-06-09 20:35:47.000000 singlestoredb-0.7.0/singlestoredb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     3095 2023-06-09 20:35:47.000000 singlestoredb-0.7.0/singlestoredb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-09 20:35:47.000000 singlestoredb-0.7.0/singlestoredb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      239 2023-06-09 20:35:47.000000 singlestoredb-0.7.0/singlestoredb.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       35 2023-06-09 20:35:47.000000 singlestoredb-0.7.0/singlestoredb.egg-info/top_level.txt
```

### Comparing `singlestoredb-0.6.1/LICENSE` & `singlestoredb-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `singlestoredb-0.6.1/PKG-INFO` & `singlestoredb-0.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: singlestoredb
-Version: 0.6.1
+Version: 0.7.0
 Summary: Interface to the SingleStore database and cluster management APIs
 Home-page: https://github.com/singlestore-labs/singlestoredb-python
 Author: SingleStore
 Author-email: support@singlestore.com
 License: Apache-2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `singlestoredb-0.6.1/README.md` & `singlestoredb-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `singlestoredb-0.6.1/setup.cfg` & `singlestoredb-0.7.0/setup.cfg`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = singlestoredb
-version = 0.6.1
+version = 0.7.0
 description = Interface to the SingleStore database and cluster management APIs
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/singlestore-labs/singlestoredb-python
 author = SingleStore
 author_email = support@singlestore.com
 license = Apache-2.0
```

### Comparing `singlestoredb-0.6.1/setup.py` & `singlestoredb-0.7.0/setup.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-0.6.1/singlestoredb/__init__.py` & `singlestoredb-0.7.0/singlestoredb/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 >>> cur = conn.cursor()
 >>> cur.execute('select * from customers')
 >>> for row in cur:
 ...     print(row)
 
 """
 
-__version__ = '0.6.1'
+__version__ = '0.7.0'
 
 from .config import options, get_option, set_option, describe_option
 from .connection import connect, apilevel, threadsafety, paramstyle
 from .exceptions import (
     Warning, Error, InterfaceError, DatabaseError, OperationalError,
     IntegrityError, InternalError, ProgrammingError, NotSupportedError,
     DataError, ManagementError,
```

### Comparing `singlestoredb-0.6.1/singlestoredb/auth.py` & `singlestoredb-0.7.0/singlestoredb/auth.py`

 * *Files 2% similar despite different names*

```diff
@@ -179,18 +179,22 @@
 
     server = None
 
     try:
         server = HTTPServer(('127.0.0.1', 0), AuthServer)
         threading.Thread(target=server.serve_forever).start()
 
+        host = server.server_address[0]
+        if isinstance(host, bytes):
+            host = host.decode('utf-8')
+
         query = urllib.parse.urlencode({
             k: v for k, v in dict(
                 email=email,
-                returnTo=f'http://{server.server_address[0]}:{server.server_address[1]}',
+                returnTo=f'http://{host}:{server.server_address[1]}',
                 db=_listify(databases),
                 cluster=_listify(clusters),
             ).items() if v is not None
         })
 
         if browser is None:
             browser = get_option('sso_browser')
```

### Comparing `singlestoredb-0.6.1/singlestoredb/config.py` & `singlestoredb-0.7.0/singlestoredb/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 #!/usr/bin/env python
 """SingleStoreDB package options."""
 import functools
 
 from . import auth
 from .utils.config import check_bool  # noqa: F401
+from .utils.config import check_dict_str_str  # noqa: F401
 from .utils.config import check_float  # noqa: F401
 from .utils.config import check_int  # noqa: F401
 from .utils.config import check_optional_bool  # noqa: F401
 from .utils.config import check_str  # noqa: F401
 from .utils.config import check_url  # noqa: F401
 from .utils.config import describe_option  # noqa: F401
 from .utils.config import get_default  # noqa: F401
@@ -128,14 +129,24 @@
 register_option(
     'ssl_verify_identity', 'bool', check_optional_bool, None,
     'Verify the server\'s identity',
     environ='SINGLESTOREDB_SSL_VERIFY_IDENTITY',
 )
 
 register_option(
+    'program_name', 'string', check_str, None,
+    'Name of the program',
+)
+
+register_option(
+    'conn_attrs', 'dict', check_dict_str_str, None,
+    'Additional connection attributes for telemetry',
+)
+
+register_option(
     'credential_type', 'str',
     functools.partial(
         check_str, valid_values=[
             auth.PASSWORD,
             auth.JWT,
             auth.BROWSER_SSO,
         ],
```

### Comparing `singlestoredb-0.6.1/singlestoredb/connection.py` & `singlestoredb-0.7.0/singlestoredb/connection.py`

 * *Files 1% similar despite different names*

```diff
@@ -1270,14 +1270,16 @@
     ssl_verify_identity: Optional[bool] = None,
     conv: Optional[Dict[int, Callable[..., Any]]] = None,
     credential_type: Optional[str] = None,
     autocommit: Optional[bool] = None,
     results_type: Optional[str] = None,
     buffered: Optional[bool] = None,
     results_format: Optional[str] = None,
+    program_name: Optional[str] = None,
+    conn_attrs: Optional[Dict[str, str]] = None,
 ) -> Connection:
     """
     Return a SingleStoreDB connection.
 
     Parameters
     ----------
     host : str, optional
@@ -1326,14 +1328,19 @@
         Type of authentication to use: auth.PASSWORD, auth.JWT, or auth.BROWSER_SSO
     autocommit : bool, optional
         Enable autocommits
     results_type : str, optional
         The form of the query results: tuples, namedtuples, dicts
     results_format : str, optional
         Deprecated. This option has been renamed to results_type.
+    program_name: str, optional
+        Name of the program
+    conn_attrs: dict, optional
+        Additional connection attributes for telemetry. Example:
+        {'program_version': "1.0.2", "_connector_name": "dbt connector"}
 
     Examples
     --------
     Standard database connection
 
     >>> conn = s2.connect('me:p455w0rd@s2-host.com/my_db')
```

### Comparing `singlestoredb-0.6.1/singlestoredb/converters.py` & `singlestoredb-0.7.0/singlestoredb/converters.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,14 +9,26 @@
 from typing import Callable
 from typing import Dict
 from typing import List
 from typing import Optional
 from typing import Set
 from typing import Union
 
+try:
+    import shapely.wkt
+    has_shapely = True
+except ImportError:
+    has_shapely = False
+
+try:
+    import pygeos
+    has_pygeos = True
+except ImportError:
+    has_pygeos = False
+
 
 # Cache fromisoformat methods if they exist
 _dt_datetime_fromisoformat = None
 if hasattr(datetime.datetime, 'fromisoformat'):
     _dt_datetime_fromisoformat = datetime.datetime.fromisoformat  # type: ignore
 _dt_time_fromisoformat = None
 if hasattr(datetime.time, 'fromisoformat'):
@@ -496,22 +508,26 @@
     Parameters
     ----------
     x : Any
         Geometry value
 
     Returns
     -------
-    ???
+    shapely object or pygeos object or str
         If value is valid geometry value
     None
-        If input value is None
+        If input value is None or empty
 
     """
-    if x is None:
+    if x is None or not x:
         return None
+    if has_shapely:
+        return shapely.wkt.loads(x)
+    if has_pygeos:
+        return pygeos.io.from_wkt(x)
     return x
 
 
 # Map of database types and conversion functions
 converters: Dict[int, Callable[..., Any]] = {
     0: decimal_or_none,
     1: int_or_none,
```

### Comparing `singlestoredb-0.6.1/singlestoredb/exceptions.py` & `singlestoredb-0.7.0/singlestoredb/exceptions.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-0.6.1/singlestoredb/http/__init__.py` & `singlestoredb-0.7.0/singlestoredb/http/__init__.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-0.6.1/singlestoredb/http/connection.py` & `singlestoredb-0.7.0/singlestoredb/http/connection.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,14 +13,33 @@
 from typing import Sequence
 from typing import Tuple
 from typing import Union
 from urllib.parse import urljoin
 
 import requests
 
+try:
+    import numpy as np
+    has_numpy = True
+except ImportError:
+    has_numpy = False
+
+try:
+    import pygeos
+    has_pygeos = True
+except ImportError:
+    has_pygeos = False
+
+try:
+    import shapely.geometry
+    import shapely.wkt
+    has_shapely = True
+except ImportError:
+    has_shapely = False
+
 from .. import connection
 from .. import types
 from ..config import get_option
 from ..converters import converters
 from ..exceptions import DatabaseError  # noqa: F401
 from ..exceptions import DataError
 from ..exceptions import Error  # noqa: F401
@@ -140,14 +159,60 @@
     if x is None:
         return None
     if converter is None:
         return b64decode(x)
     return converter(b64decode(x))
 
 
+shapely_Point = None
+shapely_Polygon = None
+shapely_LineString = None
+np_ndarray = None
+pygeos_Geometry = None
+
+
+if has_shapely:
+    shapely_Point = shapely.geometry.Point
+    shapely_Polygon = shapely.geometry.Polygon
+    shapely_LineString = shapely.geometry.LineString
+
+if has_numpy:
+    np_ndarray = np.ndarray
+
+if has_pygeos:
+    pygeos_Geometry = pygeos.Geometry
+
+
+def convert_special_type(arg: Any) -> Any:
+    """Convert special data type objects."""
+    dtype = type(arg)
+    if dtype is np_ndarray:
+        return arg.tobytes()
+    if dtype is shapely_Point:
+        return shapely.wkt.dumps(arg)
+    if dtype is shapely_Polygon:
+        return shapely.wkt.dumps(arg)
+    if dtype is shapely_LineString:
+        return shapely.wkt.dumps(arg)
+    if dtype is pygeos_Geometry:
+        return pygeos.io.to_wkt(arg)
+    return arg
+
+
+def convert_special_params(
+    params: Optional[Union[Sequence[Any], Dict[str, Any]]] = None,
+) -> Optional[Union[Sequence[Any], Dict[str, Any]]]:
+    """Convert parameters of special data types."""
+    if params is None:
+        return params
+    if isinstance(params, Dict):
+        return {k: convert_special_type(v) for k, v in params.items()}
+    return tuple(map(convert_special_type, params))
+
+
 class PyMyField(object):
     """Field for PyMySQL compatibility."""
 
     def __init__(self, name: str, flags: int, charset: int) -> None:
         self.name = name
         self.flags = flags
         self.charsetnr = charset
@@ -280,15 +345,18 @@
 
     def _validate_param_subs(
         self, query: str,
         args: Optional[Union[Sequence[Any], Dict[str, Any]]] = None,
     ) -> None:
         """Make sure the parameter substitions are valid."""
         if args is not None:
-            query = query % args
+            if isinstance(args, Sequence):
+                query = query % tuple(args)
+            else:
+                query = query % args
 
     def _execute(
         self, oper: str,
         params: Optional[Union[Sequence[Any], Dict[str, Any]]] = None,
         is_callproc: bool = False,
     ) -> int:
         if self._connection is None:
@@ -298,15 +366,15 @@
 
         oper, params = self._connection._convert_params(oper, params)
 
         log_query(oper, params)
 
         data: Dict[str, Any] = dict(sql=oper)
         if params is not None:
-            data['args'] = params
+            data['args'] = convert_special_params(params)
         if self._connection._database:
             data['database'] = self._connection._database
 
         self._expect_results = False
         sql_type = 'exec'
         if re.match(r'^\s*(select|show|call|echo)\s+', oper, flags=re.I):
             self._expect_results = True
@@ -752,15 +820,15 @@
 
     @property
     def messages(self) -> List[Tuple[int, str]]:
         return self._messages
 
     def connect(self) -> 'Connection':
         """Connect to the server."""
-        pass
+        return self
 
     def _post(self, path: str, *args: Any, **kwargs: Any) -> requests.Response:
         """
         Invoke a POST request on the HTTP connection.
 
         Parameters
         ----------
```

### Comparing `singlestoredb-0.6.1/singlestoredb/management/cluster.py` & `singlestoredb-0.7.0/singlestoredb/management/cluster.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-0.6.1/singlestoredb/management/manager.py` & `singlestoredb-0.7.0/singlestoredb/management/manager.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-0.6.1/singlestoredb/management/region.py` & `singlestoredb-0.7.0/singlestoredb/management/region.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-0.6.1/singlestoredb/management/utils.py` & `singlestoredb-0.7.0/singlestoredb/management/utils.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-0.6.1/singlestoredb/management/workspace.py` & `singlestoredb-0.7.0/singlestoredb/management/workspace.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-0.6.1/singlestoredb/mysql/__init__.py` & `singlestoredb-0.7.0/singlestoredb/mysql/__init__.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-0.6.1/singlestoredb/mysql/_auth.py` & `singlestoredb-0.7.0/singlestoredb/mysql/_auth.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-0.6.1/singlestoredb/mysql/accel.c` & `singlestoredb-0.7.0/singlestoredb/mysql/accel.c`

 * *Files identical despite different names*

### Comparing `singlestoredb-0.6.1/singlestoredb/mysql/charset.py` & `singlestoredb-0.7.0/singlestoredb/mysql/charset.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-0.6.1/singlestoredb/mysql/connection.py` & `singlestoredb-0.7.0/singlestoredb/mysql/connection.py`

 * *Files 0% similar despite different names*

```diff
@@ -287,14 +287,15 @@
         buffered=True,
         results_type='tuples',
         compress=None,  # not supported
         named_pipe=None,  # not supported
         passwd=None,  # deprecated
         db=None,  # deprecated
         driver=None,  # internal use
+        conn_attrs=None,
     ):
         BaseConnection.__init__(**dict(locals()))
 
         if db is not None and database is None:
             # We will raise warning in 2022 or later.
             # See https://github.com/PyMySQL/PyMySQL/issues/939
             # warnings.warn("'db' is deprecated, use 'database'", DeprecationWarning, 3)
@@ -486,21 +487,27 @@
         self._auth_plugin_map = auth_plugin_map or {}
         self._binary_prefix = binary_prefix
         self.server_public_key = server_public_key
 
         from .. import __version__ as VERSION_STRING
 
         self._connect_attrs = {
-            '_client_name': 'singlestoredb.mysql',
+            '_os': str(sys.platform),
             '_pid': str(os.getpid()),
+            '_client_name': 'SingleStoreDB Python Client',
             '_client_version': VERSION_STRING,
         }
 
         if program_name:
             self._connect_attrs['program_name'] = program_name
+        if conn_attrs is not None:
+            # do not overwrite the attributes that we set ourselves
+            for k, v in conn_attrs.items():
+                if k not in self._connect_attrs:
+                    self._connect_attrs[k] = v
 
         if defer_connect:
             self._sock = None
         else:
             self.connect()
 
     @property
```

### Comparing `singlestoredb-0.6.1/singlestoredb/mysql/constants/CLIENT.py` & `singlestoredb-0.7.0/singlestoredb/mysql/constants/CLIENT.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-0.6.1/singlestoredb/mysql/constants/COMMAND.py` & `singlestoredb-0.7.0/singlestoredb/mysql/constants/COMMAND.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-0.6.1/singlestoredb/mysql/constants/CR.py` & `singlestoredb-0.7.0/singlestoredb/mysql/constants/CR.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-0.6.1/singlestoredb/mysql/constants/ER.py` & `singlestoredb-0.7.0/singlestoredb/mysql/constants/ER.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-0.6.1/singlestoredb/mysql/converters.py` & `singlestoredb-0.7.0/singlestoredb/mysql/converters.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,14 +2,33 @@
 import datetime
 import time
 from decimal import Decimal
 
 from ..converters import converters as decoders
 from .err import ProgrammingError
 
+try:
+    import numpy as np
+    has_numpy = True
+except ImportError:
+    has_numpy = False
+
+try:
+    import shapely.geometry
+    import shapely.wkt
+    has_shapely = True
+except ImportError:
+    has_shapely = False
+
+try:
+    import pygeos
+    has_pygeos = True
+except ImportError:
+    has_pygeos = False
+
 
 def escape_item(val, charset, mapping=None):
     if mapping is None:
         mapping = encoders
     encoder = mapping.get(type(val))
 
     # Fallback to default when no encoder found
@@ -172,14 +191,40 @@
     datetime.datetime: escape_datetime,
     datetime.timedelta: escape_timedelta,
     datetime.time: escape_time,
     time.struct_time: escape_struct_time,
     Decimal: Decimal2Literal,
 }
 
+if has_numpy:
+
+    def escape_numpy(value, mapping=None):
+        """Convert numpy arrays to vectors of bytes."""
+        return escape_bytes(value.tobytes(), mapping=mapping)
+
+    encoders[np.ndarray] = escape_numpy
+
+if has_shapely:
+
+    def escape_shapely(value, mapping=None):
+        """Convert shapely geo objects."""
+        return escape_str(shapely.wkt.dumps(value), mapping=mapping)
+
+    encoders[shapely.geometry.Polygon] = escape_shapely
+    encoders[shapely.geometry.Point] = escape_shapely
+    encoders[shapely.geometry.LineString] = escape_shapely
+
+if has_pygeos:
+
+    def escape_pygeos(value, mapping=None):
+        """Convert pygeos objects."""
+        return escape_str(pygeos.io.to_wkt(value), mapping=mapping)
+
+    encoders[pygeos.Geometry] = escape_pygeos
+
 
 # for MySQLdb compatibility
 conversions = encoders.copy()
 conversions.update(decoders)
 Thing2Literal = escape_str
 
 # Run doctests with `pytest --doctest-modules pymysql/converters.py`
```

### Comparing `singlestoredb-0.6.1/singlestoredb/mysql/cursors.py` & `singlestoredb-0.7.0/singlestoredb/mysql/cursors.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-0.6.1/singlestoredb/mysql/err.py` & `singlestoredb-0.7.0/singlestoredb/mysql/err.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-0.6.1/singlestoredb/mysql/optionfile.py` & `singlestoredb-0.7.0/singlestoredb/mysql/optionfile.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-0.6.1/singlestoredb/mysql/protocol.py` & `singlestoredb-0.7.0/singlestoredb/mysql/protocol.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-0.6.1/singlestoredb/mysql/tests/__init__.py` & `singlestoredb-0.7.0/singlestoredb/mysql/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-0.6.1/singlestoredb/mysql/tests/base.py` & `singlestoredb-0.7.0/singlestoredb/mysql/tests/base.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-0.6.1/singlestoredb/mysql/tests/conftest.py` & `singlestoredb-0.7.0/singlestoredb/mysql/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-0.6.1/singlestoredb/mysql/tests/test_DictCursor.py` & `singlestoredb-0.7.0/singlestoredb/mysql/tests/test_DictCursor.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-0.6.1/singlestoredb/mysql/tests/test_SSCursor.py` & `singlestoredb-0.7.0/singlestoredb/mysql/tests/test_SSCursor.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-0.6.1/singlestoredb/mysql/tests/test_basic.py` & `singlestoredb-0.7.0/singlestoredb/mysql/tests/test_basic.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-0.6.1/singlestoredb/mysql/tests/test_connection.py` & `singlestoredb-0.7.0/singlestoredb/mysql/tests/test_connection.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-0.6.1/singlestoredb/mysql/tests/test_converters.py` & `singlestoredb-0.7.0/singlestoredb/mysql/tests/test_converters.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-0.6.1/singlestoredb/mysql/tests/test_cursor.py` & `singlestoredb-0.7.0/singlestoredb/mysql/tests/test_cursor.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-0.6.1/singlestoredb/mysql/tests/test_issues.py` & `singlestoredb-0.7.0/singlestoredb/mysql/tests/test_issues.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-0.6.1/singlestoredb/mysql/tests/test_load_local.py` & `singlestoredb-0.7.0/singlestoredb/mysql/tests/test_load_local.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-0.6.1/singlestoredb/mysql/tests/test_nextset.py` & `singlestoredb-0.7.0/singlestoredb/mysql/tests/test_nextset.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-0.6.1/singlestoredb/mysql/tests/test_optionfile.py` & `singlestoredb-0.7.0/singlestoredb/mysql/tests/test_optionfile.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-0.6.1/singlestoredb/mysql/tests/thirdparty/test_MySQLdb/capabilities.py` & `singlestoredb-0.7.0/singlestoredb/mysql/tests/thirdparty/test_MySQLdb/capabilities.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-0.6.1/singlestoredb/mysql/tests/thirdparty/test_MySQLdb/dbapi20.py` & `singlestoredb-0.7.0/singlestoredb/mysql/tests/thirdparty/test_MySQLdb/dbapi20.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-0.6.1/singlestoredb/mysql/tests/thirdparty/test_MySQLdb/test_MySQLdb_capabilities.py` & `singlestoredb-0.7.0/singlestoredb/mysql/tests/thirdparty/test_MySQLdb/test_MySQLdb_capabilities.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-0.6.1/singlestoredb/mysql/tests/thirdparty/test_MySQLdb/test_MySQLdb_dbapi20.py` & `singlestoredb-0.7.0/singlestoredb/mysql/tests/thirdparty/test_MySQLdb/test_MySQLdb_dbapi20.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-0.6.1/singlestoredb/mysql/tests/thirdparty/test_MySQLdb/test_MySQLdb_nonstandard.py` & `singlestoredb-0.7.0/singlestoredb/mysql/tests/thirdparty/test_MySQLdb/test_MySQLdb_nonstandard.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-0.6.1/singlestoredb/tests/test.sql` & `singlestoredb-0.7.0/singlestoredb/tests/test.sql`

 * *Files 1% similar despite different names*

```diff
@@ -343,8 +343,22 @@
     `tinyblob`=x'',
     `json`='{}',
     `enum`='one',
     `set`='two',
     `bit`=0
 ;
 
+
+--
+-- Table of extended data types
+--
+CREATE ROWSTORE TABLE IF NOT EXISTS `extended_types` (
+    `id` INT(11),
+    `geography` GEOGRAPHY,
+    `geographypoint` GEOGRAPHYPOINT,
+    `vectors` BLOB,
+    `testkey` LONGTEXT
+)
+COLLATE='utf8_unicode_ci';
+
+
 COMMIT;
```

### Comparing `singlestoredb-0.6.1/singlestoredb/tests/test_basics.py` & `singlestoredb-0.7.0/singlestoredb/tests/test_basics.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,14 +2,33 @@
 # type: ignore
 """Basic SingleStoreDB connection testing."""
 import datetime
 import decimal
 import os
 import unittest
 
+try:
+    import numpy as np
+    has_numpy = True
+except ImportError:
+    has_numpy = False
+
+try:
+    import shapely.wkt
+    has_shapely = True
+except ImportError:
+    has_shapely = False
+
+try:
+    import pygeos
+    from pygeos.testing import assert_geometries_equal
+    has_pygeos = True
+except ImportError:
+    has_pygeos = False
+
 import singlestoredb as s2
 from . import utils
 # import traceback
 
 
 class TestBasics(unittest.TestCase):
 
@@ -476,14 +495,108 @@
         with self.assertRaises(s2.ProgrammingError) as cm:
             self.cur.execute('garbage syntax')
 
         exc = cm.exception
         assert exc.errno == 1064, exc.errno
         assert 'You have an error in your SQL syntax' in exc.errmsg, exc.errmsg
 
+    def test_extended_types(self):
+        if not has_numpy or not has_pygeos or not has_shapely:
+            self.skipTest('Test requires numpy, pygeos, and shapely')
+
+        import uuid
+
+        key = str(uuid.uuid4())
+
+        # shapely data
+        data = [
+            (1, 'POLYGON((1 1, 2 1, 2 2, 1 2, 1 1))', 'POINT(1.5 1.5)', [0.5, 0.6], key),
+            (2, 'POLYGON((5 1, 6 1, 6 2, 5 2, 5 1))', 'POINT(5.5 1.5)', [1.3, 2.5], key),
+            (
+                3, 'POLYGON((5 5, 6 5, 6 6, 5 6, 5 5))',
+                'POINT(5.5 5.5)', [10.3, 11.1], key,
+            ),
+            (4, 'POLYGON((1 5, 2 5, 2 6, 1 6, 1 5))', 'POINT(1.5 5.5)', [3.3, 3.4], key),
+            (5, 'POLYGON((3 3, 4 3, 4 4, 3 4, 3 3))', 'POINT(3.5 3.5)', [2.9, 9.5], key),
+        ]
+
+        new_data = []
+        for i, row in enumerate(data):
+            row = list(row)
+            row[1] = shapely.wkt.loads(row[1])
+            row[2] = shapely.wkt.loads(row[2])
+            if 'http' in self.conn.driver:
+                row[3] = ''
+            else:
+                row[3] = np.array(row[3], dtype='<f4')
+            new_data.append(row)
+
+        self.cur.executemany(
+            'INSERT INTO extended_types '
+            '(id, geography, geographypoint, vectors, testkey) '
+            'VALUES (%s, %s, %s, %s, %s)', new_data,
+        )
+
+        self.cur.execute(
+            'SELECT * FROM extended_types WHERE testkey = %s ORDER BY id', [key],
+        )
+
+        for data_row, row in zip(new_data, self.cur):
+            assert data_row[0] == row[0]
+            assert data_row[1].equals_exact(shapely.wkt.loads(row[1]), 1e-4)
+            assert data_row[2].equals_exact(shapely.wkt.loads(row[2]), 1e-4)
+            if 'http' in self.conn.driver:
+                assert row[3] == b''
+            else:
+                assert (data_row[3] == np.frombuffer(row[3], dtype='<f4')).all()
+
+        # pygeos data
+        data = [
+            (6, 'POLYGON((1 1, 2 1, 2 2, 1 2, 1 1))', 'POINT(1.5 1.5)', [0.5, 0.6], key),
+            (7, 'POLYGON((5 1, 6 1, 6 2, 5 2, 5 1))', 'POINT(5.5 1.5)', [1.3, 2.5], key),
+            (
+                8, 'POLYGON((5 5, 6 5, 6 6, 5 6, 5 5))',
+                'POINT(5.5 5.5)', [10.3, 11.1], key,
+            ),
+            (9, 'POLYGON((1 5, 2 5, 2 6, 1 6, 1 5))', 'POINT(1.5 5.5)', [3.3, 3.4], key),
+            (10, 'POLYGON((3 3, 4 3, 4 4, 3 4, 3 3))', 'POINT(3.5 3.5)', [2.9, 9.5], key),
+        ]
+
+        new_data = []
+        for i, row in enumerate(data):
+            row = list(row)
+            row[1] = pygeos.io.from_wkt(row[1])
+            row[2] = pygeos.io.from_wkt(row[2])
+            if 'http' in self.conn.driver:
+                row[3] = ''
+            else:
+                row[3] = np.array(row[3], dtype='<f4')
+            new_data.append(row)
+
+        self.cur.executemany(
+            'INSERT INTO extended_types '
+            '(id, geography, geographypoint, vectors, testkey) '
+            'VALUES (%s, %s, %s, %s, %s)', new_data,
+        )
+
+        self.cur.execute(
+            'SELECT * FROM extended_types WHERE id >= 6 and testkey = %s ORDER BY id', [
+                key,
+            ],
+        )
+
+        for data_row, row in zip(new_data, self.cur):
+            assert data_row[0] == row[0]
+            assert_geometries_equal(data_row[1], pygeos.io.from_wkt(row[1]))
+            assert_geometries_equal(data_row[2], pygeos.io.from_wkt(row[2]))
+            if 'http' in self.conn.driver:
+                assert row[3] == b''
+            else:
+                assert (data_row[3] == np.frombuffer(row[3], dtype='<f4')).all()
+
     def test_alltypes(self):
         self.cur.execute('select * from alltypes where id = 0')
         names = [x[0] for x in self.cur.description]
         types = [x[1] for x in self.cur.description]
         out = self.cur.fetchone()
         row = dict(zip(names, out))
         typ = dict(zip(names, types))
```

### Comparing `singlestoredb-0.6.1/singlestoredb/tests/test_config.py` & `singlestoredb-0.7.0/singlestoredb/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-0.6.1/singlestoredb/tests/test_connection.py` & `singlestoredb-0.7.0/singlestoredb/tests/test_connection.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-0.6.1/singlestoredb/tests/test_dbapi.py` & `singlestoredb-0.7.0/singlestoredb/tests/test_dbapi.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-0.6.1/singlestoredb/tests/test_exceptions.py` & `singlestoredb-0.7.0/singlestoredb/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-0.6.1/singlestoredb/tests/test_http.py` & `singlestoredb-0.7.0/singlestoredb/tests/test_http.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-0.6.1/singlestoredb/tests/test_management.py` & `singlestoredb-0.7.0/singlestoredb/tests/test_management.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-0.6.1/singlestoredb/tests/test_results.py` & `singlestoredb-0.7.0/singlestoredb/tests/test_results.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-0.6.1/singlestoredb/tests/test_types.py` & `singlestoredb-0.7.0/singlestoredb/tests/test_types.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-0.6.1/singlestoredb/tests/test_xdict.py` & `singlestoredb-0.7.0/singlestoredb/tests/test_xdict.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-0.6.1/singlestoredb/tests/utils.py` & `singlestoredb-0.7.0/singlestoredb/tests/utils.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-0.6.1/singlestoredb/types.py` & `singlestoredb-0.7.0/singlestoredb/types.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-0.6.1/singlestoredb/utils/config.py` & `singlestoredb-0.7.0/singlestoredb/utils/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,14 +28,15 @@
 import os
 import re
 from typing import Any
 from typing import Callable
 from typing import Dict
 from typing import Iterator
 from typing import List
+from typing import Mapping
 from typing import Optional
 from typing import Tuple
 from typing import Union
 from urllib.parse import urlparse
 
 from .xdict import xdict
 
@@ -641,14 +642,49 @@
             '%s is not one of the possible values: %s' %
             (out, ', '.join(valid_values)),
         )
 
     return out
 
 
+def check_dict_str_str(
+    value: Any,
+) -> Optional[Dict[str, str]]:
+    """
+    Validate a string value.
+
+    Parameters
+    ----------
+    value : dict
+        The value to validate. Keys and values must be strings.
+
+    Returns
+    -------
+    dict
+        The validated dict value
+    """
+    if value is None:
+        return None
+
+    if not isinstance(value, Mapping):
+        raise ValueError(
+            'value {} must be of type dict'.format(value),
+        )
+
+    out = {}
+    for k, v in value.items():
+        if not isinstance(k, str) or not isinstance(v, str):
+            raise ValueError(
+                'keys and values in {} must be strings'.format(value),
+            )
+        out[k] = v
+
+    return out
+
+
 def check_url(
     value: str,
     pattern: Optional[str] = None,
     max_length: Optional[int] = None,
     min_length: Optional[int] = None,
     valid_values: Optional[List[str]] = None,
 ) -> Optional[str]:
```

### Comparing `singlestoredb-0.6.1/singlestoredb/utils/convert_rows.py` & `singlestoredb-0.7.0/singlestoredb/utils/convert_rows.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-0.6.1/singlestoredb/utils/results.py` & `singlestoredb-0.7.0/singlestoredb/utils/results.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-0.6.1/singlestoredb/utils/xdict.py` & `singlestoredb-0.7.0/singlestoredb/utils/xdict.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-0.6.1/singlestoredb.egg-info/PKG-INFO` & `singlestoredb-0.7.0/singlestoredb.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: singlestoredb
-Version: 0.6.1
+Version: 0.7.0
 Summary: Interface to the SingleStore database and cluster management APIs
 Home-page: https://github.com/singlestore-labs/singlestoredb-python
 Author: SingleStore
 Author-email: support@singlestore.com
 License: Apache-2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `singlestoredb-0.6.1/singlestoredb.egg-info/SOURCES.txt` & `singlestoredb-0.7.0/singlestoredb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

