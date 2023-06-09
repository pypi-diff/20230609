# Comparing `tmp/dcrx-api-0.0.6.tar.gz` & `tmp/dcrx-api-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dcrx-api-0.0.6.tar", last modified: Fri Jun  9 01:54:12 2023, max compression
+gzip compressed data, was "dcrx-api-0.0.7.tar", last modified: Fri Jun  9 02:03:25 2023, max compression
```

## Comparing `dcrx-api-0.0.6.tar` & `dcrx-api-0.0.7.tar`

### file list

```diff
@@ -1,76 +1,76 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 01:54:12.599820 dcrx-api-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-09 01:54:04.000000 dcrx-api-0.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6101 2023-06-09 01:54:12.595819 dcrx-api-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5427 2023-06-09 01:54:04.000000 dcrx-api-0.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 01:54:12.587819 dcrx-api-0.0.6/dcrx_api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 01:54:04.000000 dcrx-api-0.0.6/dcrx_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-06-09 01:54:04.000000 dcrx-api-0.0.6/dcrx_api/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 01:54:12.591819 dcrx-api-0.0.6/dcrx_api/auth/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 01:54:04.000000 dcrx-api-0.0.6/dcrx_api/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5557 2023-06-09 01:54:04.000000 dcrx-api-0.0.6/dcrx_api/auth/auth_context.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 01:54:12.591819 dcrx-api-0.0.6/dcrx_api/auth/models/
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-06-09 01:54:04.000000 dcrx-api-0.0.6/dcrx_api/auth/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-09 01:54:04.000000 dcrx-api-0.0.6/dcrx_api/auth/models/auth_claims.py
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-06-09 01:54:04.000000 dcrx-api-0.0.6/dcrx_api/auth/models/auth_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-09 01:54:04.000000 dcrx-api-0.0.6/dcrx_api/auth/models/authentication_failure_exception.py
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-06-09 01:54:04.000000 dcrx-api-0.0.6/dcrx_api/auth/models/generated_token.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 01:54:12.591819 dcrx-api-0.0.6/dcrx_api/cli/
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-09 01:54:04.000000 dcrx-api-0.0.6/dcrx_api/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-06-09 01:54:04.000000 dcrx-api-0.0.6/dcrx_api/cli/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2640 2023-06-09 01:54:04.000000 dcrx-api-0.0.6/dcrx_api/cli/database.py
--rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-06-09 01:54:04.000000 dcrx-api-0.0.6/dcrx_api/cli/server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 01:54:12.591819 dcrx-api-0.0.6/dcrx_api/database/
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-09 01:54:04.000000 dcrx-api-0.0.6/dcrx_api/database/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3220 2023-06-09 01:54:04.000000 dcrx-api-0.0.6/dcrx_api/database/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-06-09 01:54:04.000000 dcrx-api-0.0.6/dcrx_api/database/connection_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 01:54:12.595819 dcrx-api-0.0.6/dcrx_api/env/
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-09 01:54:04.000000 dcrx-api-0.0.6/dcrx_api/env/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-06-09 01:54:04.000000 dcrx-api-0.0.6/dcrx_api/env/env.py
--rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-06-09 01:54:04.000000 dcrx-api-0.0.6/dcrx_api/env/load_env.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 01:54:12.595819 dcrx-api-0.0.6/dcrx_api/jobs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 01:54:04.000000 dcrx-api-0.0.6/dcrx_api/jobs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3417 2023-06-09 01:54:04.000000 dcrx-api-0.0.6/dcrx_api/jobs/job.py
--rw-r--r--   0 runner    (1001) docker     (123)     3348 2023-06-09 01:54:04.000000 dcrx-api-0.0.6/dcrx_api/jobs/job_queue.py
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-09 01:54:04.000000 dcrx-api-0.0.6/dcrx_api/jobs/job_status.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 01:54:12.595819 dcrx-api-0.0.6/dcrx_api/jobs/models/
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-06-09 01:54:04.000000 dcrx-api-0.0.6/dcrx_api/jobs/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-06-09 01:54:04.000000 dcrx-api-0.0.6/dcrx_api/jobs/models/build_options.py
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-06-09 01:54:04.000000 dcrx-api-0.0.6/dcrx_api/jobs/models/job_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-06-09 01:54:04.000000 dcrx-api-0.0.6/dcrx_api/jobs/models/job_not_found_exception.py
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-06-09 01:54:04.000000 dcrx-api-0.0.6/dcrx_api/jobs/models/new_image.py
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-06-09 01:54:04.000000 dcrx-api-0.0.6/dcrx_api/jobs/models/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     1646 2023-06-09 01:54:04.000000 dcrx-api-0.0.6/dcrx_api/jobs/service.py
--rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-06-09 01:54:04.000000 dcrx-api-0.0.6/dcrx_api/lifespan.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 01:54:12.595819 dcrx-api-0.0.6/dcrx_api/middleware/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 01:54:04.000000 dcrx-api-0.0.6/dcrx_api/middleware/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-06-09 01:54:04.000000 dcrx-api-0.0.6/dcrx_api/middleware/auth_middleware.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 01:54:12.595819 dcrx-api-0.0.6/dcrx_api/users/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 01:54:04.000000 dcrx-api-0.0.6/dcrx_api/users/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 01:54:12.595819 dcrx-api-0.0.6/dcrx_api/users/models/
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-06-09 01:54:04.000000 dcrx-api-0.0.6/dcrx_api/users/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-06-09 01:54:04.000000 dcrx-api-0.0.6/dcrx_api/users/models/authorized_user.py
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-06-09 01:54:04.000000 dcrx-api-0.0.6/dcrx_api/users/models/base_user.py
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-06-09 01:54:04.000000 dcrx-api-0.0.6/dcrx_api/users/models/db_user.py
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-06-09 01:54:04.000000 dcrx-api-0.0.6/dcrx_api/users/models/login_user.py
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-06-09 01:54:04.000000 dcrx-api-0.0.6/dcrx_api/users/models/new_user.py
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-06-09 01:54:04.000000 dcrx-api-0.0.6/dcrx_api/users/models/updated_user.py
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-06-09 01:54:04.000000 dcrx-api-0.0.6/dcrx_api/users/models/user_not_found_exception.py
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-06-09 01:54:04.000000 dcrx-api-0.0.6/dcrx_api/users/models/user_transaction_success_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3888 2023-06-09 01:54:04.000000 dcrx-api-0.0.6/dcrx_api/users/service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 01:54:12.595819 dcrx-api-0.0.6/dcrx_api/users/table/
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-09 01:54:04.000000 dcrx-api-0.0.6/dcrx_api/users/table/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-06-09 01:54:04.000000 dcrx-api-0.0.6/dcrx_api/users/table/table_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     1905 2023-06-09 01:54:04.000000 dcrx-api-0.0.6/dcrx_api/users/table/users_mysql_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-06-09 01:54:04.000000 dcrx-api-0.0.6/dcrx_api/users/table/users_postgres_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     1910 2023-06-09 01:54:04.000000 dcrx-api-0.0.6/dcrx_api/users/table/users_sqllite_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     3247 2023-06-09 01:54:04.000000 dcrx-api-0.0.6/dcrx_api/users/table/users_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-06-09 01:54:04.000000 dcrx-api-0.0.6/dcrx_api/users/users_connection.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 01:54:12.591819 dcrx-api-0.0.6/dcrx_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6101 2023-06-09 01:54:12.000000 dcrx-api-0.0.6/dcrx_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1908 2023-06-09 01:54:12.000000 dcrx-api-0.0.6/dcrx_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 01:54:12.000000 dcrx-api-0.0.6/dcrx_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-09 01:54:12.000000 dcrx-api-0.0.6/dcrx_api.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-09 01:54:12.000000 dcrx-api-0.0.6/dcrx_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-09 01:54:12.000000 dcrx-api-0.0.6/dcrx_api.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-09 01:54:12.599820 dcrx-api-0.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2013 2023-06-09 01:54:04.000000 dcrx-api-0.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 02:03:25.337756 dcrx-api-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-09 02:03:16.000000 dcrx-api-0.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6375 2023-06-09 02:03:25.337756 dcrx-api-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5701 2023-06-09 02:03:16.000000 dcrx-api-0.0.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 02:03:25.329756 dcrx-api-0.0.7/dcrx_api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 02:03:16.000000 dcrx-api-0.0.7/dcrx_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-06-09 02:03:16.000000 dcrx-api-0.0.7/dcrx_api/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 02:03:25.329756 dcrx-api-0.0.7/dcrx_api/auth/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 02:03:16.000000 dcrx-api-0.0.7/dcrx_api/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5557 2023-06-09 02:03:16.000000 dcrx-api-0.0.7/dcrx_api/auth/auth_context.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 02:03:25.329756 dcrx-api-0.0.7/dcrx_api/auth/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-06-09 02:03:16.000000 dcrx-api-0.0.7/dcrx_api/auth/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-09 02:03:16.000000 dcrx-api-0.0.7/dcrx_api/auth/models/auth_claims.py
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-06-09 02:03:16.000000 dcrx-api-0.0.7/dcrx_api/auth/models/auth_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-09 02:03:16.000000 dcrx-api-0.0.7/dcrx_api/auth/models/authentication_failure_exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-06-09 02:03:16.000000 dcrx-api-0.0.7/dcrx_api/auth/models/generated_token.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 02:03:25.329756 dcrx-api-0.0.7/dcrx_api/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-09 02:03:16.000000 dcrx-api-0.0.7/dcrx_api/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-06-09 02:03:16.000000 dcrx-api-0.0.7/dcrx_api/cli/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2640 2023-06-09 02:03:16.000000 dcrx-api-0.0.7/dcrx_api/cli/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-06-09 02:03:16.000000 dcrx-api-0.0.7/dcrx_api/cli/server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 02:03:25.333756 dcrx-api-0.0.7/dcrx_api/database/
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-09 02:03:16.000000 dcrx-api-0.0.7/dcrx_api/database/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3220 2023-06-09 02:03:16.000000 dcrx-api-0.0.7/dcrx_api/database/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-06-09 02:03:16.000000 dcrx-api-0.0.7/dcrx_api/database/connection_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 02:03:25.333756 dcrx-api-0.0.7/dcrx_api/env/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-09 02:03:16.000000 dcrx-api-0.0.7/dcrx_api/env/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-06-09 02:03:16.000000 dcrx-api-0.0.7/dcrx_api/env/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-06-09 02:03:16.000000 dcrx-api-0.0.7/dcrx_api/env/load_env.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 02:03:25.333756 dcrx-api-0.0.7/dcrx_api/jobs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 02:03:16.000000 dcrx-api-0.0.7/dcrx_api/jobs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3417 2023-06-09 02:03:16.000000 dcrx-api-0.0.7/dcrx_api/jobs/job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3348 2023-06-09 02:03:16.000000 dcrx-api-0.0.7/dcrx_api/jobs/job_queue.py
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-09 02:03:16.000000 dcrx-api-0.0.7/dcrx_api/jobs/job_status.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 02:03:25.333756 dcrx-api-0.0.7/dcrx_api/jobs/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-06-09 02:03:16.000000 dcrx-api-0.0.7/dcrx_api/jobs/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-06-09 02:03:16.000000 dcrx-api-0.0.7/dcrx_api/jobs/models/build_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-06-09 02:03:16.000000 dcrx-api-0.0.7/dcrx_api/jobs/models/job_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-06-09 02:03:16.000000 dcrx-api-0.0.7/dcrx_api/jobs/models/job_not_found_exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-06-09 02:03:16.000000 dcrx-api-0.0.7/dcrx_api/jobs/models/new_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-06-09 02:03:16.000000 dcrx-api-0.0.7/dcrx_api/jobs/models/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1646 2023-06-09 02:03:16.000000 dcrx-api-0.0.7/dcrx_api/jobs/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-06-09 02:03:16.000000 dcrx-api-0.0.7/dcrx_api/lifespan.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 02:03:25.333756 dcrx-api-0.0.7/dcrx_api/middleware/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 02:03:16.000000 dcrx-api-0.0.7/dcrx_api/middleware/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-06-09 02:03:16.000000 dcrx-api-0.0.7/dcrx_api/middleware/auth_middleware.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 02:03:25.333756 dcrx-api-0.0.7/dcrx_api/users/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 02:03:16.000000 dcrx-api-0.0.7/dcrx_api/users/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 02:03:25.337756 dcrx-api-0.0.7/dcrx_api/users/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-06-09 02:03:16.000000 dcrx-api-0.0.7/dcrx_api/users/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-06-09 02:03:16.000000 dcrx-api-0.0.7/dcrx_api/users/models/authorized_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-06-09 02:03:16.000000 dcrx-api-0.0.7/dcrx_api/users/models/base_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-06-09 02:03:16.000000 dcrx-api-0.0.7/dcrx_api/users/models/db_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-06-09 02:03:16.000000 dcrx-api-0.0.7/dcrx_api/users/models/login_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-06-09 02:03:16.000000 dcrx-api-0.0.7/dcrx_api/users/models/new_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-06-09 02:03:16.000000 dcrx-api-0.0.7/dcrx_api/users/models/updated_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-06-09 02:03:16.000000 dcrx-api-0.0.7/dcrx_api/users/models/user_not_found_exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-06-09 02:03:16.000000 dcrx-api-0.0.7/dcrx_api/users/models/user_transaction_success_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3888 2023-06-09 02:03:16.000000 dcrx-api-0.0.7/dcrx_api/users/service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 02:03:25.337756 dcrx-api-0.0.7/dcrx_api/users/table/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-09 02:03:16.000000 dcrx-api-0.0.7/dcrx_api/users/table/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-06-09 02:03:16.000000 dcrx-api-0.0.7/dcrx_api/users/table/table_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1905 2023-06-09 02:03:16.000000 dcrx-api-0.0.7/dcrx_api/users/table/users_mysql_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-06-09 02:03:16.000000 dcrx-api-0.0.7/dcrx_api/users/table/users_postgres_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1910 2023-06-09 02:03:16.000000 dcrx-api-0.0.7/dcrx_api/users/table/users_sqllite_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3247 2023-06-09 02:03:16.000000 dcrx-api-0.0.7/dcrx_api/users/table/users_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-06-09 02:03:16.000000 dcrx-api-0.0.7/dcrx_api/users/users_connection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 02:03:25.329756 dcrx-api-0.0.7/dcrx_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6375 2023-06-09 02:03:25.000000 dcrx-api-0.0.7/dcrx_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1908 2023-06-09 02:03:25.000000 dcrx-api-0.0.7/dcrx_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 02:03:25.000000 dcrx-api-0.0.7/dcrx_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-09 02:03:25.000000 dcrx-api-0.0.7/dcrx_api.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-09 02:03:25.000000 dcrx-api-0.0.7/dcrx_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-09 02:03:25.000000 dcrx-api-0.0.7/dcrx_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-09 02:03:25.337756 dcrx-api-0.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2013 2023-06-09 02:03:16.000000 dcrx-api-0.0.7/setup.py
```

### Comparing `dcrx-api-0.0.6/LICENSE` & `dcrx-api-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.0.6/PKG-INFO` & `dcrx-api-0.0.7/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,7 @@
-Metadata-Version: 2.1
-Name: dcrx-api
-Version: 0.0.6
-Summary: A RESTful implementation of the DCRX Docker library.
-Home-page: https://github.com/scorbettUM/dcrx-api
-Author: Sean Corbett
-Author-email: sean.corbett@umontana.edu
-Keywords: pypi,cicd,python,setup,docker,infra,devops,fastapi
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # dcrx-api
 Dcrx-api is a RESTful implementation of the dcrx library, allowing you to create Docker images on request! Dcrx-api extends dcrx, providing integrations with the Docker API and dcrx that allow images to be built by making REST requests.
 
 Dcrx-api also includes basic JWT authorization and user management (no-RBAC), and is intended to be deployed as an internal-facing service. dcrx also provides OpenAPI documentation to make getting started intuitive, and features integrations with SQLite, Postgres, and MySQL for storing and managing users.
 
 
 # Setup and Installation
