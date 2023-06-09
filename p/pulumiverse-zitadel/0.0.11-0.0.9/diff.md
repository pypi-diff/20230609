# Comparing `tmp/pulumiverse_zitadel-0.0.11.tar.gz` & `tmp/pulumiverse_zitadel-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumiverse_zitadel-0.0.11.tar", last modified: Fri Jun  9 15:15:42 2023, max compression
+gzip compressed data, was "pulumiverse_zitadel-0.0.9.tar", last modified: Tue Jun  6 12:43:48 2023, max compression
```

## Comparing `pulumiverse_zitadel-0.0.11.tar` & `pulumiverse_zitadel-0.0.9.tar`

### file list

```diff
@@ -1,97 +1,97 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 15:15:42.153008 pulumiverse_zitadel-0.0.11/
--rw-r--r--   0 runner    (1001) docker     (123)     1929 2023-06-09 15:15:42.153008 pulumiverse_zitadel-0.0.11/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-06-09 15:15:41.000000 pulumiverse_zitadel-0.0.11/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 15:15:42.149008 pulumiverse_zitadel-0.0.11/pulumiverse_zitadel/
--rw-r--r--   0 runner    (1001) docker     (123)    12043 2023-06-09 15:15:41.000000 pulumiverse_zitadel-0.0.11/pulumiverse_zitadel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8114 2023-06-09 15:15:41.000000 pulumiverse_zitadel-0.0.11/pulumiverse_zitadel/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)    13457 2023-06-09 15:15:41.000000 pulumiverse_zitadel-0.0.11/pulumiverse_zitadel/action.py
--rw-r--r--   0 runner    (1001) docker     (123)    14287 2023-06-09 15:15:41.000000 pulumiverse_zitadel-0.0.11/pulumiverse_zitadel/application_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    15119 2023-06-09 15:15:41.000000 pulumiverse_zitadel-0.0.11/pulumiverse_zitadel/application_key.py
--rw-r--r--   0 runner    (1001) docker     (123)    45742 2023-06-09 15:15:41.000000 pulumiverse_zitadel-0.0.11/pulumiverse_zitadel/application_oidc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 15:15:42.153008 pulumiverse_zitadel-0.0.11/pulumiverse_zitadel/config/
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-06-09 15:15:41.000000 pulumiverse_zitadel-0.0.11/pulumiverse_zitadel/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-06-09 15:15:41.000000 pulumiverse_zitadel-0.0.11/pulumiverse_zitadel/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (123)    11580 2023-06-09 15:15:41.000000 pulumiverse_zitadel-0.0.11/pulumiverse_zitadel/default_domain_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)    45360 2023-06-09 15:15:41.000000 pulumiverse_zitadel-0.0.11/pulumiverse_zitadel/default_label_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)     7462 2023-06-09 15:15:41.000000 pulumiverse_zitadel-0.0.11/pulumiverse_zitadel/default_lockout_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)    50208 2023-06-09 15:15:41.000000 pulumiverse_zitadel-0.0.11/pulumiverse_zitadel/default_login_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)     6670 2023-06-09 15:15:41.000000 pulumiverse_zitadel-0.0.11/pulumiverse_zitadel/default_notification_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)    15233 2023-06-09 15:15:41.000000 pulumiverse_zitadel-0.0.11/pulumiverse_zitadel/default_password_complexity_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)     8693 2023-06-09 15:15:41.000000 pulumiverse_zitadel-0.0.11/pulumiverse_zitadel/default_privacy_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)    11147 2023-06-09 15:15:41.000000 pulumiverse_zitadel-0.0.11/pulumiverse_zitadel/domain.py
--rw-r--r--   0 runner    (1001) docker     (123)    13246 2023-06-09 15:15:41.000000 pulumiverse_zitadel-0.0.11/pulumiverse_zitadel/domain_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)     5857 2023-06-09 15:15:41.000000 pulumiverse_zitadel-0.0.11/pulumiverse_zitadel/get_action.py
--rw-r--r--   0 runner    (1001) docker     (123)     5843 2023-06-09 15:15:41.000000 pulumiverse_zitadel-0.0.11/pulumiverse_zitadel/get_application_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    12969 2023-06-09 15:15:41.000000 pulumiverse_zitadel-0.0.11/pulumiverse_zitadel/get_application_oidc.py
--rw-r--r--   0 runner    (1001) docker     (123)    10756 2023-06-09 15:15:41.000000 pulumiverse_zitadel-0.0.11/pulumiverse_zitadel/get_human_user.py
--rw-r--r--   0 runner    (1001) docker     (123)     8287 2023-06-09 15:15:41.000000 pulumiverse_zitadel-0.0.11/pulumiverse_zitadel/get_idp_azure_ad.py
--rw-r--r--   0 runner    (1001) docker     (123)     6764 2023-06-09 15:15:41.000000 pulumiverse_zitadel-0.0.11/pulumiverse_zitadel/get_idp_github.py
--rw-r--r--   0 runner    (1001) docker     (123)     8527 2023-06-09 15:15:41.000000 pulumiverse_zitadel-0.0.11/pulumiverse_zitadel/get_idp_github_es.py
--rw-r--r--   0 runner    (1001) docker     (123)     6764 2023-06-09 15:15:41.000000 pulumiverse_zitadel-0.0.11/pulumiverse_zitadel/get_idp_gitlab.py
--rw-r--r--   0 runner    (1001) docker     (123)     7452 2023-06-09 15:15:41.000000 pulumiverse_zitadel-0.0.11/pulumiverse_zitadel/get_idp_gitlab_self_hosted.py
--rw-r--r--   0 runner    (1001) docker     (123)     6764 2023-06-09 15:15:41.000000 pulumiverse_zitadel-0.0.11/pulumiverse_zitadel/get_idp_google.py
--rw-r--r--   0 runner    (1001) docker     (123)    17580 2023-06-09 15:15:41.000000 pulumiverse_zitadel-0.0.11/pulumiverse_zitadel/get_idp_ldap.py
--rw-r--r--   0 runner    (1001) docker     (123)     7401 2023-06-09 15:15:41.000000 pulumiverse_zitadel-0.0.11/pulumiverse_zitadel/get_machine_user.py
--rw-r--r--   0 runner    (1001) docker     (123)     3534 2023-06-09 15:15:41.000000 pulumiverse_zitadel-0.0.11/pulumiverse_zitadel/get_org.py
--rw-r--r--   0 runner    (1001) docker     (123)     9042 2023-06-09 15:15:41.000000 pulumiverse_zitadel-0.0.11/pulumiverse_zitadel/get_org_idp_azure_ad.py
--rw-r--r--   0 runner    (1001) docker     (123)     7515 2023-06-09 15:15:41.000000 pulumiverse_zitadel-0.0.11/pulumiverse_zitadel/get_org_idp_github.py
--rw-r--r--   0 runner    (1001) docker     (123)     9284 2023-06-09 15:15:41.000000 pulumiverse_zitadel-0.0.11/pulumiverse_zitadel/get_org_idp_github_es.py
--rw-r--r--   0 runner    (1001) docker     (123)     7515 2023-06-09 15:15:41.000000 pulumiverse_zitadel-0.0.11/pulumiverse_zitadel/get_org_idp_gitlab.py
--rw-r--r--   0 runner    (1001) docker     (123)     8227 2023-06-09 15:15:41.000000 pulumiverse_zitadel-0.0.11/pulumiverse_zitadel/get_org_idp_gitlab_self_hosted.py
--rw-r--r--   0 runner    (1001) docker     (123)     7515 2023-06-09 15:15:41.000000 pulumiverse_zitadel-0.0.11/pulumiverse_zitadel/get_org_idp_google.py
--rw-r--r--   0 runner    (1001) docker     (123)    18327 2023-06-09 15:15:41.000000 pulumiverse_zitadel-0.0.11/pulumiverse_zitadel/get_org_idp_ldap.py
--rw-r--r--   0 runner    (1001) docker     (123)     7296 2023-06-09 15:15:41.000000 pulumiverse_zitadel-0.0.11/pulumiverse_zitadel/get_org_jwt_idp.py
--rw-r--r--   0 runner    (1001) docker     (123)     8438 2023-06-09 15:15:41.000000 pulumiverse_zitadel-0.0.11/pulumiverse_zitadel/get_org_oidc_idp.py
--rw-r--r--   0 runner    (1001) docker     (123)     7367 2023-06-09 15:15:41.000000 pulumiverse_zitadel-0.0.11/pulumiverse_zitadel/get_project.py
--rw-r--r--   0 runner    (1001) docker     (123)     5689 2023-06-09 15:15:41.000000 pulumiverse_zitadel-0.0.11/pulumiverse_zitadel/get_project_role.py
--rw-r--r--   0 runner    (1001) docker     (123)     5601 2023-06-09 15:15:41.000000 pulumiverse_zitadel-0.0.11/pulumiverse_zitadel/get_trigger_actions.py
--rw-r--r--   0 runner    (1001) docker     (123)    33529 2023-06-09 15:15:41.000000 pulumiverse_zitadel-0.0.11/pulumiverse_zitadel/human_user.py
--rw-r--r--   0 runner    (1001) docker     (123)    28937 2023-06-09 15:15:41.000000 pulumiverse_zitadel-0.0.11/pulumiverse_zitadel/idp_azure_ad.py
--rw-r--r--   0 runner    (1001) docker     (123)    22799 2023-06-09 15:15:41.000000 pulumiverse_zitadel-0.0.11/pulumiverse_zitadel/idp_github.py
--rw-r--r--   0 runner    (1001) docker     (123)    29524 2023-06-09 15:15:41.000000 pulumiverse_zitadel-0.0.11/pulumiverse_zitadel/idp_github_es.py
--rw-r--r--   0 runner    (1001) docker     (123)    22795 2023-06-09 15:15:41.000000 pulumiverse_zitadel-0.0.11/pulumiverse_zitadel/idp_gitlab.py
--rw-r--r--   0 runner    (1001) docker     (123)    24794 2023-06-09 15:15:41.000000 pulumiverse_zitadel-0.0.11/pulumiverse_zitadel/idp_gitlab_self_hosted.py
--rw-r--r--   0 runner    (1001) docker     (123)    22797 2023-06-09 15:15:41.000000 pulumiverse_zitadel-0.0.11/pulumiverse_zitadel/idp_google.py
--rw-r--r--   0 runner    (1001) docker     (123)    64252 2023-06-09 15:15:41.000000 pulumiverse_zitadel-0.0.11/pulumiverse_zitadel/idp_ldap.py
--rw-r--r--   0 runner    (1001) docker     (123)     8645 2023-06-09 15:15:41.000000 pulumiverse_zitadel-0.0.11/pulumiverse_zitadel/instance_member.py
--rw-r--r--   0 runner    (1001) docker     (123)    47062 2023-06-09 15:15:41.000000 pulumiverse_zitadel-0.0.11/pulumiverse_zitadel/label_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)     9092 2023-06-09 15:15:41.000000 pulumiverse_zitadel-0.0.11/pulumiverse_zitadel/lockout_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)    52162 2023-06-09 15:15:41.000000 pulumiverse_zitadel-0.0.11/pulumiverse_zitadel/login_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)    13142 2023-06-09 15:15:41.000000 pulumiverse_zitadel-0.0.11/pulumiverse_zitadel/machine_key.py
--rw-r--r--   0 runner    (1001) docker     (123)    16891 2023-06-09 15:15:41.000000 pulumiverse_zitadel-0.0.11/pulumiverse_zitadel/machine_user.py
--rw-r--r--   0 runner    (1001) docker     (123)     8360 2023-06-09 15:15:41.000000 pulumiverse_zitadel-0.0.11/pulumiverse_zitadel/notification_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)     5717 2023-06-09 15:15:41.000000 pulumiverse_zitadel-0.0.11/pulumiverse_zitadel/org.py
--rw-r--r--   0 runner    (1001) docker     (123)    30788 2023-06-09 15:15:41.000000 pulumiverse_zitadel-0.0.11/pulumiverse_zitadel/org_idp_azure_ad.py
--rw-r--r--   0 runner    (1001) docker     (123)    24650 2023-06-09 15:15:41.000000 pulumiverse_zitadel-0.0.11/pulumiverse_zitadel/org_idp_github.py
--rw-r--r--   0 runner    (1001) docker     (123)    31375 2023-06-09 15:15:41.000000 pulumiverse_zitadel-0.0.11/pulumiverse_zitadel/org_idp_github_es.py
--rw-r--r--   0 runner    (1001) docker     (123)    24646 2023-06-09 15:15:41.000000 pulumiverse_zitadel-0.0.11/pulumiverse_zitadel/org_idp_gitlab.py
--rw-r--r--   0 runner    (1001) docker     (123)    26645 2023-06-09 15:15:41.000000 pulumiverse_zitadel-0.0.11/pulumiverse_zitadel/org_idp_gitlab_self_hosted.py
--rw-r--r--   0 runner    (1001) docker     (123)    24648 2023-06-09 15:15:41.000000 pulumiverse_zitadel-0.0.11/pulumiverse_zitadel/org_idp_google.py
--rw-r--r--   0 runner    (1001) docker     (123)    20863 2023-06-09 15:15:41.000000 pulumiverse_zitadel-0.0.11/pulumiverse_zitadel/org_idp_jwt.py
--rw-r--r--   0 runner    (1001) docker     (123)    66103 2023-06-09 15:15:41.000000 pulumiverse_zitadel-0.0.11/pulumiverse_zitadel/org_idp_ldap.py
--rw-r--r--   0 runner    (1001) docker     (123)    25923 2023-06-09 15:15:41.000000 pulumiverse_zitadel-0.0.11/pulumiverse_zitadel/org_idp_oidc.py
--rw-r--r--   0 runner    (1001) docker     (123)     9677 2023-06-09 15:15:41.000000 pulumiverse_zitadel-0.0.11/pulumiverse_zitadel/org_member.py
--rw-r--r--   0 runner    (1001) docker     (123)    16899 2023-06-09 15:15:41.000000 pulumiverse_zitadel-0.0.11/pulumiverse_zitadel/password_complexity_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)    10929 2023-06-09 15:15:41.000000 pulumiverse_zitadel-0.0.11/pulumiverse_zitadel/personal_access_token.py
--rw-r--r--   0 runner    (1001) docker     (123)    10359 2023-06-09 15:15:41.000000 pulumiverse_zitadel-0.0.11/pulumiverse_zitadel/privacy_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)    19824 2023-06-09 15:15:41.000000 pulumiverse_zitadel-0.0.11/pulumiverse_zitadel/project.py
--rw-r--r--   0 runner    (1001) docker     (123)    12627 2023-06-09 15:15:41.000000 pulumiverse_zitadel-0.0.11/pulumiverse_zitadel/project_grant.py
--rw-r--r--   0 runner    (1001) docker     (123)    13871 2023-06-09 15:15:41.000000 pulumiverse_zitadel-0.0.11/pulumiverse_zitadel/project_grant_member.py
--rw-r--r--   0 runner    (1001) docker     (123)    11853 2023-06-09 15:15:41.000000 pulumiverse_zitadel-0.0.11/pulumiverse_zitadel/project_member.py
--rw-r--r--   0 runner    (1001) docker     (123)    13359 2023-06-09 15:15:41.000000 pulumiverse_zitadel-0.0.11/pulumiverse_zitadel/project_role.py
--rw-r--r--   0 runner    (1001) docker     (123)    10540 2023-06-09 15:15:41.000000 pulumiverse_zitadel-0.0.11/pulumiverse_zitadel/provider.py
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-06-09 15:15:41.000000 pulumiverse_zitadel-0.0.11/pulumiverse_zitadel/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 15:15:41.000000 pulumiverse_zitadel-0.0.11/pulumiverse_zitadel/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     9878 2023-06-09 15:15:41.000000 pulumiverse_zitadel-0.0.11/pulumiverse_zitadel/sms_provider_twilio.py
--rw-r--r--   0 runner    (1001) docker     (123)    15380 2023-06-09 15:15:41.000000 pulumiverse_zitadel-0.0.11/pulumiverse_zitadel/smtp_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    14150 2023-06-09 15:15:41.000000 pulumiverse_zitadel-0.0.11/pulumiverse_zitadel/trigger_actions.py
--rw-r--r--   0 runner    (1001) docker     (123)    13866 2023-06-09 15:15:41.000000 pulumiverse_zitadel-0.0.11/pulumiverse_zitadel/user_grant.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 15:15:42.153008 pulumiverse_zitadel-0.0.11/pulumiverse_zitadel.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1929 2023-06-09 15:15:42.000000 pulumiverse_zitadel-0.0.11/pulumiverse_zitadel.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3513 2023-06-09 15:15:42.000000 pulumiverse_zitadel-0.0.11/pulumiverse_zitadel.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 15:15:42.000000 pulumiverse_zitadel-0.0.11/pulumiverse_zitadel.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 15:15:42.000000 pulumiverse_zitadel-0.0.11/pulumiverse_zitadel.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-09 15:15:42.000000 pulumiverse_zitadel-0.0.11/pulumiverse_zitadel.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-09 15:15:42.000000 pulumiverse_zitadel-0.0.11/pulumiverse_zitadel.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-09 15:15:42.153008 pulumiverse_zitadel-0.0.11/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2184 2023-06-09 15:15:41.000000 pulumiverse_zitadel-0.0.11/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:43:48.174273 pulumiverse_zitadel-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1937 2023-06-06 12:43:48.174273 pulumiverse_zitadel-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-06-06 12:43:47.000000 pulumiverse_zitadel-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:43:48.170273 pulumiverse_zitadel-0.0.9/pulumiverse_zitadel/
+-rw-r--r--   0 runner    (1001) docker     (123)    12043 2023-06-06 12:43:47.000000 pulumiverse_zitadel-0.0.9/pulumiverse_zitadel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8114 2023-06-06 12:43:47.000000 pulumiverse_zitadel-0.0.9/pulumiverse_zitadel/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13457 2023-06-06 12:43:47.000000 pulumiverse_zitadel-0.0.9/pulumiverse_zitadel/action.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14287 2023-06-06 12:43:47.000000 pulumiverse_zitadel-0.0.9/pulumiverse_zitadel/application_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15119 2023-06-06 12:43:47.000000 pulumiverse_zitadel-0.0.9/pulumiverse_zitadel/application_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45742 2023-06-06 12:43:47.000000 pulumiverse_zitadel-0.0.9/pulumiverse_zitadel/application_oidc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:43:48.174273 pulumiverse_zitadel-0.0.9/pulumiverse_zitadel/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-06-06 12:43:47.000000 pulumiverse_zitadel-0.0.9/pulumiverse_zitadel/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-06-06 12:43:47.000000 pulumiverse_zitadel-0.0.9/pulumiverse_zitadel/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11580 2023-06-06 12:43:47.000000 pulumiverse_zitadel-0.0.9/pulumiverse_zitadel/default_domain_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45360 2023-06-06 12:43:47.000000 pulumiverse_zitadel-0.0.9/pulumiverse_zitadel/default_label_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7462 2023-06-06 12:43:47.000000 pulumiverse_zitadel-0.0.9/pulumiverse_zitadel/default_lockout_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50208 2023-06-06 12:43:47.000000 pulumiverse_zitadel-0.0.9/pulumiverse_zitadel/default_login_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6670 2023-06-06 12:43:47.000000 pulumiverse_zitadel-0.0.9/pulumiverse_zitadel/default_notification_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15233 2023-06-06 12:43:47.000000 pulumiverse_zitadel-0.0.9/pulumiverse_zitadel/default_password_complexity_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8693 2023-06-06 12:43:47.000000 pulumiverse_zitadel-0.0.9/pulumiverse_zitadel/default_privacy_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11147 2023-06-06 12:43:47.000000 pulumiverse_zitadel-0.0.9/pulumiverse_zitadel/domain.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13246 2023-06-06 12:43:47.000000 pulumiverse_zitadel-0.0.9/pulumiverse_zitadel/domain_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5857 2023-06-06 12:43:47.000000 pulumiverse_zitadel-0.0.9/pulumiverse_zitadel/get_action.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5843 2023-06-06 12:43:47.000000 pulumiverse_zitadel-0.0.9/pulumiverse_zitadel/get_application_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12969 2023-06-06 12:43:47.000000 pulumiverse_zitadel-0.0.9/pulumiverse_zitadel/get_application_oidc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10756 2023-06-06 12:43:47.000000 pulumiverse_zitadel-0.0.9/pulumiverse_zitadel/get_human_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8287 2023-06-06 12:43:47.000000 pulumiverse_zitadel-0.0.9/pulumiverse_zitadel/get_idp_azure_ad.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6764 2023-06-06 12:43:47.000000 pulumiverse_zitadel-0.0.9/pulumiverse_zitadel/get_idp_github.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8527 2023-06-06 12:43:47.000000 pulumiverse_zitadel-0.0.9/pulumiverse_zitadel/get_idp_github_es.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6764 2023-06-06 12:43:47.000000 pulumiverse_zitadel-0.0.9/pulumiverse_zitadel/get_idp_gitlab.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7452 2023-06-06 12:43:47.000000 pulumiverse_zitadel-0.0.9/pulumiverse_zitadel/get_idp_gitlab_self_hosted.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6764 2023-06-06 12:43:47.000000 pulumiverse_zitadel-0.0.9/pulumiverse_zitadel/get_idp_google.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17580 2023-06-06 12:43:47.000000 pulumiverse_zitadel-0.0.9/pulumiverse_zitadel/get_idp_ldap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7401 2023-06-06 12:43:47.000000 pulumiverse_zitadel-0.0.9/pulumiverse_zitadel/get_machine_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3534 2023-06-06 12:43:47.000000 pulumiverse_zitadel-0.0.9/pulumiverse_zitadel/get_org.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9042 2023-06-06 12:43:47.000000 pulumiverse_zitadel-0.0.9/pulumiverse_zitadel/get_org_idp_azure_ad.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7515 2023-06-06 12:43:47.000000 pulumiverse_zitadel-0.0.9/pulumiverse_zitadel/get_org_idp_github.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9284 2023-06-06 12:43:47.000000 pulumiverse_zitadel-0.0.9/pulumiverse_zitadel/get_org_idp_github_es.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7515 2023-06-06 12:43:47.000000 pulumiverse_zitadel-0.0.9/pulumiverse_zitadel/get_org_idp_gitlab.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8227 2023-06-06 12:43:47.000000 pulumiverse_zitadel-0.0.9/pulumiverse_zitadel/get_org_idp_gitlab_self_hosted.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7515 2023-06-06 12:43:47.000000 pulumiverse_zitadel-0.0.9/pulumiverse_zitadel/get_org_idp_google.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18327 2023-06-06 12:43:47.000000 pulumiverse_zitadel-0.0.9/pulumiverse_zitadel/get_org_idp_ldap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7296 2023-06-06 12:43:47.000000 pulumiverse_zitadel-0.0.9/pulumiverse_zitadel/get_org_jwt_idp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8438 2023-06-06 12:43:47.000000 pulumiverse_zitadel-0.0.9/pulumiverse_zitadel/get_org_oidc_idp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7367 2023-06-06 12:43:47.000000 pulumiverse_zitadel-0.0.9/pulumiverse_zitadel/get_project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5689 2023-06-06 12:43:47.000000 pulumiverse_zitadel-0.0.9/pulumiverse_zitadel/get_project_role.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5601 2023-06-06 12:43:47.000000 pulumiverse_zitadel-0.0.9/pulumiverse_zitadel/get_trigger_actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33529 2023-06-06 12:43:47.000000 pulumiverse_zitadel-0.0.9/pulumiverse_zitadel/human_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28937 2023-06-06 12:43:47.000000 pulumiverse_zitadel-0.0.9/pulumiverse_zitadel/idp_azure_ad.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22799 2023-06-06 12:43:47.000000 pulumiverse_zitadel-0.0.9/pulumiverse_zitadel/idp_github.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29524 2023-06-06 12:43:47.000000 pulumiverse_zitadel-0.0.9/pulumiverse_zitadel/idp_github_es.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22795 2023-06-06 12:43:47.000000 pulumiverse_zitadel-0.0.9/pulumiverse_zitadel/idp_gitlab.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24794 2023-06-06 12:43:47.000000 pulumiverse_zitadel-0.0.9/pulumiverse_zitadel/idp_gitlab_self_hosted.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22797 2023-06-06 12:43:47.000000 pulumiverse_zitadel-0.0.9/pulumiverse_zitadel/idp_google.py
+-rw-r--r--   0 runner    (1001) docker     (123)    64252 2023-06-06 12:43:47.000000 pulumiverse_zitadel-0.0.9/pulumiverse_zitadel/idp_ldap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8645 2023-06-06 12:43:47.000000 pulumiverse_zitadel-0.0.9/pulumiverse_zitadel/instance_member.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47062 2023-06-06 12:43:47.000000 pulumiverse_zitadel-0.0.9/pulumiverse_zitadel/label_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9092 2023-06-06 12:43:47.000000 pulumiverse_zitadel-0.0.9/pulumiverse_zitadel/lockout_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52162 2023-06-06 12:43:47.000000 pulumiverse_zitadel-0.0.9/pulumiverse_zitadel/login_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13142 2023-06-06 12:43:47.000000 pulumiverse_zitadel-0.0.9/pulumiverse_zitadel/machine_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16891 2023-06-06 12:43:47.000000 pulumiverse_zitadel-0.0.9/pulumiverse_zitadel/machine_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8360 2023-06-06 12:43:47.000000 pulumiverse_zitadel-0.0.9/pulumiverse_zitadel/notification_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5717 2023-06-06 12:43:47.000000 pulumiverse_zitadel-0.0.9/pulumiverse_zitadel/org.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30788 2023-06-06 12:43:47.000000 pulumiverse_zitadel-0.0.9/pulumiverse_zitadel/org_idp_azure_ad.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24650 2023-06-06 12:43:47.000000 pulumiverse_zitadel-0.0.9/pulumiverse_zitadel/org_idp_github.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31375 2023-06-06 12:43:47.000000 pulumiverse_zitadel-0.0.9/pulumiverse_zitadel/org_idp_github_es.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24646 2023-06-06 12:43:47.000000 pulumiverse_zitadel-0.0.9/pulumiverse_zitadel/org_idp_gitlab.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26645 2023-06-06 12:43:47.000000 pulumiverse_zitadel-0.0.9/pulumiverse_zitadel/org_idp_gitlab_self_hosted.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24648 2023-06-06 12:43:47.000000 pulumiverse_zitadel-0.0.9/pulumiverse_zitadel/org_idp_google.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20863 2023-06-06 12:43:47.000000 pulumiverse_zitadel-0.0.9/pulumiverse_zitadel/org_idp_jwt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    66103 2023-06-06 12:43:47.000000 pulumiverse_zitadel-0.0.9/pulumiverse_zitadel/org_idp_ldap.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25923 2023-06-06 12:43:47.000000 pulumiverse_zitadel-0.0.9/pulumiverse_zitadel/org_idp_oidc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9677 2023-06-06 12:43:47.000000 pulumiverse_zitadel-0.0.9/pulumiverse_zitadel/org_member.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16899 2023-06-06 12:43:47.000000 pulumiverse_zitadel-0.0.9/pulumiverse_zitadel/password_complexity_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10929 2023-06-06 12:43:47.000000 pulumiverse_zitadel-0.0.9/pulumiverse_zitadel/personal_access_token.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10359 2023-06-06 12:43:47.000000 pulumiverse_zitadel-0.0.9/pulumiverse_zitadel/privacy_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19824 2023-06-06 12:43:47.000000 pulumiverse_zitadel-0.0.9/pulumiverse_zitadel/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12627 2023-06-06 12:43:47.000000 pulumiverse_zitadel-0.0.9/pulumiverse_zitadel/project_grant.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13871 2023-06-06 12:43:47.000000 pulumiverse_zitadel-0.0.9/pulumiverse_zitadel/project_grant_member.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11853 2023-06-06 12:43:47.000000 pulumiverse_zitadel-0.0.9/pulumiverse_zitadel/project_member.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13359 2023-06-06 12:43:47.000000 pulumiverse_zitadel-0.0.9/pulumiverse_zitadel/project_role.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10540 2023-06-06 12:43:47.000000 pulumiverse_zitadel-0.0.9/pulumiverse_zitadel/provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-06-06 12:43:47.000000 pulumiverse_zitadel-0.0.9/pulumiverse_zitadel/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 12:43:47.000000 pulumiverse_zitadel-0.0.9/pulumiverse_zitadel/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     9878 2023-06-06 12:43:47.000000 pulumiverse_zitadel-0.0.9/pulumiverse_zitadel/sms_provider_twilio.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15380 2023-06-06 12:43:47.000000 pulumiverse_zitadel-0.0.9/pulumiverse_zitadel/smtp_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14150 2023-06-06 12:43:47.000000 pulumiverse_zitadel-0.0.9/pulumiverse_zitadel/trigger_actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13866 2023-06-06 12:43:47.000000 pulumiverse_zitadel-0.0.9/pulumiverse_zitadel/user_grant.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:43:48.174273 pulumiverse_zitadel-0.0.9/pulumiverse_zitadel.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1937 2023-06-06 12:43:48.000000 pulumiverse_zitadel-0.0.9/pulumiverse_zitadel.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3513 2023-06-06 12:43:48.000000 pulumiverse_zitadel-0.0.9/pulumiverse_zitadel.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 12:43:48.000000 pulumiverse_zitadel-0.0.9/pulumiverse_zitadel.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 12:43:48.000000 pulumiverse_zitadel-0.0.9/pulumiverse_zitadel.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-06 12:43:48.000000 pulumiverse_zitadel-0.0.9/pulumiverse_zitadel.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-06 12:43:48.000000 pulumiverse_zitadel-0.0.9/pulumiverse_zitadel.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-06 12:43:48.174273 pulumiverse_zitadel-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-06-06 12:43:47.000000 pulumiverse_zitadel-0.0.9/setup.py
```

### Comparing `pulumiverse_zitadel-0.0.11/PKG-INFO` & `pulumiverse_zitadel-0.0.9/pulumiverse_zitadel.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
-Name: pulumiverse_zitadel
-Version: 0.0.11
+Name: pulumiverse-zitadel
+Version: 0.0.9
 Summary: A Pulumi package for creating and managing zitadel cloud resources.
 Home-page: https://www.pulumi.com
 License: Apache-2.0
