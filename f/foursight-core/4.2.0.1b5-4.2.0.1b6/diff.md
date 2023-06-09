# Comparing `tmp/foursight_core-4.2.0.1b5.tar.gz` & `tmp/foursight_core-4.2.0.1b6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "foursight_core-4.2.0.1b5.tar", max compression
+gzip compressed data, was "foursight_core-4.2.0.1b6.tar", max compression
```

## Comparing `foursight_core-4.2.0.1b5.tar` & `foursight_core-4.2.0.1b6.tar`

### file list

```diff
@@ -1,77 +1,77 @@
--rw-r--r--   0        0        0     1083 2023-06-08 17:29:21.521993 foursight_core-4.2.0.1b5/LICENSE.txt
--rw-r--r--   0        0        0        0 2023-06-08 17:29:21.526873 foursight_core-4.2.0.1b5/foursight_core/__init__.py
--rw-r--r--   0        0        0     1901 2023-06-08 17:29:21.526949 foursight_core-4.2.0.1b5/foursight_core/abstract_connection.py
--rw-r--r--   0        0        0       69 2023-06-08 17:29:21.527000 foursight_core-4.2.0.1b5/foursight_core/app.py
--rw-r--r--   0        0        0   105128 2023-06-08 17:29:21.527440 foursight_core-4.2.0.1b5/foursight_core/app_utils.py
--rw-r--r--   0        0        0     2571 2023-06-08 17:29:21.527526 foursight_core-4.2.0.1b5/foursight_core/buckets.py
--rw-r--r--   0        0        0      638 2023-06-08 17:29:21.527588 foursight_core-4.2.0.1b5/foursight_core/check_schema.py
--rw-r--r--   0        0        0        3 2023-06-08 17:29:21.527638 foursight_core-4.2.0.1b5/foursight_core/check_setup.json
--rw-r--r--   0        0        0    22858 2023-06-08 17:29:21.527760 foursight_core-4.2.0.1b5/foursight_core/check_utils.py
--rw-r--r--   0        0        0      270 2023-06-08 17:29:21.527854 foursight_core-4.2.0.1b5/foursight_core/checks/__init__.py
--rw-r--r--   0        0        0     4476 2023-06-08 17:29:21.527928 foursight_core-4.2.0.1b5/foursight_core/checks/access_key_expiration_detection.py
--rw-r--r--   0        0        0     2899 2023-06-08 17:29:21.527988 foursight_core-4.2.0.1b5/foursight_core/checks/codebuild_checks.py
--rw-r--r--   0        0        0     3305 2023-06-08 17:29:21.528055 foursight_core-4.2.0.1b5/foursight_core/checks/ecs_checks.py
--rw-r--r--   0        0        0     4683 2023-06-08 17:29:21.528131 foursight_core-4.2.0.1b5/foursight_core/checks/ecs_recovery_check.py
--rw-r--r--   0        0        0        0 2023-06-08 17:29:21.528189 foursight_core-4.2.0.1b5/foursight_core/checks/helpers/__init__.py
--rw-r--r--   0        0        0      348 2023-06-08 17:29:21.528252 foursight_core-4.2.0.1b5/foursight_core/checks/helpers/confchecks.py
--rw-r--r--   0        0        0     3519 2023-06-08 17:29:21.528315 foursight_core-4.2.0.1b5/foursight_core/checks/helpers/sys_utils.py
--rw-r--r--   0        0        0     2055 2023-06-08 17:29:21.528380 foursight_core-4.2.0.1b5/foursight_core/checks/helpers/wrangler_utils.py
--rw-r--r--   0        0        0     8375 2023-06-08 17:29:21.528450 foursight_core-4.2.0.1b5/foursight_core/checks/scaling_checks.py
--rw-r--r--   0        0        0     2658 2023-06-08 17:29:21.528510 foursight_core-4.2.0.1b5/foursight_core/checks/test_checks.py
--rw-r--r--   0        0        0    11929 2023-06-08 17:29:21.528602 foursight_core-4.2.0.1b5/foursight_core/decorators.py
--rw-r--r--   0        0        0    15050 2023-06-08 17:29:21.528695 foursight_core-4.2.0.1b5/foursight_core/deploy.py
--rw-r--r--   0        0        0     8302 2023-06-08 17:29:21.528782 foursight_core-4.2.0.1b5/foursight_core/environment.py
--rw-r--r--   0        0        0    11792 2023-06-08 17:29:21.528862 foursight_core-4.2.0.1b5/foursight_core/es_connection.py
--rw-r--r--   0        0        0     1176 2023-06-08 17:29:21.529002 foursight_core-4.2.0.1b5/foursight_core/exceptions.py
--rw-r--r--   0        0        0     5215 2023-06-08 17:29:28.845472 foursight_core-4.2.0.1b5/foursight_core/fs_connection.py
--rw-r--r--   0        0        0     8423 2023-06-08 17:29:21.529157 foursight_core-4.2.0.1b5/foursight_core/identity.py
--rw-r--r--   0        0        0     3082 2023-06-08 17:29:21.529223 foursight_core-4.2.0.1b5/foursight_core/mapping.json
--rw-r--r--   0        0        0     1014 2023-06-08 17:29:21.529277 foursight_core-4.2.0.1b5/foursight_core/package.py
--rw-r--r--   0        0        0    16912 2023-06-08 17:29:21.529456 foursight_core-4.2.0.1b5/foursight_core/react/api/auth.py
--rw-r--r--   0        0        0     6629 2023-06-08 17:29:21.529548 foursight_core-4.2.0.1b5/foursight_core/react/api/auth0_config.py
--rw-r--r--   0        0        0    22994 2023-06-08 17:29:21.529665 foursight_core-4.2.0.1b5/foursight_core/react/api/aws_network.py
--rw-r--r--   0        0        0     3038 2023-06-08 17:29:21.529880 foursight_core-4.2.0.1b5/foursight_core/react/api/aws_s3.py
--rw-r--r--   0        0        0     6116 2023-06-08 17:29:21.529963 foursight_core-4.2.0.1b5/foursight_core/react/api/aws_stacks.py
--rw-r--r--   0        0        0    28009 2023-06-08 17:29:21.530084 foursight_core-4.2.0.1b5/foursight_core/react/api/checks.py
--rw-r--r--   0        0        0    20464 2023-06-08 17:29:21.530276 foursight_core-4.2.0.1b5/foursight_core/react/api/cognito.py
--rw-r--r--   0        0        0     3952 2023-06-08 17:29:21.530400 foursight_core-4.2.0.1b5/foursight_core/react/api/cookie_utils.py
--rw-r--r--   0        0        0     6189 2023-06-08 17:29:21.530486 foursight_core-4.2.0.1b5/foursight_core/react/api/datetime_utils.py
--rw-r--r--   0        0        0     1841 2023-06-08 17:29:21.530563 foursight_core-4.2.0.1b5/foursight_core/react/api/encoding_utils.py
--rw-r--r--   0        0        0     3649 2023-06-08 17:29:21.530634 foursight_core-4.2.0.1b5/foursight_core/react/api/encryption.py
--rw-r--r--   0        0        0     4720 2023-06-08 17:29:21.530710 foursight_core-4.2.0.1b5/foursight_core/react/api/envs.py
--rw-r--r--   0        0        0     3196 2023-06-08 17:29:21.530775 foursight_core-4.2.0.1b5/foursight_core/react/api/gac.py
--rw-r--r--   0        0        0     3516 2023-06-08 17:29:21.530838 foursight_core-4.2.0.1b5/foursight_core/react/api/jwt_utils.py
--rw-r--r--   0        0        0     9466 2023-06-08 17:29:21.530928 foursight_core-4.2.0.1b5/foursight_core/react/api/misc_utils.py
--rw-r--r--   0        0        0     5164 2023-06-08 17:29:21.531018 foursight_core-4.2.0.1b5/foursight_core/react/api/portal_access_key_utils.py
--rw-r--r--   0        0        0    80447 2023-06-08 17:29:28.846043 foursight_core-4.2.0.1b5/foursight_core/react/api/react_api.py
--rw-r--r--   0        0        0    11210 2023-06-08 17:29:21.531406 foursight_core-4.2.0.1b5/foursight_core/react/api/react_api_base.py
--rw-r--r--   0        0        0     8025 2023-06-08 17:29:21.531496 foursight_core-4.2.0.1b5/foursight_core/react/api/react_route_decorator.py
--rw-r--r--   0        0        0    34216 2023-06-08 17:29:28.846377 foursight_core-4.2.0.1b5/foursight_core/react/api/react_routes.py
--rw-r--r--   0        0        0     4805 2023-06-08 17:29:21.531697 foursight_core-4.2.0.1b5/foursight_core/react/api/react_ui.py
--rw-r--r--   0        0        0      806 2023-06-08 17:29:21.531762 foursight_core-4.2.0.1b5/foursight_core/react/api/yaml_utils.py
--rw-r--r--   0        0        0      234 2023-06-08 17:29:21.531853 foursight_core-4.2.0.1b5/foursight_core/react/ui/asset-manifest.json
--rw-r--r--   0        0        0     1681 2023-06-08 17:29:21.531916 foursight_core-4.2.0.1b5/foursight_core/react/ui/index.html
--rw-r--r--   0        0        0        3 2023-06-08 17:29:21.531964 foursight_core-4.2.0.1b5/foursight_core/react/ui/manifest.json
--rw-r--r--   0        0        0    11735 2023-06-08 17:29:21.532567 foursight_core-4.2.0.1b5/foursight_core/react/ui/static/css/main.css
--rw-r--r--   0        0        0  1934060 2023-06-08 17:29:28.862200 foursight_core-4.2.0.1b5/foursight_core/react/ui/static/js/main.js
--rw-r--r--   0        0        0      597 2023-06-08 17:29:21.541812 foursight_core-4.2.0.1b5/foursight_core/route_prefixes.py
--rw-r--r--   0        0        0    10496 2023-06-08 17:29:21.541900 foursight_core-4.2.0.1b5/foursight_core/routes.py
--rw-r--r--   0        0        0    22442 2023-06-08 17:29:21.541974 foursight_core-4.2.0.1b5/foursight_core/run_result.py
--rw-r--r--   0        0        0     6330 2023-06-08 17:29:21.542064 foursight_core-4.2.0.1b5/foursight_core/s3_connection.py
--rw-r--r--   0        0        0     5282 2023-06-08 17:29:21.542130 foursight_core-4.2.0.1b5/foursight_core/schedule_decorator.py
--rw-r--r--   0        0        0     1402 2023-06-08 17:29:21.542227 foursight_core-4.2.0.1b5/foursight_core/scripts/decrypt_accounts_file.py
--rw-r--r--   0        0        0     1406 2023-06-08 17:29:21.542277 foursight_core-4.2.0.1b5/foursight_core/scripts/encrypt_accounts_file.py
--rw-r--r--   0        0        0     5370 2023-06-08 17:29:21.542349 foursight_core-4.2.0.1b5/foursight_core/sqs_utils.py
--rw-r--r--   0        0        0     1715 2023-06-08 17:29:21.542414 foursight_core-4.2.0.1b5/foursight_core/stage.py
--rw-r--r--   0        0        0     7763 2023-06-08 17:29:21.542590 foursight_core-4.2.0.1b5/foursight_core/templates/base.html
--rw-r--r--   0        0        0    20532 2023-06-08 17:29:21.542697 foursight_core-4.2.0.1b5/foursight_core/templates/header.html
--rw-r--r--   0        0        0     4090 2023-06-08 17:29:21.542772 foursight_core-4.2.0.1b5/foursight_core/templates/history.html
--rw-r--r--   0        0        0    19634 2023-06-08 17:29:21.542860 foursight_core-4.2.0.1b5/foursight_core/templates/info.html
--rw-r--r--   0        0        0     1297 2023-06-08 17:29:21.542929 foursight_core-4.2.0.1b5/foursight_core/templates/unused.html
--rw-r--r--   0        0        0     2259 2023-06-08 17:29:21.542988 foursight_core-4.2.0.1b5/foursight_core/templates/user.html
--rw-r--r--   0        0        0     1669 2023-06-08 17:29:21.543055 foursight_core-4.2.0.1b5/foursight_core/templates/users.html
--rw-r--r--   0        0        0      572 2023-06-08 17:29:21.543139 foursight_core-4.2.0.1b5/foursight_core/templates/view_checks.html
--rw-r--r--   0        0        0     2248 2023-06-08 17:29:21.543191 foursight_core-4.2.0.1b5/foursight_core/templates/view_groups.html
--rw-r--r--   0        0        0     1627 2023-06-08 17:30:11.806677 foursight_core-4.2.0.1b5/pyproject.toml
--rw-r--r--   0        0        0     1950 1970-01-01 00:00:00.000000 foursight_core-4.2.0.1b5/setup.py
--rw-r--r--   0        0        0     1200 1970-01-01 00:00:00.000000 foursight_core-4.2.0.1b5/PKG-INFO
+-rw-r--r--   0        0        0     1083 2023-06-08 17:29:21.521993 foursight_core-4.2.0.1b6/LICENSE.txt
+-rw-r--r--   0        0        0        0 2023-06-08 17:29:21.526873 foursight_core-4.2.0.1b6/foursight_core/__init__.py
+-rw-r--r--   0        0        0     1901 2023-06-08 17:29:21.526949 foursight_core-4.2.0.1b6/foursight_core/abstract_connection.py
+-rw-r--r--   0        0        0       69 2023-06-08 17:29:21.527000 foursight_core-4.2.0.1b6/foursight_core/app.py
+-rw-r--r--   0        0        0   105128 2023-06-08 17:29:21.527440 foursight_core-4.2.0.1b6/foursight_core/app_utils.py
+-rw-r--r--   0        0        0     2571 2023-06-08 17:29:21.527526 foursight_core-4.2.0.1b6/foursight_core/buckets.py
+-rw-r--r--   0        0        0      638 2023-06-08 17:29:21.527588 foursight_core-4.2.0.1b6/foursight_core/check_schema.py
+-rw-r--r--   0        0        0        3 2023-06-08 17:29:21.527638 foursight_core-4.2.0.1b6/foursight_core/check_setup.json
+-rw-r--r--   0        0        0    22858 2023-06-08 17:29:21.527760 foursight_core-4.2.0.1b6/foursight_core/check_utils.py
+-rw-r--r--   0        0        0      270 2023-06-08 17:29:21.527854 foursight_core-4.2.0.1b6/foursight_core/checks/__init__.py
+-rw-r--r--   0        0        0     4476 2023-06-08 17:29:21.527928 foursight_core-4.2.0.1b6/foursight_core/checks/access_key_expiration_detection.py
+-rw-r--r--   0        0        0     2899 2023-06-08 17:29:21.527988 foursight_core-4.2.0.1b6/foursight_core/checks/codebuild_checks.py
+-rw-r--r--   0        0        0     3305 2023-06-08 17:29:21.528055 foursight_core-4.2.0.1b6/foursight_core/checks/ecs_checks.py
+-rw-r--r--   0        0        0     4683 2023-06-08 17:29:21.528131 foursight_core-4.2.0.1b6/foursight_core/checks/ecs_recovery_check.py
+-rw-r--r--   0        0        0        0 2023-06-08 17:29:21.528189 foursight_core-4.2.0.1b6/foursight_core/checks/helpers/__init__.py
+-rw-r--r--   0        0        0      348 2023-06-08 17:29:21.528252 foursight_core-4.2.0.1b6/foursight_core/checks/helpers/confchecks.py
+-rw-r--r--   0        0        0     3519 2023-06-08 17:29:21.528315 foursight_core-4.2.0.1b6/foursight_core/checks/helpers/sys_utils.py
+-rw-r--r--   0        0        0     2055 2023-06-08 17:29:21.528380 foursight_core-4.2.0.1b6/foursight_core/checks/helpers/wrangler_utils.py
+-rw-r--r--   0        0        0     8375 2023-06-08 17:29:21.528450 foursight_core-4.2.0.1b6/foursight_core/checks/scaling_checks.py
+-rw-r--r--   0        0        0     2658 2023-06-08 17:29:21.528510 foursight_core-4.2.0.1b6/foursight_core/checks/test_checks.py
+-rw-r--r--   0        0        0    11929 2023-06-08 17:29:21.528602 foursight_core-4.2.0.1b6/foursight_core/decorators.py
+-rw-r--r--   0        0        0    15050 2023-06-08 17:29:21.528695 foursight_core-4.2.0.1b6/foursight_core/deploy.py
+-rw-r--r--   0        0        0     8302 2023-06-08 17:29:21.528782 foursight_core-4.2.0.1b6/foursight_core/environment.py
+-rw-r--r--   0        0        0    11792 2023-06-08 17:29:21.528862 foursight_core-4.2.0.1b6/foursight_core/es_connection.py
+-rw-r--r--   0        0        0     1176 2023-06-08 17:29:21.529002 foursight_core-4.2.0.1b6/foursight_core/exceptions.py
+-rw-r--r--   0        0        0     5408 2023-06-09 17:22:22.577742 foursight_core-4.2.0.1b6/foursight_core/fs_connection.py
+-rw-r--r--   0        0        0     8423 2023-06-08 17:29:21.529157 foursight_core-4.2.0.1b6/foursight_core/identity.py
+-rw-r--r--   0        0        0     3082 2023-06-08 17:29:21.529223 foursight_core-4.2.0.1b6/foursight_core/mapping.json
+-rw-r--r--   0        0        0     1014 2023-06-08 17:29:21.529277 foursight_core-4.2.0.1b6/foursight_core/package.py
+-rw-r--r--   0        0        0    16912 2023-06-08 17:29:21.529456 foursight_core-4.2.0.1b6/foursight_core/react/api/auth.py
+-rw-r--r--   0        0        0     6629 2023-06-08 17:29:21.529548 foursight_core-4.2.0.1b6/foursight_core/react/api/auth0_config.py
+-rw-r--r--   0        0        0    22994 2023-06-08 17:29:21.529665 foursight_core-4.2.0.1b6/foursight_core/react/api/aws_network.py
+-rw-r--r--   0        0        0     3038 2023-06-08 17:29:21.529880 foursight_core-4.2.0.1b6/foursight_core/react/api/aws_s3.py
+-rw-r--r--   0        0        0     6116 2023-06-08 17:29:21.529963 foursight_core-4.2.0.1b6/foursight_core/react/api/aws_stacks.py
+-rw-r--r--   0        0        0    28009 2023-06-08 17:29:21.530084 foursight_core-4.2.0.1b6/foursight_core/react/api/checks.py
+-rw-r--r--   0        0        0    20464 2023-06-08 17:29:21.530276 foursight_core-4.2.0.1b6/foursight_core/react/api/cognito.py
+-rw-r--r--   0        0        0     3952 2023-06-08 17:29:21.530400 foursight_core-4.2.0.1b6/foursight_core/react/api/cookie_utils.py
+-rw-r--r--   0        0        0     6189 2023-06-08 17:29:21.530486 foursight_core-4.2.0.1b6/foursight_core/react/api/datetime_utils.py
+-rw-r--r--   0        0        0     1841 2023-06-08 17:29:21.530563 foursight_core-4.2.0.1b6/foursight_core/react/api/encoding_utils.py
+-rw-r--r--   0        0        0     3649 2023-06-08 17:29:21.530634 foursight_core-4.2.0.1b6/foursight_core/react/api/encryption.py
+-rw-r--r--   0        0        0     4720 2023-06-08 17:29:21.530710 foursight_core-4.2.0.1b6/foursight_core/react/api/envs.py
+-rw-r--r--   0        0        0     3196 2023-06-08 17:29:21.530775 foursight_core-4.2.0.1b6/foursight_core/react/api/gac.py
+-rw-r--r--   0        0        0     3516 2023-06-08 17:29:21.530838 foursight_core-4.2.0.1b6/foursight_core/react/api/jwt_utils.py
+-rw-r--r--   0        0        0     9466 2023-06-08 17:29:21.530928 foursight_core-4.2.0.1b6/foursight_core/react/api/misc_utils.py
+-rw-r--r--   0        0        0     5164 2023-06-08 17:29:21.531018 foursight_core-4.2.0.1b6/foursight_core/react/api/portal_access_key_utils.py
+-rw-r--r--   0        0        0    80660 2023-06-09 17:22:22.578116 foursight_core-4.2.0.1b6/foursight_core/react/api/react_api.py
+-rw-r--r--   0        0        0    11210 2023-06-08 17:29:21.531406 foursight_core-4.2.0.1b6/foursight_core/react/api/react_api_base.py
+-rw-r--r--   0        0        0     8025 2023-06-08 17:29:21.531496 foursight_core-4.2.0.1b6/foursight_core/react/api/react_route_decorator.py
+-rw-r--r--   0        0        0    34216 2023-06-08 17:29:28.846377 foursight_core-4.2.0.1b6/foursight_core/react/api/react_routes.py
+-rw-r--r--   0        0        0     4805 2023-06-08 17:29:21.531697 foursight_core-4.2.0.1b6/foursight_core/react/api/react_ui.py
+-rw-r--r--   0        0        0      806 2023-06-08 17:29:21.531762 foursight_core-4.2.0.1b6/foursight_core/react/api/yaml_utils.py
+-rw-r--r--   0        0        0      234 2023-06-08 17:29:21.531853 foursight_core-4.2.0.1b6/foursight_core/react/ui/asset-manifest.json
+-rw-r--r--   0        0        0     1681 2023-06-08 17:29:21.531916 foursight_core-4.2.0.1b6/foursight_core/react/ui/index.html
+-rw-r--r--   0        0        0        3 2023-06-08 17:29:21.531964 foursight_core-4.2.0.1b6/foursight_core/react/ui/manifest.json
+-rw-r--r--   0        0        0    11735 2023-06-08 17:29:21.532567 foursight_core-4.2.0.1b6/foursight_core/react/ui/static/css/main.css
+-rw-r--r--   0        0        0  1935185 2023-06-09 17:22:22.585038 foursight_core-4.2.0.1b6/foursight_core/react/ui/static/js/main.js
+-rw-r--r--   0        0        0      597 2023-06-08 17:29:21.541812 foursight_core-4.2.0.1b6/foursight_core/route_prefixes.py
+-rw-r--r--   0        0        0    10496 2023-06-08 17:29:21.541900 foursight_core-4.2.0.1b6/foursight_core/routes.py
+-rw-r--r--   0        0        0    22442 2023-06-08 17:29:21.541974 foursight_core-4.2.0.1b6/foursight_core/run_result.py
+-rw-r--r--   0        0        0     6330 2023-06-08 17:29:21.542064 foursight_core-4.2.0.1b6/foursight_core/s3_connection.py
+-rw-r--r--   0        0        0     5282 2023-06-08 17:29:21.542130 foursight_core-4.2.0.1b6/foursight_core/schedule_decorator.py
+-rw-r--r--   0        0        0     1402 2023-06-08 17:29:21.542227 foursight_core-4.2.0.1b6/foursight_core/scripts/decrypt_accounts_file.py
+-rw-r--r--   0        0        0     1406 2023-06-08 17:29:21.542277 foursight_core-4.2.0.1b6/foursight_core/scripts/encrypt_accounts_file.py
+-rw-r--r--   0        0        0     5370 2023-06-08 17:29:21.542349 foursight_core-4.2.0.1b6/foursight_core/sqs_utils.py
+-rw-r--r--   0        0        0     1715 2023-06-08 17:29:21.542414 foursight_core-4.2.0.1b6/foursight_core/stage.py
+-rw-r--r--   0        0        0     7763 2023-06-08 17:29:21.542590 foursight_core-4.2.0.1b6/foursight_core/templates/base.html
+-rw-r--r--   0        0        0    20532 2023-06-08 17:29:21.542697 foursight_core-4.2.0.1b6/foursight_core/templates/header.html
+-rw-r--r--   0        0        0     4090 2023-06-08 17:29:21.542772 foursight_core-4.2.0.1b6/foursight_core/templates/history.html
+-rw-r--r--   0        0        0    19634 2023-06-08 17:29:21.542860 foursight_core-4.2.0.1b6/foursight_core/templates/info.html
+-rw-r--r--   0        0        0     1297 2023-06-08 17:29:21.542929 foursight_core-4.2.0.1b6/foursight_core/templates/unused.html
+-rw-r--r--   0        0        0     2259 2023-06-08 17:29:21.542988 foursight_core-4.2.0.1b6/foursight_core/templates/user.html
+-rw-r--r--   0        0        0     1669 2023-06-08 17:29:21.543055 foursight_core-4.2.0.1b6/foursight_core/templates/users.html
+-rw-r--r--   0        0        0      572 2023-06-08 17:29:21.543139 foursight_core-4.2.0.1b6/foursight_core/templates/view_checks.html
+-rw-r--r--   0        0        0     2248 2023-06-08 17:29:21.543191 foursight_core-4.2.0.1b6/foursight_core/templates/view_groups.html
+-rw-r--r--   0        0        0     1627 2023-06-09 17:22:22.585934 foursight_core-4.2.0.1b6/pyproject.toml
+-rw-r--r--   0        0        0     1950 1970-01-01 00:00:00.000000 foursight_core-4.2.0.1b6/setup.py
+-rw-r--r--   0        0        0     1200 1970-01-01 00:00:00.000000 foursight_core-4.2.0.1b6/PKG-INFO
```

### Comparing `foursight_core-4.2.0.1b5/LICENSE.txt` & `foursight_core-4.2.0.1b6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `foursight_core-4.2.0.1b5/foursight_core/abstract_connection.py` & `foursight_core-4.2.0.1b6/foursight_core/abstract_connection.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.2.0.1b5/foursight_core/app_utils.py` & `foursight_core-4.2.0.1b6/foursight_core/app_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.2.0.1b5/foursight_core/buckets.py` & `foursight_core-4.2.0.1b6/foursight_core/buckets.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.2.0.1b5/foursight_core/check_schema.py` & `foursight_core-4.2.0.1b6/foursight_core/check_schema.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.2.0.1b5/foursight_core/check_utils.py` & `foursight_core-4.2.0.1b6/foursight_core/check_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.2.0.1b5/foursight_core/checks/access_key_expiration_detection.py` & `foursight_core-4.2.0.1b6/foursight_core/checks/access_key_expiration_detection.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.2.0.1b5/foursight_core/checks/codebuild_checks.py` & `foursight_core-4.2.0.1b6/foursight_core/checks/codebuild_checks.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.2.0.1b5/foursight_core/checks/ecs_checks.py` & `foursight_core-4.2.0.1b6/foursight_core/checks/ecs_checks.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.2.0.1b5/foursight_core/checks/ecs_recovery_check.py` & `foursight_core-4.2.0.1b6/foursight_core/checks/ecs_recovery_check.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.2.0.1b5/foursight_core/checks/helpers/sys_utils.py` & `foursight_core-4.2.0.1b6/foursight_core/checks/helpers/sys_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.2.0.1b5/foursight_core/checks/helpers/wrangler_utils.py` & `foursight_core-4.2.0.1b6/foursight_core/checks/helpers/wrangler_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.2.0.1b5/foursight_core/checks/scaling_checks.py` & `foursight_core-4.2.0.1b6/foursight_core/checks/scaling_checks.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.2.0.1b5/foursight_core/checks/test_checks.py` & `foursight_core-4.2.0.1b6/foursight_core/checks/test_checks.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.2.0.1b5/foursight_core/decorators.py` & `foursight_core-4.2.0.1b6/foursight_core/decorators.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.2.0.1b5/foursight_core/deploy.py` & `foursight_core-4.2.0.1b6/foursight_core/deploy.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.2.0.1b5/foursight_core/environment.py` & `foursight_core-4.2.0.1b6/foursight_core/environment.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.2.0.1b5/foursight_core/es_connection.py` & `foursight_core-4.2.0.1b6/foursight_core/es_connection.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.2.0.1b5/foursight_core/exceptions.py` & `foursight_core-4.2.0.1b6/foursight_core/exceptions.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.2.0.1b5/foursight_core/fs_connection.py` & `foursight_core-4.2.0.1b6/foursight_core/fs_connection.py`

 * *Files 3% similar despite different names*

