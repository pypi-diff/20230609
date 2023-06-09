# Comparing `tmp/hdn-research-environment-2.1.4.tar.gz` & `tmp/hdn-research-environment-2.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/hdn-research-environment-2.1.4.tar", last modified: Fri Jun  9 09:49:12 2023, max compression
+gzip compressed data, was "dist/hdn-research-environment-2.1.5.tar", last modified: Fri Jun  9 10:25:21 2023, max compression
```

## Comparing `hdn-research-environment-2.1.4.tar` & `hdn-research-environment-2.1.5.tar`

### file list

```diff
@@ -1,95 +1,96 @@
-drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-09 09:49:12.000000 hdn-research-environment-2.1.4/
--rw-r--r--   0 karolszuster   (501) staff       (20)     1551 2022-03-29 08:15:30.000000 hdn-research-environment-2.1.4/LICENSE
--rw-r--r--   0 karolszuster   (501) staff       (20)      115 2022-03-29 08:32:41.000000 hdn-research-environment-2.1.4/MANIFEST.in
--rw-r--r--   0 karolszuster   (501) staff       (20)      995 2023-06-09 09:49:12.000000 hdn-research-environment-2.1.4/PKG-INFO
--rw-r--r--   0 karolszuster   (501) staff       (20)       90 2022-03-29 07:59:09.000000 hdn-research-environment-2.1.4/README.md
-drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-09 09:49:12.000000 hdn-research-environment-2.1.4/environment/
--rw-r--r--   0 karolszuster   (501) staff       (20)        0 2022-03-29 08:08:24.000000 hdn-research-environment-2.1.4/environment/__init__.py
-drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-09 09:49:12.000000 hdn-research-environment-2.1.4/environment/api/
--rw-r--r--   0 karolszuster   (501) staff       (20)        0 2023-05-29 11:59:00.000000 hdn-research-environment-2.1.4/environment/api/__init__.py
-drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-09 09:49:12.000000 hdn-research-environment-2.1.4/environment/api/v1/
--rw-r--r--   0 karolszuster   (501) staff       (20)     3242 2023-05-29 11:59:00.000000 hdn-research-environment-2.1.4/environment/api/v1/__init__.py
--rw-r--r--   0 karolszuster   (501) staff       (20)      640 2023-05-29 11:59:00.000000 hdn-research-environment-2.1.4/environment/api/v1/auth.py
--rw-r--r--   0 karolszuster   (501) staff       (20)      700 2023-05-29 11:59:00.000000 hdn-research-environment-2.1.4/environment/api/v1/decorators.py
-drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-09 09:49:12.000000 hdn-research-environment-2.1.4/environment/api/v2/
--rw-r--r--   0 karolszuster   (501) staff       (20)     1572 2023-05-29 11:59:00.000000 hdn-research-environment-2.1.4/environment/api/v2/__init__.py
--rw-r--r--   0 karolszuster   (501) staff       (20)      942 2023-05-30 18:52:36.000000 hdn-research-environment-2.1.4/environment/api/v2/decorators.py
--rw-r--r--   0 karolszuster   (501) staff       (20)      154 2022-03-29 08:08:24.000000 hdn-research-environment-2.1.4/environment/apps.py
--rw-r--r--   0 karolszuster   (501) staff       (20)     3175 2023-06-09 09:19:00.000000 hdn-research-environment-2.1.4/environment/constants.py
--rw-r--r--   0 karolszuster   (501) staff       (20)     1005 2023-05-29 11:59:00.000000 hdn-research-environment-2.1.4/environment/decorators.py
--rw-r--r--   0 karolszuster   (501) staff       (20)     1878 2023-05-29 11:59:00.000000 hdn-research-environment-2.1.4/environment/deserializers.py
--rw-r--r--   0 karolszuster   (501) staff       (20)     2928 2023-05-29 12:32:30.000000 hdn-research-environment-2.1.4/environment/entities.py
--rw-r--r--   0 karolszuster   (501) staff       (20)      818 2023-05-29 11:59:00.000000 hdn-research-environment-2.1.4/environment/exceptions.py
--rw-r--r--   0 karolszuster   (501) staff       (20)     3711 2023-06-05 16:43:26.000000 hdn-research-environment-2.1.4/environment/forms.py
--rw-r--r--   0 karolszuster   (501) staff       (20)     1720 2023-06-06 14:41:05.000000 hdn-research-environment-2.1.4/environment/mailers.py
--rw-r--r--   0 karolszuster   (501) staff       (20)      155 2022-03-29 08:08:24.000000 hdn-research-environment-2.1.4/environment/managers.py
-drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-09 09:49:12.000000 hdn-research-environment-2.1.4/environment/migrations/
--rw-r--r--   0 karolszuster   (501) staff       (20)     1443 2023-05-29 11:59:00.000000 hdn-research-environment-2.1.4/environment/migrations/0001_initial.py
--rw-r--r--   0 karolszuster   (501) staff       (20)     1579 2023-05-29 11:59:00.000000 hdn-research-environment-2.1.4/environment/migrations/0002_billingsetup.py
--rw-r--r--   0 karolszuster   (501) staff       (20)      403 2023-05-29 11:59:00.000000 hdn-research-environment-2.1.4/environment/migrations/0003_cloudidentity_is_workspace_done.py
--rw-r--r--   0 karolszuster   (501) staff       (20)      420 2023-05-29 11:59:00.000000 hdn-research-environment-2.1.4/environment/migrations/0004_auto_20220309_0330.py
--rw-r--r--   0 karolszuster   (501) staff       (20)     2220 2023-05-29 11:59:00.000000 hdn-research-environment-2.1.4/environment/migrations/0005_workflow.py
--rw-r--r--   0 karolszuster   (501) staff       (20)      394 2023-05-29 11:59:00.000000 hdn-research-environment-2.1.4/environment/migrations/0006_delete_billingsetup.py
--rw-r--r--   0 karolszuster   (501) staff       (20)     2347 2023-05-29 11:59:00.000000 hdn-research-environment-2.1.4/environment/migrations/0007_billingaccountsharinginvite.py
--rw-r--r--   0 karolszuster   (501) staff       (20)      476 2023-05-29 11:59:00.000000 hdn-research-environment-2.1.4/environment/migrations/0008_workflow_workspace_name.py
--rw-r--r--   0 karolszuster   (501) staff       (20)      420 2023-05-29 11:59:00.000000 hdn-research-environment-2.1.4/environment/migrations/0009_billingaccountsharinginvite_is_revoked.py
--rw-r--r--   0 karolszuster   (501) staff       (20)     1364 2023-05-31 14:40:16.000000 hdn-research-environment-2.1.4/environment/migrations/0010_alter_workflow_project_alter_workflow_type_and_more.py
--rw-r--r--   0 karolszuster   (501) staff       (20)        0 2022-03-29 08:08:24.000000 hdn-research-environment-2.1.4/environment/migrations/__init__.py
--rw-r--r--   0 karolszuster   (501) staff       (20)     2518 2023-05-31 14:40:16.000000 hdn-research-environment-2.1.4/environment/models.py
--rw-r--r--   0 karolszuster   (501) staff       (20)    19730 2023-06-09 09:19:00.000000 hdn-research-environment-2.1.4/environment/services.py
--rw-r--r--   0 karolszuster   (501) staff       (20)     4545 2023-06-02 15:32:09.000000 hdn-research-environment-2.1.4/environment/signals.py
-drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-09 09:49:12.000000 hdn-research-environment-2.1.4/environment/static/
-drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-09 09:49:12.000000 hdn-research-environment-2.1.4/environment/static/environment/
-drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-09 09:49:12.000000 hdn-research-environment-2.1.4/environment/static/environment/css/
--rw-r--r--   0 karolszuster   (501) staff       (20)      342 2023-02-22 22:00:03.000000 hdn-research-environment-2.1.4/environment/static/environment/css/create_research_environment.css
--rw-r--r--   0 karolszuster   (501) staff       (20)     6583 2022-03-29 08:08:24.000000 hdn-research-environment-2.1.4/environment/static/environment/css/environment-base.css
--rw-r--r--   0 karolszuster   (501) staff       (20)      117 2023-05-29 11:59:00.000000 hdn-research-environment-2.1.4/environment/static/environment/css/manage_billing_account.css
-drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-09 09:49:12.000000 hdn-research-environment-2.1.4/environment/static/environment/js/
--rw-r--r--   0 karolszuster   (501) staff       (20)      564 2022-03-30 12:50:58.000000 hdn-research-environment-2.1.4/environment/static/environment/js/cookie.js
--rw-r--r--   0 karolszuster   (501) staff       (20)      516 2023-05-29 11:59:00.000000 hdn-research-environment-2.1.4/environment/static/environment/js/gpu_disabling.js
--rw-r--r--   0 karolszuster   (501) staff       (20)     3154 2023-05-29 11:59:00.000000 hdn-research-environment-2.1.4/environment/static/environment/js/pricing_change.js
--rw-r--r--   0 karolszuster   (501) staff       (20)     2652 2023-06-05 06:46:01.000000 hdn-research-environment-2.1.4/environment/tasks.py
-drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-09 09:49:12.000000 hdn-research-environment-2.1.4/environment/templates/
-drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-09 09:49:12.000000 hdn-research-environment-2.1.4/environment/templates/environment/
--rw-r--r--   0 karolszuster   (501) staff       (20)     8010 2023-06-09 09:47:58.000000 hdn-research-environment-2.1.4/environment/templates/environment/_available_environments_list.html
--rw-r--r--   0 karolszuster   (501) staff       (20)     1423 2023-06-02 15:30:03.000000 hdn-research-environment-2.1.4/environment/templates/environment/_available_projects_list.html
--rw-r--r--   0 karolszuster   (501) staff       (20)     1916 2023-06-05 16:02:13.000000 hdn-research-environment-2.1.4/environment/templates/environment/_billing_accounts_list.html
--rw-r--r--   0 karolszuster   (501) staff       (20)      801 2022-03-30 12:51:12.000000 hdn-research-environment-2.1.4/environment/templates/environment/base_environment_home.html
--rw-r--r--   0 karolszuster   (501) staff       (20)     4327 2023-05-29 11:59:00.000000 hdn-research-environment-2.1.4/environment/templates/environment/create_research_environment.html
--rw-r--r--   0 karolszuster   (501) staff       (20)     1018 2023-05-29 11:59:00.000000 hdn-research-environment-2.1.4/environment/templates/environment/create_workspace.html
-drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-09 09:49:12.000000 hdn-research-environment-2.1.4/environment/templates/environment/email/
--rw-r--r--   0 karolszuster   (501) staff       (20)      272 2023-06-09 09:19:00.000000 hdn-research-environment-2.1.4/environment/templates/environment/email/billing_sharing_confirmation.html
--rw-r--r--   0 karolszuster   (501) staff       (20)      351 2023-06-05 06:46:01.000000 hdn-research-environment-2.1.4/environment/templates/environment/email/environment_access_expired.html
--rw-r--r--   0 karolszuster   (501) staff       (20)     1455 2023-05-29 11:58:57.000000 hdn-research-environment-2.1.4/environment/templates/environment/identity_provisioning.html
--rw-r--r--   0 karolszuster   (501) staff       (20)     5942 2023-06-05 06:46:01.000000 hdn-research-environment-2.1.4/environment/templates/environment/manage_billing_account.html
--rw-r--r--   0 karolszuster   (501) staff       (20)      562 2023-06-05 16:02:13.000000 hdn-research-environment-2.1.4/environment/templates/environment/manage_shared_billing_invitation.html
--rw-r--r--   0 karolszuster   (501) staff       (20)     3870 2023-06-05 16:02:13.000000 hdn-research-environment-2.1.4/environment/templates/environment/research_environments.html
-drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-09 09:49:12.000000 hdn-research-environment-2.1.4/environment/templates/tag/
--rw-r--r--   0 karolszuster   (501) staff       (20)      241 2022-03-29 08:08:24.000000 hdn-research-environment-2.1.4/environment/templates/tag/environment_action_button.html
--rw-r--r--   0 karolszuster   (501) staff       (20)     1473 2023-06-06 14:41:05.000000 hdn-research-environment-2.1.4/environment/templates/tag/environment_modal_button.html
-drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-09 09:49:12.000000 hdn-research-environment-2.1.4/environment/templatetags/
--rw-r--r--   0 karolszuster   (501) staff       (20)        0 2022-03-29 08:08:24.000000 hdn-research-environment-2.1.4/environment/templatetags/__init__.py
--rw-r--r--   0 karolszuster   (501) staff       (20)     3518 2023-06-05 16:02:13.000000 hdn-research-environment-2.1.4/environment/templatetags/action_buttons.py
-drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-09 09:49:12.000000 hdn-research-environment-2.1.4/environment/tests/
--rw-r--r--   0 karolszuster   (501) staff       (20)        0 2022-03-29 08:08:24.000000 hdn-research-environment-2.1.4/environment/tests/__init__.py
--rw-r--r--   0 karolszuster   (501) staff       (20)      645 2023-05-29 11:59:00.000000 hdn-research-environment-2.1.4/environment/tests/helpers.py
--rw-r--r--   0 karolszuster   (501) staff       (20)    12158 2023-05-29 11:59:00.000000 hdn-research-environment-2.1.4/environment/tests/mocks.py
--rw-r--r--   0 karolszuster   (501) staff       (20)     3007 2023-05-29 11:59:00.000000 hdn-research-environment-2.1.4/environment/tests/test_decorators.py
--rw-r--r--   0 karolszuster   (501) staff       (20)    10693 2023-05-29 11:59:00.000000 hdn-research-environment-2.1.4/environment/tests/test_services.py
--rw-r--r--   0 karolszuster   (501) staff       (20)     5328 2023-05-29 11:59:00.000000 hdn-research-environment-2.1.4/environment/tests/test_signals.py
--rw-r--r--   0 karolszuster   (501) staff       (20)     2909 2023-05-29 11:59:00.000000 hdn-research-environment-2.1.4/environment/tests/test_utilities.py
--rw-r--r--   0 karolszuster   (501) staff       (20)      640 2023-05-29 11:58:39.000000 hdn-research-environment-2.1.4/environment/tests/test_validators.py
--rw-r--r--   0 karolszuster   (501) staff       (20)     3380 2023-05-29 11:59:00.000000 hdn-research-environment-2.1.4/environment/tests/test_views.py
--rw-r--r--   0 karolszuster   (501) staff       (20)     1555 2023-05-29 11:59:00.000000 hdn-research-environment-2.1.4/environment/urls.py
--rw-r--r--   0 karolszuster   (501) staff       (20)     1135 2023-05-29 11:59:00.000000 hdn-research-environment-2.1.4/environment/utilities.py
--rw-r--r--   0 karolszuster   (501) staff       (20)      236 2022-03-29 08:08:24.000000 hdn-research-environment-2.1.4/environment/validators.py
--rw-r--r--   0 karolszuster   (501) staff       (20)    14146 2023-06-09 09:47:58.000000 hdn-research-environment-2.1.4/environment/views.py
-drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-09 09:49:12.000000 hdn-research-environment-2.1.4/hdn_research_environment.egg-info/
--rw-r--r--   0 karolszuster   (501) staff       (20)      995 2023-06-09 09:49:12.000000 hdn-research-environment-2.1.4/hdn_research_environment.egg-info/PKG-INFO
--rw-r--r--   0 karolszuster   (501) staff       (20)     3100 2023-06-09 09:49:12.000000 hdn-research-environment-2.1.4/hdn_research_environment.egg-info/SOURCES.txt
--rw-r--r--   0 karolszuster   (501) staff       (20)        1 2023-06-09 09:49:12.000000 hdn-research-environment-2.1.4/hdn_research_environment.egg-info/dependency_links.txt
--rw-r--r--   0 karolszuster   (501) staff       (20)       84 2023-06-09 09:49:12.000000 hdn-research-environment-2.1.4/hdn_research_environment.egg-info/requires.txt
--rw-r--r--   0 karolszuster   (501) staff       (20)       12 2023-06-09 09:49:12.000000 hdn-research-environment-2.1.4/hdn_research_environment.egg-info/top_level.txt
--rw-r--r--   0 karolszuster   (501) staff       (20)      109 2022-03-29 08:03:11.000000 hdn-research-environment-2.1.4/pyproject.toml
--rw-r--r--   0 karolszuster   (501) staff       (20)     1056 2023-06-09 09:49:12.000000 hdn-research-environment-2.1.4/setup.cfg
--rw-r--r--   0 karolszuster   (501) staff       (20)       38 2022-03-29 08:03:11.000000 hdn-research-environment-2.1.4/setup.py
+drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-09 10:25:21.000000 hdn-research-environment-2.1.5/
+-rw-r--r--   0 karolszuster   (501) staff       (20)     1551 2022-03-29 08:15:30.000000 hdn-research-environment-2.1.5/LICENSE
+-rw-r--r--   0 karolszuster   (501) staff       (20)      115 2022-03-29 08:32:41.000000 hdn-research-environment-2.1.5/MANIFEST.in
+-rw-r--r--   0 karolszuster   (501) staff       (20)      995 2023-06-09 10:25:21.000000 hdn-research-environment-2.1.5/PKG-INFO
+-rw-r--r--   0 karolszuster   (501) staff       (20)       90 2022-03-29 07:59:09.000000 hdn-research-environment-2.1.5/README.md
+drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-09 10:25:21.000000 hdn-research-environment-2.1.5/environment/
+-rw-r--r--   0 karolszuster   (501) staff       (20)        0 2022-03-29 08:08:24.000000 hdn-research-environment-2.1.5/environment/__init__.py
+drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-09 10:25:21.000000 hdn-research-environment-2.1.5/environment/api/
+-rw-r--r--   0 karolszuster   (501) staff       (20)        0 2023-05-29 11:59:00.000000 hdn-research-environment-2.1.5/environment/api/__init__.py
+drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-09 10:25:21.000000 hdn-research-environment-2.1.5/environment/api/v1/
+-rw-r--r--   0 karolszuster   (501) staff       (20)     3242 2023-05-29 11:59:00.000000 hdn-research-environment-2.1.5/environment/api/v1/__init__.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)      640 2023-05-29 11:59:00.000000 hdn-research-environment-2.1.5/environment/api/v1/auth.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)      700 2023-05-29 11:59:00.000000 hdn-research-environment-2.1.5/environment/api/v1/decorators.py
+drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-09 10:25:21.000000 hdn-research-environment-2.1.5/environment/api/v2/
+-rw-r--r--   0 karolszuster   (501) staff       (20)     1572 2023-05-29 11:59:00.000000 hdn-research-environment-2.1.5/environment/api/v2/__init__.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)      942 2023-05-30 18:52:36.000000 hdn-research-environment-2.1.5/environment/api/v2/decorators.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)      154 2022-03-29 08:08:24.000000 hdn-research-environment-2.1.5/environment/apps.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)     3175 2023-06-09 09:19:00.000000 hdn-research-environment-2.1.5/environment/constants.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)     1005 2023-05-29 11:59:00.000000 hdn-research-environment-2.1.5/environment/decorators.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)     1878 2023-05-29 11:59:00.000000 hdn-research-environment-2.1.5/environment/deserializers.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)     2928 2023-05-29 12:32:30.000000 hdn-research-environment-2.1.5/environment/entities.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)      818 2023-05-29 11:59:00.000000 hdn-research-environment-2.1.5/environment/exceptions.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)     3711 2023-06-05 16:43:26.000000 hdn-research-environment-2.1.5/environment/forms.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)     1720 2023-06-06 14:41:05.000000 hdn-research-environment-2.1.5/environment/mailers.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)      155 2022-03-29 08:08:24.000000 hdn-research-environment-2.1.5/environment/managers.py
+drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-09 10:25:21.000000 hdn-research-environment-2.1.5/environment/migrations/
+-rw-r--r--   0 karolszuster   (501) staff       (20)     1443 2023-05-29 11:59:00.000000 hdn-research-environment-2.1.5/environment/migrations/0001_initial.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)     1579 2023-05-29 11:59:00.000000 hdn-research-environment-2.1.5/environment/migrations/0002_billingsetup.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)      403 2023-05-29 11:59:00.000000 hdn-research-environment-2.1.5/environment/migrations/0003_cloudidentity_is_workspace_done.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)      420 2023-05-29 11:59:00.000000 hdn-research-environment-2.1.5/environment/migrations/0004_auto_20220309_0330.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)     2220 2023-05-29 11:59:00.000000 hdn-research-environment-2.1.5/environment/migrations/0005_workflow.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)      394 2023-05-29 11:59:00.000000 hdn-research-environment-2.1.5/environment/migrations/0006_delete_billingsetup.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)     2347 2023-05-29 11:59:00.000000 hdn-research-environment-2.1.5/environment/migrations/0007_billingaccountsharinginvite.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)      476 2023-05-29 11:59:00.000000 hdn-research-environment-2.1.5/environment/migrations/0008_workflow_workspace_name.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)      420 2023-05-29 11:59:00.000000 hdn-research-environment-2.1.5/environment/migrations/0009_billingaccountsharinginvite_is_revoked.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)     1364 2023-05-31 14:40:16.000000 hdn-research-environment-2.1.5/environment/migrations/0010_alter_workflow_project_alter_workflow_type_and_more.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)        0 2022-03-29 08:08:24.000000 hdn-research-environment-2.1.5/environment/migrations/__init__.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)     2518 2023-05-31 14:40:16.000000 hdn-research-environment-2.1.5/environment/models.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)    19730 2023-06-09 09:19:00.000000 hdn-research-environment-2.1.5/environment/services.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)     4545 2023-06-02 15:32:09.000000 hdn-research-environment-2.1.5/environment/signals.py
+drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-09 10:25:21.000000 hdn-research-environment-2.1.5/environment/static/
+drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-09 10:25:21.000000 hdn-research-environment-2.1.5/environment/static/environment/
+drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-09 10:25:21.000000 hdn-research-environment-2.1.5/environment/static/environment/css/
+-rw-r--r--   0 karolszuster   (501) staff       (20)      342 2023-02-22 22:00:03.000000 hdn-research-environment-2.1.5/environment/static/environment/css/create_research_environment.css
+-rw-r--r--   0 karolszuster   (501) staff       (20)     6583 2022-03-29 08:08:24.000000 hdn-research-environment-2.1.5/environment/static/environment/css/environment-base.css
+-rw-r--r--   0 karolszuster   (501) staff       (20)      117 2023-05-29 11:59:00.000000 hdn-research-environment-2.1.5/environment/static/environment/css/manage_billing_account.css
+drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-09 10:25:21.000000 hdn-research-environment-2.1.5/environment/static/environment/js/
+-rw-r--r--   0 karolszuster   (501) staff       (20)      564 2022-03-30 12:50:58.000000 hdn-research-environment-2.1.5/environment/static/environment/js/cookie.js
+-rw-r--r--   0 karolszuster   (501) staff       (20)      291 2023-06-09 10:25:06.000000 hdn-research-environment-2.1.5/environment/static/environment/js/forms.js
+-rw-r--r--   0 karolszuster   (501) staff       (20)      516 2023-05-29 11:59:00.000000 hdn-research-environment-2.1.5/environment/static/environment/js/gpu_disabling.js
+-rw-r--r--   0 karolszuster   (501) staff       (20)     3154 2023-05-29 11:59:00.000000 hdn-research-environment-2.1.5/environment/static/environment/js/pricing_change.js
+-rw-r--r--   0 karolszuster   (501) staff       (20)     2652 2023-06-05 06:46:01.000000 hdn-research-environment-2.1.5/environment/tasks.py
+drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-09 10:25:21.000000 hdn-research-environment-2.1.5/environment/templates/
+drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-09 10:25:21.000000 hdn-research-environment-2.1.5/environment/templates/environment/
+-rw-r--r--   0 karolszuster   (501) staff       (20)     8010 2023-06-09 09:47:58.000000 hdn-research-environment-2.1.5/environment/templates/environment/_available_environments_list.html
+-rw-r--r--   0 karolszuster   (501) staff       (20)     1423 2023-06-02 15:30:03.000000 hdn-research-environment-2.1.5/environment/templates/environment/_available_projects_list.html
+-rw-r--r--   0 karolszuster   (501) staff       (20)     1916 2023-06-05 16:02:13.000000 hdn-research-environment-2.1.5/environment/templates/environment/_billing_accounts_list.html
+-rw-r--r--   0 karolszuster   (501) staff       (20)      864 2023-06-09 10:25:06.000000 hdn-research-environment-2.1.5/environment/templates/environment/base_environment_home.html
+-rw-r--r--   0 karolszuster   (501) staff       (20)     4417 2023-06-09 10:25:06.000000 hdn-research-environment-2.1.5/environment/templates/environment/create_research_environment.html
+-rw-r--r--   0 karolszuster   (501) staff       (20)     1149 2023-06-09 10:25:06.000000 hdn-research-environment-2.1.5/environment/templates/environment/create_workspace.html
+drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-09 10:25:21.000000 hdn-research-environment-2.1.5/environment/templates/environment/email/
+-rw-r--r--   0 karolszuster   (501) staff       (20)      272 2023-06-09 09:19:00.000000 hdn-research-environment-2.1.5/environment/templates/environment/email/billing_sharing_confirmation.html
+-rw-r--r--   0 karolszuster   (501) staff       (20)      351 2023-06-05 06:46:01.000000 hdn-research-environment-2.1.5/environment/templates/environment/email/environment_access_expired.html
+-rw-r--r--   0 karolszuster   (501) staff       (20)     1455 2023-05-29 11:58:57.000000 hdn-research-environment-2.1.5/environment/templates/environment/identity_provisioning.html
+-rw-r--r--   0 karolszuster   (501) staff       (20)     5942 2023-06-05 06:46:01.000000 hdn-research-environment-2.1.5/environment/templates/environment/manage_billing_account.html
+-rw-r--r--   0 karolszuster   (501) staff       (20)      562 2023-06-05 16:02:13.000000 hdn-research-environment-2.1.5/environment/templates/environment/manage_shared_billing_invitation.html
+-rw-r--r--   0 karolszuster   (501) staff       (20)     3870 2023-06-05 16:02:13.000000 hdn-research-environment-2.1.5/environment/templates/environment/research_environments.html
+drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-09 10:25:21.000000 hdn-research-environment-2.1.5/environment/templates/tag/
+-rw-r--r--   0 karolszuster   (501) staff       (20)      241 2022-03-29 08:08:24.000000 hdn-research-environment-2.1.5/environment/templates/tag/environment_action_button.html
+-rw-r--r--   0 karolszuster   (501) staff       (20)     1473 2023-06-06 14:41:05.000000 hdn-research-environment-2.1.5/environment/templates/tag/environment_modal_button.html
+drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-09 10:25:21.000000 hdn-research-environment-2.1.5/environment/templatetags/
+-rw-r--r--   0 karolszuster   (501) staff       (20)        0 2022-03-29 08:08:24.000000 hdn-research-environment-2.1.5/environment/templatetags/__init__.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)     3518 2023-06-05 16:02:13.000000 hdn-research-environment-2.1.5/environment/templatetags/action_buttons.py
+drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-09 10:25:21.000000 hdn-research-environment-2.1.5/environment/tests/
+-rw-r--r--   0 karolszuster   (501) staff       (20)        0 2022-03-29 08:08:24.000000 hdn-research-environment-2.1.5/environment/tests/__init__.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)      645 2023-05-29 11:59:00.000000 hdn-research-environment-2.1.5/environment/tests/helpers.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)    12158 2023-05-29 11:59:00.000000 hdn-research-environment-2.1.5/environment/tests/mocks.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)     3007 2023-05-29 11:59:00.000000 hdn-research-environment-2.1.5/environment/tests/test_decorators.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)    10693 2023-05-29 11:59:00.000000 hdn-research-environment-2.1.5/environment/tests/test_services.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)     5328 2023-05-29 11:59:00.000000 hdn-research-environment-2.1.5/environment/tests/test_signals.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)     2909 2023-05-29 11:59:00.000000 hdn-research-environment-2.1.5/environment/tests/test_utilities.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)      640 2023-05-29 11:58:39.000000 hdn-research-environment-2.1.5/environment/tests/test_validators.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)     3380 2023-05-29 11:59:00.000000 hdn-research-environment-2.1.5/environment/tests/test_views.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)     1555 2023-05-29 11:59:00.000000 hdn-research-environment-2.1.5/environment/urls.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)     1135 2023-05-29 11:59:00.000000 hdn-research-environment-2.1.5/environment/utilities.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)      236 2022-03-29 08:08:24.000000 hdn-research-environment-2.1.5/environment/validators.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)    14146 2023-06-09 09:47:58.000000 hdn-research-environment-2.1.5/environment/views.py
+drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-09 10:25:21.000000 hdn-research-environment-2.1.5/hdn_research_environment.egg-info/
+-rw-r--r--   0 karolszuster   (501) staff       (20)      995 2023-06-09 10:25:21.000000 hdn-research-environment-2.1.5/hdn_research_environment.egg-info/PKG-INFO
+-rw-r--r--   0 karolszuster   (501) staff       (20)     3143 2023-06-09 10:25:21.000000 hdn-research-environment-2.1.5/hdn_research_environment.egg-info/SOURCES.txt
+-rw-r--r--   0 karolszuster   (501) staff       (20)        1 2023-06-09 10:25:21.000000 hdn-research-environment-2.1.5/hdn_research_environment.egg-info/dependency_links.txt
+-rw-r--r--   0 karolszuster   (501) staff       (20)       84 2023-06-09 10:25:21.000000 hdn-research-environment-2.1.5/hdn_research_environment.egg-info/requires.txt
+-rw-r--r--   0 karolszuster   (501) staff       (20)       12 2023-06-09 10:25:21.000000 hdn-research-environment-2.1.5/hdn_research_environment.egg-info/top_level.txt
+-rw-r--r--   0 karolszuster   (501) staff       (20)      109 2022-03-29 08:03:11.000000 hdn-research-environment-2.1.5/pyproject.toml
+-rw-r--r--   0 karolszuster   (501) staff       (20)     1056 2023-06-09 10:25:21.000000 hdn-research-environment-2.1.5/setup.cfg
+-rw-r--r--   0 karolszuster   (501) staff       (20)       38 2022-03-29 08:03:11.000000 hdn-research-environment-2.1.5/setup.py
```

### Comparing `hdn-research-environment-2.1.4/LICENSE` & `hdn-research-environment-2.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.1.4/PKG-INFO` & `hdn-research-environment-2.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: hdn-research-environment
-Version: 2.1.4
+Version: 2.1.5
 Summary: A Django app for supporting cloud-native research environments
 Home-page: https://www.healthdatanexus.ai/
 Author: Your Name
 Author-email: yourname@example.com
 License: BSD-3-Clause  # Example license
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `hdn-research-environment-2.1.4/environment/api/v1/__init__.py` & `hdn-research-environment-2.1.5/environment/api/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.1.4/environment/api/v1/auth.py` & `hdn-research-environment-2.1.5/environment/api/v1/auth.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.1.4/environment/api/v1/decorators.py` & `hdn-research-environment-2.1.5/environment/api/v1/decorators.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.1.4/environment/api/v2/__init__.py` & `hdn-research-environment-2.1.5/environment/api/v2/__init__.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.1.4/environment/api/v2/decorators.py` & `hdn-research-environment-2.1.5/environment/api/v2/decorators.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.1.4/environment/constants.py` & `hdn-research-environment-2.1.5/environment/constants.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.1.4/environment/decorators.py` & `hdn-research-environment-2.1.5/environment/decorators.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.1.4/environment/deserializers.py` & `hdn-research-environment-2.1.5/environment/deserializers.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.1.4/environment/entities.py` & `hdn-research-environment-2.1.5/environment/entities.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.1.4/environment/exceptions.py` & `hdn-research-environment-2.1.5/environment/exceptions.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.1.4/environment/forms.py` & `hdn-research-environment-2.1.5/environment/forms.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.1.4/environment/mailers.py` & `hdn-research-environment-2.1.5/environment/mailers.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.1.4/environment/migrations/0001_initial.py` & `hdn-research-environment-2.1.5/environment/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.1.4/environment/migrations/0002_billingsetup.py` & `hdn-research-environment-2.1.5/environment/migrations/0002_billingsetup.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.1.4/environment/migrations/0005_workflow.py` & `hdn-research-environment-2.1.5/environment/migrations/0005_workflow.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.1.4/environment/migrations/0007_billingaccountsharinginvite.py` & `hdn-research-environment-2.1.5/environment/migrations/0007_billingaccountsharinginvite.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.1.4/environment/migrations/0010_alter_workflow_project_alter_workflow_type_and_more.py` & `hdn-research-environment-2.1.5/environment/migrations/0010_alter_workflow_project_alter_workflow_type_and_more.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.1.4/environment/models.py` & `hdn-research-environment-2.1.5/environment/models.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.1.4/environment/services.py` & `hdn-research-environment-2.1.5/environment/services.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.1.4/environment/signals.py` & `hdn-research-environment-2.1.5/environment/signals.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.1.4/environment/static/environment/css/environment-base.css` & `hdn-research-environment-2.1.5/environment/static/environment/css/environment-base.css`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.1.4/environment/static/environment/js/cookie.js` & `hdn-research-environment-2.1.5/environment/static/environment/js/cookie.js`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.1.4/environment/static/environment/js/gpu_disabling.js` & `hdn-research-environment-2.1.5/environment/static/environment/js/gpu_disabling.js`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.1.4/environment/static/environment/js/pricing_change.js` & `hdn-research-environment-2.1.5/environment/static/environment/js/pricing_change.js`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.1.4/environment/tasks.py` & `hdn-research-environment-2.1.5/environment/tasks.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.1.4/environment/templates/environment/_available_environments_list.html` & `hdn-research-environment-2.1.5/environment/templates/environment/_available_environments_list.html`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.1.4/environment/templates/environment/_available_projects_list.html` & `hdn-research-environment-2.1.5/environment/templates/environment/_available_projects_list.html`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.1.4/environment/templates/environment/_billing_accounts_list.html` & `hdn-research-environment-2.1.5/environment/templates/environment/_billing_accounts_list.html`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.1.4/environment/templates/environment/base_environment_home.html` & `hdn-research-environment-2.1.5/environment/templates/environment/base_environment_home.html`

 * *Files 4% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 
 {% block local_css %}
 <link rel="stylesheet" type="text/css" href="{% static 'environment/css/environment-base.css' %}">
 {% endblock %}
 
 {% block local_js_top %}
 <script src="{% static 'environment/js/cookie.js' %}"></script>
+<script src="{% static 'environment/js/forms.js' %}"></script>
 {% endblock %}
 
 {% block content %}
     <div class="container">
       {% include "message_snippet.html" %}
         <div class="jumbotron">
           <h1>Research Environments Home</h1>
```

