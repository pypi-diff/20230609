# Comparing `tmp/hdn-research-environment-2.1.5.tar.gz` & `tmp/hdn-research-environment-2.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/hdn-research-environment-2.1.5.tar", last modified: Fri Jun  9 10:25:21 2023, max compression
+gzip compressed data, was "dist/hdn-research-environment-2.1.6.tar", last modified: Fri Jun  9 13:15:25 2023, max compression
```

## Comparing `hdn-research-environment-2.1.5.tar` & `hdn-research-environment-2.1.6.tar`

### file list

```diff
@@ -1,96 +1,96 @@
-drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-09 10:25:21.000000 hdn-research-environment-2.1.5/
--rw-r--r--   0 karolszuster   (501) staff       (20)     1551 2022-03-29 08:15:30.000000 hdn-research-environment-2.1.5/LICENSE
--rw-r--r--   0 karolszuster   (501) staff       (20)      115 2022-03-29 08:32:41.000000 hdn-research-environment-2.1.5/MANIFEST.in
--rw-r--r--   0 karolszuster   (501) staff       (20)      995 2023-06-09 10:25:21.000000 hdn-research-environment-2.1.5/PKG-INFO
--rw-r--r--   0 karolszuster   (501) staff       (20)       90 2022-03-29 07:59:09.000000 hdn-research-environment-2.1.5/README.md
-drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-09 10:25:21.000000 hdn-research-environment-2.1.5/environment/
--rw-r--r--   0 karolszuster   (501) staff       (20)        0 2022-03-29 08:08:24.000000 hdn-research-environment-2.1.5/environment/__init__.py
-drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-09 10:25:21.000000 hdn-research-environment-2.1.5/environment/api/
--rw-r--r--   0 karolszuster   (501) staff       (20)        0 2023-05-29 11:59:00.000000 hdn-research-environment-2.1.5/environment/api/__init__.py
-drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-09 10:25:21.000000 hdn-research-environment-2.1.5/environment/api/v1/
--rw-r--r--   0 karolszuster   (501) staff       (20)     3242 2023-05-29 11:59:00.000000 hdn-research-environment-2.1.5/environment/api/v1/__init__.py
--rw-r--r--   0 karolszuster   (501) staff       (20)      640 2023-05-29 11:59:00.000000 hdn-research-environment-2.1.5/environment/api/v1/auth.py
--rw-r--r--   0 karolszuster   (501) staff       (20)      700 2023-05-29 11:59:00.000000 hdn-research-environment-2.1.5/environment/api/v1/decorators.py
-drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-09 10:25:21.000000 hdn-research-environment-2.1.5/environment/api/v2/
--rw-r--r--   0 karolszuster   (501) staff       (20)     1572 2023-05-29 11:59:00.000000 hdn-research-environment-2.1.5/environment/api/v2/__init__.py
--rw-r--r--   0 karolszuster   (501) staff       (20)      942 2023-05-30 18:52:36.000000 hdn-research-environment-2.1.5/environment/api/v2/decorators.py
--rw-r--r--   0 karolszuster   (501) staff       (20)      154 2022-03-29 08:08:24.000000 hdn-research-environment-2.1.5/environment/apps.py
--rw-r--r--   0 karolszuster   (501) staff       (20)     3175 2023-06-09 09:19:00.000000 hdn-research-environment-2.1.5/environment/constants.py
--rw-r--r--   0 karolszuster   (501) staff       (20)     1005 2023-05-29 11:59:00.000000 hdn-research-environment-2.1.5/environment/decorators.py
--rw-r--r--   0 karolszuster   (501) staff       (20)     1878 2023-05-29 11:59:00.000000 hdn-research-environment-2.1.5/environment/deserializers.py
--rw-r--r--   0 karolszuster   (501) staff       (20)     2928 2023-05-29 12:32:30.000000 hdn-research-environment-2.1.5/environment/entities.py
--rw-r--r--   0 karolszuster   (501) staff       (20)      818 2023-05-29 11:59:00.000000 hdn-research-environment-2.1.5/environment/exceptions.py
--rw-r--r--   0 karolszuster   (501) staff       (20)     3711 2023-06-05 16:43:26.000000 hdn-research-environment-2.1.5/environment/forms.py
--rw-r--r--   0 karolszuster   (501) staff       (20)     1720 2023-06-06 14:41:05.000000 hdn-research-environment-2.1.5/environment/mailers.py
--rw-r--r--   0 karolszuster   (501) staff       (20)      155 2022-03-29 08:08:24.000000 hdn-research-environment-2.1.5/environment/managers.py
-drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-09 10:25:21.000000 hdn-research-environment-2.1.5/environment/migrations/
--rw-r--r--   0 karolszuster   (501) staff       (20)     1443 2023-05-29 11:59:00.000000 hdn-research-environment-2.1.5/environment/migrations/0001_initial.py
--rw-r--r--   0 karolszuster   (501) staff       (20)     1579 2023-05-29 11:59:00.000000 hdn-research-environment-2.1.5/environment/migrations/0002_billingsetup.py
--rw-r--r--   0 karolszuster   (501) staff       (20)      403 2023-05-29 11:59:00.000000 hdn-research-environment-2.1.5/environment/migrations/0003_cloudidentity_is_workspace_done.py
--rw-r--r--   0 karolszuster   (501) staff       (20)      420 2023-05-29 11:59:00.000000 hdn-research-environment-2.1.5/environment/migrations/0004_auto_20220309_0330.py
--rw-r--r--   0 karolszuster   (501) staff       (20)     2220 2023-05-29 11:59:00.000000 hdn-research-environment-2.1.5/environment/migrations/0005_workflow.py
--rw-r--r--   0 karolszuster   (501) staff       (20)      394 2023-05-29 11:59:00.000000 hdn-research-environment-2.1.5/environment/migrations/0006_delete_billingsetup.py
--rw-r--r--   0 karolszuster   (501) staff       (20)     2347 2023-05-29 11:59:00.000000 hdn-research-environment-2.1.5/environment/migrations/0007_billingaccountsharinginvite.py
--rw-r--r--   0 karolszuster   (501) staff       (20)      476 2023-05-29 11:59:00.000000 hdn-research-environment-2.1.5/environment/migrations/0008_workflow_workspace_name.py
--rw-r--r--   0 karolszuster   (501) staff       (20)      420 2023-05-29 11:59:00.000000 hdn-research-environment-2.1.5/environment/migrations/0009_billingaccountsharinginvite_is_revoked.py
--rw-r--r--   0 karolszuster   (501) staff       (20)     1364 2023-05-31 14:40:16.000000 hdn-research-environment-2.1.5/environment/migrations/0010_alter_workflow_project_alter_workflow_type_and_more.py
--rw-r--r--   0 karolszuster   (501) staff       (20)        0 2022-03-29 08:08:24.000000 hdn-research-environment-2.1.5/environment/migrations/__init__.py
--rw-r--r--   0 karolszuster   (501) staff       (20)     2518 2023-05-31 14:40:16.000000 hdn-research-environment-2.1.5/environment/models.py
--rw-r--r--   0 karolszuster   (501) staff       (20)    19730 2023-06-09 09:19:00.000000 hdn-research-environment-2.1.5/environment/services.py
--rw-r--r--   0 karolszuster   (501) staff       (20)     4545 2023-06-02 15:32:09.000000 hdn-research-environment-2.1.5/environment/signals.py
-drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-09 10:25:21.000000 hdn-research-environment-2.1.5/environment/static/
-drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-09 10:25:21.000000 hdn-research-environment-2.1.5/environment/static/environment/
-drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-09 10:25:21.000000 hdn-research-environment-2.1.5/environment/static/environment/css/
--rw-r--r--   0 karolszuster   (501) staff       (20)      342 2023-02-22 22:00:03.000000 hdn-research-environment-2.1.5/environment/static/environment/css/create_research_environment.css
--rw-r--r--   0 karolszuster   (501) staff       (20)     6583 2022-03-29 08:08:24.000000 hdn-research-environment-2.1.5/environment/static/environment/css/environment-base.css
--rw-r--r--   0 karolszuster   (501) staff       (20)      117 2023-05-29 11:59:00.000000 hdn-research-environment-2.1.5/environment/static/environment/css/manage_billing_account.css
-drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-09 10:25:21.000000 hdn-research-environment-2.1.5/environment/static/environment/js/
--rw-r--r--   0 karolszuster   (501) staff       (20)      564 2022-03-30 12:50:58.000000 hdn-research-environment-2.1.5/environment/static/environment/js/cookie.js
--rw-r--r--   0 karolszuster   (501) staff       (20)      291 2023-06-09 10:25:06.000000 hdn-research-environment-2.1.5/environment/static/environment/js/forms.js
--rw-r--r--   0 karolszuster   (501) staff       (20)      516 2023-05-29 11:59:00.000000 hdn-research-environment-2.1.5/environment/static/environment/js/gpu_disabling.js
--rw-r--r--   0 karolszuster   (501) staff       (20)     3154 2023-05-29 11:59:00.000000 hdn-research-environment-2.1.5/environment/static/environment/js/pricing_change.js
--rw-r--r--   0 karolszuster   (501) staff       (20)     2652 2023-06-05 06:46:01.000000 hdn-research-environment-2.1.5/environment/tasks.py
-drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-09 10:25:21.000000 hdn-research-environment-2.1.5/environment/templates/
-drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-09 10:25:21.000000 hdn-research-environment-2.1.5/environment/templates/environment/
--rw-r--r--   0 karolszuster   (501) staff       (20)     8010 2023-06-09 09:47:58.000000 hdn-research-environment-2.1.5/environment/templates/environment/_available_environments_list.html
--rw-r--r--   0 karolszuster   (501) staff       (20)     1423 2023-06-02 15:30:03.000000 hdn-research-environment-2.1.5/environment/templates/environment/_available_projects_list.html
--rw-r--r--   0 karolszuster   (501) staff       (20)     1916 2023-06-05 16:02:13.000000 hdn-research-environment-2.1.5/environment/templates/environment/_billing_accounts_list.html
--rw-r--r--   0 karolszuster   (501) staff       (20)      864 2023-06-09 10:25:06.000000 hdn-research-environment-2.1.5/environment/templates/environment/base_environment_home.html
--rw-r--r--   0 karolszuster   (501) staff       (20)     4417 2023-06-09 10:25:06.000000 hdn-research-environment-2.1.5/environment/templates/environment/create_research_environment.html
--rw-r--r--   0 karolszuster   (501) staff       (20)     1149 2023-06-09 10:25:06.000000 hdn-research-environment-2.1.5/environment/templates/environment/create_workspace.html
-drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-09 10:25:21.000000 hdn-research-environment-2.1.5/environment/templates/environment/email/
--rw-r--r--   0 karolszuster   (501) staff       (20)      272 2023-06-09 09:19:00.000000 hdn-research-environment-2.1.5/environment/templates/environment/email/billing_sharing_confirmation.html
--rw-r--r--   0 karolszuster   (501) staff       (20)      351 2023-06-05 06:46:01.000000 hdn-research-environment-2.1.5/environment/templates/environment/email/environment_access_expired.html
--rw-r--r--   0 karolszuster   (501) staff       (20)     1455 2023-05-29 11:58:57.000000 hdn-research-environment-2.1.5/environment/templates/environment/identity_provisioning.html
--rw-r--r--   0 karolszuster   (501) staff       (20)     5942 2023-06-05 06:46:01.000000 hdn-research-environment-2.1.5/environment/templates/environment/manage_billing_account.html
--rw-r--r--   0 karolszuster   (501) staff       (20)      562 2023-06-05 16:02:13.000000 hdn-research-environment-2.1.5/environment/templates/environment/manage_shared_billing_invitation.html
--rw-r--r--   0 karolszuster   (501) staff       (20)     3870 2023-06-05 16:02:13.000000 hdn-research-environment-2.1.5/environment/templates/environment/research_environments.html
-drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-09 10:25:21.000000 hdn-research-environment-2.1.5/environment/templates/tag/
--rw-r--r--   0 karolszuster   (501) staff       (20)      241 2022-03-29 08:08:24.000000 hdn-research-environment-2.1.5/environment/templates/tag/environment_action_button.html
--rw-r--r--   0 karolszuster   (501) staff       (20)     1473 2023-06-06 14:41:05.000000 hdn-research-environment-2.1.5/environment/templates/tag/environment_modal_button.html
-drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-09 10:25:21.000000 hdn-research-environment-2.1.5/environment/templatetags/
--rw-r--r--   0 karolszuster   (501) staff       (20)        0 2022-03-29 08:08:24.000000 hdn-research-environment-2.1.5/environment/templatetags/__init__.py
--rw-r--r--   0 karolszuster   (501) staff       (20)     3518 2023-06-05 16:02:13.000000 hdn-research-environment-2.1.5/environment/templatetags/action_buttons.py
-drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-09 10:25:21.000000 hdn-research-environment-2.1.5/environment/tests/
--rw-r--r--   0 karolszuster   (501) staff       (20)        0 2022-03-29 08:08:24.000000 hdn-research-environment-2.1.5/environment/tests/__init__.py
--rw-r--r--   0 karolszuster   (501) staff       (20)      645 2023-05-29 11:59:00.000000 hdn-research-environment-2.1.5/environment/tests/helpers.py
--rw-r--r--   0 karolszuster   (501) staff       (20)    12158 2023-05-29 11:59:00.000000 hdn-research-environment-2.1.5/environment/tests/mocks.py
--rw-r--r--   0 karolszuster   (501) staff       (20)     3007 2023-05-29 11:59:00.000000 hdn-research-environment-2.1.5/environment/tests/test_decorators.py
--rw-r--r--   0 karolszuster   (501) staff       (20)    10693 2023-05-29 11:59:00.000000 hdn-research-environment-2.1.5/environment/tests/test_services.py
--rw-r--r--   0 karolszuster   (501) staff       (20)     5328 2023-05-29 11:59:00.000000 hdn-research-environment-2.1.5/environment/tests/test_signals.py
--rw-r--r--   0 karolszuster   (501) staff       (20)     2909 2023-05-29 11:59:00.000000 hdn-research-environment-2.1.5/environment/tests/test_utilities.py
--rw-r--r--   0 karolszuster   (501) staff       (20)      640 2023-05-29 11:58:39.000000 hdn-research-environment-2.1.5/environment/tests/test_validators.py
--rw-r--r--   0 karolszuster   (501) staff       (20)     3380 2023-05-29 11:59:00.000000 hdn-research-environment-2.1.5/environment/tests/test_views.py
--rw-r--r--   0 karolszuster   (501) staff       (20)     1555 2023-05-29 11:59:00.000000 hdn-research-environment-2.1.5/environment/urls.py
--rw-r--r--   0 karolszuster   (501) staff       (20)     1135 2023-05-29 11:59:00.000000 hdn-research-environment-2.1.5/environment/utilities.py
--rw-r--r--   0 karolszuster   (501) staff       (20)      236 2022-03-29 08:08:24.000000 hdn-research-environment-2.1.5/environment/validators.py
--rw-r--r--   0 karolszuster   (501) staff       (20)    14146 2023-06-09 09:47:58.000000 hdn-research-environment-2.1.5/environment/views.py
-drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-09 10:25:21.000000 hdn-research-environment-2.1.5/hdn_research_environment.egg-info/
--rw-r--r--   0 karolszuster   (501) staff       (20)      995 2023-06-09 10:25:21.000000 hdn-research-environment-2.1.5/hdn_research_environment.egg-info/PKG-INFO
--rw-r--r--   0 karolszuster   (501) staff       (20)     3143 2023-06-09 10:25:21.000000 hdn-research-environment-2.1.5/hdn_research_environment.egg-info/SOURCES.txt
--rw-r--r--   0 karolszuster   (501) staff       (20)        1 2023-06-09 10:25:21.000000 hdn-research-environment-2.1.5/hdn_research_environment.egg-info/dependency_links.txt
--rw-r--r--   0 karolszuster   (501) staff       (20)       84 2023-06-09 10:25:21.000000 hdn-research-environment-2.1.5/hdn_research_environment.egg-info/requires.txt
--rw-r--r--   0 karolszuster   (501) staff       (20)       12 2023-06-09 10:25:21.000000 hdn-research-environment-2.1.5/hdn_research_environment.egg-info/top_level.txt
--rw-r--r--   0 karolszuster   (501) staff       (20)      109 2022-03-29 08:03:11.000000 hdn-research-environment-2.1.5/pyproject.toml
--rw-r--r--   0 karolszuster   (501) staff       (20)     1056 2023-06-09 10:25:21.000000 hdn-research-environment-2.1.5/setup.cfg
--rw-r--r--   0 karolszuster   (501) staff       (20)       38 2022-03-29 08:03:11.000000 hdn-research-environment-2.1.5/setup.py
+drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-09 13:15:25.000000 hdn-research-environment-2.1.6/
+-rw-r--r--   0 karolszuster   (501) staff       (20)     1551 2022-03-29 08:15:30.000000 hdn-research-environment-2.1.6/LICENSE
+-rw-r--r--   0 karolszuster   (501) staff       (20)      115 2022-03-29 08:32:41.000000 hdn-research-environment-2.1.6/MANIFEST.in
+-rw-r--r--   0 karolszuster   (501) staff       (20)      995 2023-06-09 13:15:25.000000 hdn-research-environment-2.1.6/PKG-INFO
+-rw-r--r--   0 karolszuster   (501) staff       (20)       90 2022-03-29 07:59:09.000000 hdn-research-environment-2.1.6/README.md
+drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-09 13:15:25.000000 hdn-research-environment-2.1.6/environment/
+-rw-r--r--   0 karolszuster   (501) staff       (20)        0 2022-03-29 08:08:24.000000 hdn-research-environment-2.1.6/environment/__init__.py
+drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-09 13:15:25.000000 hdn-research-environment-2.1.6/environment/api/
+-rw-r--r--   0 karolszuster   (501) staff       (20)        0 2023-05-29 11:59:00.000000 hdn-research-environment-2.1.6/environment/api/__init__.py
+drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-09 13:15:25.000000 hdn-research-environment-2.1.6/environment/api/v1/
+-rw-r--r--   0 karolszuster   (501) staff       (20)     3242 2023-05-29 11:59:00.000000 hdn-research-environment-2.1.6/environment/api/v1/__init__.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)      640 2023-05-29 11:59:00.000000 hdn-research-environment-2.1.6/environment/api/v1/auth.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)      700 2023-05-29 11:59:00.000000 hdn-research-environment-2.1.6/environment/api/v1/decorators.py
+drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-09 13:15:25.000000 hdn-research-environment-2.1.6/environment/api/v2/
+-rw-r--r--   0 karolszuster   (501) staff       (20)     1572 2023-05-29 11:59:00.000000 hdn-research-environment-2.1.6/environment/api/v2/__init__.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)      942 2023-05-30 18:52:36.000000 hdn-research-environment-2.1.6/environment/api/v2/decorators.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)      154 2022-03-29 08:08:24.000000 hdn-research-environment-2.1.6/environment/apps.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)     3175 2023-06-09 09:19:00.000000 hdn-research-environment-2.1.6/environment/constants.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)     1005 2023-05-29 11:59:00.000000 hdn-research-environment-2.1.6/environment/decorators.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)     1878 2023-05-29 11:59:00.000000 hdn-research-environment-2.1.6/environment/deserializers.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)     2928 2023-05-29 12:32:30.000000 hdn-research-environment-2.1.6/environment/entities.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)      818 2023-05-29 11:59:00.000000 hdn-research-environment-2.1.6/environment/exceptions.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)     3711 2023-06-05 16:43:26.000000 hdn-research-environment-2.1.6/environment/forms.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)     1720 2023-06-06 14:41:05.000000 hdn-research-environment-2.1.6/environment/mailers.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)      155 2022-03-29 08:08:24.000000 hdn-research-environment-2.1.6/environment/managers.py
+drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-09 13:15:25.000000 hdn-research-environment-2.1.6/environment/migrations/
+-rw-r--r--   0 karolszuster   (501) staff       (20)     1443 2023-05-29 11:59:00.000000 hdn-research-environment-2.1.6/environment/migrations/0001_initial.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)     1579 2023-05-29 11:59:00.000000 hdn-research-environment-2.1.6/environment/migrations/0002_billingsetup.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)      403 2023-05-29 11:59:00.000000 hdn-research-environment-2.1.6/environment/migrations/0003_cloudidentity_is_workspace_done.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)      420 2023-05-29 11:59:00.000000 hdn-research-environment-2.1.6/environment/migrations/0004_auto_20220309_0330.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)     2220 2023-05-29 11:59:00.000000 hdn-research-environment-2.1.6/environment/migrations/0005_workflow.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)      394 2023-05-29 11:59:00.000000 hdn-research-environment-2.1.6/environment/migrations/0006_delete_billingsetup.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)     2347 2023-05-29 11:59:00.000000 hdn-research-environment-2.1.6/environment/migrations/0007_billingaccountsharinginvite.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)      476 2023-05-29 11:59:00.000000 hdn-research-environment-2.1.6/environment/migrations/0008_workflow_workspace_name.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)      420 2023-05-29 11:59:00.000000 hdn-research-environment-2.1.6/environment/migrations/0009_billingaccountsharinginvite_is_revoked.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)     1364 2023-05-31 14:40:16.000000 hdn-research-environment-2.1.6/environment/migrations/0010_alter_workflow_project_alter_workflow_type_and_more.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)        0 2022-03-29 08:08:24.000000 hdn-research-environment-2.1.6/environment/migrations/__init__.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)     2518 2023-05-31 14:40:16.000000 hdn-research-environment-2.1.6/environment/models.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)    19730 2023-06-09 09:19:00.000000 hdn-research-environment-2.1.6/environment/services.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)     4545 2023-06-02 15:32:09.000000 hdn-research-environment-2.1.6/environment/signals.py
+drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-09 13:15:25.000000 hdn-research-environment-2.1.6/environment/static/
+drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-09 13:15:25.000000 hdn-research-environment-2.1.6/environment/static/environment/
+drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-09 13:15:25.000000 hdn-research-environment-2.1.6/environment/static/environment/css/
+-rw-r--r--   0 karolszuster   (501) staff       (20)      342 2023-02-22 22:00:03.000000 hdn-research-environment-2.1.6/environment/static/environment/css/create_research_environment.css
+-rw-r--r--   0 karolszuster   (501) staff       (20)     6583 2022-03-29 08:08:24.000000 hdn-research-environment-2.1.6/environment/static/environment/css/environment-base.css
+-rw-r--r--   0 karolszuster   (501) staff       (20)      117 2023-05-29 11:59:00.000000 hdn-research-environment-2.1.6/environment/static/environment/css/manage_billing_account.css
+drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-09 13:15:25.000000 hdn-research-environment-2.1.6/environment/static/environment/js/
+-rw-r--r--   0 karolszuster   (501) staff       (20)      564 2022-03-30 12:50:58.000000 hdn-research-environment-2.1.6/environment/static/environment/js/cookie.js
+-rw-r--r--   0 karolszuster   (501) staff       (20)      291 2023-06-09 10:25:06.000000 hdn-research-environment-2.1.6/environment/static/environment/js/forms.js
+-rw-r--r--   0 karolszuster   (501) staff       (20)      516 2023-05-29 11:59:00.000000 hdn-research-environment-2.1.6/environment/static/environment/js/gpu_disabling.js
+-rw-r--r--   0 karolszuster   (501) staff       (20)     3154 2023-05-29 11:59:00.000000 hdn-research-environment-2.1.6/environment/static/environment/js/pricing_change.js
+-rw-r--r--   0 karolszuster   (501) staff       (20)     2652 2023-06-05 06:46:01.000000 hdn-research-environment-2.1.6/environment/tasks.py
+drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-09 13:15:25.000000 hdn-research-environment-2.1.6/environment/templates/
+drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-09 13:15:25.000000 hdn-research-environment-2.1.6/environment/templates/environment/
+-rw-r--r--   0 karolszuster   (501) staff       (20)     8010 2023-06-09 09:47:58.000000 hdn-research-environment-2.1.6/environment/templates/environment/_available_environments_list.html
+-rw-r--r--   0 karolszuster   (501) staff       (20)     1423 2023-06-02 15:30:03.000000 hdn-research-environment-2.1.6/environment/templates/environment/_available_projects_list.html
+-rw-r--r--   0 karolszuster   (501) staff       (20)     1916 2023-06-05 16:02:13.000000 hdn-research-environment-2.1.6/environment/templates/environment/_billing_accounts_list.html
+-rw-r--r--   0 karolszuster   (501) staff       (20)     1073 2023-06-09 13:14:55.000000 hdn-research-environment-2.1.6/environment/templates/environment/base_environment_home.html
+-rw-r--r--   0 karolszuster   (501) staff       (20)     4417 2023-06-09 10:25:06.000000 hdn-research-environment-2.1.6/environment/templates/environment/create_research_environment.html
+-rw-r--r--   0 karolszuster   (501) staff       (20)     1149 2023-06-09 10:25:06.000000 hdn-research-environment-2.1.6/environment/templates/environment/create_workspace.html
+drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-09 13:15:25.000000 hdn-research-environment-2.1.6/environment/templates/environment/email/
+-rw-r--r--   0 karolszuster   (501) staff       (20)      272 2023-06-09 09:19:00.000000 hdn-research-environment-2.1.6/environment/templates/environment/email/billing_sharing_confirmation.html
+-rw-r--r--   0 karolszuster   (501) staff       (20)      351 2023-06-05 06:46:01.000000 hdn-research-environment-2.1.6/environment/templates/environment/email/environment_access_expired.html
+-rw-r--r--   0 karolszuster   (501) staff       (20)     1455 2023-05-29 11:58:57.000000 hdn-research-environment-2.1.6/environment/templates/environment/identity_provisioning.html
+-rw-r--r--   0 karolszuster   (501) staff       (20)     5942 2023-06-05 06:46:01.000000 hdn-research-environment-2.1.6/environment/templates/environment/manage_billing_account.html
+-rw-r--r--   0 karolszuster   (501) staff       (20)      562 2023-06-05 16:02:13.000000 hdn-research-environment-2.1.6/environment/templates/environment/manage_shared_billing_invitation.html
+-rw-r--r--   0 karolszuster   (501) staff       (20)     3870 2023-06-05 16:02:13.000000 hdn-research-environment-2.1.6/environment/templates/environment/research_environments.html
+drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-09 13:15:25.000000 hdn-research-environment-2.1.6/environment/templates/tag/
+-rw-r--r--   0 karolszuster   (501) staff       (20)      241 2022-03-29 08:08:24.000000 hdn-research-environment-2.1.6/environment/templates/tag/environment_action_button.html
+-rw-r--r--   0 karolszuster   (501) staff       (20)     1473 2023-06-06 14:41:05.000000 hdn-research-environment-2.1.6/environment/templates/tag/environment_modal_button.html
+drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-09 13:15:25.000000 hdn-research-environment-2.1.6/environment/templatetags/
+-rw-r--r--   0 karolszuster   (501) staff       (20)        0 2022-03-29 08:08:24.000000 hdn-research-environment-2.1.6/environment/templatetags/__init__.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)     3518 2023-06-05 16:02:13.000000 hdn-research-environment-2.1.6/environment/templatetags/action_buttons.py
+drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-09 13:15:25.000000 hdn-research-environment-2.1.6/environment/tests/
+-rw-r--r--   0 karolszuster   (501) staff       (20)        0 2022-03-29 08:08:24.000000 hdn-research-environment-2.1.6/environment/tests/__init__.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)      645 2023-05-29 11:59:00.000000 hdn-research-environment-2.1.6/environment/tests/helpers.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)    12158 2023-05-29 11:59:00.000000 hdn-research-environment-2.1.6/environment/tests/mocks.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)     3007 2023-05-29 11:59:00.000000 hdn-research-environment-2.1.6/environment/tests/test_decorators.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)    10693 2023-05-29 11:59:00.000000 hdn-research-environment-2.1.6/environment/tests/test_services.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)     5328 2023-05-29 11:59:00.000000 hdn-research-environment-2.1.6/environment/tests/test_signals.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)     2909 2023-05-29 11:59:00.000000 hdn-research-environment-2.1.6/environment/tests/test_utilities.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)      640 2023-05-29 11:58:39.000000 hdn-research-environment-2.1.6/environment/tests/test_validators.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)     3380 2023-05-29 11:59:00.000000 hdn-research-environment-2.1.6/environment/tests/test_views.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)     1555 2023-05-29 11:59:00.000000 hdn-research-environment-2.1.6/environment/urls.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)     1135 2023-05-29 11:59:00.000000 hdn-research-environment-2.1.6/environment/utilities.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)      236 2022-03-29 08:08:24.000000 hdn-research-environment-2.1.6/environment/validators.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)    14417 2023-06-09 13:14:55.000000 hdn-research-environment-2.1.6/environment/views.py
+drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-09 13:15:25.000000 hdn-research-environment-2.1.6/hdn_research_environment.egg-info/
+-rw-r--r--   0 karolszuster   (501) staff       (20)      995 2023-06-09 13:15:25.000000 hdn-research-environment-2.1.6/hdn_research_environment.egg-info/PKG-INFO
+-rw-r--r--   0 karolszuster   (501) staff       (20)     3143 2023-06-09 13:15:25.000000 hdn-research-environment-2.1.6/hdn_research_environment.egg-info/SOURCES.txt
+-rw-r--r--   0 karolszuster   (501) staff       (20)        1 2023-06-09 13:15:25.000000 hdn-research-environment-2.1.6/hdn_research_environment.egg-info/dependency_links.txt
+-rw-r--r--   0 karolszuster   (501) staff       (20)       84 2023-06-09 13:15:25.000000 hdn-research-environment-2.1.6/hdn_research_environment.egg-info/requires.txt
+-rw-r--r--   0 karolszuster   (501) staff       (20)       12 2023-06-09 13:15:25.000000 hdn-research-environment-2.1.6/hdn_research_environment.egg-info/top_level.txt
+-rw-r--r--   0 karolszuster   (501) staff       (20)      109 2022-03-29 08:03:11.000000 hdn-research-environment-2.1.6/pyproject.toml
+-rw-r--r--   0 karolszuster   (501) staff       (20)     1056 2023-06-09 13:15:25.000000 hdn-research-environment-2.1.6/setup.cfg
+-rw-r--r--   0 karolszuster   (501) staff       (20)       38 2022-03-29 08:03:11.000000 hdn-research-environment-2.1.6/setup.py
```

### Comparing `hdn-research-environment-2.1.5/LICENSE` & `hdn-research-environment-2.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.1.5/PKG-INFO` & `hdn-research-environment-2.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: hdn-research-environment
-Version: 2.1.5
+Version: 2.1.6
 Summary: A Django app for supporting cloud-native research environments
 Home-page: https://www.healthdatanexus.ai/
 Author: Your Name
 Author-email: yourname@example.com
 License: BSD-3-Clause  # Example license
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `hdn-research-environment-2.1.5/environment/api/v1/__init__.py` & `hdn-research-environment-2.1.6/environment/api/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.1.5/environment/api/v1/auth.py` & `hdn-research-environment-2.1.6/environment/api/v1/auth.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.1.5/environment/api/v1/decorators.py` & `hdn-research-environment-2.1.6/environment/api/v1/decorators.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.1.5/environment/api/v2/__init__.py` & `hdn-research-environment-2.1.6/environment/api/v2/__init__.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.1.5/environment/api/v2/decorators.py` & `hdn-research-environment-2.1.6/environment/api/v2/decorators.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.1.5/environment/constants.py` & `hdn-research-environment-2.1.6/environment/constants.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.1.5/environment/decorators.py` & `hdn-research-environment-2.1.6/environment/decorators.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.1.5/environment/deserializers.py` & `hdn-research-environment-2.1.6/environment/deserializers.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.1.5/environment/entities.py` & `hdn-research-environment-2.1.6/environment/entities.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.1.5/environment/exceptions.py` & `hdn-research-environment-2.1.6/environment/exceptions.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.1.5/environment/forms.py` & `hdn-research-environment-2.1.6/environment/forms.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.1.5/environment/mailers.py` & `hdn-research-environment-2.1.6/environment/mailers.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.1.5/environment/migrations/0001_initial.py` & `hdn-research-environment-2.1.6/environment/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.1.5/environment/migrations/0002_billingsetup.py` & `hdn-research-environment-2.1.6/environment/migrations/0002_billingsetup.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.1.5/environment/migrations/0005_workflow.py` & `hdn-research-environment-2.1.6/environment/migrations/0005_workflow.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.1.5/environment/migrations/0007_billingaccountsharinginvite.py` & `hdn-research-environment-2.1.6/environment/migrations/0007_billingaccountsharinginvite.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.1.5/environment/migrations/0010_alter_workflow_project_alter_workflow_type_and_more.py` & `hdn-research-environment-2.1.6/environment/migrations/0010_alter_workflow_project_alter_workflow_type_and_more.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.1.5/environment/models.py` & `hdn-research-environment-2.1.6/environment/models.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.1.5/environment/services.py` & `hdn-research-environment-2.1.6/environment/services.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.1.5/environment/signals.py` & `hdn-research-environment-2.1.6/environment/signals.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.1.5/environment/static/environment/css/environment-base.css` & `hdn-research-environment-2.1.6/environment/static/environment/css/environment-base.css`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.1.5/environment/static/environment/js/cookie.js` & `hdn-research-environment-2.1.6/environment/static/environment/js/cookie.js`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.1.5/environment/static/environment/js/gpu_disabling.js` & `hdn-research-environment-2.1.6/environment/static/environment/js/gpu_disabling.js`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.1.5/environment/static/environment/js/pricing_change.js` & `hdn-research-environment-2.1.6/environment/static/environment/js/pricing_change.js`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.1.5/environment/tasks.py` & `hdn-research-environment-2.1.6/environment/tasks.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.1.5/environment/templates/environment/_available_environments_list.html` & `hdn-research-environment-2.1.6/environment/templates/environment/_available_environments_list.html`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.1.5/environment/templates/environment/_available_projects_list.html` & `hdn-research-environment-2.1.6/environment/templates/environment/_available_projects_list.html`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.1.5/environment/templates/environment/_billing_accounts_list.html` & `hdn-research-environment-2.1.6/environment/templates/environment/_billing_accounts_list.html`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.1.5/environment/templates/environment/base_environment_home.html` & `hdn-research-environment-2.1.6/environment/templates/environment/create_workspace.html`

 * *Files 16% similar despite different names*

```diff
@@ -1,33 +1,41 @@
 {% extends 'base.html' %}
 
 {% load static %}
 
 {% load project_templatetags %}
 