@@ -58,19 +40,19 @@
 
 DCRX_API_DATABASE_PASSWORD=test1234 # Password used for database connection authentrication
 
 DCRX_API_DATABASE_NAME=dcrx # Name of database to use for storing users. Default is dcrx.
 
 DCRX_API_DATABASE_URI=sqlite+aiosqlite:///dcrx # URL/URI of SQL database for storing users
 
-DOCKER_REGISTRY_URI='https://docker.io/v1/corpheus91/test-images' # Docker image registry to push images to.
+DOCKER_REGISTRY_URI=https://docker.io/v1/myrepo/test-images # Docker image registry to push images to.
 
-DOCKER_REGISTRY_USERNAME='corpheus91' # Username to authenticate Docker pushes to the provided registry.
+DOCKER_REGISTRY_USERNAME=test # Username to authenticate Docker pushes to the provided registry.
 
-DOCKER_REGISTRY_PASSWORD='Goldeneye006*' # Password to authenticate Docker pushes to the provided registry.
+DOCKER_REGISTRY_PASSWORD=test-repo-password # Password to authenticate Docker pushes to the provided registry.
 ```
 
 Prior to starting the server, we recommend seeding the database with an initial user. To do so, run the command:
 
 ```bash
 dcrx-api database initialize --username $USERNAME --password $PASSWORD --first-name $FIRST_NAME --last-name $LAST_NAME --email $EMAIL
 ```
@@ -138,12 +120,22 @@
 ])
 ```
 
 Go ahead and submit the request via the `Execute` button. This will start a job to build the specified image and push it to the repository specified in dcrx-api's environmental variables.
 
 Note that dcrx-api doesn't wait for the image to be built, instead returning a `JobMetadata` response with a status code of `200`, including the `job_id`. Building images is time-intensive and could potentially bog down a server, so dcrx-api builds and pushes images in the background. We can use the `job_id` of a Job to make further `GET` requests to the `/jobs/images/{job_id}/get` endpoint to monitor and check how our job is progressing. If we need to cancel a job for any reason, we can simple make a `DELETE` request to `/jobs/images/{job_id}/cancel`.
 