```diff
@@ -47,23 +47,28 @@
         self.ff_es = fs_environ_info['es']
         self.ff_bucket = fs_environ_info['bucket']
         self.redis = None
         self.redis_url = None
         try:
             if 'redis' in fs_environ_info:
                 self.redis_url = fs_environ_info['redis']
-                self.redis = RedisBase(create_redis_client(url=self.redis_url))
             elif 'REDIS_HOST' in os.environ:  # temporary patch in until env config is fully sorted - Will
                 self.redis_url = os.environ['REDIS_HOST']
+            if self.redis_url:
                 self.redis = RedisBase(create_redis_client(url=self.redis_url))
+            else:
+                PRINT("Redis URL was not specified in any way so running without Redis.")
         except redis.exceptions.ConnectionError:
-            PRINT('Cannot connect to Redis')
-            PRINT('This error is expected when deploying with remote (ElastiCache) Redis')
-        PRINT(self.redis)
-        PRINT(self.redis_url)
+            PRINT(f"Cannot connect to Redis ({self.redis_url}); but can run without it so continuing.")
+            self.redis = None
+            self.redis_url = None
+        if self.redis:
+            PRINT(f"Redis server is being used: {self.redis_url}")
+        else:
+            PRINT(f"Redis server is not being used.")
         if not test:
             self.ff_s3 = s3Utils(env=self.ff_env)
             try:  # TODO: make this configurable from env variables?
                 self.ff_keys = self.ff_s3.get_access_keys('access_key_foursight')
             except Exception as e:
                 raise Exception('Could not initiate connection to Fourfront; it is probably a bad ff_env. '
                       'You gave: %s. Error message: %s' % (self.ff_env, str(e)))
```