-{% block title %}Research environments{% endblock %}
-
-{% block local_css %}
-<link rel="stylesheet" type="text/css" href="{% static 'environment/css/environment-base.css' %}">
-{% endblock %}
+{% block title %}Create Research Environment{% endblock %}
 
 {% block local_js_top %}
-<script src="{% static 'environment/js/cookie.js' %}"></script>
 <script src="{% static 'environment/js/forms.js' %}"></script>
 {% endblock %}
 
+{% block local_css %}
+<link rel="stylesheet" type="text/css" href="{% static 'environment/css/environment-base.css' %}">
+<link rel="stylesheet" type="text/css" href="{% static 'environment/css/create_research_environment.css' %}">
+{% endblock %}
+
 {% block content %}
-    <div class="container">
-      {% include "message_snippet.html" %}
-        <div class="jumbotron">
-          <h1>Research Environments Home</h1>
-          <p class="lead">
-            Here you can manage the research environments for your projects.
-          </p>
+<div class="container">
+  {% include "message_snippet.html" %}
+    <h1 class="mb-4">
+      Create Workspace
+    </h1>
+    <div class="container-body">
+      <div class="card" style="width: 36rem;">
+        <div class="card-body">
+          <form class="single-submit-form" action="{% url 'create_workspace' %}" method="post" style="width: 24rem;">
+            {% csrf_token %}
+            {{ form }}
+            <button
+              class="btn btn-primary mt-3"
+              type="submit"
+            >
+                Create workspace
+            </button>
+          </form>
         </div>
