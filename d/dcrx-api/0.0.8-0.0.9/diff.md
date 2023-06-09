# Comparing `tmp/dcrx-api-0.0.8.tar.gz` & `tmp/dcrx-api-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dcrx-api-0.0.8.tar", last modified: Fri Jun  9 03:09:18 2023, max compression
+gzip compressed data, was "dcrx-api-0.0.9.tar", last modified: Fri Jun  9 03:16:19 2023, max compression
```

## Comparing `dcrx-api-0.0.8.tar` & `dcrx-api-0.0.9.tar`

### file list

```diff
@@ -1,76 +1,76 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 03:09:18.543249 dcrx-api-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-09 03:09:11.000000 dcrx-api-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6380 2023-06-09 03:09:18.543249 dcrx-api-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5706 2023-06-09 03:09:11.000000 dcrx-api-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 03:09:18.535249 dcrx-api-0.0.8/dcrx_api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 03:09:11.000000 dcrx-api-0.0.8/dcrx_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-06-09 03:09:11.000000 dcrx-api-0.0.8/dcrx_api/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 03:09:18.539249 dcrx-api-0.0.8/dcrx_api/auth/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 03:09:11.000000 dcrx-api-0.0.8/dcrx_api/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5557 2023-06-09 03:09:11.000000 dcrx-api-0.0.8/dcrx_api/auth/auth_context.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 03:09:18.539249 dcrx-api-0.0.8/dcrx_api/auth/models/
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-06-09 03:09:11.000000 dcrx-api-0.0.8/dcrx_api/auth/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-09 03:09:11.000000 dcrx-api-0.0.8/dcrx_api/auth/models/auth_claims.py
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-06-09 03:09:11.000000 dcrx-api-0.0.8/dcrx_api/auth/models/auth_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-09 03:09:11.000000 dcrx-api-0.0.8/dcrx_api/auth/models/authentication_failure_exception.py
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-06-09 03:09:11.000000 dcrx-api-0.0.8/dcrx_api/auth/models/generated_token.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 03:09:18.539249 dcrx-api-0.0.8/dcrx_api/cli/
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-09 03:09:11.000000 dcrx-api-0.0.8/dcrx_api/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-06-09 03:09:11.000000 dcrx-api-0.0.8/dcrx_api/cli/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2640 2023-06-09 03:09:11.000000 dcrx-api-0.0.8/dcrx_api/cli/database.py
--rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-06-09 03:09:11.000000 dcrx-api-0.0.8/dcrx_api/cli/server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 03:09:18.539249 dcrx-api-0.0.8/dcrx_api/database/
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-09 03:09:11.000000 dcrx-api-0.0.8/dcrx_api/database/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3220 2023-06-09 03:09:11.000000 dcrx-api-0.0.8/dcrx_api/database/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-06-09 03:09:11.000000 dcrx-api-0.0.8/dcrx_api/database/connection_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 03:09:18.539249 dcrx-api-0.0.8/dcrx_api/env/
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-09 03:09:11.000000 dcrx-api-0.0.8/dcrx_api/env/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-06-09 03:09:11.000000 dcrx-api-0.0.8/dcrx_api/env/env.py
--rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-06-09 03:09:11.000000 dcrx-api-0.0.8/dcrx_api/env/load_env.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 03:09:18.539249 dcrx-api-0.0.8/dcrx_api/jobs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 03:09:11.000000 dcrx-api-0.0.8/dcrx_api/jobs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3417 2023-06-09 03:09:11.000000 dcrx-api-0.0.8/dcrx_api/jobs/job.py
--rw-r--r--   0 runner    (1001) docker     (123)     3348 2023-06-09 03:09:11.000000 dcrx-api-0.0.8/dcrx_api/jobs/job_queue.py
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-09 03:09:11.000000 dcrx-api-0.0.8/dcrx_api/jobs/job_status.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 03:09:18.543249 dcrx-api-0.0.8/dcrx_api/jobs/models/
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-06-09 03:09:11.000000 dcrx-api-0.0.8/dcrx_api/jobs/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-06-09 03:09:11.000000 dcrx-api-0.0.8/dcrx_api/jobs/models/build_options.py
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-06-09 03:09:11.000000 dcrx-api-0.0.8/dcrx_api/jobs/models/job_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-06-09 03:09:11.000000 dcrx-api-0.0.8/dcrx_api/jobs/models/job_not_found_exception.py
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-06-09 03:09:11.000000 dcrx-api-0.0.8/dcrx_api/jobs/models/new_image.py
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-06-09 03:09:11.000000 dcrx-api-0.0.8/dcrx_api/jobs/models/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     1646 2023-06-09 03:09:11.000000 dcrx-api-0.0.8/dcrx_api/jobs/service.py
--rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-06-09 03:09:11.000000 dcrx-api-0.0.8/dcrx_api/lifespan.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 03:09:18.543249 dcrx-api-0.0.8/dcrx_api/middleware/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 03:09:11.000000 dcrx-api-0.0.8/dcrx_api/middleware/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-06-09 03:09:11.000000 dcrx-api-0.0.8/dcrx_api/middleware/auth_middleware.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 03:09:18.543249 dcrx-api-0.0.8/dcrx_api/users/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 03:09:11.000000 dcrx-api-0.0.8/dcrx_api/users/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 03:09:18.543249 dcrx-api-0.0.8/dcrx_api/users/models/
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-06-09 03:09:11.000000 dcrx-api-0.0.8/dcrx_api/users/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-06-09 03:09:11.000000 dcrx-api-0.0.8/dcrx_api/users/models/authorized_user.py
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-06-09 03:09:11.000000 dcrx-api-0.0.8/dcrx_api/users/models/base_user.py
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-06-09 03:09:11.000000 dcrx-api-0.0.8/dcrx_api/users/models/db_user.py
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-06-09 03:09:11.000000 dcrx-api-0.0.8/dcrx_api/users/models/login_user.py
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-06-09 03:09:11.000000 dcrx-api-0.0.8/dcrx_api/users/models/new_user.py
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-06-09 03:09:11.000000 dcrx-api-0.0.8/dcrx_api/users/models/updated_user.py
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-06-09 03:09:11.000000 dcrx-api-0.0.8/dcrx_api/users/models/user_not_found_exception.py
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-06-09 03:09:11.000000 dcrx-api-0.0.8/dcrx_api/users/models/user_transaction_success_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3888 2023-06-09 03:09:11.000000 dcrx-api-0.0.8/dcrx_api/users/service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 03:09:18.543249 dcrx-api-0.0.8/dcrx_api/users/table/
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-09 03:09:11.000000 dcrx-api-0.0.8/dcrx_api/users/table/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-06-09 03:09:11.000000 dcrx-api-0.0.8/dcrx_api/users/table/table_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     1905 2023-06-09 03:09:11.000000 dcrx-api-0.0.8/dcrx_api/users/table/users_mysql_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-06-09 03:09:11.000000 dcrx-api-0.0.8/dcrx_api/users/table/users_postgres_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     1910 2023-06-09 03:09:11.000000 dcrx-api-0.0.8/dcrx_api/users/table/users_sqllite_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     3247 2023-06-09 03:09:11.000000 dcrx-api-0.0.8/dcrx_api/users/table/users_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-06-09 03:09:11.000000 dcrx-api-0.0.8/dcrx_api/users/users_connection.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 03:09:18.539249 dcrx-api-0.0.8/dcrx_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6380 2023-06-09 03:09:18.000000 dcrx-api-0.0.8/dcrx_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1908 2023-06-09 03:09:18.000000 dcrx-api-0.0.8/dcrx_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 03:09:18.000000 dcrx-api-0.0.8/dcrx_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-09 03:09:18.000000 dcrx-api-0.0.8/dcrx_api.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-09 03:09:18.000000 dcrx-api-0.0.8/dcrx_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-09 03:09:18.000000 dcrx-api-0.0.8/dcrx_api.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-09 03:09:18.543249 dcrx-api-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2013 2023-06-09 03:09:11.000000 dcrx-api-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 03:16:19.624742 dcrx-api-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-09 03:16:14.000000 dcrx-api-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6890 2023-06-09 03:16:19.624742 dcrx-api-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6216 2023-06-09 03:16:14.000000 dcrx-api-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 03:16:19.620742 dcrx-api-0.0.9/dcrx_api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 03:16:14.000000 dcrx-api-0.0.9/dcrx_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-06-09 03:16:14.000000 dcrx-api-0.0.9/dcrx_api/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 03:16:19.620742 dcrx-api-0.0.9/dcrx_api/auth/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 03:16:14.000000 dcrx-api-0.0.9/dcrx_api/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5557 2023-06-09 03:16:14.000000 dcrx-api-0.0.9/dcrx_api/auth/auth_context.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 03:16:19.620742 dcrx-api-0.0.9/dcrx_api/auth/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-06-09 03:16:14.000000 dcrx-api-0.0.9/dcrx_api/auth/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-09 03:16:14.000000 dcrx-api-0.0.9/dcrx_api/auth/models/auth_claims.py
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-06-09 03:16:14.000000 dcrx-api-0.0.9/dcrx_api/auth/models/auth_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-09 03:16:14.000000 dcrx-api-0.0.9/dcrx_api/auth/models/authentication_failure_exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-06-09 03:16:14.000000 dcrx-api-0.0.9/dcrx_api/auth/models/generated_token.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 03:16:19.620742 dcrx-api-0.0.9/dcrx_api/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-09 03:16:14.000000 dcrx-api-0.0.9/dcrx_api/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-06-09 03:16:14.000000 dcrx-api-0.0.9/dcrx_api/cli/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2640 2023-06-09 03:16:14.000000 dcrx-api-0.0.9/dcrx_api/cli/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-06-09 03:16:14.000000 dcrx-api-0.0.9/dcrx_api/cli/server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 03:16:19.620742 dcrx-api-0.0.9/dcrx_api/database/
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-09 03:16:14.000000 dcrx-api-0.0.9/dcrx_api/database/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3220 2023-06-09 03:16:14.000000 dcrx-api-0.0.9/dcrx_api/database/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-06-09 03:16:14.000000 dcrx-api-0.0.9/dcrx_api/database/connection_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 03:16:19.624742 dcrx-api-0.0.9/dcrx_api/env/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-09 03:16:14.000000 dcrx-api-0.0.9/dcrx_api/env/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-06-09 03:16:14.000000 dcrx-api-0.0.9/dcrx_api/env/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-06-09 03:16:14.000000 dcrx-api-0.0.9/dcrx_api/env/load_env.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 03:16:19.624742 dcrx-api-0.0.9/dcrx_api/jobs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 03:16:14.000000 dcrx-api-0.0.9/dcrx_api/jobs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3417 2023-06-09 03:16:14.000000 dcrx-api-0.0.9/dcrx_api/jobs/job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3348 2023-06-09 03:16:14.000000 dcrx-api-0.0.9/dcrx_api/jobs/job_queue.py
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-09 03:16:14.000000 dcrx-api-0.0.9/dcrx_api/jobs/job_status.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 03:16:19.624742 dcrx-api-0.0.9/dcrx_api/jobs/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-06-09 03:16:14.000000 dcrx-api-0.0.9/dcrx_api/jobs/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-06-09 03:16:14.000000 dcrx-api-0.0.9/dcrx_api/jobs/models/build_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-06-09 03:16:14.000000 dcrx-api-0.0.9/dcrx_api/jobs/models/job_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-06-09 03:16:14.000000 dcrx-api-0.0.9/dcrx_api/jobs/models/job_not_found_exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-06-09 03:16:14.000000 dcrx-api-0.0.9/dcrx_api/jobs/models/new_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-06-09 03:16:14.000000 dcrx-api-0.0.9/dcrx_api/jobs/models/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1646 2023-06-09 03:16:14.000000 dcrx-api-0.0.9/dcrx_api/jobs/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-06-09 03:16:14.000000 dcrx-api-0.0.9/dcrx_api/lifespan.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 03:16:19.624742 dcrx-api-0.0.9/dcrx_api/middleware/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 03:16:14.000000 dcrx-api-0.0.9/dcrx_api/middleware/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-06-09 03:16:14.000000 dcrx-api-0.0.9/dcrx_api/middleware/auth_middleware.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 03:16:19.624742 dcrx-api-0.0.9/dcrx_api/users/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 03:16:14.000000 dcrx-api-0.0.9/dcrx_api/users/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 03:16:19.624742 dcrx-api-0.0.9/dcrx_api/users/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-06-09 03:16:14.000000 dcrx-api-0.0.9/dcrx_api/users/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-06-09 03:16:14.000000 dcrx-api-0.0.9/dcrx_api/users/models/authorized_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-06-09 03:16:14.000000 dcrx-api-0.0.9/dcrx_api/users/models/base_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-06-09 03:16:14.000000 dcrx-api-0.0.9/dcrx_api/users/models/db_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-06-09 03:16:14.000000 dcrx-api-0.0.9/dcrx_api/users/models/login_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-06-09 03:16:14.000000 dcrx-api-0.0.9/dcrx_api/users/models/new_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-06-09 03:16:14.000000 dcrx-api-0.0.9/dcrx_api/users/models/updated_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-06-09 03:16:14.000000 dcrx-api-0.0.9/dcrx_api/users/models/user_not_found_exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-06-09 03:16:14.000000 dcrx-api-0.0.9/dcrx_api/users/models/user_transaction_success_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3888 2023-06-09 03:16:14.000000 dcrx-api-0.0.9/dcrx_api/users/service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 03:16:19.624742 dcrx-api-0.0.9/dcrx_api/users/table/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-09 03:16:14.000000 dcrx-api-0.0.9/dcrx_api/users/table/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-06-09 03:16:14.000000 dcrx-api-0.0.9/dcrx_api/users/table/table_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1905 2023-06-09 03:16:14.000000 dcrx-api-0.0.9/dcrx_api/users/table/users_mysql_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-06-09 03:16:14.000000 dcrx-api-0.0.9/dcrx_api/users/table/users_postgres_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1910 2023-06-09 03:16:14.000000 dcrx-api-0.0.9/dcrx_api/users/table/users_sqllite_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3247 2023-06-09 03:16:14.000000 dcrx-api-0.0.9/dcrx_api/users/table/users_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-06-09 03:16:14.000000 dcrx-api-0.0.9/dcrx_api/users/users_connection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 03:16:19.620742 dcrx-api-0.0.9/dcrx_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6890 2023-06-09 03:16:19.000000 dcrx-api-0.0.9/dcrx_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1908 2023-06-09 03:16:19.000000 dcrx-api-0.0.9/dcrx_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 03:16:19.000000 dcrx-api-0.0.9/dcrx_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-09 03:16:19.000000 dcrx-api-0.0.9/dcrx_api.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-09 03:16:19.000000 dcrx-api-0.0.9/dcrx_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-09 03:16:19.000000 dcrx-api-0.0.9/dcrx_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-09 03:16:19.624742 dcrx-api-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2013 2023-06-09 03:16:14.000000 dcrx-api-0.0.9/setup.py
```

### Comparing `dcrx-api-0.0.8/LICENSE` & `dcrx-api-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.0.8/PKG-INFO` & `dcrx-api-0.0.9/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,26 +1,13 @@
-Metadata-Version: 2.1
-Name: dcrx-api
-Version: 0.0.8
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
+[![PyPI version](https://img.shields.io/pypi/v/dcrx-api?color=gre)](https://pypi.org/project/dcrx-api/)
+[![License](https://img.shields.io/github/license/scorbettUM/dcrx-api)](https://github.com/scorbettUM/dcrx-api/blob/main/LICENSE)
+[![Contributor Covenant](https://img.shields.io/badge/Contributor%20Covenant-2.1-4baaaa.svg)](https://github.com/scorbettUM/dcrx-api/blob/main/CODE_OF_CONDUCT.md)
+[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/dcrx-api)](https://pypi.org/project/dcrx-api/)
+
 Dcrx-api is a RESTful implementation of the dcrx library, allowing you to create Docker images on request! Dcrx-api extends dcrx, providing integrations with the Docker API and dcrx that allow images to be built by making REST requests.
 
 Dcrx-api also includes basic JWT authorization and user management (no-RBAC), and is intended to be deployed as an internal-facing service. dcrx also provides OpenAPI documentation to make getting started intuitive, and features integrations with SQLite, Postgres, and MySQL for storing and managing users.
 
 
 # Setup and Installation
 
@@ -152,8 +139,8 @@
 ```
 
 
 # Notes and Gotchas
 
 1. Does dcrx-api require a volume to run? - Yes. While dcrx-api builds images in-memory, Docker still (frustratingly) requires that a physical file be present in the build directory. This means that, if running dcrx-api in Docker or via Kubernetes, you will need to have a volume with the correct permissions mounted.
 
-2. Does the dcrx-api Docker image require root? - Currently yes. The dcrx-api image is based on the latest version of Docker's `dind` image, which runs as and requires root privlidges. We're working on getting the rootless version of `dind` working though!
+2. Does the dcrx-api Docker image require root? - Currently yes. The dcrx-api image is based on the latest version of Docker's `dind` image, which runs as and requires root privlidges. We're working on getting the rootless version of `dind` working though!
```

### Comparing `dcrx-api-0.0.8/README.md` & `dcrx-api-0.0.9/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,8 +1,31 @@
+Metadata-Version: 2.1
+Name: dcrx-api
+Version: 0.0.9
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
+[![PyPI version](https://img.shields.io/pypi/v/dcrx-api?color=gre)](https://pypi.org/project/dcrx-api/)
+[![License](https://img.shields.io/github/license/scorbettUM/dcrx-api)](https://github.com/scorbettUM/dcrx-api/blob/main/LICENSE)
+[![Contributor Covenant](https://img.shields.io/badge/Contributor%20Covenant-2.1-4baaaa.svg)](https://github.com/scorbettUM/dcrx-api/blob/main/CODE_OF_CONDUCT.md)
+[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/dcrx-api)](https://pypi.org/project/dcrx-api/)
+
 Dcrx-api is a RESTful implementation of the dcrx library, allowing you to create Docker images on request! Dcrx-api extends dcrx, providing integrations with the Docker API and dcrx that allow images to be built by making REST requests.
 
 Dcrx-api also includes basic JWT authorization and user management (no-RBAC), and is intended to be deployed as an internal-facing service. dcrx also provides OpenAPI documentation to make getting started intuitive, and features integrations with SQLite, Postgres, and MySQL for storing and managing users.
 
 
 # Setup and Installation
 
@@ -134,8 +157,8 @@
 ```
 
 
 # Notes and Gotchas
 
 1. Does dcrx-api require a volume to run? - Yes. While dcrx-api builds images in-memory, Docker still (frustratingly) requires that a physical file be present in the build directory. This means that, if running dcrx-api in Docker or via Kubernetes, you will need to have a volume with the correct permissions mounted.
 
-2. Does the dcrx-api Docker image require root? - Currently yes. The dcrx-api image is based on the latest version of Docker's `dind` image, which runs as and requires root privlidges. We're working on getting the rootless version of `dind` working though!
+2. Does the dcrx-api Docker image require root? - Currently yes. The dcrx-api image is based on the latest version of Docker's `dind` image, which runs as and requires root privlidges. We're working on getting the rootless version of `dind` working though!
```

### Comparing `dcrx-api-0.0.8/dcrx_api/auth/auth_context.py` & `dcrx-api-0.0.9/dcrx_api/auth/auth_context.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.0.8/dcrx_api/cli/base.py` & `dcrx-api-0.0.9/dcrx_api/cli/base.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.0.8/dcrx_api/cli/database.py` & `dcrx-api-0.0.9/dcrx_api/cli/database.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.0.8/dcrx_api/cli/server.py` & `dcrx-api-0.0.9/dcrx_api/cli/server.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.0.8/dcrx_api/database/connection.py` & `dcrx-api-0.0.9/dcrx_api/database/connection.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.0.8/dcrx_api/env/env.py` & `dcrx-api-0.0.9/dcrx_api/env/env.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.0.8/dcrx_api/env/load_env.py` & `dcrx-api-0.0.9/dcrx_api/env/load_env.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.0.8/dcrx_api/jobs/job.py` & `dcrx-api-0.0.9/dcrx_api/jobs/job.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.0.8/dcrx_api/jobs/job_queue.py` & `dcrx-api-0.0.9/dcrx_api/jobs/job_queue.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.0.8/dcrx_api/jobs/models/new_image.py` & `dcrx-api-0.0.9/dcrx_api/jobs/models/new_image.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.0.8/dcrx_api/jobs/service.py` & `dcrx-api-0.0.9/dcrx_api/jobs/service.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.0.8/dcrx_api/lifespan.py` & `dcrx-api-0.0.9/dcrx_api/lifespan.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.0.8/dcrx_api/middleware/auth_middleware.py` & `dcrx-api-0.0.9/dcrx_api/middleware/auth_middleware.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.0.8/dcrx_api/users/service.py` & `dcrx-api-0.0.9/dcrx_api/users/service.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.0.8/dcrx_api/users/table/users_mysql_table.py` & `dcrx-api-0.0.9/dcrx_api/users/table/users_mysql_table.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.0.8/dcrx_api/users/table/users_postgres_table.py` & `dcrx-api-0.0.9/dcrx_api/users/table/users_postgres_table.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.0.8/dcrx_api/users/table/users_sqllite_table.py` & `dcrx-api-0.0.9/dcrx_api/users/table/users_sqllite_table.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.0.8/dcrx_api/users/table/users_table.py` & `dcrx-api-0.0.9/dcrx_api/users/table/users_table.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.0.8/dcrx_api/users/users_connection.py` & `dcrx-api-0.0.9/dcrx_api/users/users_connection.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.0.8/dcrx_api.egg-info/PKG-INFO` & `dcrx-api-0.0.9/dcrx_api.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dcrx-api
-Version: 0.0.8
+Version: 0.0.9
 Summary: A RESTful implementation of the DCRX Docker library.
 Home-page: https://github.com/scorbettUM/dcrx-api
 Author: Sean Corbett
 Author-email: sean.corbett@umontana.edu
 Keywords: pypi,cicd,python,setup,docker,infra,devops,fastapi
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -13,14 +13,19 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # dcrx-api
+[![PyPI version](https://img.shields.io/pypi/v/dcrx-api?color=gre)](https://pypi.org/project/dcrx-api/)
+[![License](https://img.shields.io/github/license/scorbettUM/dcrx-api)](https://github.com/scorbettUM/dcrx-api/blob/main/LICENSE)
+[![Contributor Covenant](https://img.shields.io/badge/Contributor%20Covenant-2.1-4baaaa.svg)](https://github.com/scorbettUM/dcrx-api/blob/main/CODE_OF_CONDUCT.md)
+[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/dcrx-api)](https://pypi.org/project/dcrx-api/)
+
 Dcrx-api is a RESTful implementation of the dcrx library, allowing you to create Docker images on request! Dcrx-api extends dcrx, providing integrations with the Docker API and dcrx that allow images to be built by making REST requests.
 
 Dcrx-api also includes basic JWT authorization and user management (no-RBAC), and is intended to be deployed as an internal-facing service. dcrx also provides OpenAPI documentation to make getting started intuitive, and features integrations with SQLite, Postgres, and MySQL for storing and managing users.
 
 
 # Setup and Installation
```

### Comparing `dcrx-api-0.0.8/dcrx_api.egg-info/SOURCES.txt` & `dcrx-api-0.0.9/dcrx_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.0.8/setup.py` & `dcrx-api-0.0.9/setup.py`

 * *Files identical despite different names*

