# Comparing `tmp/dcrx-api-0.0.5.tar.gz` & `tmp/dcrx-api-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dcrx-api-0.0.5.tar", last modified: Fri Jun  9 01:13:49 2023, max compression
+gzip compressed data, was "dcrx-api-0.0.6.tar", last modified: Fri Jun  9 01:54:12 2023, max compression
```

## Comparing `dcrx-api-0.0.5.tar` & `dcrx-api-0.0.6.tar`

### file list

```diff
@@ -1,76 +1,76 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 01:13:49.487390 dcrx-api-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-09 01:13:44.000000 dcrx-api-0.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6101 2023-06-09 01:13:49.487390 dcrx-api-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5427 2023-06-09 01:13:44.000000 dcrx-api-0.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 01:13:49.479390 dcrx-api-0.0.5/dcrx_api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 01:13:44.000000 dcrx-api-0.0.5/dcrx_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-06-09 01:13:44.000000 dcrx-api-0.0.5/dcrx_api/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 01:13:49.479390 dcrx-api-0.0.5/dcrx_api/auth/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 01:13:44.000000 dcrx-api-0.0.5/dcrx_api/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5557 2023-06-09 01:13:44.000000 dcrx-api-0.0.5/dcrx_api/auth/auth_context.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 01:13:49.479390 dcrx-api-0.0.5/dcrx_api/auth/models/
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-06-09 01:13:44.000000 dcrx-api-0.0.5/dcrx_api/auth/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-09 01:13:44.000000 dcrx-api-0.0.5/dcrx_api/auth/models/auth_claims.py
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-06-09 01:13:44.000000 dcrx-api-0.0.5/dcrx_api/auth/models/auth_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-09 01:13:44.000000 dcrx-api-0.0.5/dcrx_api/auth/models/authentication_failure_exception.py
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-06-09 01:13:44.000000 dcrx-api-0.0.5/dcrx_api/auth/models/generated_token.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 01:13:49.479390 dcrx-api-0.0.5/dcrx_api/cli/
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-09 01:13:44.000000 dcrx-api-0.0.5/dcrx_api/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-06-09 01:13:44.000000 dcrx-api-0.0.5/dcrx_api/cli/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2640 2023-06-09 01:13:44.000000 dcrx-api-0.0.5/dcrx_api/cli/database.py
--rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-06-09 01:13:44.000000 dcrx-api-0.0.5/dcrx_api/cli/server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 01:13:49.479390 dcrx-api-0.0.5/dcrx_api/database/
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-09 01:13:44.000000 dcrx-api-0.0.5/dcrx_api/database/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3220 2023-06-09 01:13:44.000000 dcrx-api-0.0.5/dcrx_api/database/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-06-09 01:13:44.000000 dcrx-api-0.0.5/dcrx_api/database/connection_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 01:13:49.479390 dcrx-api-0.0.5/dcrx_api/env/
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-09 01:13:44.000000 dcrx-api-0.0.5/dcrx_api/env/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-06-09 01:13:44.000000 dcrx-api-0.0.5/dcrx_api/env/env.py
--rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-06-09 01:13:44.000000 dcrx-api-0.0.5/dcrx_api/env/load_env.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 01:13:49.483390 dcrx-api-0.0.5/dcrx_api/jobs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 01:13:44.000000 dcrx-api-0.0.5/dcrx_api/jobs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3471 2023-06-09 01:13:44.000000 dcrx-api-0.0.5/dcrx_api/jobs/job.py
--rw-r--r--   0 runner    (1001) docker     (123)     3348 2023-06-09 01:13:44.000000 dcrx-api-0.0.5/dcrx_api/jobs/job_queue.py
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-09 01:13:44.000000 dcrx-api-0.0.5/dcrx_api/jobs/job_status.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 01:13:49.483390 dcrx-api-0.0.5/dcrx_api/jobs/models/
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-06-09 01:13:44.000000 dcrx-api-0.0.5/dcrx_api/jobs/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-06-09 01:13:44.000000 dcrx-api-0.0.5/dcrx_api/jobs/models/build_options.py
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-06-09 01:13:44.000000 dcrx-api-0.0.5/dcrx_api/jobs/models/job_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-06-09 01:13:44.000000 dcrx-api-0.0.5/dcrx_api/jobs/models/job_not_found_exception.py
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-06-09 01:13:44.000000 dcrx-api-0.0.5/dcrx_api/jobs/models/new_image.py
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-06-09 01:13:44.000000 dcrx-api-0.0.5/dcrx_api/jobs/models/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     1646 2023-06-09 01:13:44.000000 dcrx-api-0.0.5/dcrx_api/jobs/service.py
--rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-06-09 01:13:44.000000 dcrx-api-0.0.5/dcrx_api/lifespan.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 01:13:49.483390 dcrx-api-0.0.5/dcrx_api/middleware/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 01:13:44.000000 dcrx-api-0.0.5/dcrx_api/middleware/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-06-09 01:13:44.000000 dcrx-api-0.0.5/dcrx_api/middleware/auth_middleware.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 01:13:49.483390 dcrx-api-0.0.5/dcrx_api/users/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 01:13:44.000000 dcrx-api-0.0.5/dcrx_api/users/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 01:13:49.483390 dcrx-api-0.0.5/dcrx_api/users/models/
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-06-09 01:13:44.000000 dcrx-api-0.0.5/dcrx_api/users/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-06-09 01:13:44.000000 dcrx-api-0.0.5/dcrx_api/users/models/authorized_user.py
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-06-09 01:13:44.000000 dcrx-api-0.0.5/dcrx_api/users/models/base_user.py
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-06-09 01:13:44.000000 dcrx-api-0.0.5/dcrx_api/users/models/db_user.py
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-06-09 01:13:44.000000 dcrx-api-0.0.5/dcrx_api/users/models/login_user.py
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-06-09 01:13:44.000000 dcrx-api-0.0.5/dcrx_api/users/models/new_user.py
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-06-09 01:13:44.000000 dcrx-api-0.0.5/dcrx_api/users/models/updated_user.py
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-06-09 01:13:44.000000 dcrx-api-0.0.5/dcrx_api/users/models/user_not_found_exception.py
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-06-09 01:13:44.000000 dcrx-api-0.0.5/dcrx_api/users/models/user_transaction_success_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3888 2023-06-09 01:13:44.000000 dcrx-api-0.0.5/dcrx_api/users/service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 01:13:49.483390 dcrx-api-0.0.5/dcrx_api/users/table/
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-09 01:13:44.000000 dcrx-api-0.0.5/dcrx_api/users/table/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-06-09 01:13:44.000000 dcrx-api-0.0.5/dcrx_api/users/table/table_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     1905 2023-06-09 01:13:44.000000 dcrx-api-0.0.5/dcrx_api/users/table/users_mysql_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-06-09 01:13:44.000000 dcrx-api-0.0.5/dcrx_api/users/table/users_postgres_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     1910 2023-06-09 01:13:44.000000 dcrx-api-0.0.5/dcrx_api/users/table/users_sqllite_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     3247 2023-06-09 01:13:44.000000 dcrx-api-0.0.5/dcrx_api/users/table/users_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-06-09 01:13:44.000000 dcrx-api-0.0.5/dcrx_api/users/users_connection.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 01:13:49.479390 dcrx-api-0.0.5/dcrx_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6101 2023-06-09 01:13:49.000000 dcrx-api-0.0.5/dcrx_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1908 2023-06-09 01:13:49.000000 dcrx-api-0.0.5/dcrx_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 01:13:49.000000 dcrx-api-0.0.5/dcrx_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-09 01:13:49.000000 dcrx-api-0.0.5/dcrx_api.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-09 01:13:49.000000 dcrx-api-0.0.5/dcrx_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-09 01:13:49.000000 dcrx-api-0.0.5/dcrx_api.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-09 01:13:49.487390 dcrx-api-0.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2013 2023-06-09 01:13:44.000000 dcrx-api-0.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 01:54:12.599820 dcrx-api-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-09 01:54:04.000000 dcrx-api-0.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6101 2023-06-09 01:54:12.595819 dcrx-api-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5427 2023-06-09 01:54:04.000000 dcrx-api-0.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 01:54:12.587819 dcrx-api-0.0.6/dcrx_api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 01:54:04.000000 dcrx-api-0.0.6/dcrx_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-06-09 01:54:04.000000 dcrx-api-0.0.6/dcrx_api/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 01:54:12.591819 dcrx-api-0.0.6/dcrx_api/auth/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 01:54:04.000000 dcrx-api-0.0.6/dcrx_api/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5557 2023-06-09 01:54:04.000000 dcrx-api-0.0.6/dcrx_api/auth/auth_context.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 01:54:12.591819 dcrx-api-0.0.6/dcrx_api/auth/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-06-09 01:54:04.000000 dcrx-api-0.0.6/dcrx_api/auth/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-09 01:54:04.000000 dcrx-api-0.0.6/dcrx_api/auth/models/auth_claims.py
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-06-09 01:54:04.000000 dcrx-api-0.0.6/dcrx_api/auth/models/auth_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-09 01:54:04.000000 dcrx-api-0.0.6/dcrx_api/auth/models/authentication_failure_exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-06-09 01:54:04.000000 dcrx-api-0.0.6/dcrx_api/auth/models/generated_token.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 01:54:12.591819 dcrx-api-0.0.6/dcrx_api/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-09 01:54:04.000000 dcrx-api-0.0.6/dcrx_api/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-06-09 01:54:04.000000 dcrx-api-0.0.6/dcrx_api/cli/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2640 2023-06-09 01:54:04.000000 dcrx-api-0.0.6/dcrx_api/cli/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-06-09 01:54:04.000000 dcrx-api-0.0.6/dcrx_api/cli/server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 01:54:12.591819 dcrx-api-0.0.6/dcrx_api/database/
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-09 01:54:04.000000 dcrx-api-0.0.6/dcrx_api/database/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3220 2023-06-09 01:54:04.000000 dcrx-api-0.0.6/dcrx_api/database/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-06-09 01:54:04.000000 dcrx-api-0.0.6/dcrx_api/database/connection_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 01:54:12.595819 dcrx-api-0.0.6/dcrx_api/env/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-09 01:54:04.000000 dcrx-api-0.0.6/dcrx_api/env/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-06-09 01:54:04.000000 dcrx-api-0.0.6/dcrx_api/env/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-06-09 01:54:04.000000 dcrx-api-0.0.6/dcrx_api/env/load_env.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 01:54:12.595819 dcrx-api-0.0.6/dcrx_api/jobs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 01:54:04.000000 dcrx-api-0.0.6/dcrx_api/jobs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3417 2023-06-09 01:54:04.000000 dcrx-api-0.0.6/dcrx_api/jobs/job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3348 2023-06-09 01:54:04.000000 dcrx-api-0.0.6/dcrx_api/jobs/job_queue.py
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-09 01:54:04.000000 dcrx-api-0.0.6/dcrx_api/jobs/job_status.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 01:54:12.595819 dcrx-api-0.0.6/dcrx_api/jobs/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-06-09 01:54:04.000000 dcrx-api-0.0.6/dcrx_api/jobs/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-06-09 01:54:04.000000 dcrx-api-0.0.6/dcrx_api/jobs/models/build_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-06-09 01:54:04.000000 dcrx-api-0.0.6/dcrx_api/jobs/models/job_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-06-09 01:54:04.000000 dcrx-api-0.0.6/dcrx_api/jobs/models/job_not_found_exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-06-09 01:54:04.000000 dcrx-api-0.0.6/dcrx_api/jobs/models/new_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-06-09 01:54:04.000000 dcrx-api-0.0.6/dcrx_api/jobs/models/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1646 2023-06-09 01:54:04.000000 dcrx-api-0.0.6/dcrx_api/jobs/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-06-09 01:54:04.000000 dcrx-api-0.0.6/dcrx_api/lifespan.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 01:54:12.595819 dcrx-api-0.0.6/dcrx_api/middleware/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 01:54:04.000000 dcrx-api-0.0.6/dcrx_api/middleware/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-06-09 01:54:04.000000 dcrx-api-0.0.6/dcrx_api/middleware/auth_middleware.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 01:54:12.595819 dcrx-api-0.0.6/dcrx_api/users/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 01:54:04.000000 dcrx-api-0.0.6/dcrx_api/users/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 01:54:12.595819 dcrx-api-0.0.6/dcrx_api/users/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-06-09 01:54:04.000000 dcrx-api-0.0.6/dcrx_api/users/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-06-09 01:54:04.000000 dcrx-api-0.0.6/dcrx_api/users/models/authorized_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-06-09 01:54:04.000000 dcrx-api-0.0.6/dcrx_api/users/models/base_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-06-09 01:54:04.000000 dcrx-api-0.0.6/dcrx_api/users/models/db_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-06-09 01:54:04.000000 dcrx-api-0.0.6/dcrx_api/users/models/login_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-06-09 01:54:04.000000 dcrx-api-0.0.6/dcrx_api/users/models/new_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-06-09 01:54:04.000000 dcrx-api-0.0.6/dcrx_api/users/models/updated_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-06-09 01:54:04.000000 dcrx-api-0.0.6/dcrx_api/users/models/user_not_found_exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-06-09 01:54:04.000000 dcrx-api-0.0.6/dcrx_api/users/models/user_transaction_success_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3888 2023-06-09 01:54:04.000000 dcrx-api-0.0.6/dcrx_api/users/service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 01:54:12.595819 dcrx-api-0.0.6/dcrx_api/users/table/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-09 01:54:04.000000 dcrx-api-0.0.6/dcrx_api/users/table/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-06-09 01:54:04.000000 dcrx-api-0.0.6/dcrx_api/users/table/table_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1905 2023-06-09 01:54:04.000000 dcrx-api-0.0.6/dcrx_api/users/table/users_mysql_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-06-09 01:54:04.000000 dcrx-api-0.0.6/dcrx_api/users/table/users_postgres_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1910 2023-06-09 01:54:04.000000 dcrx-api-0.0.6/dcrx_api/users/table/users_sqllite_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3247 2023-06-09 01:54:04.000000 dcrx-api-0.0.6/dcrx_api/users/table/users_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-06-09 01:54:04.000000 dcrx-api-0.0.6/dcrx_api/users/users_connection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 01:54:12.591819 dcrx-api-0.0.6/dcrx_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6101 2023-06-09 01:54:12.000000 dcrx-api-0.0.6/dcrx_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1908 2023-06-09 01:54:12.000000 dcrx-api-0.0.6/dcrx_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 01:54:12.000000 dcrx-api-0.0.6/dcrx_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-09 01:54:12.000000 dcrx-api-0.0.6/dcrx_api.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-09 01:54:12.000000 dcrx-api-0.0.6/dcrx_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-09 01:54:12.000000 dcrx-api-0.0.6/dcrx_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-09 01:54:12.599820 dcrx-api-0.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2013 2023-06-09 01:54:04.000000 dcrx-api-0.0.6/setup.py
```

### Comparing `dcrx-api-0.0.5/LICENSE` & `dcrx-api-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.0.5/PKG-INFO` & `dcrx-api-0.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dcrx-api
-Version: 0.0.5
+Version: 0.0.6
 Summary: A RESTful implementation of the DCRX Docker library.
 Home-page: https://github.com/scorbettUM/dcrx-api
 Author: Sean Corbett
 Author-email: sean.corbett@umontana.edu
 Keywords: pypi,cicd,python,setup,docker,infra,devops,fastapi
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `dcrx-api-0.0.5/README.md` & `dcrx-api-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.0.5/dcrx_api/auth/auth_context.py` & `dcrx-api-0.0.6/dcrx_api/auth/auth_context.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.0.5/dcrx_api/cli/base.py` & `dcrx-api-0.0.6/dcrx_api/cli/base.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.0.5/dcrx_api/cli/database.py` & `dcrx-api-0.0.6/dcrx_api/cli/database.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.0.5/dcrx_api/cli/server.py` & `dcrx-api-0.0.6/dcrx_api/cli/server.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.0.5/dcrx_api/database/connection.py` & `dcrx-api-0.0.6/dcrx_api/database/connection.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.0.5/dcrx_api/env/env.py` & `dcrx-api-0.0.6/dcrx_api/env/env.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.0.5/dcrx_api/env/load_env.py` & `dcrx-api-0.0.6/dcrx_api/env/load_env.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.0.5/dcrx_api/jobs/job.py` & `dcrx-api-0.0.6/dcrx_api/jobs/job.py`

 * *Files 8% similar despite different names*