+
+# Running the Docker Image
+
+To run the Docker image, we recommend first creating a `.env` file with the required environment variables noted above. Then run the image:
+
+```bash
+docker run -p 2277:2277 --env-file .env -v /var/run/docker.sock:/var/run/docker.sock dcrx-api:latest
+```
+
+
 # Notes and Gotchas
 
 1. Does dcrx-api require a volume to run? - Yes. While dcrx-api builds images in-memory, Docker still (frustratingly) requires that a physical file be present in the build directory. This means that, if running dcrx-api in Docker or via Kubernetes, you will need to have a volume with the correct permissions mounted.
 
-2. Does the dcrx-api Docker image require root? - Currently yes. The dcrx-api image is based on the latest version of Docker's `dind` image, which runs as and requires root privlidges. We're working on getting the rootless version of `dind` working though!
+2. Does the dcrx-api Docker image require root? - Currently yes. The dcrx-api image is based on the latest version of Docker's `dind` image, which runs as and requires root privlidges. We're working on getting the rootless version of `dind` working though!
```

### Comparing `dcrx-api-0.0.6/README.md` & `dcrx-api-0.0.7/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,7 +1,25 @@
+Metadata-Version: 2.1
+Name: dcrx-api
+Version: 0.0.7
+Summary: A RESTful implementation of the DCRX Docker library.
+Home-page: https://github.com/scorbettUM/dcrx-api
+Author: Sean Corbett
+Author-email: sean.corbett@umontana.edu
+Keywords: pypi,cicd,python,setup,docker,infra,devops,fastapi
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.10
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # dcrx-api
 Dcrx-api is a RESTful implementation of the dcrx library, allowing you to create Docker images on request! Dcrx-api extends dcrx, providing integrations with the Docker API and dcrx that allow images to be built by making REST requests.
 
 Dcrx-api also includes basic JWT authorization and user management (no-RBAC), and is intended to be deployed as an internal-facing service. dcrx also provides OpenAPI documentation to make getting started intuitive, and features integrations with SQLite, Postgres, and MySQL for storing and managing users.
 
 
 # Setup and Installation