### Comparing `hdn-research-environment-2.1.4/environment/templates/environment/create_research_environment.html` & `hdn-research-environment-2.1.5/environment/templates/environment/create_research_environment.html`

 * *Files 3% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 {% load project_templatetags %}
 
 {% block title %}Create Research Environment{% endblock %}
 
 {% block local_js_top %}
 <script src="{% static 'environment/js/pricing_change.js' %}"></script>
 <script src="{% static 'environment/js/gpu_disabling.js' %}"></script>
+<script src="{% static 'environment/js/forms.js' %}"></script>
 {% endblock %}
 
 {% block local_css %}
 <link rel="stylesheet" type="text/css" href="{% static 'environment/css/environment-base.css' %}">
 <link rel="stylesheet" type="text/css" href="{% static 'environment/css/create_research_environment.css' %}">
 {% endblock %}
 
@@ -36,15 +37,15 @@
                       {% for quota in exceeded_quotas %}
                           <li>{{ quota }}</li>
                       {% endfor %}
                   </ul>
                   <a href="{% url 'research_environments' %}"><button class="btn btn-primary">Return</button></a>
               </div>
           {% else %}
-              <form action="{% url 'create_research_environment' project_slug=project.slug project_version=project.version %}" method="post" style="width: 24rem;">
+              <form class="single-submit-form" action="{% url 'create_research_environment' project_slug=project.slug project_version=project.version %}" method="post" style="width: 24rem;">
                   {% csrf_token %}
                   {{ form }}
                   <button class="btn btn-primary mt-3" type="submit">
                       Create environment
                   </button>
               </form>
           {% endif %}