```diff
@@ -33,15 +33,14 @@
         self.job_name = image.full_name
 
         self.image = image
         self.registry = registry
         self.build_options = build_options
 
         self.client = docker.DockerClient(
-            base_url=registry.registry_password,
             max_pool_size=pool_size,
         )
 
         self.context: Union[MemoryFile, None] = None
         self._executor = ThreadPoolExecutor(max_workers=pool_size)
         self.loop = asyncio.get_event_loop()
         self.status = JobStatus.CREATED
@@ -60,14 +59,15 @@
 
         await self.clear()
         await self.close()
 
     async def login_to_registry(self):
 
         self.status = JobStatus.AUTHORIZING
+
         await self.loop.run_in_executor(
             self._executor,
             functools.partial(
                 self.client.api.login,
                 self.registry.registry_user,
                 password=self.registry.registry_password,
                 registry=self.registry.registry_uri,
@@ -93,15 +93,15 @@
 
         if self.build_options:
             build_options = self.build_options.dict()
 
         await self.loop.run_in_executor(
             self._executor,
             functools.partial(
-                self.client.images.build,
+                self.client.api.build,
                 dockerfile=self.image.filename,
                 fileobj=self.context,
                 tag=self.image.full_name,
                 custom_context=True,
                 **build_options
             )   
         )
@@ -109,15 +109,15 @@
     async def push_image(self):
 
         self.status = JobStatus.PUSHING
 
         await self.loop.run_in_executor(
             self._executor,
             functools.partial(
-                self.client.images.push,
+                self.client.api.push,
                 self.image.name,
                 tag=self.image.tag
             )
         )
 
     async def clear(self):
         await self.loop.run_in_executor(
```