@@ -40,19 +58,19 @@
 
 DCRX_API_DATABASE_PASSWORD=test1234 # Password used for database connection authentrication
 
 DCRX_API_DATABASE_NAME=dcrx # Name of database to use for storing users. Default is dcrx.
 
 DCRX_API_DATABASE_URI=sqlite+aiosqlite:///dcrx # URL/URI of SQL database for storing users
 
-DOCKER_REGISTRY_URI='https://docker.io/v1/corpheus91/test-images' # Docker image registry to push images to.
+DOCKER_REGISTRY_URI=https://docker.io/v1/myrepo/test-images # Docker image registry to push images to.
 
-DOCKER_REGISTRY_USERNAME='corpheus91' # Username to authenticate Docker pushes to the provided registry.
+DOCKER_REGISTRY_USERNAME=test # Username to authenticate Docker pushes to the provided registry.
 
-DOCKER_REGISTRY_PASSWORD='Goldeneye006*' # Password to authenticate Docker pushes to the provided registry.
+DOCKER_REGISTRY_PASSWORD=test-repo-password # Password to authenticate Docker pushes to the provided registry.
 ```
 
 Prior to starting the server, we recommend seeding the database with an initial user. To do so, run the command:
 
 ```bash
 dcrx-api database initialize --username $USERNAME --password $PASSWORD --first-name $FIRST_NAME --last-name $LAST_NAME --email $EMAIL
 ```
@@ -120,12 +138,22 @@
 ])
 ```
 
 Go ahead and submit the request via the `Execute` button. This will start a job to build the specified image and push it to the repository specified in dcrx-api's environmental variables.
 
 Note that dcrx-api doesn't wait for the image to be built, instead returning a `JobMetadata` response with a status code of `200`, including the `job_id`. Building images is time-intensive and could potentially bog down a server, so dcrx-api builds and pushes images in the background. We can use the `job_id` of a Job to make further `GET` requests to the `/jobs/images/{job_id}/get` endpoint to monitor and check how our job is progressing. If we need to cancel a job for any reason, we can simple make a `DELETE` request to `/jobs/images/{job_id}/cancel`.
 