### Comparing `foursight_core-4.2.0.1b5/foursight_core/identity.py` & `foursight_core-4.2.0.1b6/foursight_core/identity.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.2.0.1b5/foursight_core/mapping.json` & `foursight_core-4.2.0.1b6/foursight_core/mapping.json`

 * *Files identical despite different names*

### Comparing `foursight_core-4.2.0.1b5/foursight_core/package.py` & `foursight_core-4.2.0.1b6/foursight_core/package.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.2.0.1b5/foursight_core/react/api/auth.py` & `foursight_core-4.2.0.1b6/foursight_core/react/api/auth.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.2.0.1b5/foursight_core/react/api/auth0_config.py` & `foursight_core-4.2.0.1b6/foursight_core/react/api/auth0_config.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.2.0.1b5/foursight_core/react/api/aws_network.py` & `foursight_core-4.2.0.1b6/foursight_core/react/api/aws_network.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.2.0.1b5/foursight_core/react/api/aws_s3.py` & `foursight_core-4.2.0.1b6/foursight_core/react/api/aws_s3.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.2.0.1b5/foursight_core/react/api/aws_stacks.py` & `foursight_core-4.2.0.1b6/foursight_core/react/api/aws_stacks.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.2.0.1b5/foursight_core/react/api/checks.py` & `foursight_core-4.2.0.1b6/foursight_core/react/api/checks.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.2.0.1b5/foursight_core/react/api/cognito.py` & `foursight_core-4.2.0.1b6/foursight_core/react/api/cognito.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.2.0.1b5/foursight_core/react/api/cookie_utils.py` & `foursight_core-4.2.0.1b6/foursight_core/react/api/cookie_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.2.0.1b5/foursight_core/react/api/datetime_utils.py` & `foursight_core-4.2.0.1b6/foursight_core/react/api/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.2.0.1b5/foursight_core/react/api/encoding_utils.py` & `foursight_core-4.2.0.1b6/foursight_core/react/api/encoding_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.2.0.1b5/foursight_core/react/api/encryption.py` & `foursight_core-4.2.0.1b6/foursight_core/react/api/encryption.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.2.0.1b5/foursight_core/react/api/envs.py` & `foursight_core-4.2.0.1b6/foursight_core/react/api/envs.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.2.0.1b5/foursight_core/react/api/gac.py` & `foursight_core-4.2.0.1b6/foursight_core/react/api/gac.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.2.0.1b5/foursight_core/react/api/jwt_utils.py` & `foursight_core-4.2.0.1b6/foursight_core/react/api/jwt_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.2.0.1b5/foursight_core/react/api/misc_utils.py` & `foursight_core-4.2.0.1b6/foursight_core/react/api/misc_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.2.0.1b5/foursight_core/react/api/portal_access_key_utils.py` & `foursight_core-4.2.0.1b6/foursight_core/react/api/portal_access_key_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.2.0.1b5/foursight_core/react/api/react_api.py` & `foursight_core-4.2.0.1b6/foursight_core/react/api/react_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -82,23 +82,31 @@
                 "dcicutils": get_package_version("dcicutils"),
                 "tibanna": get_package_version("tibanna"),
                 "tibanna_ff": get_package_version("tibanna-ff"),
                 "python": platform.python_version(),
                 "chalice": chalice_version,
                 "elasticsearch_server": self._get_elasticsearch_server_version(),
                 "elasticsearch": get_package_version("elasticsearch"),