### Comparing `dcrx-api-0.0.5/dcrx_api/jobs/job_queue.py` & `dcrx-api-0.0.6/dcrx_api/jobs/job_queue.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.0.5/dcrx_api/jobs/models/new_image.py` & `dcrx-api-0.0.6/dcrx_api/jobs/models/new_image.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.0.5/dcrx_api/jobs/service.py` & `dcrx-api-0.0.6/dcrx_api/jobs/service.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.0.5/dcrx_api/lifespan.py` & `dcrx-api-0.0.6/dcrx_api/lifespan.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.0.5/dcrx_api/middleware/auth_middleware.py` & `dcrx-api-0.0.6/dcrx_api/middleware/auth_middleware.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.0.5/dcrx_api/users/service.py` & `dcrx-api-0.0.6/dcrx_api/users/service.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.0.5/dcrx_api/users/table/users_mysql_table.py` & `dcrx-api-0.0.6/dcrx_api/users/table/users_mysql_table.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.0.5/dcrx_api/users/table/users_postgres_table.py` & `dcrx-api-0.0.6/dcrx_api/users/table/users_postgres_table.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.0.5/dcrx_api/users/table/users_sqllite_table.py` & `dcrx-api-0.0.6/dcrx_api/users/table/users_sqllite_table.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.0.5/dcrx_api/users/table/users_table.py` & `dcrx-api-0.0.6/dcrx_api/users/table/users_table.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.0.5/dcrx_api/users/users_connection.py` & `dcrx-api-0.0.6/dcrx_api/users/users_connection.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.0.5/dcrx_api.egg-info/PKG-INFO` & `dcrx-api-0.0.6/dcrx_api.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dcrx-api
-Version: 0.0.5
+Version: 0.0.6
 Summary: A RESTful implementation of the DCRX Docker library.
 Home-page: https://github.com/scorbettUM/dcrx-api
 Author: Sean Corbett
 Author-email: sean.corbett@umontana.edu
 Keywords: pypi,cicd,python,setup,docker,infra,devops,fastapi
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `dcrx-api-0.0.5/dcrx_api.egg-info/SOURCES.txt` & `dcrx-api-0.0.6/dcrx_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.0.5/setup.py` & `dcrx-api-0.0.6/setup.py`

 * *Files identical despite different names*