+
+# Running the Docker Image
+
+To run the Docker image, we recommend first creating a `.env` file with the required environment variables noted above. Then run the image:
+
+```bash
+docker run -p 2277:2277 --env-file .env -v /var/run/docker.sock:/var/run/docker.sock dcrx-api:latest
+```
+
+
 # Notes and Gotchas
 
 1. Does dcrx-api require a volume to run? - Yes. While dcrx-api builds images in-memory, Docker still (frustratingly) requires that a physical file be present in the build directory. This means that, if running dcrx-api in Docker or via Kubernetes, you will need to have a volume with the correct permissions mounted.
 
-2. Does the dcrx-api Docker image require root? - Currently yes. The dcrx-api image is based on the latest version of Docker's `dind` image, which runs as and requires root privlidges. We're working on getting the rootless version of `dind` working though!
+2. Does the dcrx-api Docker image require root? - Currently yes. The dcrx-api image is based on the latest version of Docker's `dind` image, which runs as and requires root privlidges. We're working on getting the rootless version of `dind` working though!
```

### Comparing `dcrx-api-0.0.6/dcrx_api/auth/auth_context.py` & `dcrx-api-0.0.7/dcrx_api/auth/auth_context.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.0.6/dcrx_api/cli/base.py` & `dcrx-api-0.0.7/dcrx_api/cli/base.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.0.6/dcrx_api/cli/database.py` & `dcrx-api-0.0.7/dcrx_api/cli/database.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.0.6/dcrx_api/cli/server.py` & `dcrx-api-0.0.7/dcrx_api/cli/server.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.0.6/dcrx_api/database/connection.py` & `dcrx-api-0.0.7/dcrx_api/database/connection.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.0.6/dcrx_api/env/env.py` & `dcrx-api-0.0.7/dcrx_api/env/env.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.0.6/dcrx_api/env/load_env.py` & `dcrx-api-0.0.7/dcrx_api/env/load_env.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.0.6/dcrx_api/jobs/job.py` & `dcrx-api-0.0.7/dcrx_api/jobs/job.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.0.6/dcrx_api/jobs/job_queue.py` & `dcrx-api-0.0.7/dcrx_api/jobs/job_queue.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.0.6/dcrx_api/jobs/models/new_image.py` & `dcrx-api-0.0.7/dcrx_api/jobs/models/new_image.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.0.6/dcrx_api/jobs/service.py` & `dcrx-api-0.0.7/dcrx_api/jobs/service.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.0.6/dcrx_api/lifespan.py` & `dcrx-api-0.0.7/dcrx_api/lifespan.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.0.6/dcrx_api/middleware/auth_middleware.py` & `dcrx-api-0.0.7/dcrx_api/middleware/auth_middleware.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.0.6/dcrx_api/users/service.py` & `dcrx-api-0.0.7/dcrx_api/users/service.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.0.6/dcrx_api/users/table/users_mysql_table.py` & `dcrx-api-0.0.7/dcrx_api/users/table/users_mysql_table.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.0.6/dcrx_api/users/table/users_postgres_table.py` & `dcrx-api-0.0.7/dcrx_api/users/table/users_postgres_table.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.0.6/dcrx_api/users/table/users_sqllite_table.py` & `dcrx-api-0.0.7/dcrx_api/users/table/users_sqllite_table.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.0.6/dcrx_api/users/table/users_table.py` & `dcrx-api-0.0.7/dcrx_api/users/table/users_table.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.0.6/dcrx_api/users/users_connection.py` & `dcrx-api-0.0.7/dcrx_api/users/users_connection.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.0.6/dcrx_api.egg-info/PKG-INFO` & `dcrx-api-0.0.7/dcrx_api.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dcrx-api
-Version: 0.0.6
+Version: 0.0.7
 Summary: A RESTful implementation of the DCRX Docker library.
 Home-page: https://github.com/scorbettUM/dcrx-api
 Author: Sean Corbett
 Author-email: sean.corbett@umontana.edu
 Keywords: pypi,cicd,python,setup,docker,infra,devops,fastapi
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -58,19 +58,19 @@
 
 DCRX_API_DATABASE_PASSWORD=test1234 # Password used for database connection authentrication
 
 DCRX_API_DATABASE_NAME=dcrx # Name of database to use for storing users. Default is dcrx.
 
 DCRX_API_DATABASE_URI=sqlite+aiosqlite:///dcrx # URL/URI of SQL database for storing users
 