-                "elasticsearch_dsl": get_package_version("elasticsearch-dsl")
+                "elasticsearch_dsl": get_package_version("elasticsearch-dsl"),
+                "redis": get_package_version("redis"),
+                "redis_server": self._get_redis_server_version()
             }
 
     @function_cache(nokey=True, nocache=None)
     def _get_elasticsearch_server_version(self) -> Optional[str]:
         connection = app.core.init_connection(self._envs.get_default_env())
         es_info = connection.es_info()
         return es_info.get("version", {}).get("number")
 
+    @function_cache(nokey=True, nocache=None)
+    def _get_redis_server_version(self) -> Optional[str]:
+        connection = app.core.init_connection(self._envs.get_default_env())
+        redis_info = connection.redis_info()
+        return redis_info.get("redis_version") if redis_info else None
+
     @function_cache
     def _get_user_projects(self, env: str, raw: bool = False) -> list:
         """
         Returns the list of available user projects.
         """
         connection = app.core.init_connection(env)
         projects = ff_utils.search_metadata(f'/search/?type=Project&datastore=database', key=connection.ff_keys)
@@ -363,14 +371,15 @@
                 "health_url": portal_base_url + "/health?format=json",
                 "health_ui_url": portal_base_url + "/health"
             },
             "resources": {
                 "es": app.core.host,
                 "foursight": self.foursight_instance_url(request),
                 "portal": portal_url,
+                # TODO: May later want to rds_username and/or such.
                 "rds": os.environ["RDS_HOSTNAME"],
                 "redis": redis_url,
                 "redis_running": redis is not None,
                 "sqs": self._get_sqs_queue_url(),
             },
             "s3": {
                 "bucket_org": os.environ.get("ENCODED_S3_BUCKET_ORG", os.environ.get("S3_BUCKET_ORG", None)),
@@ -1124,25 +1133,20 @@
 
     def reactapi_checks_validation(self, request: dict, env: str) -> Response:
         """
         Called from react_routes for endpoint: GET /{env}/checks_validation
         Returns information about any problems with the checks setup.
         """
         ignored(request, env)
-        checks_actions_registry = self._checks.get_registry()
-        actions_with_no_assocated_check = [name for name in checks_actions_registry
-                                           if checks_actions_registry[name].get("kind") == "action"
-                                           and not checks_actions_registry[name].get("checks")]
         response = {}
-        if actions_with_no_assocated_check:
-            response["actions_with_no_associated_check"] = [
-                checks_actions_registry[item]
-                for item in checks_actions_registry
-                if checks_actions_registry[item]["kind"] == "action" and item in actions_with_no_assocated_check
-            ]
+        checks_actions_registry = self._checks.get_registry()
+        actions_with_no_associated_check = [item for _, item in checks_actions_registry.items()
+                                            if item.get("kind") == "action" and not item.get("checks")]
+        if actions_with_no_associated_check:
+            response["actions_with_no_associated_check"] = actions_with_no_associated_check
         return self.create_success_response(response)
 
     def reactapi_lambdas(self, request: dict, env: str) -> Response:
         """
         Called from react_routes for endpoint: GET /{env}/lambdas
         Returns a summary (list) of all defined AWS lambdas for the current AWS environment.
         """
```

### Comparing `foursight_core-4.2.0.1b5/foursight_core/react/api/react_api_base.py` & `foursight_core-4.2.0.1b6/foursight_core/react/api/react_api_base.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.2.0.1b5/foursight_core/react/api/react_route_decorator.py` & `foursight_core-4.2.0.1b6/foursight_core/react/api/react_route_decorator.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.2.0.1b5/foursight_core/react/api/react_routes.py` & `foursight_core-4.2.0.1b6/foursight_core/react/api/react_routes.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.2.0.1b5/foursight_core/react/api/react_ui.py` & `foursight_core-4.2.0.1b6/foursight_core/react/api/react_ui.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.2.0.1b5/foursight_core/react/api/yaml_utils.py` & `foursight_core-4.2.0.1b6/foursight_core/react/api/yaml_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.2.0.1b5/foursight_core/react/ui/index.html` & `foursight_core-4.2.0.1b6/foursight_core/react/ui/index.html`

 * *Files identical despite different names*

### Comparing `foursight_core-4.2.0.1b5/foursight_core/react/ui/static/css/main.css` & `foursight_core-4.2.0.1b6/foursight_core/react/ui/static/css/main.css`

 * *Files identical despite different names*

### Comparing `foursight_core-4.2.0.1b5/foursight_core/react/ui/static/js/main.js` & `foursight_core-4.2.0.1b6/foursight_core/react/ui/static/js/main.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -1,8 +1,8 @@
-/*! For license information please see main.b7685537.js.LICENSE.txt */
+/*! For license information please see main.a8bddaf8.js.LICENSE.txt */
 (function() {
     var __webpack_modules__ = {
             4189: function(e, t) {
                 "use strict";
                 Object.defineProperty(t, "__esModule", {
                     value: !0
                 })
@@ -50994,14 +50994,30 @@
                                     children: (0, Kr.jsx)("b", {
                                         children: t.get("foursight.versions.elasticsearch_dsl")
                                     })
                                 }) : (0, Kr.jsx)(Kr.Fragment, {
                                     children: Fr.EmptySet
                                 })
                             })]