-
-        {% block main_view %}
-        {% endblock %}
+      </div>
     </div>
+</div>
 {% endblock %}
-
-{% block local_js_bottom %}{% endblock %}
```

#### html2text {}

```diff
@@ -1,9 +1,10 @@
 {% extends 'base.html' %} {% load static %} {% load project_templatetags %} {%
-block title %}Research environments{% endblock %} {% block local_css %}
- {% endblock %} {% block local_js_top %}
+block title %}Create Research Environment{% endblock %} {% block local_js_top
+%}
+ {% endblock %} {% block local_css %}
+
  {% endblock %} {% block content %}
 {% include "message_snippet.html" %}
-****** Research Environments Home ******
-Here you can manage the research environments for your projects.
-{% block main_view %} {% endblock %}
-{% endblock %} {% block local_js_bottom %}{% endblock %}
+****** Create Workspace ******
+{% csrf_token %} {{ form }}  Create workspace
+{% endblock %}
```

### Comparing `hdn-research-environment-2.1.5/environment/templates/environment/create_research_environment.html` & `hdn-research-environment-2.1.6/environment/templates/environment/create_research_environment.html`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.1.5/environment/templates/environment/identity_provisioning.html` & `hdn-research-environment-2.1.6/environment/templates/environment/identity_provisioning.html`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.1.5/environment/templates/environment/manage_billing_account.html` & `hdn-research-environment-2.1.6/environment/templates/environment/manage_billing_account.html`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.1.5/environment/templates/environment/manage_shared_billing_invitation.html` & `hdn-research-environment-2.1.6/environment/templates/environment/manage_shared_billing_invitation.html`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.1.5/environment/templates/environment/research_environments.html` & `hdn-research-environment-2.1.6/environment/templates/environment/research_environments.html`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.1.5/environment/templates/tag/environment_modal_button.html` & `hdn-research-environment-2.1.6/environment/templates/tag/environment_modal_button.html`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.1.5/environment/templatetags/action_buttons.py` & `hdn-research-environment-2.1.6/environment/templatetags/action_buttons.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.1.5/environment/tests/helpers.py` & `hdn-research-environment-2.1.6/environment/tests/helpers.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.1.5/environment/tests/mocks.py` & `hdn-research-environment-2.1.6/environment/tests/mocks.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.1.5/environment/tests/test_decorators.py` & `hdn-research-environment-2.1.6/environment/tests/test_decorators.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.1.5/environment/tests/test_services.py` & `hdn-research-environment-2.1.6/environment/tests/test_services.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.1.5/environment/tests/test_signals.py` & `hdn-research-environment-2.1.6/environment/tests/test_signals.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.1.5/environment/tests/test_utilities.py` & `hdn-research-environment-2.1.6/environment/tests/test_utilities.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.1.5/environment/tests/test_validators.py` & `hdn-research-environment-2.1.6/environment/tests/test_validators.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.1.5/environment/tests/test_views.py` & `hdn-research-environment-2.1.6/environment/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.1.5/environment/urls.py` & `hdn-research-environment-2.1.6/environment/urls.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.1.5/environment/utilities.py` & `hdn-research-environment-2.1.6/environment/utilities.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.1.5/environment/views.py` & `hdn-research-environment-2.1.6/environment/views.py`

 * *Files 2% similar despite different names*

```diff
@@ -257,14 +257,15 @@
 
 
 @require_http_methods(["GET", "POST"])
 @login_required
 @cloud_identity_required
 @transaction.atomic
 def manage_billing_account(request, billing_account_id):