-Project-URL: Repository, https://github.com/pulumiverse/pulumi-zitadel
+Project-URL: Repository, https://github.com/pulumi/pulumi-zitadel
 Keywords: pulumi zitadel category/cloud
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 
 # Zitadel Resource Provider
 
 The Zitadel Resource Provider lets you manage [Zitadel](https://zitadel.com/) resources.
@@ -18,21 +18,21 @@
 This package is available for several languages/platforms:
 
 ### Node.js (JavaScript/TypeScript)
 
 To use from JavaScript or TypeScript in Node.js, install using either `npm`:
 
 ```bash
-npm install @pulumiverse/zitadel
+npm install @pulumiverse/pulumi-zitadel
 ```
 
 or `yarn`:
 
 ```bash
-yarn add @pulumiverse/zitadel
+yarn add @pulumiverse/pulumi-zitadel
 ```
 
 ### Python
 
 To use from Python, install using `pip`:
 
 ```bash
```

### Comparing `pulumiverse_zitadel-0.0.11/README.md` & `pulumiverse_zitadel-0.0.9/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -7,21 +7,21 @@
 This package is available for several languages/platforms:
 
 ### Node.js (JavaScript/TypeScript)
 
 To use from JavaScript or TypeScript in Node.js, install using either `npm`:
 
 ```bash
-npm install @pulumiverse/zitadel
+npm install @pulumiverse/pulumi-zitadel
 ```
 
 or `yarn`:
 
 ```bash
-yarn add @pulumiverse/zitadel
+yarn add @pulumiverse/pulumi-zitadel
 ```
 
 ### Python
 
 To use from Python, install using `pip`:
 
 ```bash
```

### Comparing `pulumiverse_zitadel-0.0.11/pulumiverse_zitadel/__init__.py` & `pulumiverse_zitadel-0.0.9/pulumiverse_zitadel/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_zitadel-0.0.11/pulumiverse_zitadel/_utilities.py` & `pulumiverse_zitadel-0.0.9/pulumiverse_zitadel/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_zitadel-0.0.11/pulumiverse_zitadel/action.py` & `pulumiverse_zitadel-0.0.9/pulumiverse_zitadel/action.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_zitadel-0.0.11/pulumiverse_zitadel/application_api.py` & `pulumiverse_zitadel-0.0.9/pulumiverse_zitadel/application_api.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_zitadel-0.0.11/pulumiverse_zitadel/application_key.py` & `pulumiverse_zitadel-0.0.9/pulumiverse_zitadel/application_key.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_zitadel-0.0.11/pulumiverse_zitadel/application_oidc.py` & `pulumiverse_zitadel-0.0.9/pulumiverse_zitadel/application_oidc.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_zitadel-0.0.11/pulumiverse_zitadel/config/vars.py` & `pulumiverse_zitadel-0.0.9/pulumiverse_zitadel/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_zitadel-0.0.11/pulumiverse_zitadel/default_domain_policy.py` & `pulumiverse_zitadel-0.0.9/pulumiverse_zitadel/default_domain_policy.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_zitadel-0.0.11/pulumiverse_zitadel/default_label_policy.py` & `pulumiverse_zitadel-0.0.9/pulumiverse_zitadel/default_label_policy.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_zitadel-0.0.11/pulumiverse_zitadel/default_lockout_policy.py` & `pulumiverse_zitadel-0.0.9/pulumiverse_zitadel/default_lockout_policy.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_zitadel-0.0.11/pulumiverse_zitadel/default_login_policy.py` & `pulumiverse_zitadel-0.0.9/pulumiverse_zitadel/default_login_policy.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_zitadel-0.0.11/pulumiverse_zitadel/default_notification_policy.py` & `pulumiverse_zitadel-0.0.9/pulumiverse_zitadel/default_notification_policy.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_zitadel-0.0.11/pulumiverse_zitadel/default_password_complexity_policy.py` & `pulumiverse_zitadel-0.0.9/pulumiverse_zitadel/default_password_complexity_policy.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_zitadel-0.0.11/pulumiverse_zitadel/default_privacy_policy.py` & `pulumiverse_zitadel-0.0.9/pulumiverse_zitadel/default_privacy_policy.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_zitadel-0.0.11/pulumiverse_zitadel/domain.py` & `pulumiverse_zitadel-0.0.9/pulumiverse_zitadel/domain.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_zitadel-0.0.11/pulumiverse_zitadel/domain_policy.py` & `pulumiverse_zitadel-0.0.9/pulumiverse_zitadel/domain_policy.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_zitadel-0.0.11/pulumiverse_zitadel/get_action.py` & `pulumiverse_zitadel-0.0.9/pulumiverse_zitadel/get_action.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_zitadel-0.0.11/pulumiverse_zitadel/get_application_api.py` & `pulumiverse_zitadel-0.0.9/pulumiverse_zitadel/get_application_api.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_zitadel-0.0.11/pulumiverse_zitadel/get_application_oidc.py` & `pulumiverse_zitadel-0.0.9/pulumiverse_zitadel/get_application_oidc.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_zitadel-0.0.11/pulumiverse_zitadel/get_human_user.py` & `pulumiverse_zitadel-0.0.9/pulumiverse_zitadel/get_human_user.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_zitadel-0.0.11/pulumiverse_zitadel/get_idp_azure_ad.py` & `pulumiverse_zitadel-0.0.9/pulumiverse_zitadel/get_idp_azure_ad.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_zitadel-0.0.11/pulumiverse_zitadel/get_idp_github.py` & `pulumiverse_zitadel-0.0.9/pulumiverse_zitadel/get_idp_github.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_zitadel-0.0.11/pulumiverse_zitadel/get_idp_github_es.py` & `pulumiverse_zitadel-0.0.9/pulumiverse_zitadel/get_idp_github_es.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_zitadel-0.0.11/pulumiverse_zitadel/get_idp_gitlab.py` & `pulumiverse_zitadel-0.0.9/pulumiverse_zitadel/get_idp_gitlab.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_zitadel-0.0.11/pulumiverse_zitadel/get_idp_gitlab_self_hosted.py` & `pulumiverse_zitadel-0.0.9/pulumiverse_zitadel/get_idp_gitlab_self_hosted.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_zitadel-0.0.11/pulumiverse_zitadel/get_idp_google.py` & `pulumiverse_zitadel-0.0.9/pulumiverse_zitadel/get_idp_google.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_zitadel-0.0.11/pulumiverse_zitadel/get_idp_ldap.py` & `pulumiverse_zitadel-0.0.9/pulumiverse_zitadel/get_idp_ldap.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_zitadel-0.0.11/pulumiverse_zitadel/get_machine_user.py` & `pulumiverse_zitadel-0.0.9/pulumiverse_zitadel/get_machine_user.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_zitadel-0.0.11/pulumiverse_zitadel/get_org.py` & `pulumiverse_zitadel-0.0.9/pulumiverse_zitadel/get_org.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_zitadel-0.0.11/pulumiverse_zitadel/get_org_idp_azure_ad.py` & `pulumiverse_zitadel-0.0.9/pulumiverse_zitadel/get_org_idp_azure_ad.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_zitadel-0.0.11/pulumiverse_zitadel/get_org_idp_github.py` & `pulumiverse_zitadel-0.0.9/pulumiverse_zitadel/get_org_idp_github.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_zitadel-0.0.11/pulumiverse_zitadel/get_org_idp_github_es.py` & `pulumiverse_zitadel-0.0.9/pulumiverse_zitadel/get_org_idp_github_es.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_zitadel-0.0.11/pulumiverse_zitadel/get_org_idp_gitlab.py` & `pulumiverse_zitadel-0.0.9/pulumiverse_zitadel/get_org_idp_gitlab.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_zitadel-0.0.11/pulumiverse_zitadel/get_org_idp_gitlab_self_hosted.py` & `pulumiverse_zitadel-0.0.9/pulumiverse_zitadel/get_org_idp_gitlab_self_hosted.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_zitadel-0.0.11/pulumiverse_zitadel/get_org_idp_google.py` & `pulumiverse_zitadel-0.0.9/pulumiverse_zitadel/get_org_idp_google.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_zitadel-0.0.11/pulumiverse_zitadel/get_org_idp_ldap.py` & `pulumiverse_zitadel-0.0.9/pulumiverse_zitadel/get_org_idp_ldap.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_zitadel-0.0.11/pulumiverse_zitadel/get_org_jwt_idp.py` & `pulumiverse_zitadel-0.0.9/pulumiverse_zitadel/get_org_jwt_idp.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_zitadel-0.0.11/pulumiverse_zitadel/get_org_oidc_idp.py` & `pulumiverse_zitadel-0.0.9/pulumiverse_zitadel/get_org_oidc_idp.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_zitadel-0.0.11/pulumiverse_zitadel/get_project.py` & `pulumiverse_zitadel-0.0.9/pulumiverse_zitadel/get_project.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_zitadel-0.0.11/pulumiverse_zitadel/get_project_role.py` & `pulumiverse_zitadel-0.0.9/pulumiverse_zitadel/get_project_role.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_zitadel-0.0.11/pulumiverse_zitadel/get_trigger_actions.py` & `pulumiverse_zitadel-0.0.9/pulumiverse_zitadel/get_trigger_actions.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_zitadel-0.0.11/pulumiverse_zitadel/human_user.py` & `pulumiverse_zitadel-0.0.9/pulumiverse_zitadel/human_user.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_zitadel-0.0.11/pulumiverse_zitadel/idp_azure_ad.py` & `pulumiverse_zitadel-0.0.9/pulumiverse_zitadel/idp_azure_ad.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_zitadel-0.0.11/pulumiverse_zitadel/idp_github.py` & `pulumiverse_zitadel-0.0.9/pulumiverse_zitadel/idp_github.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_zitadel-0.0.11/pulumiverse_zitadel/idp_github_es.py` & `pulumiverse_zitadel-0.0.9/pulumiverse_zitadel/idp_github_es.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_zitadel-0.0.11/pulumiverse_zitadel/idp_gitlab.py` & `pulumiverse_zitadel-0.0.9/pulumiverse_zitadel/idp_gitlab.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_zitadel-0.0.11/pulumiverse_zitadel/idp_gitlab_self_hosted.py` & `pulumiverse_zitadel-0.0.9/pulumiverse_zitadel/idp_gitlab_self_hosted.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_zitadel-0.0.11/pulumiverse_zitadel/idp_google.py` & `pulumiverse_zitadel-0.0.9/pulumiverse_zitadel/idp_google.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_zitadel-0.0.11/pulumiverse_zitadel/idp_ldap.py` & `pulumiverse_zitadel-0.0.9/pulumiverse_zitadel/idp_ldap.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_zitadel-0.0.11/pulumiverse_zitadel/instance_member.py` & `pulumiverse_zitadel-0.0.9/pulumiverse_zitadel/instance_member.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_zitadel-0.0.11/pulumiverse_zitadel/label_policy.py` & `pulumiverse_zitadel-0.0.9/pulumiverse_zitadel/label_policy.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_zitadel-0.0.11/pulumiverse_zitadel/lockout_policy.py` & `pulumiverse_zitadel-0.0.9/pulumiverse_zitadel/lockout_policy.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_zitadel-0.0.11/pulumiverse_zitadel/login_policy.py` & `pulumiverse_zitadel-0.0.9/pulumiverse_zitadel/login_policy.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_zitadel-0.0.11/pulumiverse_zitadel/machine_key.py` & `pulumiverse_zitadel-0.0.9/pulumiverse_zitadel/machine_key.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_zitadel-0.0.11/pulumiverse_zitadel/machine_user.py` & `pulumiverse_zitadel-0.0.9/pulumiverse_zitadel/machine_user.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_zitadel-0.0.11/pulumiverse_zitadel/notification_policy.py` & `pulumiverse_zitadel-0.0.9/pulumiverse_zitadel/notification_policy.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_zitadel-0.0.11/pulumiverse_zitadel/org.py` & `pulumiverse_zitadel-0.0.9/pulumiverse_zitadel/org.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_zitadel-0.0.11/pulumiverse_zitadel/org_idp_azure_ad.py` & `pulumiverse_zitadel-0.0.9/pulumiverse_zitadel/org_idp_azure_ad.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_zitadel-0.0.11/pulumiverse_zitadel/org_idp_github.py` & `pulumiverse_zitadel-0.0.9/pulumiverse_zitadel/org_idp_github.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_zitadel-0.0.11/pulumiverse_zitadel/org_idp_github_es.py` & `pulumiverse_zitadel-0.0.9/pulumiverse_zitadel/org_idp_github_es.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_zitadel-0.0.11/pulumiverse_zitadel/org_idp_gitlab.py` & `pulumiverse_zitadel-0.0.9/pulumiverse_zitadel/org_idp_gitlab.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_zitadel-0.0.11/pulumiverse_zitadel/org_idp_gitlab_self_hosted.py` & `pulumiverse_zitadel-0.0.9/pulumiverse_zitadel/org_idp_gitlab_self_hosted.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_zitadel-0.0.11/pulumiverse_zitadel/org_idp_google.py` & `pulumiverse_zitadel-0.0.9/pulumiverse_zitadel/org_idp_google.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_zitadel-0.0.11/pulumiverse_zitadel/org_idp_jwt.py` & `pulumiverse_zitadel-0.0.9/pulumiverse_zitadel/org_idp_jwt.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_zitadel-0.0.11/pulumiverse_zitadel/org_idp_ldap.py` & `pulumiverse_zitadel-0.0.9/pulumiverse_zitadel/org_idp_ldap.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_zitadel-0.0.11/pulumiverse_zitadel/org_idp_oidc.py` & `pulumiverse_zitadel-0.0.9/pulumiverse_zitadel/org_idp_oidc.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_zitadel-0.0.11/pulumiverse_zitadel/org_member.py` & `pulumiverse_zitadel-0.0.9/pulumiverse_zitadel/org_member.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_zitadel-0.0.11/pulumiverse_zitadel/password_complexity_policy.py` & `pulumiverse_zitadel-0.0.9/pulumiverse_zitadel/password_complexity_policy.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_zitadel-0.0.11/pulumiverse_zitadel/personal_access_token.py` & `pulumiverse_zitadel-0.0.9/pulumiverse_zitadel/personal_access_token.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_zitadel-0.0.11/pulumiverse_zitadel/privacy_policy.py` & `pulumiverse_zitadel-0.0.9/pulumiverse_zitadel/privacy_policy.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_zitadel-0.0.11/pulumiverse_zitadel/project.py` & `pulumiverse_zitadel-0.0.9/pulumiverse_zitadel/project.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_zitadel-0.0.11/pulumiverse_zitadel/project_grant.py` & `pulumiverse_zitadel-0.0.9/pulumiverse_zitadel/project_grant.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_zitadel-0.0.11/pulumiverse_zitadel/project_grant_member.py` & `pulumiverse_zitadel-0.0.9/pulumiverse_zitadel/project_grant_member.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_zitadel-0.0.11/pulumiverse_zitadel/project_member.py` & `pulumiverse_zitadel-0.0.9/pulumiverse_zitadel/project_member.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_zitadel-0.0.11/pulumiverse_zitadel/project_role.py` & `pulumiverse_zitadel-0.0.9/pulumiverse_zitadel/project_role.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_zitadel-0.0.11/pulumiverse_zitadel/provider.py` & `pulumiverse_zitadel-0.0.9/pulumiverse_zitadel/provider.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_zitadel-0.0.11/pulumiverse_zitadel/sms_provider_twilio.py` & `pulumiverse_zitadel-0.0.9/pulumiverse_zitadel/sms_provider_twilio.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_zitadel-0.0.11/pulumiverse_zitadel/smtp_config.py` & `pulumiverse_zitadel-0.0.9/pulumiverse_zitadel/smtp_config.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_zitadel-0.0.11/pulumiverse_zitadel/trigger_actions.py` & `pulumiverse_zitadel-0.0.9/pulumiverse_zitadel/trigger_actions.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_zitadel-0.0.11/pulumiverse_zitadel/user_grant.py` & `pulumiverse_zitadel-0.0.9/pulumiverse_zitadel/user_grant.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_zitadel-0.0.11/pulumiverse_zitadel.egg-info/PKG-INFO` & `pulumiverse_zitadel-0.0.9/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
-Name: pulumiverse-zitadel
-Version: 0.0.11
+Name: pulumiverse_zitadel
+Version: 0.0.9
 Summary: A Pulumi package for creating and managing zitadel cloud resources.
 Home-page: https://www.pulumi.com
 License: Apache-2.0
-Project-URL: Repository, https://github.com/pulumiverse/pulumi-zitadel
+Project-URL: Repository, https://github.com/pulumi/pulumi-zitadel
 Keywords: pulumi zitadel category/cloud
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 
 # Zitadel Resource Provider
 
 The Zitadel Resource Provider lets you manage [Zitadel](https://zitadel.com/) resources.
@@ -18,21 +18,21 @@
 This package is available for several languages/platforms:
 
 ### Node.js (JavaScript/TypeScript)
 
 To use from JavaScript or TypeScript in Node.js, install using either `npm`:
 
 ```bash
-npm install @pulumiverse/zitadel
+npm install @pulumiverse/pulumi-zitadel
 ```
 
 or `yarn`:
 
 ```bash
-yarn add @pulumiverse/zitadel
+yarn add @pulumiverse/pulumi-zitadel
 ```
 
 ### Python
 
 To use from Python, install using `pip`:
 
 ```bash
```

### Comparing `pulumiverse_zitadel-0.0.11/pulumiverse_zitadel.egg-info/SOURCES.txt` & `pulumiverse_zitadel-0.0.9/pulumiverse_zitadel.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumiverse_zitadel-0.0.11/setup.py` & `pulumiverse_zitadel-0.0.9/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 import errno
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "0.0.11"
-PLUGIN_VERSION = "0.0.11"
+VERSION = "0.0.9"
+PLUGIN_VERSION = "0.0.9"
 
 class InstallPluginCommand(install):
     def run(self):
         install.run(self)
         try:
             check_call(['pulumi', 'plugin', 'install', 'resource', 'zitadel', PLUGIN_VERSION, '--server', 'github://api.github.com/pulumiverse'])
         except OSError as error:
@@ -44,15 +44,15 @@
       long_description_content_type='text/markdown',
       cmdclass={
           'install': InstallPluginCommand,
       },
       keywords='pulumi zitadel category/cloud',
       url='https://www.pulumi.com',
       project_urls={
-          'Repository': 'https://github.com/pulumiverse/pulumi-zitadel'
+          'Repository': 'https://github.com/pulumi/pulumi-zitadel'
       },
       license='Apache-2.0',
       packages=find_packages(),
       package_data={
           'pulumiverse_zitadel': [
               'py.typed',
               'pulumi-plugin.json',
```