+                        }), (0, Kr.jsxs)("tr", {
+                            children: [(0, Kr.jsx)("td", {
+                                style: {
+                                    whiteSpace: "nowrap",
+                                    paddingRight: "4pt"
+                                },
+                                children: "redis-server:"
+                            }), (0, Kr.jsx)("td", {
+                                children: t.get("foursight.versions.redis_server") ? (0, Kr.jsx)(Kr.Fragment, {
+                                    children: (0, Kr.jsx)("b", {
+                                        children: t.get("foursight.versions.redis_server")
+                                    })
+                                }) : (0, Kr.jsx)(Kr.Fragment, {
+                                    children: Fr.EmptySet
+                                })
+                            })]
                         })]
                     })
                 })
             },
             aa = function(e) {
                 var n, r, o, i, a, s, u = e.account,
                     l = e.header,
@@ -59311,86 +59327,88 @@
                     u = void 0 === s ? "4" : s,
                     l = e.pypi,
                     c = void 0 === l ? null : l,
                     d = e.github,
                     f = void 0 === d ? null : d,
                     p = e.elasticsearch,
                     h = void 0 !== p && p,
-                    g = e.python,
+                    g = e.redis,
                     y = void 0 !== g && g,
-                    m = (e.chalice, e.check),
+                    m = e.python,
                     v = void 0 !== m && m,
-                    M = e.nocheck,
+                    M = (e.chalice, e.check),
                     b = void 0 !== M && M,
-                    j = e.link,
-                    w = void 0 === j ? null : j,
-                    x = e.optional,
-                    N = void 0 !== x && x,
-                    I = e.portalCertificate,
+                    j = e.nocheck,
+                    w = void 0 !== j && j,
+                    x = e.link,
+                    N = void 0 === x ? null : x,
+                    I = e.optional,
                     D = void 0 !== I && I,
-                    S = e.portalAccessKey,
+                    S = e.portalCertificate,
                     L = void 0 !== S && S,
-                    k = e.apiCache,
-                    C = void 0 !== k && k;
-                var E = {
+                    k = e.portalAccessKey,
+                    C = void 0 !== k && k,
+                    E = e.apiCache,
+                    _ = void 0 !== E && E;
+                var T = {
                         fontSize: "11pt",
                         fontFamily: o ? "monospace" : "inherit",
                         fontWeight: "bold",
                         wordWrap: "break-word",
                         cursor: a ? "copy" : "inherit",
                         align: "left"
                     },
-                    _ = a ? {
+                    A = a ? {
                         onClick: function() {
                             return Yr.Copy(t)
                         }
                     } : {},
-                    T = v ? (0, Kr.jsxs)("span", {
+                    O = b ? (0, Kr.jsxs)("span", {
                         children: ["\xa0", (0, Kr.jsx)("b", {
                             style: {
                                 fontSize: "13pt",
                                 color: "green"
                             },
                             children: Fr.Check
                         })]
                     }) : (0, Kr.jsx)("span", {}),
-                    A = b ? (0, Kr.jsxs)("span", {
+                    z = w ? (0, Kr.jsxs)("span", {
                         children: ["\xa0", (0, Kr.jsx)("b", {
                             style: {
                                 fontSize: "13pt",
                                 color: "red"
                             },
                             children: Fr.X
                         })]
                     }) : (0, Kr.jsx)("span", {}),
-                    O = c ? (0, Kr.jsxs)("span", {
+                    U = c ? (0, Kr.jsxs)("span", {
                         children: [(0, Kr.jsx)("a", {
                             target: "_blank",
                             rel: "noreferrer",
                             href: "https://pypi.org/project/" + t + "/" + n + "/",
                             children: (0, Kr.jsx)("img", {
                                 alt: "pypi",
                                 src: Ut.PyPi(),
                                 height: "21"
                             })
                         }), "\xa0"]
                     }) : (0, Kr.jsx)("span", {}),
-                    z = f ? (0, Kr.jsxs)("span", {
+                    P = f ? (0, Kr.jsxs)("span", {
                         children: [(0, Kr.jsx)("a", {
                             target: "_blank",
                             rel: "noreferrer",
                             href: "https://github.com/" + f + "/" + ("dcicutils" === t ? "utils" : t) + "/releases/tag/" + ("chalice" !== t ? "v" : "") + n,
                             children: (0, Kr.jsx)("img", {
                                 alt: "github",
                                 src: Ut.GitHub(),
                                 height: "15"
                             })
                         }), "\xa0"]
                     }) : (0, Kr.jsx)("span", {}),
-                    U = h ? (0, Kr.jsxs)("span", {
+                    R = h ? (0, Kr.jsxs)("span", {
                         children: [(0, Kr.jsx)("a", {
                             target: "_blank",
                             rel: "noreferrer",
                             href: "https://www.elastic.co/guide/en/elasticsearch/reference/".concat(function(e) {
                                 var t = null === e || void 0 === e ? void 0 : e.split(".");
                                 return (null === t || void 0 === t ? void 0 : t.length) >= 2 ? t[0] + "." + t[1] : e
                             }(n), "/release-notes-").concat(n, ".html"),
@@ -59400,33 +59418,51 @@
                             children: (0, Kr.jsx)("img", {
                                 alt: "github",
                                 src: Ut.ElasticsearchLogo(),
                                 height: "18"
                             })
                         }), "\xa0"]
                     }) : (0, Kr.jsx)("span", {}),
-                    P = y ? (0, Kr.jsxs)("span", {
+                    B = y ? (0, Kr.jsxs)("span", {
+                        children: [(0, Kr.jsx)("a", {
+                            target: "_blank",
+                            rel: "noreferrer",
+                            href: "https://raw.githubusercontent.com/redis/redis/".concat(n, "/00-RELEASENOTES"),
+                            style: {
+                                marginLeft: "-2px"
+                            },
+                            children: (0, Kr.jsx)("img", {
+                                alt: "github",
+                                src: "https://1000logos.net/wp-content/uploads/2020/08/Redis-Logo-1280x800.png",
+                                height: "21",
+                                style: {
+                                    marginLeft: "3pt"
+                                }
+                            })
+                        }), "\xa0"]
+                    }) : (0, Kr.jsx)("span", {}),
+                    F = v ? (0, Kr.jsxs)("span", {
                         children: [(0, Kr.jsx)("a", {
                             target: "_blank",
                             rel: "noreferrer",
                             href: "https://docs.python.org/release/" + n + "/",
                             children: (0, Kr.jsx)("img", {
                                 alt: "python",
                                 src: Ut.Python(),
                                 height: "19"
                             })
                         }), "\xa0"]
                     }) : (0, Kr.jsx)("span", {}),
-                    R = (0, Kr.jsx)("span", {});
+                    Y = (0, Kr.jsx)("span", {});
                 return (0, Kr.jsx)(Kr.Fragment, {
                     children: (0, Kr.jsx)("div", {
                         style: {
                             marginTop: "1px"
                         },
-                        children: !N || n ? (0, Kr.jsxs)("div", {
+                        children: !D || n ? (0, Kr.jsxs)("div", {
                             className: "row",
                             children: [(0, Kr.jsx)("div", {
                                 className: "col-sm-" + u,
                                 children: (0, Kr.jsxs)("div", {
                                     style: {
                                         fontSize: "11pt",
                                         fontFamily: "inherit",
@@ -59435,322 +59471,336 @@
                                         align: "left"
                                     },
                                     children: [t, ":"]
                                 })
                             }), (0, Kr.jsxs)("div", Ye(Ye({
                                 id: t,
                                 className: "col-sm-8",
-                                style: E,
+                                style: T,
                                 align: "left"
-                            }, _), {}, {
-                                children: [O, z, U, P, R, w && n ? (0, Kr.jsx)("span", {
+                            }, A), {}, {
+                                children: [U, P, R, B, F, Y, N && n ? (0, Kr.jsx)("span", {
                                     children: (0, Kr.jsx)(Oe, {
-                                        to: w,
+                                        to: N,
                                         children: n
                                     })
                                 }) : (0, Kr.jsxs)("span", {
                                     children: [st.IsNonEmptyObject(n) ? (0, Kr.jsx)(Kr.Fragment, {
                                         children: n
                                     }) : (0, Kr.jsx)(Kr.Fragment, {
                                         children: n || (0, Kr.jsx)("span", {
                                             children: Fr.EmptySet
                                         })
-                                    }), L && (0, Kr.jsxs)(Kr.Fragment, {
+                                    }), C && (0, Kr.jsxs)(Kr.Fragment, {
                                         children: ["\xa0", Fr.RightArrow, "\xa0", (0, Kr.jsx)(Oe, {
                                             to: kr.Path("/portal_access_key"),
                                             children: "View Details"
                                         })]
-                                    }), D && (0, Kr.jsxs)(Kr.Fragment, {
+                                    }), L && (0, Kr.jsxs)(Kr.Fragment, {
                                         children: ["\xa0", Fr.RightArrow, "\xa0", (0, Kr.jsx)(Oe, {
                                             to: kr.Path("/certificates"),
                                             children: "View Certificate"
                                         })]
-                                    }), C && (0, Kr.jsxs)(Kr.Fragment, {
+                                    }), _ && (0, Kr.jsxs)(Kr.Fragment, {
                                         children: ["\xa0", Fr.RightArrow, "\xa0", (0, Kr.jsx)(Oe, {
                                             to: kr.Path("/apicache"),
                                             children: "View API Cache"
                                         })]
                                     })]
-                                }), T, A]
+                                }), O, z]
                             }))]
                         }) : (0, Kr.jsx)("span", {})
                     })
                 })
             },
             Ds = function() {
-                var e, n, r, o, i, s, u, l, c, d, f, p, h, g, y, m, v, M, b, j, w, x, N, I, D, S, L, k, C, E, _, T, A, O, z, U, P, R, B, F, Y, Q, G, W, H, Z, V = ta(),
-                    q = Xi("/info"),
-                    J = a((0, t.useState)(!1), 2),
-                    K = J[0],
-                    X = J[1],
-                    $ = a((0, t.useState)(!1), 2),
-                    ee = $[0],
-                    te = $[1],
-                    ne = a((0, t.useState)(!1), 2),
-                    re = ne[0],
-                    oe = ne[1],
-                    ie = Xi("/portal_access_key"),
-                    ae = la();
-                return q.error ? (0, Kr.jsx)(xi, {
-                    error: q.error,
+                var e, n, r, o, i, s, u, l, c, d, f, p, h, g, y, m, v, M, b, j, w, x, N, I, D, S, L, k, C, E, _, T, A, O, z, U, P, R, B, F, Y, Q, G, W, H, Z, V, q, J, K, X = ta(),
+                    $ = Xi("/info"),
+                    ee = a((0, t.useState)(!1), 2),
+                    te = ee[0],
+                    ne = ee[1],
+                    re = a((0, t.useState)(!1), 2),
+                    oe = re[0],
+                    ie = re[1],
+                    ae = a((0, t.useState)(!1), 2),
+                    se = ae[0],
+                    ue = ae[1],
+                    le = Xi("/portal_access_key"),
+                    ce = la();
+                return $.error ? (0, Kr.jsx)(xi, {
+                    error: $.error,
                     message: "Error loading info from Foursight API"
                 }) : (0, Kr.jsxs)("div", {
                     className: "container",
                     children: [(0, Kr.jsxs)(Ns, {
-                        info: q,
+                        info: $,
                         title: "Versions",
                         children: [(0, Kr.jsx)(Is, {
-                            name: null === (e = V.app) || void 0 === e ? void 0 : e.package,
-                            value: null === (n = V.versions) || void 0 === n ? void 0 : n.foursight,
+                            name: null === (e = X.app) || void 0 === e ? void 0 : e.package,
+                            value: null === (n = X.versions) || void 0 === n ? void 0 : n.foursight,
                             monospace: !0,
                             copy: !0,
                             pypi: !0,
-                            github: At.IsFoursightFourfront(V) ? "4dn-dcic" : "dbmi-bgm",
+                            github: At.IsFoursightFourfront(X) ? "4dn-dcic" : "dbmi-bgm",
                             size: "2"
                         }), (0, Kr.jsx)(Is, {
                             name: "foursight-core",
-                            value: null === (r = V.versions) || void 0 === r ? void 0 : r.foursight_core,
+                            value: null === (r = X.versions) || void 0 === r ? void 0 : r.foursight_core,
                             monospace: !0,
                             copy: !0,
                             pypi: !0,
                             github: "4dn-dcic",
                             size: "2"
                         }), (0, Kr.jsx)(Is, {
                             name: "dcicutils",
-                            value: null === (o = V.versions) || void 0 === o ? void 0 : o.dcicutils,
+                            value: null === (o = X.versions) || void 0 === o ? void 0 : o.dcicutils,
                             monospace: !0,
                             copy: !0,
                             pypi: !0,
                             github: "4dn-dcic",
                             size: "2"
                         }), (0, Kr.jsx)(Is, {
                             name: "tibanna",
-                            value: null === (i = V.versions) || void 0 === i ? void 0 : i.tibanna,
+                            value: null === (i = X.versions) || void 0 === i ? void 0 : i.tibanna,
                             monospace: !0,
                             copy: !0,
                             size: "2",
                             pypi: !0
                         }), (0, Kr.jsx)(Is, {
                             name: "tibanna-ff",
-                            value: null === (s = V.versions) || void 0 === s ? void 0 : s.tibanna_ff,
+                            value: null === (s = X.versions) || void 0 === s ? void 0 : s.tibanna_ff,
                             monospace: !0,
                             copy: !0,
                             size: "2",
                             pypi: !0
                         }), (0, Kr.jsx)(Is, {
                             name: "chalice",
-                            value: null === (u = V.versions) || void 0 === u ? void 0 : u.chalice,
+                            value: null === (u = X.versions) || void 0 === u ? void 0 : u.chalice,
                             monospace: !0,
                             copy: !0,
                             chalice: !0,
                             size: "2",
                             pypi: !0,
                             github: "aws"
                         }), (0, Kr.jsx)(Is, {
                             name: "python",
-                            value: null === (l = V.versions) || void 0 === l ? void 0 : l.python,
+                            value: null === (l = X.versions) || void 0 === l ? void 0 : l.python,
                             monospace: !0,
                             copy: !0,
                             python: !0,
                             size: "2"
                         }), (0, Kr.jsx)(Is, {
                             name: "elasticsearch-server",
-                            value: (null === (c = V.versions) || void 0 === c ? void 0 : c.elasticsearch_server) || (null === (d = q.data) || void 0 === d || null === (f = d.versions) || void 0 === f ? void 0 : f.elasticsearch_server),
+                            value: (null === (c = X.versions) || void 0 === c ? void 0 : c.elasticsearch_server) || (null === (d = $.data) || void 0 === d || null === (f = d.versions) || void 0 === f ? void 0 : f.elasticsearch_server),
                             monospace: !0,
                             copy: !0,
                             size: "2",
                             elasticsearch: !0
                         }), (0, Kr.jsx)(Is, {
                             name: "elasticsearch",
-                            value: null === (p = V.versions) || void 0 === p ? void 0 : p.elasticsearch,
+                            value: null === (p = X.versions) || void 0 === p ? void 0 : p.elasticsearch,
                             monospace: !0,
                             copy: !0,
                             size: "2",
                             pypi: !0
                         }), (0, Kr.jsx)(Is, {
                             name: "elasticsearch-dsl",
-                            value: null === (h = V.versions) || void 0 === h ? void 0 : h.elasticsearch_dsl,
+                            value: null === (h = X.versions) || void 0 === h ? void 0 : h.elasticsearch_dsl,
+                            monospace: !0,
+                            copy: !0,
+                            size: "2",
+                            pypi: !0
+                        }), (0, Kr.jsx)(Is, {
+                            name: "redis-server",
+                            value: (null === (g = X.versions) || void 0 === g ? void 0 : g.redis_server) || (null === (y = $.data) || void 0 === y || null === (m = y.versions) || void 0 === m ? void 0 : m.redis_server),
+                            monospace: !0,
+                            copy: !0,
+                            size: "2",
+                            redis: !0
+                        }), (0, Kr.jsx)(Is, {
+                            name: "redis",
+                            value: null === (v = X.versions) || void 0 === v ? void 0 : v.redis,
                             monospace: !0,
                             copy: !0,
                             size: "2",
                             pypi: !0
                         })]
                     }), (0, Kr.jsxs)(Ns, {
-                        info: q,
+                        info: $,
                         title: "Credentials Info",
                         children: [(0, Kr.jsx)(Is, {
                             name: "AWS Account Number",
-                            value: q.get("app.credentials.aws_account_number"),
+                            value: $.get("app.credentials.aws_account_number"),
                             monospace: !0,
                             copy: !0,
                             size: "2"
                         }), (0, Kr.jsx)(Is, {
                             name: "AWS Region Name",
-                            value: q.get("app.credentials.aws_region"),
+                            value: $.get("app.credentials.aws_region"),
                             monospace: !0,
                             copy: !0,
                             size: "2"
                         }), (0, Kr.jsx)(Is, {
                             name: "AWS User ARN",
-                            value: q.get("app.credentials.aws_user_arn"),
+                            value: $.get("app.credentials.aws_user_arn"),
                             monospace: !0,
                             copy: !0,
                             size: "2"
                         }), (0, Kr.jsx)(Is, {
                             name: "AWS Access Key ID",
-                            value: q.get("app.credentials.aws_access_key_id"),
+                            value: $.get("app.credentials.aws_access_key_id"),
                             monospace: !0,
                             copy: !0,
                             size: "2"
-                        }), q.get("environ.S3_AWS_ACCESS_KEY_ID") && (0, Kr.jsx)(Is, {
+                        }), $.get("environ.S3_AWS_ACCESS_KEY_ID") && (0, Kr.jsx)(Is, {
                             name: "AWS S3 Access Key ID",
-                            value: q.get("environ.S3_AWS_ACCESS_KEY_ID"),
+                            value: $.get("environ.S3_AWS_ACCESS_KEY_ID"),
                             monospace: !0,
                             copy: !0,
                             size: "2"
                         }), (0, Kr.jsx)(Is, {
                             name: "Portal Access Key",
-                            value: ie.get("key"),
+                            value: le.get("key"),
                             monospace: !0,
                             copy: !0,
                             size: "2",
                             portalAccessKey: !0
                         }), (0, Kr.jsx)(Is, {
                             name: "Auth0 Client ID",
-                            value: q.get("app.credentials.auth0_client_id"),
+                            value: $.get("app.credentials.auth0_client_id"),
                             monospace: !0,
                             copy: !0,
                             size: "2"
                         })]
                     }), (0, Kr.jsxs)(Ns, {
-                        info: q,
+                        info: $,
                         title: "Resources",
                         children: [(0, Kr.jsx)(Is, {
                             name: "Foursight Server",
-                            value: q.get("server.foursight"),
+                            value: $.get("server.foursight"),
                             monospace: !0,
                             copy: !0,
                             size: "2"
                         }), (0, Kr.jsx)(Is, {
                             name: "Foursight",
-                            value: null === (g = V.resources) || void 0 === g ? void 0 : g.foursight,
+                            value: null === (M = X.resources) || void 0 === M ? void 0 : M.foursight,
                             monospace: !0,
                             copy: !0,
                             size: "2"
                         }), (0, Kr.jsx)(Is, {
                             name: "Portal",
-                            value: null === (y = V.resources) || void 0 === y ? void 0 : y.portal,
+                            value: null === (b = X.resources) || void 0 === b ? void 0 : b.portal,
                             monospace: !0,
                             copy: !0,
                             size: "2",
                             portalCertificate: !0
                         }), (0, Kr.jsx)(Is, {
                             name: "ElasticSearch",
-                            value: null === (m = V.resources) || void 0 === m ? void 0 : m.es,
+                            value: null === (j = X.resources) || void 0 === j ? void 0 : j.es,
                             monospace: !0,
                             copy: !0,
                             size: "2"
                         }), (0, Kr.jsx)(Is, {
                             name: "RDS",
-                            value: null === (v = V.resources) || void 0 === v ? void 0 : v.rds,
+                            value: null === (w = X.resources) || void 0 === w ? void 0 : w.rds,
                             monospace: !0,
                             copy: !0,
                             size: "2"
                         }), (0, Kr.jsx)(Is, {
                             name: "SQS",
-                            value: null === (M = V.resources) || void 0 === M ? void 0 : M.sqs,
+                            value: null === (x = X.resources) || void 0 === x ? void 0 : x.sqs,
                             monospace: !0,
                             copy: !0,
                             size: "2"
                         }), (0, Kr.jsx)(Is, {
                             name: "Redis",
-                            value: null === (b = V.resources) || void 0 === b ? void 0 : b.redis,
-                            nocheck: !(null !== (j = V.resources) && void 0 !== j && j.redis_running),
-                            check: null === (w = V.resources) || void 0 === w ? void 0 : w.redis_running,
+                            value: null === (N = X.resources) || void 0 === N ? void 0 : N.redis,
+                            nocheck: !(null !== (I = X.resources) && void 0 !== I && I.redis_running),
+                            check: null === (D = X.resources) || void 0 === D ? void 0 : D.redis_running,
                             monospace: !0,
                             copy: !0,
                             size: "2"
                         })]
                     }), (0, Kr.jsxs)(Ns, {
-                        info: q,
+                        info: $,
                         title: "Authentication/Authorization Info",
                         show: !0,
                         children: [(0, Kr.jsx)(Is, {
                             name: "Email",
-                            value: null === (x = Br.Token()) || void 0 === x ? void 0 : x.user,
+                            value: null === (S = Br.Token()) || void 0 === S ? void 0 : S.user,
                             monospace: !0,
                             copy: !0,
-                            check: null === (N = Br.Token()) || void 0 === N ? void 0 : N.user_verified,
-                            link: kr.Path("/users/" + Br.LoggedInUser(V), !0),
+                            check: null === (L = Br.Token()) || void 0 === L ? void 0 : L.user_verified,
+                            link: kr.Path("/users/" + Br.LoggedInUser(X), !0),
                             size: "2"
                         }), (0, Kr.jsx)(Is, {
                             name: "First Name",
-                            value: null === (I = Br.Token()) || void 0 === I ? void 0 : I.first_name,
+                            value: null === (k = Br.Token()) || void 0 === k ? void 0 : k.first_name,
                             monospace: !0,
                             copy: !0,
                             size: "2"
                         }), (0, Kr.jsx)(Is, {
                             name: "Last Name",
-                            value: null === (D = Br.Token()) || void 0 === D ? void 0 : D.last_name,
+                            value: null === (C = Br.Token()) || void 0 === C ? void 0 : C.last_name,
                             monospace: !0,
                             copy: !0,
                             size: "2"
                         }), (0, Kr.jsx)(Is, {
                             name: "Environments",
-                            value: null === (S = Br.Token()) || void 0 === S ? void 0 : S.allowed_envs.join(", "),
+                            value: null === (E = Br.Token()) || void 0 === E ? void 0 : E.allowed_envs.join(", "),
                             monospace: !0,
                             copy: !0,
                             size: "2"
                         }), (0, Kr.jsx)(Is, {
                             name: "Audience",
-                            value: null === (L = Br.Token()) || void 0 === L ? void 0 : L.aud,
+                            value: null === (_ = Br.Token()) || void 0 === _ ? void 0 : _.aud,
                             monospace: !0,
                             copy: !0,
                             size: "2"
                         }), (0, Kr.jsx)(Is, {
                             name: "Issued At",
                             monospace: !0,
                             copy: !0,
                             size: "2",
                             value: (0, Kr.jsx)(ja.FormatDuration, {
-                                start: null === (k = Br.Token()) || void 0 === k ? void 0 : k.authenticated_at,
+                                start: null === (T = Br.Token()) || void 0 === T ? void 0 : T.authenticated_at,
                                 verbose: !0,
                                 fallback: "just now",
                                 suffix: "ago",
                                 tooltip: !0,
                                 prefix: "datetime"
                             })
                         }), (0, Kr.jsx)(Is, {
                             name: "Expires At",
                             monospace: !0,
                             copy: !0,
                             size: "2",
                             value: (0, Kr.jsx)(ja.FormatDuration, {
-                                end: null === (C = Br.Token()) || void 0 === C ? void 0 : C.authenticated_until,
+                                end: null === (A = Br.Token()) || void 0 === A ? void 0 : A.authenticated_until,
                                 verbose: !0,
                                 fallback: "now",
                                 suffix: "from now",
                                 tooltip: !0,
                                 prefix: "datetime"
                             })
                         }), (0, Kr.jsx)(Is, {
                             name: "Using Redis",
                             monospace: !0,
                             size: "2",
-                            value: null !== (E = V.resources) && void 0 !== E && E.redis_running ? "Yes" : "No"
+                            value: null !== (O = X.resources) && void 0 !== O && O.redis_running ? "Yes" : "No"
                         }), (0, Kr.jsx)("hr", {
                             style: {
                                 borderTop: "1px solid darkblue",
                                 marginTop: "8",
                                 marginBottom: "8"
                             }
-                        }), K ? (0, Kr.jsxs)(Kr.Fragment, {
+                        }), te ? (0, Kr.jsxs)(Kr.Fragment, {
                             children: [(0, Kr.jsx)("small", {
                                 onClick: function() {
-                                    return X(!1)
+                                    return ne(!1)
                                 },
                                 style: {
                                     cursor: "pointer",
                                     color: "inherit"
                                 },
                                 children: (0, Kr.jsxs)("b", {
                                     children: [(0, Kr.jsx)("u", {
@@ -59784,209 +59834,209 @@
                                         cursor: "copy"
                                     }
                                 }), Bi.Format(Br.Token())]
                             })]
                         }) : (0, Kr.jsxs)(Kr.Fragment, {
                             children: [(0, Kr.jsx)("small", {
                                 onClick: function() {
-                                    return X(!0)
+                                    return ne(!0)
                                 },
                                 style: {
                                     cursor: "pointer",
                                     color: "darkblue"
                                 },
                                 children: (0, Kr.jsxs)("b", {
                                     children: [(0, Kr.jsx)("u", {
                                         children: "AuthToken"
                                     }), "\xa0", Fr.UpArrow]
                                 })
                             }), (0, Kr.jsx)("br", {})]
                         })]
                     }), (0, Kr.jsxs)(Ns, {
-                        info: q,
+                        info: $,
                         title: "Environment Names",
                         children: [(0, Kr.jsx)(Is, {
                             name: "Environment Name",
-                            value: At.RegularName(At.Current(), V),
+                            value: At.RegularName(At.Current(), X),
                             monospace: !0,
                             copy: !0,
                             size: "3"
                         }), (0, Kr.jsx)(Is, {
                             name: "Environment Name (Full)",
-                            value: At.FullName(At.Current(), V),
+                            value: At.FullName(At.Current(), X),
                             monospace: !0,
                             copy: !0,
                             size: "3"
                         }), (0, Kr.jsx)(Is, {
                             name: "Environment Name (Short)",
-                            value: At.ShortName(At.Current(), V),
+                            value: At.ShortName(At.Current(), X),
                             monospace: !0,
                             copy: !0,
                             size: "3"
                         }), (0, Kr.jsx)(Is, {
                             name: "Environment Name (Public)",
-                            value: At.PublicName(At.Current(), V),
+                            value: At.PublicName(At.Current(), X),
                             monospace: !0,
                             copy: !0,
                             size: "3"
                         }), (0, Kr.jsx)(Is, {
                             name: "Environment Name (Foursight)",
-                            value: At.FoursightName(At.Current(), V),
+                            value: At.FoursightName(At.Current(), X),
                             monospace: !0,
                             copy: !0,
                             size: "3"
                         }), (0, Kr.jsx)(Is, {
                             name: "Environment Name (Preferred)",
-                            value: At.PreferredName(At.Current(V), V),
+                            value: At.PreferredName(At.Current(X), X),
                             monospace: !0,
                             copy: !0,
                             size: "3"
                         })]
                     }), (0, Kr.jsxs)(Ns, {
-                        info: q,
+                        info: $,
                         title: "Bucket Names",
                         children: [(0, Kr.jsx)(Is, {
                             name: "Global Environment Bucket",
-                            value: q.get("buckets.env"),
+                            value: $.get("buckets.env"),
                             monospace: !0,
                             copy: !0,
                             size: "3"
                         }), (0, Kr.jsx)(Is, {
                             name: "Foursight Bucket Name",
-                            value: q.get("buckets.foursight"),
+                            value: $.get("buckets.foursight"),
                             monospace: !0,
                             copy: !0,
                             size: "3"
                         }), (0, Kr.jsx)(Is, {
                             name: "Foursight Bucket Prefix",
-                            value: q.get("buckets.foursight_prefix"),
+                            value: $.get("buckets.foursight_prefix"),
                             monospace: !0,
                             copy: !0,
                             size: "3"
                         })]
                     }), (0, Kr.jsx)(Ns, {
-                        info: q,
+                        info: $,
                         title: "Environment & Bucket Names",
                         children: (0, Kr.jsx)("pre", {
                             className: "box",
                             style: {
                                 border: "0",
                                 margin: "0",
                                 padding: "8",
                                 paddingBottom: "8",
                                 marginTop: "0"
                             },
                             children: (0, Kr.jsxs)("span", {
-                                children: [Bi.Format(q.get("buckets.info")), (null === (_ = q.get("buckets.info")) || void 0 === _ ? void 0 : _.length) > 1 ? (0, Kr.jsx)("div", {
+                                children: [Bi.Format($.get("buckets.info")), (null === (z = $.get("buckets.info")) || void 0 === z ? void 0 : z.length) > 1 ? (0, Kr.jsx)("div", {
                                     style: {
                                         height: "1px",
                                         marginTop: "6px",
                                         marginBottom: "6px",
                                         background: "black"
                                     }
                                 }) : (0, Kr.jsx)("span", {})]
                             }, Dr()())
                         })
                     }), (0, Kr.jsx)(Ns, {
-                        info: q,
+                        info: $,
                         title: "Ecosystem",
                         show: !1,
                         children: (0, Kr.jsx)("pre", {
                             className: "box",
                             style: {
                                 border: "0",
                                 margin: "0",
                                 paddingTop: "8",
                                 paddingBottom: "8",
                                 marginTop: "0"
                             },
-                            children: Bi.Format(q.get("buckets.ecosystem"))
+                            children: Bi.Format($.get("buckets.ecosystem"))
                         })
-                    }), q.get("environ.AWS_LAMBDA_LOG_GROUP_NAME") && q.get("environ.AWS_LAMBDA_LOG_STREAM_NAME") && (0, Kr.jsx)(Kr.Fragment, {
+                    }), $.get("environ.AWS_LAMBDA_LOG_GROUP_NAME") && $.get("environ.AWS_LAMBDA_LOG_STREAM_NAME") && (0, Kr.jsx)(Kr.Fragment, {
                         children: (0, Kr.jsxs)(Ns, {
-                            info: q,
+                            info: $,
                             title: "Logs",
                             children: [(0, Kr.jsx)(Is, {
                                 name: "Log Group",
-                                value: q.get("environ.AWS_LAMBDA_LOG_GROUP_NAME"),
+                                value: $.get("environ.AWS_LAMBDA_LOG_GROUP_NAME"),
                                 monospace: !0,
                                 size: "2"
                             }), (0, Kr.jsx)(Is, {
                                 name: "Log Stream",
-                                value: q.get("environ.AWS_LAMBDA_LOG_STREAM_NAME"),
+                                value: $.get("environ.AWS_LAMBDA_LOG_STREAM_NAME"),
                                 monospace: !0,
                                 size: "2"
                             })]
                         })
-                    }), q.get("app.lambda") && (0, Kr.jsxs)(Ns, {
-                        info: q,
+                    }), $.get("app.lambda") && (0, Kr.jsxs)(Ns, {
+                        info: $,
                         title: "Lambda",
                         show: !1,
                         children: [(0, Kr.jsx)(Is, {
                             name: "Name",
-                            value: q.get("app.lambda.lambda_name"),
+                            value: $.get("app.lambda.lambda_name"),
                             monospace: !0,
                             size: "2"
                         }), (0, Kr.jsx)(Is, {
                             name: "Function",
-                            value: q.get("app.lambda.lambda_function_name"),
+                            value: $.get("app.lambda.lambda_function_name"),
                             monospace: !0,
                             size: "2"
                         }), (0, Kr.jsx)(Is, {
                             name: "ARN",
-                            value: q.get("app.lambda.lambda_function_arn"),
+                            value: $.get("app.lambda.lambda_function_arn"),
                             monospace: !0,
                             size: "2"
                         }), (0, Kr.jsx)(Is, {
                             name: "S3 Location",
-                            value: q.get("app.lambda.lambda_code_s3_bucket") + "/" + q.get("app.lambda.lambda_code_s3_bucket_key"),
+                            value: $.get("app.lambda.lambda_code_s3_bucket") + "/" + $.get("app.lambda.lambda_code_s3_bucket_key"),
                             monospace: !0,
                             size: "2"
                         }), (0, Kr.jsx)(Is, {
                             name: "Size",
-                            value: q.get("app.lambda.lambda_code_size"),
+                            value: $.get("app.lambda.lambda_code_size"),
                             monospace: !0,
                             size: "2"
                         }), (0, Kr.jsx)(Is, {
                             name: "Modified",
-                            value: Pr.FormatDateTime(q.get("app.lambda.lambda_modified")),
+                            value: Pr.FormatDateTime($.get("app.lambda.lambda_modified")),
                             monospace: !0,
                             size: "2"
                         }), (0, Kr.jsx)(Is, {
                             name: "Role",
-                            value: q.get("app.lambda.lambda_role"),
+                            value: $.get("app.lambda.lambda_role"),
                             monospace: !0,
                             size: "2"
                         })]
                     }), (0, Kr.jsxs)(Ns, {
-                        info: q,
+                        info: $,
                         title: "Miscellany",
-                        children: [re ? (0, Kr.jsxs)(Kr.Fragment, {
+                        children: [se ? (0, Kr.jsxs)(Kr.Fragment, {
                             children: [(0, Kr.jsx)("div", {
                                 id: "tooltip-info-reloading",
                                 style: {
                                     float: "right"
                                 },
                                 children: (0, Kr.jsx)(no, {
-                                    condition: re,
+                                    condition: se,
                                     label: "",
                                     color: "darkblue"
                                 })
                             }), (0, Kr.jsx)(Mi, {
                                 id: "tooltip-info-reloading",
                                 position: "bottom",
                                 size: "small",
                                 text: "Reloading the Foursight app."
                             })]
                         }) : (0, Kr.jsxs)(Kr.Fragment, {
                             children: [(0, Kr.jsx)("b", {
                                 onClick: function() {
-                                    return oe(!0), void ae("/__reloadlambda__", {
+                                    return ue(!0), void ce("/__reloadlambda__", {
                                         onDone: function() {
-                                            return oe(!1)
+                                            return ue(!1)
                                         }
                                     })
                                 },
                                 id: "tooltip-info-reload",
                                 style: {
                                     float: "right",
                                     cursor: "pointer"
@@ -60007,72 +60057,72 @@
                                 cursor: "pointer"
                             },
                             children: ["\xa0\xa0", (0, Kr.jsx)("img", {
                                 alt: "Clear Cache",
                                 src: Ut.ClearCache(),
                                 height: "19",
                                 onClick: function() {
-                                    ae(zt.Url("/__functioncacheclear__", !1))
+                                    ce(zt.Url("/__functioncacheclear__", !1))
                                 }
                             })]
                         }), (0, Kr.jsx)(Mi, {
                             id: "tooltip-info-clear",
                             position: "bottom",
                             size: "small",
                             text: "Click to clear any server-side caches."
                         }), (0, Kr.jsx)(Is, {
                             name: "App Deployed At",
-                            value: zt.IsLocal() ? "running locally" + (Je.IsLocalCrossOrigin() ? " (cross-origin)" : "") : (null === (T = V.app) || void 0 === T ? void 0 : T.deployed) + Pr.FormatDuration(null === (A = V.app) || void 0 === A ? void 0 : A.deployed, new Date, !0, "just now", "|", "ago"),
+                            value: zt.IsLocal() ? "running locally" + (Je.IsLocalCrossOrigin() ? " (cross-origin)" : "") : (null === (U = X.app) || void 0 === U ? void 0 : U.deployed) + Pr.FormatDuration(null === (P = X.app) || void 0 === P ? void 0 : P.deployed, new Date, !0, "just now", "|", "ago"),
                             monospace: !0,
                             copy: !0,
                             optional: !0,
                             size: "2"
                         }), (0, Kr.jsx)(Is, {
                             name: "App Launched At",
-                            value: (null === (O = V.app) || void 0 === O ? void 0 : O.launched) + Pr.FormatDuration(null === (z = V.app) || void 0 === z ? void 0 : z.launched, new Date, !0, "just now", "|", "ago"),
+                            value: (null === (R = X.app) || void 0 === R ? void 0 : R.launched) + Pr.FormatDuration(null === (B = X.app) || void 0 === B ? void 0 : B.launched, new Date, !0, "just now", "|", "ago"),
                             monospace: !0,
                             size: "2"
                         }), (0, Kr.jsx)(Is, {
                             name: "Page Loaded At",
-                            value: q.get("page.loaded") + Pr.FormatDuration(q.get("page.loaded"), new Date, !0, "just now", "|", "ago"),
+                            value: $.get("page.loaded") + Pr.FormatDuration($.get("page.loaded"), new Date, !0, "just now", "|", "ago"),
                             monospace: !0,
                             size: "2"
                         }), (0, Kr.jsx)(Is, {
                             name: "Package",
-                            value: null === (U = V.app) || void 0 === U ? void 0 : U.package,
+                            value: null === (F = X.app) || void 0 === F ? void 0 : F.package,
                             monospace: !0,
                             size: "2"
                         }), (0, Kr.jsx)(Is, {
                             name: "Stage",
-                            value: null === (P = V.app) || void 0 === P ? void 0 : P.stage,
+                            value: null === (Y = X.app) || void 0 === Y ? void 0 : Y.stage,
                             monospace: !0,
                             size: "2"
                         }), (0, Kr.jsx)(Is, {
                             name: "Environment",
                             value: At.Current(),
                             monospace: !0,
                             size: "2"
                         }), (0, Kr.jsx)(Is, {
                             name: "Domain",
-                            value: null === (R = V.app) || void 0 === R ? void 0 : R.domain,
+                            value: null === (Q = X.app) || void 0 === Q ? void 0 : Q.domain,
                             monospace: !0,
                             size: "2"
                         }), (0, Kr.jsx)(Is, {
                             name: "Context",
-                            value: null === (B = V.app) || void 0 === B ? void 0 : B.context,
+                            value: null === (G = X.app) || void 0 === G ? void 0 : G.context,
                             monospace: !0,
                             size: "2"
                         }), (0, Kr.jsx)(Is, {
                             name: "Path",
-                            value: q.get("page.path"),
+                            value: $.get("page.path"),
                             monospace: !0,
                             size: "2"
                         }), (0, Kr.jsx)(Is, {
                             name: "Endpoint",
-                            value: q.get("page.endpoint"),
+                            value: $.get("page.endpoint"),
                             monospace: !0,
                             size: "2"
                         }), (0, Kr.jsx)(Is, {
                             name: "Client (React UI)",
                             value: kr.BaseUrl(),
                             monospace: !0,
                             size: "2"
@@ -60080,85 +60130,85 @@
                             name: "Server (React API)",
                             value: zt.BaseUrl(),
                             monospace: !0,
                             size: "2",
                             apiCache: !0
                         }), (0, Kr.jsx)(Is, {
                             name: "Checks File",
-                            value: null === (F = q.data) || void 0 === F || null === (Y = F.checks) || void 0 === Y ? void 0 : Y.file,
+                            value: null === (W = $.data) || void 0 === W || null === (H = W.checks) || void 0 === H ? void 0 : H.file,
                             monospace: !0,
                             size: "2"
-                        }), (null === (Q = V.app) || void 0 === Q ? void 0 : Q.accounts_file) && (0, Kr.jsx)(Is, {
+                        }), (null === (Z = X.app) || void 0 === Z ? void 0 : Z.accounts_file) && (0, Kr.jsx)(Is, {
                             name: "Accounts File",
-                            value: null === (G = V.app) || void 0 === G ? void 0 : G.accounts_file,
+                            value: null === (V = X.app) || void 0 === V ? void 0 : V.accounts_file,
                             monospace: !0,
                             size: "2"
-                        }), (null === (W = V.app) || void 0 === W ? void 0 : W.accounts_file_from_s3) && (0, Kr.jsx)(Is, {
+                        }), (null === (q = X.app) || void 0 === q ? void 0 : q.accounts_file_from_s3) && (0, Kr.jsx)(Is, {
                             name: "Accounts File (S3)",
-                            value: null === (H = V.app) || void 0 === H ? void 0 : H.accounts_file_from_s3,
+                            value: null === (J = X.app) || void 0 === J ? void 0 : J.accounts_file_from_s3,
                             monospace: !0,
                             size: "2"
                         })]
                     }), (0, Kr.jsx)(Ns, {
-                        info: q,
-                        title: "GAC: ".concat(q.get("gac.name")),
+                        info: $,
+                        title: "GAC: ".concat($.get("gac.name")),
                         show: !1,
-                        children: q.get("gac.values") ? (0, Kr.jsx)("span", {
-                            children: Object.keys(q.get("gac.values")).map((function(e) {
+                        children: $.get("gac.values") ? (0, Kr.jsx)("span", {
+                            children: Object.keys($.get("gac.values")).map((function(e) {
                                 return (0, Kr.jsx)(Is, {
                                     name: e,
-                                    value: q.get("gac.values")[e],
+                                    value: $.get("gac.values")[e],
                                     monospace: !0,
                                     copy: !0
                                 }, e)
                             }))
                         }) : (0, Kr.jsx)("span", {})
                     }), (0, Kr.jsx)(Ns, {
-                        info: q,
+                        info: $,
                         title: "Environment Variables",
                         show: !1,
-                        children: q.get("environ") ? (0, Kr.jsx)("span", {
-                            children: Object.keys(q.get("environ")).map((function(e) {
+                        children: $.get("environ") ? (0, Kr.jsx)("span", {
+                            children: Object.keys($.get("environ")).map((function(e) {
                                 return (0, Kr.jsx)(Is, {
                                     name: e,
-                                    value: q.get("environ")[e],
+                                    value: $.get("environ")[e],
                                     monospace: !0,
                                     copy: !0
                                 }, e)
                             }))
                         }) : (0, Kr.jsx)("span", {})
-                    }), (null === (Z = V.app) || void 0 === Z ? void 0 : Z.accounts) && (0, Kr.jsx)("div", {
+                    }), (null === (K = X.app) || void 0 === K ? void 0 : K.accounts) && (0, Kr.jsx)("div", {
                         className: "container",
                         style: {
                             marginTop: "4pt"
                         },
-                        children: ee ? (0, Kr.jsx)(Kr.Fragment, {
+                        children: oe ? (0, Kr.jsx)(Kr.Fragment, {
                             children: (0, Kr.jsx)(sa, {})
                         }) : (0, Kr.jsxs)(Kr.Fragment, {
                             children: [(0, Kr.jsx)("b", {
                                 onClick: function() {
-                                    return te(!0)
+                                    return ie(!0)
                                 },
                                 style: {
                                     cursor: "pointer"
                                 },
                                 children: "Show Accounts"
                             }), (0, Kr.jsxs)("div", {
                                 className: "box",
                                 children: ["Click ", (0, Kr.jsx)("b", {
                                     onClick: function() {
-                                        return te(!0)
+                                        return ie(!0)
                                     },
                                     style: {
                                         cursor: "pointer"
                                     },
                                     children: "here"
                                 }), " to ", (0, Kr.jsx)("span", {
                                     onClick: function() {
-                                        return te(!0)
+                                        return ie(!0)
                                     },
                                     style: {
                                         cursor: "pointer"
                                     },
                                     children: "show"
                                 }), "."]
                             })]
```

### Comparing `foursight_core-4.2.0.1b5/foursight_core/route_prefixes.py` & `foursight_core-4.2.0.1b6/foursight_core/route_prefixes.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.2.0.1b5/foursight_core/routes.py` & `foursight_core-4.2.0.1b6/foursight_core/routes.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.2.0.1b5/foursight_core/run_result.py` & `foursight_core-4.2.0.1b6/foursight_core/run_result.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.2.0.1b5/foursight_core/s3_connection.py` & `foursight_core-4.2.0.1b6/foursight_core/s3_connection.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.2.0.1b5/foursight_core/schedule_decorator.py` & `foursight_core-4.2.0.1b6/foursight_core/schedule_decorator.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.2.0.1b5/foursight_core/scripts/decrypt_accounts_file.py` & `foursight_core-4.2.0.1b6/foursight_core/scripts/decrypt_accounts_file.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.2.0.1b5/foursight_core/scripts/encrypt_accounts_file.py` & `foursight_core-4.2.0.1b6/foursight_core/scripts/encrypt_accounts_file.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.2.0.1b5/foursight_core/sqs_utils.py` & `foursight_core-4.2.0.1b6/foursight_core/sqs_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.2.0.1b5/foursight_core/stage.py` & `foursight_core-4.2.0.1b6/foursight_core/stage.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.2.0.1b5/foursight_core/templates/base.html` & `foursight_core-4.2.0.1b6/foursight_core/templates/base.html`

 * *Files identical despite different names*

### Comparing `foursight_core-4.2.0.1b5/foursight_core/templates/header.html` & `foursight_core-4.2.0.1b6/foursight_core/templates/header.html`

 * *Files identical despite different names*

### Comparing `foursight_core-4.2.0.1b5/foursight_core/templates/history.html` & `foursight_core-4.2.0.1b6/foursight_core/templates/history.html`

 * *Files identical despite different names*

### Comparing `foursight_core-4.2.0.1b5/foursight_core/templates/info.html` & `foursight_core-4.2.0.1b6/foursight_core/templates/info.html`

 * *Files identical despite different names*

### Comparing `foursight_core-4.2.0.1b5/foursight_core/templates/unused.html` & `foursight_core-4.2.0.1b6/foursight_core/templates/unused.html`

 * *Files identical despite different names*

### Comparing `foursight_core-4.2.0.1b5/foursight_core/templates/user.html` & `foursight_core-4.2.0.1b6/foursight_core/templates/user.html`

 * *Files identical despite different names*

### Comparing `foursight_core-4.2.0.1b5/foursight_core/templates/users.html` & `foursight_core-4.2.0.1b6/foursight_core/templates/users.html`

 * *Files identical despite different names*

### Comparing `foursight_core-4.2.0.1b5/foursight_core/templates/view_checks.html` & `foursight_core-4.2.0.1b6/foursight_core/templates/view_checks.html`

 * *Files identical despite different names*

### Comparing `foursight_core-4.2.0.1b5/foursight_core/templates/view_groups.html` & `foursight_core-4.2.0.1b6/foursight_core/templates/view_groups.html`

 * *Files identical despite different names*

### Comparing `foursight_core-4.2.0.1b5/pyproject.toml` & `foursight_core-4.2.0.1b6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "foursight-core"
-version = "4.2.0.1b5"  # to become 4.2.0
+version = "4.2.0.1b6"  # to become 4.2.0
 description = "Serverless Chalice Application for Monitoring"
 authors = ["4DN-DCIC Team <support@4dnucleome.org>"]
 license = "MIT"
 packages = [
   { include = "foursight_core" },
   { include = "checks", from = "foursight_core" },
   { include = "helpers", from = "foursight_core/checks" }
```

### Comparing `foursight_core-4.2.0.1b5/setup.py` & `foursight_core-4.2.0.1b6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -47,15 +47,15 @@
                      'encrypt-accounts-file = '
                      'foursight_core.scripts.encrypt_accounts_file:main',
                      'publish-to-pypi = '
                      'dcicutils.scripts.publish_to_pypi:main']}
 
 setup_kwargs = {
     'name': 'foursight-core',
-    'version': '4.2.0.1b5',
+    'version': '4.2.0.1b6',
     'description': 'Serverless Chalice Application for Monitoring',
     'long_description': 'None',
     'author': '4DN-DCIC Team',
     'author_email': 'support@4dnucleome.org',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `foursight_core-4.2.0.1b5/PKG-INFO` & `foursight_core-4.2.0.1b6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: foursight-core
-Version: 4.2.0.1b5
+Version: 4.2.0.1b6
 Summary: Serverless Chalice Application for Monitoring
 License: MIT
 Author: 4DN-DCIC Team
 Author-email: support@4dnucleome.org
 Requires-Python: >=3.7,<3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