+    # TODO: Check whether the user is the billing account's owner
     owner = request.user
     billing_account_sharing_form = ShareBillingAccountForm()
 
     if request.method == "POST":
         form_action = request.POST["action"]
         if form_action == "share_account":
             billing_account_sharing_form = ShareBillingAccountForm(request.POST)
@@ -300,26 +301,30 @@
 
 @require_http_methods(["GET", "POST"])
 @login_required
 def confirm_billing_account_sharing(request):
     if request.method == "POST":
         token = request.POST["token"]
         services.consume_billing_account_sharing_token(user=request.user, token=token)
-    else:
-        token = request.GET.get("token")
-        if token:
-            invite = BillingAccountSharingInvite.objects.select_related("owner").get(
-                token=token, is_revoked=False
-            )
-            context = {"token": token, "invitation_owner": invite.owner}
-            return render(
-                request, "environment/manage_shared_billing_invitation.html", context
-            )
+        messages.info(
+            request,
+            "You accepted the billing invitation! The account will be accessible in a few moments.",
+        )
+        return redirect("research_environments")
+
+    token = request.GET.get("token")
+    if not token:
+        messages.error(request, "The invitation is either invalid or expired.")
+        return redirect("research_environments")
 
-    return redirect("research_environments")
+    invite = BillingAccountSharingInvite.objects.select_related("owner").get(
+        token=token, is_revoked=False
+    )
+    context = {"token": token, "invitation_owner": invite.owner}
+    return render(request, "environment/manage_shared_billing_invitation.html", context)
 
 
 @require_PATCH
 @login_required
 @cloud_identity_required
 def stop_running_environment(request):
     data = json.loads(request.body)
```

### Comparing `hdn-research-environment-2.1.5/hdn_research_environment.egg-info/PKG-INFO` & `hdn-research-environment-2.1.6/hdn_research_environment.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: hdn-research-environment
-Version: 2.1.5
+Version: 2.1.6
 Summary: A Django app for supporting cloud-native research environments
 Home-page: https://www.healthdatanexus.ai/
 Author: Your Name
 Author-email: yourname@example.com
 License: BSD-3-Clause  # Example license
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `hdn-research-environment-2.1.5/hdn_research_environment.egg-info/SOURCES.txt` & `hdn-research-environment-2.1.6/hdn_research_environment.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.1.5/setup.cfg` & `hdn-research-environment-2.1.6/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = hdn-research-environment
-version = 2.1.5
+version = 2.1.6
 description = A Django app for supporting cloud-native research environments
 long_description = file: README.rst
 url = https://www.healthdatanexus.ai/
 author = Your Name
 author_email = yourname@example.com
 license = BSD-3-Clause  # Example license
 classifiers =
```