-DOCKER_REGISTRY_URI='https://docker.io/v1/corpheus91/test-images' # Docker image registry to push images to.
+DOCKER_REGISTRY_URI=https://docker.io/v1/myrepo/test-images # Docker image registry to push images to.
 
-DOCKER_REGISTRY_USERNAME='corpheus91' # Username to authenticate Docker pushes to the provided registry.
+DOCKER_REGISTRY_USERNAME=test # Username to authenticate Docker pushes to the provided registry.
 
-DOCKER_REGISTRY_PASSWORD='Goldeneye006*' # Password to authenticate Docker pushes to the provided registry.
+DOCKER_REGISTRY_PASSWORD=test-repo-password # Password to authenticate Docker pushes to the provided registry.
 ```
 
 Prior to starting the server, we recommend seeding the database with an initial user. To do so, run the command:
 
 ```bash
 dcrx-api database initialize --username $USERNAME --password $PASSWORD --first-name $FIRST_NAME --last-name $LAST_NAME --email $EMAIL
 ```
@@ -138,12 +138,22 @@
 ])
 ```
 
 Go ahead and submit the request via the `Execute` button. This will start a job to build the specified image and push it to the repository specified in dcrx-api's environmental variables.
 
 Note that dcrx-api doesn't wait for the image to be built, instead returning a `JobMetadata` response with a status code of `200`, including the `job_id`. Building images is time-intensive and could potentially bog down a server, so dcrx-api builds and pushes images in the background. We can use the `job_id` of a Job to make further `GET` requests to the `/jobs/images/{job_id}/get` endpoint to monitor and check how our job is progressing. If we need to cancel a job for any reason, we can simple make a `DELETE` request to `/jobs/images/{job_id}/cancel`.
 
+
+# Running the Docker Image
+
+To run the Docker image, we recommend first creating a `.env` file with the required environment variables noted above. Then run the image:
+
+```bash
+docker run -p 2277:2277 --env-file .env -v /var/run/docker.sock:/var/run/docker.sock dcrx-api:latest
+```
+
+
 # Notes and Gotchas
 
 1. Does dcrx-api require a volume to run? - Yes. While dcrx-api builds images in-memory, Docker still (frustratingly) requires that a physical file be present in the build directory. This means that, if running dcrx-api in Docker or via Kubernetes, you will need to have a volume with the correct permissions mounted.
 
 2. Does the dcrx-api Docker image require root? - Currently yes. The dcrx-api image is based on the latest version of Docker's `dind` image, which runs as and requires root privlidges. We're working on getting the rootless version of `dind` working though!
```

### Comparing `dcrx-api-0.0.6/dcrx_api.egg-info/SOURCES.txt` & `dcrx-api-0.0.7/dcrx_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.0.6/setup.py` & `dcrx-api-0.0.7/setup.py`

 * *Files identical despite different names*