```

### Comparing `hdn-research-environment-2.1.4/environment/templates/environment/create_workspace.html` & `hdn-research-environment-2.1.5/environment/templates/environment/create_workspace.html`

 * *Files 27% similar despite different names*

```diff
@@ -4,61 +4,69 @@
 00000030: 206c 6f61 6420 7072 6f6a 6563 745f 7465   load project_te
 00000040: 6d70 6c61 7465 7461 6773 2025 7d0a 0a7b  mplatetags %}..{
 00000050: 2520 626c 6f63 6b20 7469 746c 6520 257d  % block title %}
 00000060: 4372 6561 7465 2052 6573 6561 7263 6820  Create Research 
 00000070: 456e 7669 726f 6e6d 656e 747b 2520 656e  Environment{% en
 00000080: 6462 6c6f 636b 2025 7d0a 0a7b 2520 626c  dblock %}..{% bl
 00000090: 6f63 6b20 6c6f 6361 6c5f 6a73 5f74 6f70  ock local_js_top
-000000a0: 2025 7d0a 7b25 2065 6e64 626c 6f63 6b20   %}.{% endblock 
-000000b0: 257d 0a0a 7b25 2062 6c6f 636b 206c 6f63  %}..{% block loc
-000000c0: 616c 5f63 7373 2025 7d0a 3c6c 696e 6b20  al_css %}.<link 
-000000d0: 7265 6c3d 2273 7479 6c65 7368 6565 7422  rel="stylesheet"
-000000e0: 2074 7970 653d 2274 6578 742f 6373 7322   type="text/css"
-000000f0: 2068 7265 663d 227b 2520 7374 6174 6963   href="{% static
-00000100: 2027 656e 7669 726f 6e6d 656e 742f 6373   'environment/cs
-00000110: 732f 656e 7669 726f 6e6d 656e 742d 6261  s/environment-ba
-00000120: 7365 2e63 7373 2720 257d 223e 0a3c 6c69  se.css' %}">.<li
-00000130: 6e6b 2072 656c 3d22 7374 796c 6573 6865  nk rel="styleshe
-00000140: 6574 2220 7479 7065 3d22 7465 7874 2f63  et" type="text/c
-00000150: 7373 2220 6872 6566 3d22 7b25 2073 7461  ss" href="{% sta
-00000160: 7469 6320 2765 6e76 6972 6f6e 6d65 6e74  tic 'environment
-00000170: 2f63 7373 2f63 7265 6174 655f 7265 7365  /css/create_rese
-00000180: 6172 6368 5f65 6e76 6972 6f6e 6d65 6e74  arch_environment
-00000190: 2e63 7373 2720 257d 223e 0a7b 2520 656e  .css' %}">.{% en
-000001a0: 6462 6c6f 636b 2025 7d0a 0a7b 2520 626c  dblock %}..{% bl
-000001b0: 6f63 6b20 636f 6e74 656e 7420 257d 0a3c  ock content %}.<
-000001c0: 6469 7620 636c 6173 733d 2263 6f6e 7461  div class="conta
-000001d0: 696e 6572 223e 0a20 207b 2520 696e 636c  iner">.  {% incl
-000001e0: 7564 6520 226d 6573 7361 6765 5f73 6e69  ude "message_sni
-000001f0: 7070 6574 2e68 746d 6c22 2025 7d0a 2020  ppet.html" %}.  
-00000200: 2020 3c68 3120 636c 6173 733d 226d 622d    <h1 class="mb-
-00000210: 3422 3e0a 2020 2020 2020 4372 6561 7465  4">.      Create
-00000220: 2057 6f72 6b73 7061 6365 0a20 2020 203c   Workspace.    <
-00000230: 2f68 313e 0a20 2020 203c 6469 7620 636c  /h1>.    <div cl
-00000240: 6173 733d 2263 6f6e 7461 696e 6572 2d62  ass="container-b
-00000250: 6f64 7922 3e0a 2020 2020 2020 3c64 6976  ody">.      <div
-00000260: 2063 6c61 7373 3d22 6361 7264 2220 7374   class="card" st
-00000270: 796c 653d 2277 6964 7468 3a20 3336 7265  yle="width: 36re
-00000280: 6d3b 223e 0a20 2020 2020 2020 203c 6469  m;">.        <di
-00000290: 7620 636c 6173 733d 2263 6172 642d 626f  v class="card-bo
-000002a0: 6479 223e 0a20 2020 2020 2020 2020 203c  dy">.          <
-000002b0: 666f 726d 2061 6374 696f 6e3d 227b 2520  form action="{% 
-000002c0: 7572 6c20 2763 7265 6174 655f 776f 726b  url 'create_work
-000002d0: 7370 6163 6527 2025 7d22 206d 6574 686f  space' %}" metho
-000002e0: 643d 2270 6f73 7422 2073 7479 6c65 3d22  d="post" style="
-000002f0: 7769 6474 683a 2032 3472 656d 3b22 3e0a  width: 24rem;">.
-00000300: 2020 2020 2020 2020 2020 2020 7b25 2063              {% c
-00000310: 7372 665f 746f 6b65 6e20 257d 0a20 2020  srf_token %}.   
-00000320: 2020 2020 2020 2020 207b 7b20 666f 726d           {{ form
-00000330: 207d 7d0a 2020 2020 2020 2020 2020 2020   }}.            
-00000340: 3c62 7574 746f 6e20 636c 6173 733d 2262  <button class="b
-00000350: 746e 2062 746e 2d70 7269 6d61 7279 206d  tn btn-primary m
-00000360: 742d 3322 2074 7970 653d 2273 7562 6d69  t-3" type="submi
-00000370: 7422 3e0a 2020 2020 2020 2020 2020 2020  t">.            
-00000380: 2020 2020 4372 6561 7465 2077 6f72 6b73      Create works
-00000390: 7061 6365 0a20 2020 2020 2020 2020 2020  pace.           
-000003a0: 203c 2f62 7574 746f 6e3e 0a20 2020 2020   </button>.     
-000003b0: 2020 2020 203c 2f66 6f72 6d3e 0a20 2020       </form>.   
-000003c0: 2020 2020 203c 2f64 6976 3e0a 2020 2020       </div>.    
-000003d0: 2020 3c2f 6469 763e 0a20 2020 203c 2f64    </div>.    </d
-000003e0: 6976 3e0a 3c2f 6469 763e 0a7b 2520 656e  iv>.</div>.{% en
-000003f0: 6462 6c6f 636b 2025 7d0a                 dblock %}.
+000000a0: 2025 7d0a 3c73 6372 6970 7420 7372 633d   %}.<script src=
+000000b0: 227b 2520 7374 6174 6963 2027 656e 7669  "{% static 'envi
+000000c0: 726f 6e6d 656e 742f 6a73 2f66 6f72 6d73  ronment/js/forms
+000000d0: 2e6a 7327 2025 7d22 3e3c 2f73 6372 6970  .js' %}"></scrip
+000000e0: 743e 0a7b 2520 656e 6462 6c6f 636b 2025  t>.{% endblock %
+000000f0: 7d0a 0a7b 2520 626c 6f63 6b20 6c6f 6361  }..{% block loca
+00000100: 6c5f 6373 7320 257d 0a3c 6c69 6e6b 2072  l_css %}.<link r
+00000110: 656c 3d22 7374 796c 6573 6865 6574 2220  el="stylesheet" 
+00000120: 7479 7065 3d22 7465 7874 2f63 7373 2220  type="text/css" 
+00000130: 6872 6566 3d22 7b25 2073 7461 7469 6320  href="{% static 
+00000140: 2765 6e76 6972 6f6e 6d65 6e74 2f63 7373  'environment/css
+00000150: 2f65 6e76 6972 6f6e 6d65 6e74 2d62 6173  /environment-bas
+00000160: 652e 6373 7327 2025 7d22 3e0a 3c6c 696e  e.css' %}">.<lin
+00000170: 6b20 7265 6c3d 2273 7479 6c65 7368 6565  k rel="styleshee
+00000180: 7422 2074 7970 653d 2274 6578 742f 6373  t" type="text/cs
+00000190: 7322 2068 7265 663d 227b 2520 7374 6174  s" href="{% stat
+000001a0: 6963 2027 656e 7669 726f 6e6d 656e 742f  ic 'environment/
+000001b0: 6373 732f 6372 6561 7465 5f72 6573 6561  css/create_resea
+000001c0: 7263 685f 656e 7669 726f 6e6d 656e 742e  rch_environment.
+000001d0: 6373 7327 2025 7d22 3e0a 7b25 2065 6e64  css' %}">.{% end
+000001e0: 626c 6f63 6b20 257d 0a0a 7b25 2062 6c6f  block %}..{% blo
+000001f0: 636b 2063 6f6e 7465 6e74 2025 7d0a 3c64  ck content %}.<d
+00000200: 6976 2063 6c61 7373 3d22 636f 6e74 6169  iv class="contai
+00000210: 6e65 7222 3e0a 2020 7b25 2069 6e63 6c75  ner">.  {% inclu
+00000220: 6465 2022 6d65 7373 6167 655f 736e 6970  de "message_snip
+00000230: 7065 742e 6874 6d6c 2220 257d 0a20 2020  pet.html" %}.   
+00000240: 203c 6831 2063 6c61 7373 3d22 6d62 2d34   <h1 class="mb-4
+00000250: 223e 0a20 2020 2020 2043 7265 6174 6520  ">.      Create 
+00000260: 576f 726b 7370 6163 650a 2020 2020 3c2f  Workspace.    </
+00000270: 6831 3e0a 2020 2020 3c64 6976 2063 6c61  h1>.    <div cla
+00000280: 7373 3d22 636f 6e74 6169 6e65 722d 626f  ss="container-bo
+00000290: 6479 223e 0a20 2020 2020 203c 6469 7620  dy">.      <div 
+000002a0: 636c 6173 733d 2263 6172 6422 2073 7479  class="card" sty
+000002b0: 6c65 3d22 7769 6474 683a 2033 3672 656d  le="width: 36rem
+000002c0: 3b22 3e0a 2020 2020 2020 2020 3c64 6976  ;">.        <div
+000002d0: 2063 6c61 7373 3d22 6361 7264 2d62 6f64   class="card-bod
+000002e0: 7922 3e0a 2020 2020 2020 2020 2020 3c66  y">.          <f
+000002f0: 6f72 6d20 636c 6173 733d 2273 696e 676c  orm class="singl
+00000300: 652d 7375 626d 6974 2d66 6f72 6d22 2061  e-submit-form" a
+00000310: 6374 696f 6e3d 227b 2520 7572 6c20 2763  ction="{% url 'c
+00000320: 7265 6174 655f 776f 726b 7370 6163 6527  reate_workspace'
+00000330: 2025 7d22 206d 6574 686f 643d 2270 6f73   %}" method="pos
+00000340: 7422 2073 7479 6c65 3d22 7769 6474 683a  t" style="width:
+00000350: 2032 3472 656d 3b22 3e0a 2020 2020 2020   24rem;">.      
+00000360: 2020 2020 2020 7b25 2063 7372 665f 746f        {% csrf_to
+00000370: 6b65 6e20 257d 0a20 2020 2020 2020 2020  ken %}.         
+00000380: 2020 207b 7b20 666f 726d 207d 7d0a 2020     {{ form }}.  
+00000390: 2020 2020 2020 2020 2020 3c62 7574 746f            <butto
+000003a0: 6e0a 2020 2020 2020 2020 2020 2020 2020  n.              
+000003b0: 636c 6173 733d 2262 746e 2062 746e 2d70  class="btn btn-p
+000003c0: 7269 6d61 7279 206d 742d 3322 0a20 2020  rimary mt-3".   
+000003d0: 2020 2020 2020 2020 2020 2074 7970 653d             type=
+000003e0: 2273 7562 6d69 7422 0a20 2020 2020 2020  "submit".       
+000003f0: 2020 2020 203e 0a20 2020 2020 2020 2020       >.         
+00000400: 2020 2020 2020 2043 7265 6174 6520 776f         Create wo
+00000410: 726b 7370 6163 650a 2020 2020 2020 2020  rkspace.        
+00000420: 2020 2020 3c2f 6275 7474 6f6e 3e0a 2020      </button>.  
+00000430: 2020 2020 2020 2020 3c2f 666f 726d 3e0a          </form>.
+00000440: 2020 2020 2020 2020 3c2f 6469 763e 0a20          </div>. 
+00000450: 2020 2020 203c 2f64 6976 3e0a 2020 2020       </div>.    
+00000460: 3c2f 6469 763e 0a3c 2f64 6976 3e0a 7b25  </div>.</div>.{%
+00000470: 2065 6e64 626c 6f63 6b20 257d 0a          endblock %}.
```

### Comparing `hdn-research-environment-2.1.4/environment/templates/environment/identity_provisioning.html` & `hdn-research-environment-2.1.5/environment/templates/environment/identity_provisioning.html`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.1.4/environment/templates/environment/manage_billing_account.html` & `hdn-research-environment-2.1.5/environment/templates/environment/manage_billing_account.html`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.1.4/environment/templates/environment/manage_shared_billing_invitation.html` & `hdn-research-environment-2.1.5/environment/templates/environment/manage_shared_billing_invitation.html`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.1.4/environment/templates/environment/research_environments.html` & `hdn-research-environment-2.1.5/environment/templates/environment/research_environments.html`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.1.4/environment/templates/tag/environment_modal_button.html` & `hdn-research-environment-2.1.5/environment/templates/tag/environment_modal_button.html`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.1.4/environment/templatetags/action_buttons.py` & `hdn-research-environment-2.1.5/environment/templatetags/action_buttons.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.1.4/environment/tests/helpers.py` & `hdn-research-environment-2.1.5/environment/tests/helpers.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.1.4/environment/tests/mocks.py` & `hdn-research-environment-2.1.5/environment/tests/mocks.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.1.4/environment/tests/test_decorators.py` & `hdn-research-environment-2.1.5/environment/tests/test_decorators.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.1.4/environment/tests/test_services.py` & `hdn-research-environment-2.1.5/environment/tests/test_services.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.1.4/environment/tests/test_signals.py` & `hdn-research-environment-2.1.5/environment/tests/test_signals.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.1.4/environment/tests/test_utilities.py` & `hdn-research-environment-2.1.5/environment/tests/test_utilities.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.1.4/environment/tests/test_validators.py` & `hdn-research-environment-2.1.5/environment/tests/test_validators.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.1.4/environment/tests/test_views.py` & `hdn-research-environment-2.1.5/environment/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.1.4/environment/urls.py` & `hdn-research-environment-2.1.5/environment/urls.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.1.4/environment/utilities.py` & `hdn-research-environment-2.1.5/environment/utilities.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.1.4/environment/views.py` & `hdn-research-environment-2.1.5/environment/views.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.1.4/hdn_research_environment.egg-info/PKG-INFO` & `hdn-research-environment-2.1.5/hdn_research_environment.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: hdn-research-environment
-Version: 2.1.4
+Version: 2.1.5
 Summary: A Django app for supporting cloud-native research environments
 Home-page: https://www.healthdatanexus.ai/
 Author: Your Name
 Author-email: yourname@example.com
 License: BSD-3-Clause  # Example license
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `hdn-research-environment-2.1.4/hdn_research_environment.egg-info/SOURCES.txt` & `hdn-research-environment-2.1.5/hdn_research_environment.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -39,14 +39,15 @@
 environment/migrations/0009_billingaccountsharinginvite_is_revoked.py
 environment/migrations/0010_alter_workflow_project_alter_workflow_type_and_more.py
 environment/migrations/__init__.py
 environment/static/environment/css/create_research_environment.css
 environment/static/environment/css/environment-base.css
 environment/static/environment/css/manage_billing_account.css
 environment/static/environment/js/cookie.js
+environment/static/environment/js/forms.js
 environment/static/environment/js/gpu_disabling.js
 environment/static/environment/js/pricing_change.js
 environment/templates/environment/_available_environments_list.html
 environment/templates/environment/_available_projects_list.html
 environment/templates/environment/_billing_accounts_list.html
 environment/templates/environment/base_environment_home.html
 environment/templates/environment/create_research_environment.html
```

### Comparing `hdn-research-environment-2.1.4/setup.cfg` & `hdn-research-environment-2.1.5/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = hdn-research-environment
-version = 2.1.4
+version = 2.1.5
 description = A Django app for supporting cloud-native research environments
 long_description = file: README.rst
 url = https://www.healthdatanexus.ai/
 author = Your Name
 author_email = yourname@example.com
 license = BSD-3-Clause  # Example license
 classifiers =
```

