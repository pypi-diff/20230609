# Comparing `tmp/edx-enterprise-data-4.6.4.tar.gz` & `tmp/edx-enterprise-data-4.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edx-enterprise-data-4.6.4.tar", last modified: Wed Oct 26 09:26:05 2022, max compression
+gzip compressed data, was "edx-enterprise-data-4.6.5.tar", last modified: Fri Jun  9 14:49:18 2023, max compression
```

## Comparing `edx-enterprise-data-4.6.4.tar` & `edx-enterprise-data-4.6.5.tar`

### file list

```diff
@@ -1,172 +1,172 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-26 09:26:05.619389 edx-enterprise-data-4.6.4/
--rw-r--r--   0 runner    (1001) docker     (121)    16243 2022-10-26 09:26:01.000000 edx-enterprise-data-4.6.4/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (121)    34520 2022-10-26 09:26:01.000000 edx-enterprise-data-4.6.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      485 2022-10-26 09:26:01.000000 edx-enterprise-data-4.6.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)      528 2022-10-26 09:26:05.619389 edx-enterprise-data-4.6.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3975 2022-10-26 09:26:01.000000 edx-enterprise-data-4.6.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-26 09:26:05.603389 edx-enterprise-data-4.6.4/edx_enterprise_data.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      528 2022-10-26 09:26:05.000000 edx-enterprise-data-4.6.4/edx_enterprise_data.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     6668 2022-10-26 09:26:05.000000 edx-enterprise-data-4.6.4/edx_enterprise_data.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-26 09:26:05.000000 edx-enterprise-data-4.6.4/edx_enterprise_data.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-26 09:26:05.000000 edx-enterprise-data-4.6.4/edx_enterprise_data.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)      314 2022-10-26 09:26:05.000000 edx-enterprise-data-4.6.4/edx_enterprise_data.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       59 2022-10-26 09:26:05.000000 edx-enterprise-data-4.6.4/edx_enterprise_data.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-26 09:26:05.607389 edx-enterprise-data-4.6.4/enterprise_data/
--rw-r--r--   0 runner    (1001) docker     (121)      224 2022-10-26 09:26:01.000000 edx-enterprise-data-4.6.4/enterprise_data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-26 09:26:05.607389 edx-enterprise-data-4.6.4/enterprise_data/api/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-26 09:26:01.000000 edx-enterprise-data-4.6.4/enterprise_data/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      273 2022-10-26 09:26:01.000000 edx-enterprise-data-4.6.4/enterprise_data/api/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-26 09:26:05.607389 edx-enterprise-data-4.6.4/enterprise_data/api/v0/
--rw-r--r--   0 runner    (1001) docker     (121)      144 2022-10-26 09:26:01.000000 edx-enterprise-data-4.6.4/enterprise_data/api/v0/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3085 2022-10-26 09:26:01.000000 edx-enterprise-data-4.6.4/enterprise_data/api/v0/serializers.py
--rw-r--r--   0 runner    (1001) docker     (121)      699 2022-10-26 09:26:01.000000 edx-enterprise-data-4.6.4/enterprise_data/api/v0/urls.py
--rw-r--r--   0 runner    (1001) docker     (121)    14380 2022-10-26 09:26:01.000000 edx-enterprise-data-4.6.4/enterprise_data/api/v0/views.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-26 09:26:05.607389 edx-enterprise-data-4.6.4/enterprise_data/api/v1/
--rw-r--r--   0 runner    (1001) docker     (121)      144 2022-10-26 09:26:01.000000 edx-enterprise-data-4.6.4/enterprise_data/api/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3773 2022-10-26 09:26:01.000000 edx-enterprise-data-4.6.4/enterprise_data/api/v1/serializers.py
--rw-r--r--   0 runner    (1001) docker     (121)      826 2022-10-26 09:26:01.000000 edx-enterprise-data-4.6.4/enterprise_data/api/v1/urls.py
--rw-r--r--   0 runner    (1001) docker     (121)    17282 2022-10-26 09:26:01.000000 edx-enterprise-data-4.6.4/enterprise_data/api/v1/views.py
--rw-r--r--   0 runner    (1001) docker     (121)      241 2022-10-26 09:26:01.000000 edx-enterprise-data-4.6.4/enterprise_data/apps.py
--rw-r--r--   0 runner    (1001) docker     (121)     3947 2022-10-26 09:26:01.000000 edx-enterprise-data-4.6.4/enterprise_data/clients.py
--rw-r--r--   0 runner    (1001) docker     (121)      149 2022-10-26 09:26:01.000000 edx-enterprise-data-4.6.4/enterprise_data/constants.py
--rw-r--r--   0 runner    (1001) docker     (121)     5686 2022-10-26 09:26:01.000000 edx-enterprise-data-4.6.4/enterprise_data/filters.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-26 09:26:05.607389 edx-enterprise-data-4.6.4/enterprise_data/fixtures/
--rw-r--r--   0 runner    (1001) docker     (121)     5786 2022-10-26 09:26:01.000000 edx-enterprise-data-4.6.4/enterprise_data/fixtures/enterprise_enrollment.json
--rw-r--r--   0 runner    (1001) docker     (121)     1970 2022-10-26 09:26:01.000000 edx-enterprise-data-4.6.4/enterprise_data/fixtures/enterprise_user.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-26 09:26:05.607389 edx-enterprise-data-4.6.4/enterprise_data/management/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-26 09:26:01.000000 edx-enterprise-data-4.6.4/enterprise_data/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-26 09:26:05.607389 edx-enterprise-data-4.6.4/enterprise_data/management/commands/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-26 09:26:01.000000 edx-enterprise-data-4.6.4/enterprise_data/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1267 2022-10-26 09:26:01.000000 edx-enterprise-data-4.6.4/enterprise_data/management/commands/create_dummy_data.py
--rw-r--r--   0 runner    (1001) docker     (121)     1600 2022-10-26 09:26:01.000000 edx-enterprise-data-4.6.4/enterprise_data/management/commands/create_dummy_data_lpr_v1.py
--rw-r--r--   0 runner    (1001) docker     (121)     1576 2022-10-26 09:26:01.000000 edx-enterprise-data-4.6.4/enterprise_data/management/commands/create_enterprise_enrollment.py
--rw-r--r--   0 runner    (1001) docker     (121)     2087 2022-10-26 09:26:01.000000 edx-enterprise-data-4.6.4/enterprise_data/management/commands/create_enterprise_learner_enrollment_lpr_v1.py
--rw-r--r--   0 runner    (1001) docker     (121)     1799 2022-10-26 09:26:01.000000 edx-enterprise-data-4.6.4/enterprise_data/management/commands/create_enterprise_learner_lpr_v1.py
--rw-r--r--   0 runner    (1001) docker     (121)     1150 2022-10-26 09:26:01.000000 edx-enterprise-data-4.6.4/enterprise_data/management/commands/create_enterprise_offer.py
--rw-r--r--   0 runner    (1001) docker     (121)     1498 2022-10-26 09:26:01.000000 edx-enterprise-data-4.6.4/enterprise_data/management/commands/create_enterprise_user.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-26 09:26:05.607389 edx-enterprise-data-4.6.4/enterprise_data/management/commands/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-26 09:26:01.000000 edx-enterprise-data-4.6.4/enterprise_data/management/commands/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1086 2022-10-26 09:26:01.000000 edx-enterprise-data-4.6.4/enterprise_data/management/commands/tests/test_create_dummy_data_lpr_v1.py
--rw-r--r--   0 runner    (1001) docker     (121)     1742 2022-10-26 09:26:01.000000 edx-enterprise-data-4.6.4/enterprise_data/management/commands/tests/test_create_enterprise_enrollment.py
--rw-r--r--   0 runner    (1001) docker     (121)     3845 2022-10-26 09:26:01.000000 edx-enterprise-data-4.6.4/enterprise_data/management/commands/tests/test_create_enterprise_learner_enrollment_lpr_v1.py
--rw-r--r--   0 runner    (1001) docker     (121)     1637 2022-10-26 09:26:01.000000 edx-enterprise-data-4.6.4/enterprise_data/management/commands/tests/test_create_enterprise_learner_lpr_v1.py
--rw-r--r--   0 runner    (1001) docker     (121)     1469 2022-10-26 09:26:01.000000 edx-enterprise-data-4.6.4/enterprise_data/management/commands/tests/test_create_enterprise_user.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-26 09:26:05.611389 edx-enterprise-data-4.6.4/enterprise_data/migrations/
--rw-r--r--   0 runner    (1001) docker     (121)     2358 2022-10-26 09:26:01.000000 edx-enterprise-data-4.6.4/enterprise_data/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (121)      600 2022-10-26 09:26:01.000000 edx-enterprise-data-4.6.4/enterprise_data/migrations/0002_auto_20180430_1358.py
--rw-r--r--   0 runner    (1001) docker     (121)      415 2022-10-26 09:26:01.000000 edx-enterprise-data-4.6.4/enterprise_data/migrations/0003_auto_20180501_0603.py
--rw-r--r--   0 runner    (1001) docker     (121)      432 2022-10-26 09:26:01.000000 edx-enterprise-data-4.6.4/enterprise_data/migrations/0004_auto_20180501_0928.py
--rw-r--r--   0 runner    (1001) docker     (121)      424 2022-10-26 09:26:01.000000 edx-enterprise-data-4.6.4/enterprise_data/migrations/0004_auto_20180508_1652.py
--rw-r--r--   0 runner    (1001) docker     (121)      404 2022-10-26 09:26:01.000000 edx-enterprise-data-4.6.4/enterprise_data/migrations/0005_auto_20180524_2204.py
--rw-r--r--   0 runner    (1001) docker     (121)      611 2022-10-26 09:26:01.000000 edx-enterprise-data-4.6.4/enterprise_data/migrations/0006_auto_20180612_0336.py
--rw-r--r--   0 runner    (1001) docker     (121)      550 2022-10-26 09:26:01.000000 edx-enterprise-data-4.6.4/enterprise_data/migrations/0007_auto_20180612_0534.py
--rw-r--r--   0 runner    (1001) docker     (121)     1182 2022-10-26 09:26:01.000000 edx-enterprise-data-4.6.4/enterprise_data/migrations/0008_auto_20180614_0108.py
--rw-r--r--   0 runner    (1001) docker     (121)      583 2022-10-26 09:26:01.000000 edx-enterprise-data-4.6.4/enterprise_data/migrations/0009_auto_20180628_1152.py
--rw-r--r--   0 runner    (1001) docker     (121)      409 2022-10-26 09:26:01.000000 edx-enterprise-data-4.6.4/enterprise_data/migrations/0010_enterpriseenrollment_created.py
--rw-r--r--   0 runner    (1001) docker     (121)     1357 2022-10-26 09:26:01.000000 edx-enterprise-data-4.6.4/enterprise_data/migrations/0011_enterpriseuser.py
--rw-r--r--   0 runner    (1001) docker     (121)      761 2022-10-26 09:26:01.000000 edx-enterprise-data-4.6.4/enterprise_data/migrations/0012_auto_20180831_1930.py
--rw-r--r--   0 runner    (1001) docker     (121)      409 2022-10-26 09:26:01.000000 edx-enterprise-data-4.6.4/enterprise_data/migrations/0013_auto_20180831_1931.py
--rw-r--r--   0 runner    (1001) docker     (121)      404 2022-10-26 09:26:01.000000 edx-enterprise-data-4.6.4/enterprise_data/migrations/0014_enterpriseuser_created.py
--rw-r--r--   0 runner    (1001) docker     (121)      453 2022-10-26 09:26:01.000000 edx-enterprise-data-4.6.4/enterprise_data/migrations/0015_auto_20180907_1757.py
--rw-r--r--   0 runner    (1001) docker     (121)      426 2022-10-26 09:26:01.000000 edx-enterprise-data-4.6.4/enterprise_data/migrations/0016_auto_20180924_2138.py
--rw-r--r--   0 runner    (1001) docker     (121)      425 2022-10-26 09:26:01.000000 edx-enterprise-data-4.6.4/enterprise_data/migrations/0017_enterpriseenrollment_unenrollment_timestamp.py
--rw-r--r--   0 runner    (1001) docker     (121)     2082 2022-10-26 09:26:01.000000 edx-enterprise-data-4.6.4/enterprise_data/migrations/0018_enterprisedatafeaturerole_enterprisedataroleassignment.py
--rw-r--r--   0 runner    (1001) docker     (121)      913 2022-10-26 09:26:01.000000 edx-enterprise-data-4.6.4/enterprise_data/migrations/0019_add_enterprise_data_feature_roles.py
--rw-r--r--   0 runner    (1001) docker     (121)      872 2022-10-26 09:26:01.000000 edx-enterprise-data-4.6.4/enterprise_data/migrations/0020_add_role_based_access_control_switch.py
--rw-r--r--   0 runner    (1001) docker     (121)      681 2022-10-26 09:26:01.000000 edx-enterprise-data-4.6.4/enterprise_data/migrations/0021_auto_20190329_1241.py
--rw-r--r--   0 runner    (1001) docker     (121)      857 2022-10-26 09:26:01.000000 edx-enterprise-data-4.6.4/enterprise_data/migrations/0022_remove_role_based_access_control_switch.py
--rw-r--r--   0 runner    (1001) docker     (121)     5749 2022-10-26 09:26:01.000000 edx-enterprise-data-4.6.4/enterprise_data/migrations/0023_enterpriselearner_enterpriselearnerenrollment.py
--rw-r--r--   0 runner    (1001) docker     (121)      635 2022-10-26 09:26:01.000000 edx-enterprise-data-4.6.4/enterprise_data/migrations/0024_auto_20210602_1811.py
--rw-r--r--   0 runner    (1001) docker     (121)      455 2022-10-26 09:26:01.000000 edx-enterprise-data-4.6.4/enterprise_data/migrations/0025_auto_20210703_1854.py
--rw-r--r--   0 runner    (1001) docker     (121)     2380 2022-10-26 09:26:01.000000 edx-enterprise-data-4.6.4/enterprise_data/migrations/0026_auto_20210916_0414.py
--rw-r--r--   0 runner    (1001) docker     (121)      442 2022-10-26 09:26:01.000000 edx-enterprise-data-4.6.4/enterprise_data/migrations/0027_enterpriselearnerenrollment_total_learning_time_seconds.py
--rw-r--r--   0 runner    (1001) docker     (121)      460 2022-10-26 09:26:01.000000 edx-enterprise-data-4.6.4/enterprise_data/migrations/0028_enterpriselearnerenrollment_offer_id.py
--rw-r--r--   0 runner    (1001) docker     (121)     1776 2022-10-26 09:26:01.000000 edx-enterprise-data-4.6.4/enterprise_data/migrations/0029_enterpriseoffer.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-26 09:26:01.000000 edx-enterprise-data-4.6.4/enterprise_data/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    12029 2022-10-26 09:26:01.000000 edx-enterprise-data-4.6.4/enterprise_data/models.py
--rw-r--r--   0 runner    (1001) docker     (121)      269 2022-10-26 09:26:01.000000 edx-enterprise-data-4.6.4/enterprise_data/paginators.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-26 09:26:05.611389 edx-enterprise-data-4.6.4/enterprise_data/settings/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-26 09:26:01.000000 edx-enterprise-data-4.6.4/enterprise_data/settings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3988 2022-10-26 09:26:01.000000 edx-enterprise-data-4.6.4/enterprise_data/settings/test.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-26 09:26:05.611389 edx-enterprise-data-4.6.4/enterprise_data/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-26 09:26:01.000000 edx-enterprise-data-4.6.4/enterprise_data/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-26 09:26:05.611389 edx-enterprise-data-4.6.4/enterprise_data/tests/api/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-26 09:26:01.000000 edx-enterprise-data-4.6.4/enterprise_data/tests/api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-26 09:26:05.611389 edx-enterprise-data-4.6.4/enterprise_data/tests/api/v0/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-26 09:26:01.000000 edx-enterprise-data-4.6.4/enterprise_data/tests/api/v0/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6257 2022-10-26 09:26:01.000000 edx-enterprise-data-4.6.4/enterprise_data/tests/api/v0/test_serializers.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-26 09:26:05.611389 edx-enterprise-data-4.6.4/enterprise_data/tests/api/v1/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-26 09:26:01.000000 edx-enterprise-data-4.6.4/enterprise_data/tests/api/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1267 2022-10-26 09:26:01.000000 edx-enterprise-data-4.6.4/enterprise_data/tests/api/v1/test_serializers.py
--rw-r--r--   0 runner    (1001) docker     (121)     5715 2022-10-26 09:26:01.000000 edx-enterprise-data-4.6.4/enterprise_data/tests/api/v1/test_views.py
--rw-r--r--   0 runner    (1001) docker     (121)      805 2022-10-26 09:26:01.000000 edx-enterprise-data-4.6.4/enterprise_data/tests/mixins.py
--rw-r--r--   0 runner    (1001) docker     (121)     6336 2022-10-26 09:26:01.000000 edx-enterprise-data-4.6.4/enterprise_data/tests/test_clients.py
--rw-r--r--   0 runner    (1001) docker     (121)     7244 2022-10-26 09:26:01.000000 edx-enterprise-data-4.6.4/enterprise_data/tests/test_filters.py
--rw-r--r--   0 runner    (1001) docker     (121)     2292 2022-10-26 09:26:01.000000 edx-enterprise-data-4.6.4/enterprise_data/tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (121)    11811 2022-10-26 09:26:01.000000 edx-enterprise-data-4.6.4/enterprise_data/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)    69667 2022-10-26 09:26:01.000000 edx-enterprise-data-4.6.4/enterprise_data/tests/test_views.py
--rw-r--r--   0 runner    (1001) docker     (121)      243 2022-10-26 09:26:01.000000 edx-enterprise-data-4.6.4/enterprise_data/urls.py
--rw-r--r--   0 runner    (1001) docker     (121)      830 2022-10-26 09:26:01.000000 edx-enterprise-data-4.6.4/enterprise_data/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-26 09:26:05.611389 edx-enterprise-data-4.6.4/enterprise_data_roles/
--rw-r--r--   0 runner    (1001) docker     (121)      112 2022-10-26 09:26:01.000000 edx-enterprise-data-4.6.4/enterprise_data_roles/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      998 2022-10-26 09:26:01.000000 edx-enterprise-data-4.6.4/enterprise_data_roles/admin.py
--rw-r--r--   0 runner    (1001) docker     (121)      260 2022-10-26 09:26:01.000000 edx-enterprise-data-4.6.4/enterprise_data_roles/apps.py
--rw-r--r--   0 runner    (1001) docker     (121)      476 2022-10-26 09:26:01.000000 edx-enterprise-data-4.6.4/enterprise_data_roles/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-26 09:26:05.615389 edx-enterprise-data-4.6.4/enterprise_data_roles/migrations/
--rw-r--r--   0 runner    (1001) docker     (121)     2083 2022-10-26 09:26:01.000000 edx-enterprise-data-4.6.4/enterprise_data_roles/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (121)      947 2022-10-26 09:26:01.000000 edx-enterprise-data-4.6.4/enterprise_data_roles/migrations/0002_add_enterprise_data_feature_roles.py
--rw-r--r--   0 runner    (1001) docker     (121)      955 2022-10-26 09:26:01.000000 edx-enterprise-data-4.6.4/enterprise_data_roles/migrations/0003_add_role_based_access_control_switch.py
--rw-r--r--   0 runner    (1001) docker     (121)      497 2022-10-26 09:26:01.000000 edx-enterprise-data-4.6.4/enterprise_data_roles/migrations/0004_enterprisedataroleassignment_enterprise_id.py
--rw-r--r--   0 runner    (1001) docker     (121)      864 2022-10-26 09:26:01.000000 edx-enterprise-data-4.6.4/enterprise_data_roles/migrations/0005_turn_on_role_based_access_control_switch.py
--rw-r--r--   0 runner    (1001) docker     (121)      836 2022-10-26 09:26:01.000000 edx-enterprise-data-4.6.4/enterprise_data_roles/migrations/0006_remove_role_based_access_control_switch.py
--rw-r--r--   0 runner    (1001) docker     (121)      588 2022-10-26 09:26:01.000000 edx-enterprise-data-4.6.4/enterprise_data_roles/migrations/0007_enterprisedataroleassignment_applies_to_all_contexts.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-26 09:26:01.000000 edx-enterprise-data-4.6.4/enterprise_data_roles/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1679 2022-10-26 09:26:01.000000 edx-enterprise-data-4.6.4/enterprise_data_roles/models.py
--rw-r--r--   0 runner    (1001) docker     (121)     1948 2022-10-26 09:26:01.000000 edx-enterprise-data-4.6.4/enterprise_data_roles/rules.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-26 09:26:05.615389 edx-enterprise-data-4.6.4/enterprise_data_roles/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-26 09:26:01.000000 edx-enterprise-data-4.6.4/enterprise_data_roles/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1153 2022-10-26 09:26:01.000000 edx-enterprise-data-4.6.4/enterprise_data_roles/tests/factories.py
--rw-r--r--   0 runner    (1001) docker     (121)     1476 2022-10-26 09:26:01.000000 edx-enterprise-data-4.6.4/enterprise_data_roles/tests/test_models.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-26 09:26:05.615389 edx-enterprise-data-4.6.4/enterprise_reporting/
--rw-r--r--   0 runner    (1001) docker     (121)      112 2022-10-26 09:26:01.000000 edx-enterprise-data-4.6.4/enterprise_reporting/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-26 09:26:05.615389 edx-enterprise-data-4.6.4/enterprise_reporting/clients/
--rw-r--r--   0 runner    (1001) docker     (121)     4651 2022-10-26 09:26:01.000000 edx-enterprise-data-4.6.4/enterprise_reporting/clients/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    11180 2022-10-26 09:26:01.000000 edx-enterprise-data-4.6.4/enterprise_reporting/clients/enterprise.py
--rw-r--r--   0 runner    (1001) docker     (121)      559 2022-10-26 09:26:01.000000 edx-enterprise-data-4.6.4/enterprise_reporting/clients/s3.py
--rw-r--r--   0 runner    (1001) docker     (121)     1792 2022-10-26 09:26:01.000000 edx-enterprise-data-4.6.4/enterprise_reporting/clients/snowflake.py
--rw-r--r--   0 runner    (1001) docker     (121)     1900 2022-10-26 09:26:01.000000 edx-enterprise-data-4.6.4/enterprise_reporting/clients/vertica.py
--rw-r--r--   0 runner    (1001) docker     (121)     4813 2022-10-26 09:26:01.000000 edx-enterprise-data-4.6.4/enterprise_reporting/delivery_method.py
--rw-r--r--   0 runner    (1001) docker     (121)     8066 2022-10-26 09:26:01.000000 edx-enterprise-data-4.6.4/enterprise_reporting/external_resource_link_report.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-26 09:26:05.615389 edx-enterprise-data-4.6.4/enterprise_reporting/fixtures/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-26 09:26:01.000000 edx-enterprise-data-4.6.4/enterprise_reporting/fixtures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3959 2022-10-26 09:26:01.000000 edx-enterprise-data-4.6.4/enterprise_reporting/fixtures/enterprise_customer_reporting.json
--rw-r--r--   0 runner    (1001) docker     (121)    13441 2022-10-26 09:26:01.000000 edx-enterprise-data-4.6.4/enterprise_reporting/reporter.py
--rw-r--r--   0 runner    (1001) docker     (121)     4753 2022-10-26 09:26:01.000000 edx-enterprise-data-4.6.4/enterprise_reporting/send_enterprise_reports.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-26 09:26:05.615389 edx-enterprise-data-4.6.4/enterprise_reporting/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-26 09:26:01.000000 edx-enterprise-data-4.6.4/enterprise_reporting/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4808 2022-10-26 09:26:01.000000 edx-enterprise-data-4.6.4/enterprise_reporting/tests/test_clients.py
--rw-r--r--   0 runner    (1001) docker     (121)     2598 2022-10-26 09:26:01.000000 edx-enterprise-data-4.6.4/enterprise_reporting/tests/test_delivery_method.py
--rw-r--r--   0 runner    (1001) docker     (121)     1068 2022-10-26 09:26:01.000000 edx-enterprise-data-4.6.4/enterprise_reporting/tests/test_enterprise_client.py
--rw-r--r--   0 runner    (1001) docker     (121)     7029 2022-10-26 09:26:01.000000 edx-enterprise-data-4.6.4/enterprise_reporting/tests/test_external_link_report.py
--rw-r--r--   0 runner    (1001) docker     (121)     1897 2022-10-26 09:26:01.000000 edx-enterprise-data-4.6.4/enterprise_reporting/tests/test_reporter.py
--rw-r--r--   0 runner    (1001) docker     (121)     1034 2022-10-26 09:26:01.000000 edx-enterprise-data-4.6.4/enterprise_reporting/tests/test_send_enterprise_reports.py
--rw-r--r--   0 runner    (1001) docker     (121)     8871 2022-10-26 09:26:01.000000 edx-enterprise-data-4.6.4/enterprise_reporting/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)      140 2022-10-26 09:26:01.000000 edx-enterprise-data-4.6.4/enterprise_reporting/tests/test_vertica_client.py
--rw-r--r--   0 runner    (1001) docker     (121)     1401 2022-10-26 09:26:01.000000 edx-enterprise-data-4.6.4/enterprise_reporting/tests/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)    12186 2022-10-26 09:26:01.000000 edx-enterprise-data-4.6.4/enterprise_reporting/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-26 09:26:05.619389 edx-enterprise-data-4.6.4/requirements/
--rw-r--r--   0 runner    (1001) docker     (121)      347 2022-10-26 09:26:01.000000 edx-enterprise-data-4.6.4/requirements/base.in
--rw-r--r--   0 runner    (1001) docker     (121)     5285 2022-10-26 09:26:01.000000 edx-enterprise-data-4.6.4/requirements/base.txt
--rw-r--r--   0 runner    (1001) docker     (121)      879 2022-10-26 09:26:01.000000 edx-enterprise-data-4.6.4/requirements/ci.txt
--rw-r--r--   0 runner    (1001) docker     (121)      731 2022-10-26 09:26:01.000000 edx-enterprise-data-4.6.4/requirements/constraints.txt
--rw-r--r--   0 runner    (1001) docker     (121)     8635 2022-10-26 09:26:01.000000 edx-enterprise-data-4.6.4/requirements/dev.txt
--rw-r--r--   0 runner    (1001) docker     (121)       15 2022-10-26 09:26:01.000000 edx-enterprise-data-4.6.4/requirements/django.txt
--rw-r--r--   0 runner    (1001) docker     (121)      324 2022-10-26 09:26:01.000000 edx-enterprise-data-4.6.4/requirements/pip.txt
--rw-r--r--   0 runner    (1001) docker     (121)      507 2022-10-26 09:26:01.000000 edx-enterprise-data-4.6.4/requirements/pip_tools.txt
--rw-r--r--   0 runner    (1001) docker     (121)     9455 2022-10-26 09:26:01.000000 edx-enterprise-data-4.6.4/requirements/quality.txt
--rw-r--r--   0 runner    (1001) docker     (121)      684 2022-10-26 09:26:01.000000 edx-enterprise-data-4.6.4/requirements/reporting.in
--rw-r--r--   0 runner    (1001) docker     (121)     6273 2022-10-26 09:26:01.000000 edx-enterprise-data-4.6.4/requirements/test-master.txt
--rw-r--r--   0 runner    (1001) docker     (121)     4088 2022-10-26 09:26:01.000000 edx-enterprise-data-4.6.4/requirements/test-reporting.txt
--rw-r--r--   0 runner    (1001) docker     (121)     6171 2022-10-26 09:26:01.000000 edx-enterprise-data-4.6.4/requirements/test.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-10-26 09:26:05.619389 edx-enterprise-data-4.6.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2373 2022-10-26 09:26:01.000000 edx-enterprise-data-4.6.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 14:49:18.543490 edx-enterprise-data-4.6.5/
+-rw-r--r--   0 runner    (1001) docker     (122)    16348 2023-06-09 14:49:14.000000 edx-enterprise-data-4.6.5/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (122)    34520 2023-06-09 14:49:14.000000 edx-enterprise-data-4.6.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      522 2023-06-09 14:49:14.000000 edx-enterprise-data-4.6.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)      532 2023-06-09 14:49:18.543490 edx-enterprise-data-4.6.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     4003 2023-06-09 14:49:14.000000 edx-enterprise-data-4.6.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 14:49:18.523490 edx-enterprise-data-4.6.5/edx_enterprise_data.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)      532 2023-06-09 14:49:18.000000 edx-enterprise-data-4.6.5/edx_enterprise_data.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     6668 2023-06-09 14:49:18.000000 edx-enterprise-data-4.6.5/edx_enterprise_data.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-09 14:49:18.000000 edx-enterprise-data-4.6.5/edx_enterprise_data.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-09 14:49:18.000000 edx-enterprise-data-4.6.5/edx_enterprise_data.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)      324 2023-06-09 14:49:18.000000 edx-enterprise-data-4.6.5/edx_enterprise_data.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       59 2023-06-09 14:49:18.000000 edx-enterprise-data-4.6.5/edx_enterprise_data.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 14:49:18.527490 edx-enterprise-data-4.6.5/enterprise_data/
+-rw-r--r--   0 runner    (1001) docker     (122)      224 2023-06-09 14:49:14.000000 edx-enterprise-data-4.6.5/enterprise_data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 14:49:18.527490 edx-enterprise-data-4.6.5/enterprise_data/api/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-09 14:49:14.000000 edx-enterprise-data-4.6.5/enterprise_data/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      273 2023-06-09 14:49:14.000000 edx-enterprise-data-4.6.5/enterprise_data/api/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 14:49:18.527490 edx-enterprise-data-4.6.5/enterprise_data/api/v0/
+-rw-r--r--   0 runner    (1001) docker     (122)      144 2023-06-09 14:49:14.000000 edx-enterprise-data-4.6.5/enterprise_data/api/v0/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3085 2023-06-09 14:49:14.000000 edx-enterprise-data-4.6.5/enterprise_data/api/v0/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (122)      699 2023-06-09 14:49:14.000000 edx-enterprise-data-4.6.5/enterprise_data/api/v0/urls.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14380 2023-06-09 14:49:14.000000 edx-enterprise-data-4.6.5/enterprise_data/api/v0/views.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 14:49:18.527490 edx-enterprise-data-4.6.5/enterprise_data/api/v1/
+-rw-r--r--   0 runner    (1001) docker     (122)      144 2023-06-09 14:49:14.000000 edx-enterprise-data-4.6.5/enterprise_data/api/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3773 2023-06-09 14:49:14.000000 edx-enterprise-data-4.6.5/enterprise_data/api/v1/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (122)      826 2023-06-09 14:49:14.000000 edx-enterprise-data-4.6.5/enterprise_data/api/v1/urls.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17282 2023-06-09 14:49:14.000000 edx-enterprise-data-4.6.5/enterprise_data/api/v1/views.py
+-rw-r--r--   0 runner    (1001) docker     (122)      241 2023-06-09 14:49:14.000000 edx-enterprise-data-4.6.5/enterprise_data/apps.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3947 2023-06-09 14:49:14.000000 edx-enterprise-data-4.6.5/enterprise_data/clients.py
+-rw-r--r--   0 runner    (1001) docker     (122)      149 2023-06-09 14:49:14.000000 edx-enterprise-data-4.6.5/enterprise_data/constants.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5686 2023-06-09 14:49:14.000000 edx-enterprise-data-4.6.5/enterprise_data/filters.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 14:49:18.527490 edx-enterprise-data-4.6.5/enterprise_data/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (122)     5786 2023-06-09 14:49:14.000000 edx-enterprise-data-4.6.5/enterprise_data/fixtures/enterprise_enrollment.json
+-rw-r--r--   0 runner    (1001) docker     (122)     1970 2023-06-09 14:49:14.000000 edx-enterprise-data-4.6.5/enterprise_data/fixtures/enterprise_user.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 14:49:18.527490 edx-enterprise-data-4.6.5/enterprise_data/management/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-09 14:49:14.000000 edx-enterprise-data-4.6.5/enterprise_data/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 14:49:18.527490 edx-enterprise-data-4.6.5/enterprise_data/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-09 14:49:14.000000 edx-enterprise-data-4.6.5/enterprise_data/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1267 2023-06-09 14:49:14.000000 edx-enterprise-data-4.6.5/enterprise_data/management/commands/create_dummy_data.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1600 2023-06-09 14:49:14.000000 edx-enterprise-data-4.6.5/enterprise_data/management/commands/create_dummy_data_lpr_v1.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1576 2023-06-09 14:49:14.000000 edx-enterprise-data-4.6.5/enterprise_data/management/commands/create_enterprise_enrollment.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2087 2023-06-09 14:49:14.000000 edx-enterprise-data-4.6.5/enterprise_data/management/commands/create_enterprise_learner_enrollment_lpr_v1.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1799 2023-06-09 14:49:14.000000 edx-enterprise-data-4.6.5/enterprise_data/management/commands/create_enterprise_learner_lpr_v1.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1150 2023-06-09 14:49:14.000000 edx-enterprise-data-4.6.5/enterprise_data/management/commands/create_enterprise_offer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1498 2023-06-09 14:49:14.000000 edx-enterprise-data-4.6.5/enterprise_data/management/commands/create_enterprise_user.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 14:49:18.531490 edx-enterprise-data-4.6.5/enterprise_data/management/commands/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-09 14:49:14.000000 edx-enterprise-data-4.6.5/enterprise_data/management/commands/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1086 2023-06-09 14:49:14.000000 edx-enterprise-data-4.6.5/enterprise_data/management/commands/tests/test_create_dummy_data_lpr_v1.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1742 2023-06-09 14:49:14.000000 edx-enterprise-data-4.6.5/enterprise_data/management/commands/tests/test_create_enterprise_enrollment.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3845 2023-06-09 14:49:14.000000 edx-enterprise-data-4.6.5/enterprise_data/management/commands/tests/test_create_enterprise_learner_enrollment_lpr_v1.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1637 2023-06-09 14:49:14.000000 edx-enterprise-data-4.6.5/enterprise_data/management/commands/tests/test_create_enterprise_learner_lpr_v1.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1469 2023-06-09 14:49:14.000000 edx-enterprise-data-4.6.5/enterprise_data/management/commands/tests/test_create_enterprise_user.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 14:49:18.535490 edx-enterprise-data-4.6.5/enterprise_data/migrations/
+-rw-r--r--   0 runner    (1001) docker     (122)     2358 2023-06-09 14:49:14.000000 edx-enterprise-data-4.6.5/enterprise_data/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (122)      600 2023-06-09 14:49:14.000000 edx-enterprise-data-4.6.5/enterprise_data/migrations/0002_auto_20180430_1358.py
+-rw-r--r--   0 runner    (1001) docker     (122)      415 2023-06-09 14:49:14.000000 edx-enterprise-data-4.6.5/enterprise_data/migrations/0003_auto_20180501_0603.py
+-rw-r--r--   0 runner    (1001) docker     (122)      432 2023-06-09 14:49:14.000000 edx-enterprise-data-4.6.5/enterprise_data/migrations/0004_auto_20180501_0928.py
+-rw-r--r--   0 runner    (1001) docker     (122)      424 2023-06-09 14:49:14.000000 edx-enterprise-data-4.6.5/enterprise_data/migrations/0004_auto_20180508_1652.py
+-rw-r--r--   0 runner    (1001) docker     (122)      404 2023-06-09 14:49:14.000000 edx-enterprise-data-4.6.5/enterprise_data/migrations/0005_auto_20180524_2204.py
+-rw-r--r--   0 runner    (1001) docker     (122)      611 2023-06-09 14:49:14.000000 edx-enterprise-data-4.6.5/enterprise_data/migrations/0006_auto_20180612_0336.py
+-rw-r--r--   0 runner    (1001) docker     (122)      550 2023-06-09 14:49:14.000000 edx-enterprise-data-4.6.5/enterprise_data/migrations/0007_auto_20180612_0534.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1182 2023-06-09 14:49:14.000000 edx-enterprise-data-4.6.5/enterprise_data/migrations/0008_auto_20180614_0108.py
+-rw-r--r--   0 runner    (1001) docker     (122)      583 2023-06-09 14:49:14.000000 edx-enterprise-data-4.6.5/enterprise_data/migrations/0009_auto_20180628_1152.py
+-rw-r--r--   0 runner    (1001) docker     (122)      409 2023-06-09 14:49:14.000000 edx-enterprise-data-4.6.5/enterprise_data/migrations/0010_enterpriseenrollment_created.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1357 2023-06-09 14:49:14.000000 edx-enterprise-data-4.6.5/enterprise_data/migrations/0011_enterpriseuser.py
+-rw-r--r--   0 runner    (1001) docker     (122)      761 2023-06-09 14:49:14.000000 edx-enterprise-data-4.6.5/enterprise_data/migrations/0012_auto_20180831_1930.py
+-rw-r--r--   0 runner    (1001) docker     (122)      409 2023-06-09 14:49:14.000000 edx-enterprise-data-4.6.5/enterprise_data/migrations/0013_auto_20180831_1931.py
+-rw-r--r--   0 runner    (1001) docker     (122)      404 2023-06-09 14:49:14.000000 edx-enterprise-data-4.6.5/enterprise_data/migrations/0014_enterpriseuser_created.py
+-rw-r--r--   0 runner    (1001) docker     (122)      453 2023-06-09 14:49:14.000000 edx-enterprise-data-4.6.5/enterprise_data/migrations/0015_auto_20180907_1757.py
+-rw-r--r--   0 runner    (1001) docker     (122)      426 2023-06-09 14:49:14.000000 edx-enterprise-data-4.6.5/enterprise_data/migrations/0016_auto_20180924_2138.py
+-rw-r--r--   0 runner    (1001) docker     (122)      425 2023-06-09 14:49:14.000000 edx-enterprise-data-4.6.5/enterprise_data/migrations/0017_enterpriseenrollment_unenrollment_timestamp.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2082 2023-06-09 14:49:14.000000 edx-enterprise-data-4.6.5/enterprise_data/migrations/0018_enterprisedatafeaturerole_enterprisedataroleassignment.py
+-rw-r--r--   0 runner    (1001) docker     (122)      913 2023-06-09 14:49:14.000000 edx-enterprise-data-4.6.5/enterprise_data/migrations/0019_add_enterprise_data_feature_roles.py
+-rw-r--r--   0 runner    (1001) docker     (122)      872 2023-06-09 14:49:14.000000 edx-enterprise-data-4.6.5/enterprise_data/migrations/0020_add_role_based_access_control_switch.py
+-rw-r--r--   0 runner    (1001) docker     (122)      681 2023-06-09 14:49:14.000000 edx-enterprise-data-4.6.5/enterprise_data/migrations/0021_auto_20190329_1241.py
+-rw-r--r--   0 runner    (1001) docker     (122)      857 2023-06-09 14:49:14.000000 edx-enterprise-data-4.6.5/enterprise_data/migrations/0022_remove_role_based_access_control_switch.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5749 2023-06-09 14:49:14.000000 edx-enterprise-data-4.6.5/enterprise_data/migrations/0023_enterpriselearner_enterpriselearnerenrollment.py
+-rw-r--r--   0 runner    (1001) docker     (122)      635 2023-06-09 14:49:14.000000 edx-enterprise-data-4.6.5/enterprise_data/migrations/0024_auto_20210602_1811.py
+-rw-r--r--   0 runner    (1001) docker     (122)      455 2023-06-09 14:49:14.000000 edx-enterprise-data-4.6.5/enterprise_data/migrations/0025_auto_20210703_1854.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2380 2023-06-09 14:49:14.000000 edx-enterprise-data-4.6.5/enterprise_data/migrations/0026_auto_20210916_0414.py
+-rw-r--r--   0 runner    (1001) docker     (122)      442 2023-06-09 14:49:14.000000 edx-enterprise-data-4.6.5/enterprise_data/migrations/0027_enterpriselearnerenrollment_total_learning_time_seconds.py
+-rw-r--r--   0 runner    (1001) docker     (122)      460 2023-06-09 14:49:14.000000 edx-enterprise-data-4.6.5/enterprise_data/migrations/0028_enterpriselearnerenrollment_offer_id.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1776 2023-06-09 14:49:14.000000 edx-enterprise-data-4.6.5/enterprise_data/migrations/0029_enterpriseoffer.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-09 14:49:14.000000 edx-enterprise-data-4.6.5/enterprise_data/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12029 2023-06-09 14:49:14.000000 edx-enterprise-data-4.6.5/enterprise_data/models.py
+-rw-r--r--   0 runner    (1001) docker     (122)      269 2023-06-09 14:49:14.000000 edx-enterprise-data-4.6.5/enterprise_data/paginators.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 14:49:18.535490 edx-enterprise-data-4.6.5/enterprise_data/settings/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-09 14:49:14.000000 edx-enterprise-data-4.6.5/enterprise_data/settings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3988 2023-06-09 14:49:14.000000 edx-enterprise-data-4.6.5/enterprise_data/settings/test.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 14:49:18.535490 edx-enterprise-data-4.6.5/enterprise_data/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-09 14:49:14.000000 edx-enterprise-data-4.6.5/enterprise_data/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 14:49:18.535490 edx-enterprise-data-4.6.5/enterprise_data/tests/api/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-09 14:49:14.000000 edx-enterprise-data-4.6.5/enterprise_data/tests/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 14:49:18.535490 edx-enterprise-data-4.6.5/enterprise_data/tests/api/v0/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-09 14:49:14.000000 edx-enterprise-data-4.6.5/enterprise_data/tests/api/v0/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6257 2023-06-09 14:49:14.000000 edx-enterprise-data-4.6.5/enterprise_data/tests/api/v0/test_serializers.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 14:49:18.535490 edx-enterprise-data-4.6.5/enterprise_data/tests/api/v1/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-09 14:49:14.000000 edx-enterprise-data-4.6.5/enterprise_data/tests/api/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1267 2023-06-09 14:49:14.000000 edx-enterprise-data-4.6.5/enterprise_data/tests/api/v1/test_serializers.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5715 2023-06-09 14:49:14.000000 edx-enterprise-data-4.6.5/enterprise_data/tests/api/v1/test_views.py
+-rw-r--r--   0 runner    (1001) docker     (122)      805 2023-06-09 14:49:14.000000 edx-enterprise-data-4.6.5/enterprise_data/tests/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6336 2023-06-09 14:49:14.000000 edx-enterprise-data-4.6.5/enterprise_data/tests/test_clients.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7244 2023-06-09 14:49:14.000000 edx-enterprise-data-4.6.5/enterprise_data/tests/test_filters.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2292 2023-06-09 14:49:14.000000 edx-enterprise-data-4.6.5/enterprise_data/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11811 2023-06-09 14:49:14.000000 edx-enterprise-data-4.6.5/enterprise_data/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)    69667 2023-06-09 14:49:14.000000 edx-enterprise-data-4.6.5/enterprise_data/tests/test_views.py
+-rw-r--r--   0 runner    (1001) docker     (122)      243 2023-06-09 14:49:14.000000 edx-enterprise-data-4.6.5/enterprise_data/urls.py
+-rw-r--r--   0 runner    (1001) docker     (122)      830 2023-06-09 14:49:14.000000 edx-enterprise-data-4.6.5/enterprise_data/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 14:49:18.535490 edx-enterprise-data-4.6.5/enterprise_data_roles/
+-rw-r--r--   0 runner    (1001) docker     (122)      112 2023-06-09 14:49:14.000000 edx-enterprise-data-4.6.5/enterprise_data_roles/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      998 2023-06-09 14:49:14.000000 edx-enterprise-data-4.6.5/enterprise_data_roles/admin.py
+-rw-r--r--   0 runner    (1001) docker     (122)      260 2023-06-09 14:49:14.000000 edx-enterprise-data-4.6.5/enterprise_data_roles/apps.py
+-rw-r--r--   0 runner    (1001) docker     (122)      476 2023-06-09 14:49:14.000000 edx-enterprise-data-4.6.5/enterprise_data_roles/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 14:49:18.539490 edx-enterprise-data-4.6.5/enterprise_data_roles/migrations/
+-rw-r--r--   0 runner    (1001) docker     (122)     2083 2023-06-09 14:49:14.000000 edx-enterprise-data-4.6.5/enterprise_data_roles/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (122)      947 2023-06-09 14:49:14.000000 edx-enterprise-data-4.6.5/enterprise_data_roles/migrations/0002_add_enterprise_data_feature_roles.py
+-rw-r--r--   0 runner    (1001) docker     (122)      955 2023-06-09 14:49:14.000000 edx-enterprise-data-4.6.5/enterprise_data_roles/migrations/0003_add_role_based_access_control_switch.py
+-rw-r--r--   0 runner    (1001) docker     (122)      497 2023-06-09 14:49:14.000000 edx-enterprise-data-4.6.5/enterprise_data_roles/migrations/0004_enterprisedataroleassignment_enterprise_id.py
+-rw-r--r--   0 runner    (1001) docker     (122)      864 2023-06-09 14:49:14.000000 edx-enterprise-data-4.6.5/enterprise_data_roles/migrations/0005_turn_on_role_based_access_control_switch.py
+-rw-r--r--   0 runner    (1001) docker     (122)      836 2023-06-09 14:49:14.000000 edx-enterprise-data-4.6.5/enterprise_data_roles/migrations/0006_remove_role_based_access_control_switch.py
+-rw-r--r--   0 runner    (1001) docker     (122)      588 2023-06-09 14:49:14.000000 edx-enterprise-data-4.6.5/enterprise_data_roles/migrations/0007_enterprisedataroleassignment_applies_to_all_contexts.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-09 14:49:14.000000 edx-enterprise-data-4.6.5/enterprise_data_roles/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1679 2023-06-09 14:49:14.000000 edx-enterprise-data-4.6.5/enterprise_data_roles/models.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1948 2023-06-09 14:49:14.000000 edx-enterprise-data-4.6.5/enterprise_data_roles/rules.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 14:49:18.539490 edx-enterprise-data-4.6.5/enterprise_data_roles/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-09 14:49:14.000000 edx-enterprise-data-4.6.5/enterprise_data_roles/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1153 2023-06-09 14:49:14.000000 edx-enterprise-data-4.6.5/enterprise_data_roles/tests/factories.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1476 2023-06-09 14:49:14.000000 edx-enterprise-data-4.6.5/enterprise_data_roles/tests/test_models.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 14:49:18.539490 edx-enterprise-data-4.6.5/enterprise_reporting/
+-rw-r--r--   0 runner    (1001) docker     (122)      112 2023-06-09 14:49:14.000000 edx-enterprise-data-4.6.5/enterprise_reporting/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 14:49:18.539490 edx-enterprise-data-4.6.5/enterprise_reporting/clients/
+-rw-r--r--   0 runner    (1001) docker     (122)     4950 2023-06-09 14:49:14.000000 edx-enterprise-data-4.6.5/enterprise_reporting/clients/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9853 2023-06-09 14:49:14.000000 edx-enterprise-data-4.6.5/enterprise_reporting/clients/enterprise.py
+-rw-r--r--   0 runner    (1001) docker     (122)      559 2023-06-09 14:49:14.000000 edx-enterprise-data-4.6.5/enterprise_reporting/clients/s3.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1792 2023-06-09 14:49:14.000000 edx-enterprise-data-4.6.5/enterprise_reporting/clients/snowflake.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1900 2023-06-09 14:49:14.000000 edx-enterprise-data-4.6.5/enterprise_reporting/clients/vertica.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4813 2023-06-09 14:49:14.000000 edx-enterprise-data-4.6.5/enterprise_reporting/delivery_method.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8066 2023-06-09 14:49:14.000000 edx-enterprise-data-4.6.5/enterprise_reporting/external_resource_link_report.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 14:49:18.539490 edx-enterprise-data-4.6.5/enterprise_reporting/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-09 14:49:14.000000 edx-enterprise-data-4.6.5/enterprise_reporting/fixtures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3959 2023-06-09 14:49:14.000000 edx-enterprise-data-4.6.5/enterprise_reporting/fixtures/enterprise_customer_reporting.json
+-rw-r--r--   0 runner    (1001) docker     (122)    13707 2023-06-09 14:49:14.000000 edx-enterprise-data-4.6.5/enterprise_reporting/reporter.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4753 2023-06-09 14:49:14.000000 edx-enterprise-data-4.6.5/enterprise_reporting/send_enterprise_reports.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 14:49:18.543490 edx-enterprise-data-4.6.5/enterprise_reporting/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-09 14:49:14.000000 edx-enterprise-data-4.6.5/enterprise_reporting/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8474 2023-06-09 14:49:14.000000 edx-enterprise-data-4.6.5/enterprise_reporting/tests/test_clients.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2598 2023-06-09 14:49:14.000000 edx-enterprise-data-4.6.5/enterprise_reporting/tests/test_delivery_method.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1068 2023-06-09 14:49:14.000000 edx-enterprise-data-4.6.5/enterprise_reporting/tests/test_enterprise_client.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7029 2023-06-09 14:49:14.000000 edx-enterprise-data-4.6.5/enterprise_reporting/tests/test_external_link_report.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4057 2023-06-09 14:49:14.000000 edx-enterprise-data-4.6.5/enterprise_reporting/tests/test_reporter.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1034 2023-06-09 14:49:14.000000 edx-enterprise-data-4.6.5/enterprise_reporting/tests/test_send_enterprise_reports.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8871 2023-06-09 14:49:14.000000 edx-enterprise-data-4.6.5/enterprise_reporting/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)      140 2023-06-09 14:49:14.000000 edx-enterprise-data-4.6.5/enterprise_reporting/tests/test_vertica_client.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1401 2023-06-09 14:49:14.000000 edx-enterprise-data-4.6.5/enterprise_reporting/tests/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12186 2023-06-09 14:49:14.000000 edx-enterprise-data-4.6.5/enterprise_reporting/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 14:49:18.543490 edx-enterprise-data-4.6.5/requirements/
+-rw-r--r--   0 runner    (1001) docker     (122)      347 2023-06-09 14:49:14.000000 edx-enterprise-data-4.6.5/requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (122)     5173 2023-06-09 14:49:14.000000 edx-enterprise-data-4.6.5/requirements/base.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      676 2023-06-09 14:49:14.000000 edx-enterprise-data-4.6.5/requirements/ci.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      742 2023-06-09 14:49:14.000000 edx-enterprise-data-4.6.5/requirements/constraints.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     8790 2023-06-09 14:49:14.000000 edx-enterprise-data-4.6.5/requirements/dev.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       15 2023-06-09 14:49:14.000000 edx-enterprise-data-4.6.5/requirements/django.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      334 2023-06-09 14:49:14.000000 edx-enterprise-data-4.6.5/requirements/pip.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      467 2023-06-09 14:49:14.000000 edx-enterprise-data-4.6.5/requirements/pip_tools.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     9656 2023-06-09 14:49:14.000000 edx-enterprise-data-4.6.5/requirements/quality.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      684 2023-06-09 14:49:14.000000 edx-enterprise-data-4.6.5/requirements/reporting.in
+-rw-r--r--   0 runner    (1001) docker     (122)     6202 2023-06-09 14:49:14.000000 edx-enterprise-data-4.6.5/requirements/test-master.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     4171 2023-06-09 14:49:14.000000 edx-enterprise-data-4.6.5/requirements/test-reporting.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     6100 2023-06-09 14:49:14.000000 edx-enterprise-data-4.6.5/requirements/test.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-09 14:49:18.543490 edx-enterprise-data-4.6.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     4889 2023-06-09 14:49:14.000000 edx-enterprise-data-4.6.5/setup.py
```

### Comparing `edx-enterprise-data-4.6.4/CHANGELOG.rst` & `edx-enterprise-data-4.6.5/CHANGELOG.rst`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,18 @@
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 ----------
 
 =========================
 
+[4.6.5] - 2023-06-09
+--------------------
+  * Releasing a backlog of dependency upgrades and bug fixes.
+
 [4.6.4] - 2022-10-19
 --------------------
   * Refactor enterprise api client and view filters to use cache key without user and remove dependency on session.
 
 [4.6.3] - 2022-09-28
 --------------------
   * Fixed get_enterprise_customer URL.
```

### Comparing `edx-enterprise-data-4.6.4/LICENSE` & `edx-enterprise-data-4.6.5/LICENSE`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.6.4/PKG-INFO` & `edx-enterprise-data-4.6.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: edx-enterprise-data
-Version: 4.6.4
+Version: 4.6.5
 Summary: Enterprise Reporting
-Home-page: https://github.com/edx/edx-enterprise-data
+Home-page: https://github.com/openedx/edx-enterprise-data
 Author: edX
 Author-email: oscm@edx.org
 License: AGPL 3.0
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
 Classifier: Programming Language :: Python :: 3
```

### Comparing `edx-enterprise-data-4.6.4/README.md` & `edx-enterprise-data-4.6.5/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,44 +1,44 @@
 # edx-enterprise-data
 The edX Enterprise Data repo is the home to tools and products related to providing access to Enterprise related data.
 
 This repository is currently split into 2 folders: enterprise_reporting and enterprise_data
 
 ## enterprise_data app
 This django app exposes a REST api endpoint to access enterprise learner activity. The enterprise-data app is published
-to pypi as a library and installed into the [edx-analytics-data-api](https://github.com/edx/edx-analytics-data-api/) project
-and uses OAuth JWT authentication from [edx-drf-extensions](https://github.com/edx/edx-drf-extensions/blob/4569b9bf7e54a917d4acdd545b10c058c960dd1a/edx_rest_framework_extensions/auth/jwt/authentication.py#L17).
+to pypi as a library and installed into the [edx-analytics-data-api](https://github.com/openedx/edx-analytics-data-api/) project
+and uses OAuth JWT authentication from [edx-drf-extensions](https://github.com/openedx/edx-drf-extensions/blob/4569b9bf7e54a917d4acdd545b10c058c960dd1a/edx_rest_framework_extensions/auth/jwt/authentication.py#L17).
 
 ## Prerequisites for develpment
-* [LMS](https://github.com/edx/devstack)
-* [edx-analytics-data-api](https://github.com/edx/edx-analytics-data-api/) - Follow devstack setup instructions in here.
+* [LMS](https://github.com/openedx/devstack)
+* [edx-analytics-data-api](https://github.com/openedx/edx-analytics-data-api/) - Follow devstack setup instructions in here.
 
 ## Setup for local development (Deprecated, prefer running in devstack)
-This app is meant to be installed as an app in [edx-analytics-data-api](https://github.com/edx/edx-analytics-data-api/).
+This app is meant to be installed as an app in [edx-analytics-data-api](https://github.com/openedx/edx-analytics-data-api/).
 1. Create a directory in your filesystem that has the `edx-analytics-data-api` repo in it. Create a folder `src`, and clone this repo into the `src` directory.
 1. Complete the setup in the README of `edx-analytics-data-api`
 1. Navigate to `edx-analytics-data-api` and activate your virtualenv.
 1. In the `edx-analytics-data-api` folder, run `make requirements`
 1. Run `pip install -e ./src/edx-enterprise-data`
 1. Run `./manage.py runserver`
 
 ## Running migrations locally
 The default database configured by devstack is `analytics-api`. If you wish to run migrations on other databases,
 run `./manage.py migrate --database analytics_v1` or `./manage.py migrate --database analytics` in the `edx-analytics-data-api` container.
 
 ## Frontend
-Much of the data from this app is consumed by [frontend-app-admin-portal](https://github.com/edx/frontend-app-admin-portal/).
+Much of the data from this app is consumed by [frontend-app-admin-portal](https://github.com/openedx/frontend-app-admin-portal/).
 Follow the instructions in that README to set it up.
 
 Management commands for creating development data are below.
 
 ### Management Commands for Devs
 
 For the convenience of creating some test data in a local setup, there are some management commands that exist.
-To create a test enterprise, go into the [lms shell][LMS](https://github.com/edx/devstack) and run `./manage.py lms seed_enterprise_devstack_data`
+To create a test enterprise, go into the [lms shell][LMS](https://github.com/openedx/devstack) and run `./manage.py lms seed_enterprise_devstack_data`
 You can then use the test enterprise's UUID for the following commands.
 
 These commands can be run from this repo or from `edx-analytics-data-api`.
 The simplest way to start is to create dummy learner progress data for your test enterprise:
 
 To create 10 users, each with 5 enrollments, using faked data. Running multiple times will create more users and enrollments.
 ```
```

### Comparing `edx-enterprise-data-4.6.4/edx_enterprise_data.egg-info/PKG-INFO` & `edx-enterprise-data-4.6.5/edx_enterprise_data.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: edx-enterprise-data
-Version: 4.6.4
+Version: 4.6.5
 Summary: Enterprise Reporting
-Home-page: https://github.com/edx/edx-enterprise-data
+Home-page: https://github.com/openedx/edx-enterprise-data
 Author: edX
 Author-email: oscm@edx.org
 License: AGPL 3.0
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
 Classifier: Programming Language :: Python :: 3
```

### Comparing `edx-enterprise-data-4.6.4/edx_enterprise_data.egg-info/SOURCES.txt` & `edx-enterprise-data-4.6.5/edx_enterprise_data.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.6.4/enterprise_data/api/v0/serializers.py` & `edx-enterprise-data-4.6.5/enterprise_data/api/v0/serializers.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.6.4/enterprise_data/api/v0/urls.py` & `edx-enterprise-data-4.6.5/enterprise_data/api/v0/urls.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.6.4/enterprise_data/api/v0/views.py` & `edx-enterprise-data-4.6.5/enterprise_data/api/v0/views.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.6.4/enterprise_data/api/v1/serializers.py` & `edx-enterprise-data-4.6.5/enterprise_data/api/v1/serializers.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.6.4/enterprise_data/api/v1/urls.py` & `edx-enterprise-data-4.6.5/enterprise_data/api/v1/urls.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.6.4/enterprise_data/api/v1/views.py` & `edx-enterprise-data-4.6.5/enterprise_data/api/v1/views.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.6.4/enterprise_data/clients.py` & `edx-enterprise-data-4.6.5/enterprise_data/clients.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.6.4/enterprise_data/filters.py` & `edx-enterprise-data-4.6.5/enterprise_data/filters.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.6.4/enterprise_data/fixtures/enterprise_enrollment.json` & `edx-enterprise-data-4.6.5/enterprise_data/fixtures/enterprise_enrollment.json`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.6.4/enterprise_data/fixtures/enterprise_user.json` & `edx-enterprise-data-4.6.5/enterprise_data/fixtures/enterprise_user.json`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.6.4/enterprise_data/management/commands/create_dummy_data.py` & `edx-enterprise-data-4.6.5/enterprise_data/management/commands/create_dummy_data.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.6.4/enterprise_data/management/commands/create_dummy_data_lpr_v1.py` & `edx-enterprise-data-4.6.5/enterprise_data/management/commands/create_dummy_data_lpr_v1.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.6.4/enterprise_data/management/commands/create_enterprise_enrollment.py` & `edx-enterprise-data-4.6.5/enterprise_data/management/commands/create_enterprise_enrollment.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.6.4/enterprise_data/management/commands/create_enterprise_learner_enrollment_lpr_v1.py` & `edx-enterprise-data-4.6.5/enterprise_data/management/commands/create_enterprise_learner_enrollment_lpr_v1.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.6.4/enterprise_data/management/commands/create_enterprise_learner_lpr_v1.py` & `edx-enterprise-data-4.6.5/enterprise_data/management/commands/create_enterprise_learner_lpr_v1.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.6.4/enterprise_data/management/commands/create_enterprise_offer.py` & `edx-enterprise-data-4.6.5/enterprise_data/management/commands/create_enterprise_offer.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.6.4/enterprise_data/management/commands/create_enterprise_user.py` & `edx-enterprise-data-4.6.5/enterprise_data/management/commands/create_enterprise_user.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.6.4/enterprise_data/management/commands/tests/test_create_dummy_data_lpr_v1.py` & `edx-enterprise-data-4.6.5/enterprise_data/management/commands/tests/test_create_dummy_data_lpr_v1.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.6.4/enterprise_data/management/commands/tests/test_create_enterprise_enrollment.py` & `edx-enterprise-data-4.6.5/enterprise_data/management/commands/tests/test_create_enterprise_enrollment.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.6.4/enterprise_data/management/commands/tests/test_create_enterprise_learner_enrollment_lpr_v1.py` & `edx-enterprise-data-4.6.5/enterprise_data/management/commands/tests/test_create_enterprise_learner_enrollment_lpr_v1.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.6.4/enterprise_data/management/commands/tests/test_create_enterprise_learner_lpr_v1.py` & `edx-enterprise-data-4.6.5/enterprise_data/management/commands/tests/test_create_enterprise_learner_lpr_v1.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.6.4/enterprise_data/management/commands/tests/test_create_enterprise_user.py` & `edx-enterprise-data-4.6.5/enterprise_data/management/commands/tests/test_create_enterprise_user.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.6.4/enterprise_data/migrations/0001_initial.py` & `edx-enterprise-data-4.6.5/enterprise_data/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.6.4/enterprise_data/migrations/0002_auto_20180430_1358.py` & `edx-enterprise-data-4.6.5/enterprise_data/migrations/0002_auto_20180430_1358.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.6.4/enterprise_data/migrations/0006_auto_20180612_0336.py` & `edx-enterprise-data-4.6.5/enterprise_data/migrations/0006_auto_20180612_0336.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.6.4/enterprise_data/migrations/0007_auto_20180612_0534.py` & `edx-enterprise-data-4.6.5/enterprise_data/migrations/0007_auto_20180612_0534.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.6.4/enterprise_data/migrations/0008_auto_20180614_0108.py` & `edx-enterprise-data-4.6.5/enterprise_data/migrations/0008_auto_20180614_0108.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.6.4/enterprise_data/migrations/0009_auto_20180628_1152.py` & `edx-enterprise-data-4.6.5/enterprise_data/migrations/0009_auto_20180628_1152.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.6.4/enterprise_data/migrations/0011_enterpriseuser.py` & `edx-enterprise-data-4.6.5/enterprise_data/migrations/0011_enterpriseuser.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.6.4/enterprise_data/migrations/0012_auto_20180831_1930.py` & `edx-enterprise-data-4.6.5/enterprise_data/migrations/0012_auto_20180831_1930.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.6.4/enterprise_data/migrations/0018_enterprisedatafeaturerole_enterprisedataroleassignment.py` & `edx-enterprise-data-4.6.5/enterprise_data/migrations/0018_enterprisedatafeaturerole_enterprisedataroleassignment.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.6.4/enterprise_data/migrations/0019_add_enterprise_data_feature_roles.py` & `edx-enterprise-data-4.6.5/enterprise_data/migrations/0019_add_enterprise_data_feature_roles.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.6.4/enterprise_data/migrations/0020_add_role_based_access_control_switch.py` & `edx-enterprise-data-4.6.5/enterprise_data/migrations/0020_add_role_based_access_control_switch.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.6.4/enterprise_data/migrations/0021_auto_20190329_1241.py` & `edx-enterprise-data-4.6.5/enterprise_data/migrations/0021_auto_20190329_1241.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.6.4/enterprise_data/migrations/0022_remove_role_based_access_control_switch.py` & `edx-enterprise-data-4.6.5/enterprise_data/migrations/0022_remove_role_based_access_control_switch.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.6.4/enterprise_data/migrations/0023_enterpriselearner_enterpriselearnerenrollment.py` & `edx-enterprise-data-4.6.5/enterprise_data/migrations/0023_enterpriselearner_enterpriselearnerenrollment.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.6.4/enterprise_data/migrations/0024_auto_20210602_1811.py` & `edx-enterprise-data-4.6.5/enterprise_data/migrations/0024_auto_20210602_1811.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.6.4/enterprise_data/migrations/0026_auto_20210916_0414.py` & `edx-enterprise-data-4.6.5/enterprise_data/migrations/0026_auto_20210916_0414.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.6.4/enterprise_data/migrations/0029_enterpriseoffer.py` & `edx-enterprise-data-4.6.5/enterprise_data/migrations/0029_enterpriseoffer.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.6.4/enterprise_data/models.py` & `edx-enterprise-data-4.6.5/enterprise_data/models.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.6.4/enterprise_data/settings/test.py` & `edx-enterprise-data-4.6.5/enterprise_data/settings/test.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.6.4/enterprise_data/tests/api/v0/test_serializers.py` & `edx-enterprise-data-4.6.5/enterprise_data/tests/api/v0/test_serializers.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.6.4/enterprise_data/tests/api/v1/test_serializers.py` & `edx-enterprise-data-4.6.5/enterprise_data/tests/api/v1/test_serializers.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.6.4/enterprise_data/tests/api/v1/test_views.py` & `edx-enterprise-data-4.6.5/enterprise_data/tests/api/v1/test_views.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.6.4/enterprise_data/tests/mixins.py` & `edx-enterprise-data-4.6.5/enterprise_data/tests/mixins.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.6.4/enterprise_data/tests/test_clients.py` & `edx-enterprise-data-4.6.5/enterprise_data/tests/test_clients.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.6.4/enterprise_data/tests/test_filters.py` & `edx-enterprise-data-4.6.5/enterprise_data/tests/test_filters.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.6.4/enterprise_data/tests/test_models.py` & `edx-enterprise-data-4.6.5/enterprise_data/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.6.4/enterprise_data/tests/test_utils.py` & `edx-enterprise-data-4.6.5/enterprise_data/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.6.4/enterprise_data/tests/test_views.py` & `edx-enterprise-data-4.6.5/enterprise_data/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.6.4/enterprise_data/utils.py` & `edx-enterprise-data-4.6.5/enterprise_data/utils.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.6.4/enterprise_data_roles/admin.py` & `edx-enterprise-data-4.6.5/enterprise_data_roles/admin.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.6.4/enterprise_data_roles/migrations/0001_initial.py` & `edx-enterprise-data-4.6.5/enterprise_data_roles/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.6.4/enterprise_data_roles/migrations/0002_add_enterprise_data_feature_roles.py` & `edx-enterprise-data-4.6.5/enterprise_data_roles/migrations/0002_add_enterprise_data_feature_roles.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.6.4/enterprise_data_roles/migrations/0003_add_role_based_access_control_switch.py` & `edx-enterprise-data-4.6.5/enterprise_data_roles/migrations/0003_add_role_based_access_control_switch.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.6.4/enterprise_data_roles/migrations/0005_turn_on_role_based_access_control_switch.py` & `edx-enterprise-data-4.6.5/enterprise_data_roles/migrations/0005_turn_on_role_based_access_control_switch.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.6.4/enterprise_data_roles/migrations/0006_remove_role_based_access_control_switch.py` & `edx-enterprise-data-4.6.5/enterprise_data_roles/migrations/0006_remove_role_based_access_control_switch.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.6.4/enterprise_data_roles/migrations/0007_enterprisedataroleassignment_applies_to_all_contexts.py` & `edx-enterprise-data-4.6.5/enterprise_data_roles/migrations/0007_enterprisedataroleassignment_applies_to_all_contexts.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.6.4/enterprise_data_roles/models.py` & `edx-enterprise-data-4.6.5/enterprise_data_roles/models.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.6.4/enterprise_data_roles/rules.py` & `edx-enterprise-data-4.6.5/enterprise_data_roles/rules.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.6.4/enterprise_data_roles/tests/factories.py` & `edx-enterprise-data-4.6.5/enterprise_data_roles/tests/factories.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.6.4/enterprise_data_roles/tests/test_models.py` & `edx-enterprise-data-4.6.5/enterprise_data_roles/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.6.4/enterprise_reporting/clients/__init__.py` & `edx-enterprise-data-4.6.5/enterprise_reporting/clients/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,69 +1,76 @@
 """
 Clients used to access third party systems.
 """
 
 import os
-from datetime import datetime
+from datetime import datetime, timedelta
 from functools import wraps
 from urllib.parse import parse_qs, urljoin, urlparse
 from edx_rest_api_client.client import get_oauth_access_token
 
 import requests
 
 
-class EdxOAuth2APIClient:
+class EdxOAuth2APIMixin:
+    """
+    Base API Client Mixin for accessing edX IDA API endpoints.
+    """
+    @staticmethod
+    def refresh_token(func):
+        """
+        Use this method decorator to ensure the JWT token is refreshed when needed.
+        """
+        @wraps(func)
+        def inner(self, *args, **kwargs):
+            """
+            Before calling the wrapped function, we check if the JWT token is expired, and if so, re-connect.
+            """
+            if self.token_expired():
+                self.connect()
+            return func(self, *args, **kwargs)
+        return inner
+
+
+class EdxOAuth2APIClient(EdxOAuth2APIMixin):
     """
     Base API Client for accessing edX IDA API endpoints.
     """
 
     LMS_ROOT_URL = os.getenv('LMS_ROOT_URL', default='')
     ENTERPRISE_CATALOG_ROOT_URL = os.getenv('ENTERPRISE_CATALOG_ROOT_URL', default='https://enterprise-catalog.edx.org')
     LMS_OAUTH_HOST = os.getenv('LMS_OAUTH_HOST', default='')
     API_BASE_URL = LMS_ROOT_URL + '/api/'
-    APPEND_SLASH = False
+    ACCESS_TOKEN_EXPIRY_THRESHOLD_IN_SECONDS = 60
 
     DEFAULT_VALUE_SAFEGUARD = object()
 
     def __init__(self, client_id=None, client_secret=None):
         """
         Connect to the REST API.
         """
         self.client_id = client_id or os.environ.get('LMS_OAUTH_KEY')
         self.client_secret = client_secret or os.environ.get('LMS_OAUTH_SECRET')
         self.expires_at = datetime.utcnow()
+        self.access_token = None
 
     def connect(self):
         """
         Connect to the REST API, authenticating with an access token retrieved with our client credentials.
         """
         url = urljoin(f'{self.LMS_OAUTH_HOST}/', 'oauth2/access_token')
         self.access_token, self.expires_at = get_oauth_access_token(url, self.client_id, self.client_secret)
 
     def token_expired(self):
         """
         Return True if the JWT token has expired, False if not.
         """
-        return datetime.utcnow() > self.expires_at
-
-    @staticmethod
-    def refresh_token(func):
-        """
-        Use this method decorator to ensure the JWT token is refreshed when needed.
-        """
-        @wraps(func)
-        def inner(self, *args, **kwargs):
-            """
-            Before calling the wrapped function, we check if the JWT token is expired, and if so, re-connect.
-            """
-            if self.token_expired():
-                self.connect()
-            return func(self, *args, **kwargs)
-        return inner
+        return datetime.utcnow() > (self.expires_at - timedelta(seconds=self.ACCESS_TOKEN_EXPIRY_THRESHOLD_IN_SECONDS))
 
+    @EdxOAuth2APIMixin.refresh_token
     def _requests(self, url, querystring):
         headers = {'Authorization': "JWT {}".format(self.access_token)}
         response = requests.get(
             url,
             headers=headers,
             params=querystring
         )
```

### Comparing `edx-enterprise-data-4.6.4/enterprise_reporting/clients/enterprise.py` & `edx-enterprise-data-4.6.5/enterprise_reporting/clients/enterprise.py`

 * *Files 26% similar despite different names*

```diff
@@ -18,23 +18,45 @@
 
 class EnterpriseCatalogAPIClient(EdxOAuth2APIClient):
     """
     Client for connect to the Enterprise Catalog Service API.
     """
     API_BASE_URL = EdxOAuth2APIClient.ENTERPRISE_CATALOG_ROOT_URL + '/api/v1/'
 
-    APPEND_SLASH = True
-    ENTERPRISE_CATALOGS_ENDPOINT = 'enterprise-catalogs'
-    GET_CONTENT_METADATA_ENDPOINT = ENTERPRISE_CATALOGS_ENDPOINT + '/{}/get_content_metadata'
+    ENTERPRISE_CATALOGS_ENDPOINT = 'enterprise-catalogs/'
+    GET_CONTENT_METADATA_ENDPOINT = 'enterprise-catalogs/{}/get_content_metadata'
 
     ENTERPRISE_REPORTING_ENDPOINT = 'enterprise_customer_reporting'
-    ENTERPRISE_CUSTOMER_CATALOGS_ENDPOINT = 'enterprise_catalogs'
 
     PAGE_SIZE = os.getenv('PAGE_SIZE', default=1000)
 
+    @staticmethod
+    def _get_formatted_subjects(item):
+        """
+        Returns formatted subject for course and programs
+        """
+        subjects = item.get('subjects', [])
+        formatted_subjects = []
+        for subject in subjects:
+            try:
+                if isinstance(subject, str):
+                    formatted_subjects.append(subject)
+                elif isinstance(subject, dict):
+                    subject_name = subject.get('name')
+                    if subject_name:
+                        formatted_subjects.append(subject_name)
+                else:
+                    error_msg = "Subject is not a string or a dictionary: {}".format(subject)
+                    LOGGER.error("[Enterprise Reporting]. %s", error_msg)
+                    raise TypeError(error_msg)
+            except AttributeError as error:
+                LOGGER.exception("[Enterprise Reporting]. Item: %s", item)
+                raise error
+        return formatted_subjects
+
     def transform_get_content_metadata(self, traversed_metadata):
         """
         Helper method to transform a response (already traversed pagination) from the enterprise-catalog service's `get_content_metadata`.
         endpoint.
 
         Note: as of June 2022 the data source for content metadata changed from edx platform to the enterprise catalog
         service. As such, content metadata coming from the enterprise catalog service needs to be formatted to match
@@ -75,22 +97,15 @@
                         'weeks_to_complete': cr.get('weeks_to_complete'),
                         'estimated_hours': cr.get('estimated_hours'),
                         'first_enrollable_paid_seat_price': cr.get('first_enrollable_paid_seat_price'),
                         'is_enrollable': cr.get('is_enrollable'),
                     }
                     formatted_course_runs.append(formatted_course_run)
 
-                # Subject attributes also need reformatting
-                subjects = item.get('subjects', [])
-                formatted_subjects = []
-                for subject in subjects:
-                    subject_name = subject.get('name')
-                    if subject_name:
-                        formatted_subjects.append(subject_name)
-
+                formatted_subjects = self._get_formatted_subjects(item)
                 formatted_metadata = {
                     'active': item.get('active'),
                     'aggregation_key': item.get('aggregation_key'),
                     'card_image_url': item.get('card_image_url'),
                     'content_type': item.get('content_type'),
                     'course_ends': item.get('course_ends'),
                     'course_runs': formatted_course_runs,
@@ -110,15 +125,14 @@
                     'uuid': item.get('uuid'),
                 }
 
             content_metadata[content_id] = formatted_metadata
 
         return content_metadata
 
-    @EdxOAuth2APIClient.refresh_token
     def get_content_metadata(self, enterprise_customer_catalogs):
         """Return all content metadata contained in the catalogs associated with a reporting config."""
         content_metadata = OrderedDict()
         for catalog in enterprise_customer_catalogs.get('results', []):
             traversed_metadata = self._load_data(
                 self.GET_CONTENT_METADATA_ENDPOINT.format(catalog['uuid']),
                 should_traverse_pagination=True,
@@ -126,102 +140,66 @@
             )
             transformed_metadata = self.transform_get_content_metadata(traversed_metadata.get('results'))
             content_metadata.update(transformed_metadata)
 
         # We only made this a dictionary to help filter out duplicates by a common key. We just want values now.
         return list(content_metadata.values())
 
+    def get_customer_catalogs(self, enterprise_customer_uuid):
+        """Return all catalog uuids owned by an Enterprise Customer."""
+        return self._load_data(
+            self.ENTERPRISE_CATALOGS_ENDPOINT,
+            should_traverse_pagination=True,
+            querystring={
+                'enterprise_customer': enterprise_customer_uuid,
+                'page_size': self.PAGE_SIZE,
+            },
+        )
+
 
 class EnterpriseAPIClient(EdxOAuth2APIClient):
     """
     Client for connecting to the Enterprise API.
     """
     API_BASE_URL = urljoin(EdxOAuth2APIClient.LMS_ROOT_URL + '/', 'enterprise/api/v1/')
 
     ENTERPRISE_REPORTING_ENDPOINT = 'enterprise_customer_reporting'
-    ENTERPRISE_CUSTOMER_CATALOGS_ENDPOINT = 'enterprise_catalogs'
 
     PAGE_SIZE = os.getenv('PAGE_SIZE', default=1000)
 
-    @EdxOAuth2APIClient.refresh_token
     def get_all_enterprise_reporting_configs(self, **kwargs):
         """
         Query the enterprise customer reporting endpoint for all available configs.
         """
         return self._load_data(
             self.ENTERPRISE_REPORTING_ENDPOINT,
             should_traverse_pagination=True,
             **kwargs
         )
 
-    @EdxOAuth2APIClient.refresh_token
     def get_enterprise_reporting_configs(self, enterprise_customer_uuid, **kwargs):
         """
         Query the enterprise customer reporting endpoint for a given enterprise customer.
         """
         return self._load_data(
             self.ENTERPRISE_REPORTING_ENDPOINT,
             querystring={'enterprise_customer': enterprise_customer_uuid},
             should_traverse_pagination=True,
             **kwargs
         )
 
-    @EdxOAuth2APIClient.refresh_token
-    def get_content_metadata(self, enterprise_customer_uuid, reporting_config):
-        """Return all content metadata contained in the catalogs associated with an Enterprise Customer."""
-        content_metadata = OrderedDict()
-
-        enterprise_customer_catalogs = utils.extract_catalog_uuids_from_reporting_config(reporting_config)
-        if not enterprise_customer_catalogs.get('results'):
-            enterprise_customer_catalogs = self._load_data(
-                self.ENTERPRISE_CUSTOMER_CATALOGS_ENDPOINT,
-                should_traverse_pagination=True,
-                querystring={
-                    'enterprise_customer': enterprise_customer_uuid,
-                    'page_size': self.PAGE_SIZE,
-                },
-            )
-        for catalog in enterprise_customer_catalogs.get('results', []):
-            catalog_content = self._load_data(
-                self.ENTERPRISE_CUSTOMER_CATALOGS_ENDPOINT,
-                resource_id=catalog['uuid'],
-                should_traverse_pagination=True,
-                querystring={'page_size': self.PAGE_SIZE},
-            )
-            # It's possible that there are duplicate items.
-            # Filter them out by assigning common items to their common identifier in a dictionary.
-            for item in catalog_content['results']:
-                key = 'uuid' if item['content_type'] == 'program' else 'key'
-                content_metadata[item[key]] = item
-
-        # We only made this a dictionary to help filter out duplicates by a common key. We just want values now.
-        return list(content_metadata.values())
-
-    @EdxOAuth2APIClient.refresh_token
-    def get_customer_catalogs(self, enterprise_customer_uuid):
-        """Return all catalog uuids owned by an Enterprise Customer."""
-        return self._load_data(
-            self.ENTERPRISE_CUSTOMER_CATALOGS_ENDPOINT,
-            should_traverse_pagination=True,
-            querystring={
-                'enterprise_customer': enterprise_customer_uuid,
-                'page_size': self.PAGE_SIZE,
-            },
-        )
-
 
 class EnterpriseDataApiClient(EdxOAuth2APIClient):
     """
     Client for connecting to the Enterprise Data API.
     """
 
     API_BASE_URL = urljoin(os.getenv('ANALYTICS_API_URL', default='') + '/', 'enterprise/api/v0')
     PAGE_SIZE = os.getenv('PAGE_SIZE', default=1000)
 
-    @EdxOAuth2APIClient.refresh_token
     def get_enterprise_enrollments(self, enterprise_customer_uuid):
         return self._load_data(
             'enterprise',
             resource_id=enterprise_customer_uuid,
             detail_resource='enrollments',
             should_traverse_pagination=True,
             querystring={'page_size': self.PAGE_SIZE},
@@ -240,15 +218,14 @@
     """
     Client for connecting to the Analytics Data API.
     """
 
     API_BASE_URL = urljoin(os.getenv('ANALYTICS_API_URL', default='') + '/', 'api/v0')
     PAGE_SIZE = os.getenv('PAGE_SIZE', default=1000)
 
-    @EdxOAuth2APIClient.refresh_token
     def get_enterprise_engagements(self, enterprise_customer_uuid):
         return self._load_data(
             'enterprise',
             resource_id=enterprise_customer_uuid,
             detail_resource='engagements',
             should_traverse_pagination=True,
             querystring={'page_size': self.PAGE_SIZE},
```

### Comparing `edx-enterprise-data-4.6.4/enterprise_reporting/clients/s3.py` & `edx-enterprise-data-4.6.5/enterprise_reporting/clients/s3.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.6.4/enterprise_reporting/clients/snowflake.py` & `edx-enterprise-data-4.6.5/enterprise_reporting/clients/snowflake.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.6.4/enterprise_reporting/clients/vertica.py` & `edx-enterprise-data-4.6.5/enterprise_reporting/clients/vertica.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.6.4/enterprise_reporting/delivery_method.py` & `edx-enterprise-data-4.6.5/enterprise_reporting/delivery_method.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.6.4/enterprise_reporting/external_resource_link_report.py` & `edx-enterprise-data-4.6.5/enterprise_reporting/external_resource_link_report.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.6.4/enterprise_reporting/fixtures/enterprise_customer_reporting.json` & `edx-enterprise-data-4.6.5/enterprise_reporting/fixtures/enterprise_customer_reporting.json`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.6.4/enterprise_reporting/reporter.py` & `edx-enterprise-data-4.6.5/enterprise_reporting/reporter.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 """
 Classes that handle sending reports for EnterpriseCustomers.
 """
 
-
 import csv
 import datetime
 import json
 import logging
+import os
 from collections import OrderedDict
 from uuid import UUID
 
 from enterprise_reporting.clients.enterprise import (
     AnalyticsDataApiClient,
     EnterpriseAPIClient,
+    EnterpriseCatalogAPIClient,
     EnterpriseDataApiClient,
     EnterpriseDataV1ApiClient,
-    EnterpriseCatalogAPIClient,
 )
 from enterprise_reporting.clients.s3 import S3Client
 from enterprise_reporting.clients.vertica import VerticaClient
 from enterprise_reporting.delivery_method import SFTPDeliveryMethod, SMTPDeliveryMethod
-from enterprise_reporting.utils import decrypt_string, generate_data, extract_catalog_uuids_from_reporting_config
+from enterprise_reporting.utils import decrypt_string, extract_catalog_uuids_from_reporting_config, generate_data
 
 LOGGER = logging.getLogger(__name__)
 NOW = datetime.datetime.now().strftime("%Y-%m-%d")
 
 
 class EnterpriseReportSender:
     """
@@ -76,18 +76,18 @@
         enterprise_customer_name = reporting_config['enterprise_customer']['name']
         delivery_method_str = reporting_config['delivery_method']
         if delivery_method_str == 'email':
             LOGGER.debug('{} is configured to send the report via SMTP to {}'.format(
                 enterprise_customer_name,
                 reporting_config['email'],
             ))
-            delivery_method = SMTPDeliveryMethod(
-                reporting_config,
-                decrypt_string(reporting_config['encrypted_password']),
-            )
+            decrypted_password = None
+            if reporting_config['encrypted_password']:
+                decrypted_password = decrypt_string(reporting_config['encrypted_password'])
+            delivery_method = SMTPDeliveryMethod(reporting_config, decrypted_password)
         elif delivery_method_str == 'sftp':
             LOGGER.debug('{} is configured to send the report via SFTP to {}'.format(
                 enterprise_customer_name,
                 reporting_config['sftp_hostname'],
             ))
             delivery_method = SFTPDeliveryMethod(
                 reporting_config,
@@ -148,48 +148,55 @@
                 enterprise_id=UUID(self.enterprise_customer_uuid).hex
             )
             LOGGER.debug(f'Executing this Vertica query: {query}')
             data_report_file_writer.writerows(vertica_client.stream_results(query))
         vertica_client.close_connection()
         return [data_report_file]
 
+    def get_s3_csv_path(self):
+        """Return S3 CSV path for a manual report else raise an exception if path doesn't exist"""
+        # <data_type>-<enterprise uuid>
+        env_variable_name = f"{self.data_type}-{self.enterprise_customer_uuid.replace('-', '')}"
+        s3_csv_path = os.environ.get(env_variable_name)
+
+        if not s3_csv_path:
+            raise ValueError(f'Invalid S3 CSV path. Path: [{s3_csv_path}]')
+
+        LOGGER.info(
+            'Enterprise UUID: [%s], Enterprise Name: [%s], Data Type: [%s], S3 CSV Path: [%s]',
+            self.enterprise_customer_uuid,
+            self.enterprise_customer_name,
+            self.data_type,
+            s3_csv_path,
+        )
+
+        return s3_csv_path
+
     def _generate_enterprise_report_grade_csv(self):
         """Query S3 and write output to csv file."""
         s3_client = S3Client()
         with open(self.data_report_file_name, 'wb') as data_report_file:
             LOGGER.debug('Fetching enterprise grade report from S3')
-            # temporarily adding file path for PEARSON
-            s3_client.get_enterprise_report(
-                'PEARSON/ENT_REPORT_PEARSON_PERSISTENTSUBSECTIONGRADE/ENT_REPORT_PEARSON_PERSISTENTSUBSECTIONGRADE.csv',
-                data_report_file
-            )
+            s3_client.get_enterprise_report(self.get_s3_csv_path(), data_report_file)
         return [data_report_file]
 
     def _generate_enterprise_report_course_structure_csv(self):
         """Query S3 and write output to csv file."""
         s3_client = S3Client()
         with open(self.data_report_file_name, 'wb') as data_report_file:
             LOGGER.debug('Fetching enterprise course structure report from S3')
-            # temporarily adding file path for PEARSON
-            s3_client.get_enterprise_report(
-                'PEARSON/ENT_REPORT_PEARSON_COURSE_METRICS/ENT_REPORT_PEARSON_COURSE_METRICS.csv',
-                data_report_file
-            )
+            s3_client.get_enterprise_report(self.get_s3_csv_path(), data_report_file)
         return [data_report_file]
 
     def _generate_enterprise_report_completion_csv(self):
         """Query S3 and write output to csv file."""
         s3_client = S3Client()
         with open(self.data_report_file_name, 'wb') as data_report_file:
             LOGGER.debug('Fetching enterprise completion report from S3')
-            # temporarily adding file path for PEARSON
-            s3_client.get_enterprise_report(
-                'PEARSON/ENT_REPORT_PEARSON_BLOCK_COMPLETION/ENT_REPORT_PEARSON_BLOCK_COMPLETION.csv',
-                data_report_file
-            )
+            s3_client.get_enterprise_report(self.get_s3_csv_path(), data_report_file)
         return [data_report_file]
 
     def _generate_enterprise_report_progress_v2_csv(self):
         """Query the Enterprise Data API to get progress data to be turned into a CSV."""
         enrollments = EnterpriseDataApiClient().get_enterprise_enrollments(self.enterprise_customer_uuid)['results']
         if not enrollments:
             return []
@@ -278,23 +285,23 @@
                 for item in grouped_items:
                     writer.writerow(generate_data(item, target='value'))
 
                 files.append(data_report_file)
         return files
 
     def _generate_enterprise_report_catalog_json(self):
-        """Query the Enterprise Customer Catalog API and transfer the results into a JSON file."""
+        """Query the Enterprise Catalog API and transfer the results into a JSON file."""
         content_metadata = self.__get_content_metadata()
         with open(self.data_report_file_name, 'w') as data_report_file:
             json.dump(list(content_metadata), data_report_file, indent=4)
         return [data_report_file]
 
     def __get_content_metadata(self):
-        """Get content metadata from the Enterprise Customer Catalog API."""
+        """Get content metadata from the Enterprise Catalog API."""
         customer_catalogs = extract_catalog_uuids_from_reporting_config(self.reporting_config)
+        enterprise_catalog_api_client = EnterpriseCatalogAPIClient()
+
         if not customer_catalogs.get('results'):
-            platform_api_client = EnterpriseAPIClient()
-            customer_catalogs = platform_api_client.get_customer_catalogs(self.enterprise_customer_uuid)
+            customer_catalogs = enterprise_catalog_api_client.get_customer_catalogs(self.enterprise_customer_uuid)
 
-        enterprise_catalog_api_client = EnterpriseCatalogAPIClient()
         content_metadata = enterprise_catalog_api_client.get_content_metadata(customer_catalogs)
         return content_metadata
```

### Comparing `edx-enterprise-data-4.6.4/enterprise_reporting/send_enterprise_reports.py` & `edx-enterprise-data-4.6.5/enterprise_reporting/send_enterprise_reports.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.6.4/enterprise_reporting/tests/test_delivery_method.py` & `edx-enterprise-data-4.6.5/enterprise_reporting/tests/test_delivery_method.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.6.4/enterprise_reporting/tests/test_enterprise_client.py` & `edx-enterprise-data-4.6.5/enterprise_reporting/tests/test_enterprise_client.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.6.4/enterprise_reporting/tests/test_external_link_report.py` & `edx-enterprise-data-4.6.5/enterprise_reporting/tests/test_external_link_report.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.6.4/enterprise_reporting/tests/test_send_enterprise_reports.py` & `edx-enterprise-data-4.6.5/enterprise_reporting/tests/test_send_enterprise_reports.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.6.4/enterprise_reporting/tests/test_utils.py` & `edx-enterprise-data-4.6.5/enterprise_reporting/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.6.4/enterprise_reporting/tests/utils.py` & `edx-enterprise-data-4.6.5/enterprise_reporting/tests/utils.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.6.4/enterprise_reporting/utils.py` & `edx-enterprise-data-4.6.5/enterprise_reporting/utils.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.6.4/requirements/base.txt` & `edx-enterprise-data-4.6.5/requirements/base.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 #
-# This file is autogenerated by pip-compile with python 3.8
-# To update, run:
+# This file is autogenerated by pip-compile with Python 3.8
+# by the following command:
 #
 #    make upgrade
 #
 amqp==2.6.1
     # via kombu
-asgiref==3.5.2
+asgiref==3.6.0
     # via django
 asn1crypto==1.5.1
     # via
     #   oscrypto
     #   snowflake-connector-python
-awscli==1.25.74
+awscli==1.27.134
     # via -r requirements/reporting.in
-bcrypt==4.0.0
+bcrypt==4.0.1
     # via paramiko
 billiard==3.6.4.0
     # via celery
-boto3==1.24.73
+boto3==1.26.134
     # via -r requirements/reporting.in
-botocore==1.27.73
+botocore==1.29.134
     # via
     #   awscli
     #   boto3
     #   s3transfer
 celery==4.4.7
     # via -r requirements/reporting.in
-certifi==2022.9.14
+certifi==2023.5.7
     # via
     #   py2neo
     #   requests
     #   snowflake-connector-python
 cffi==1.15.1
     # via
     #   cryptography
@@ -41,24 +41,24 @@
     # via
     #   requests
     #   snowflake-connector-python
 click==8.1.3
     # via edx-django-utils
 colorama==0.4.4
     # via awscli
-cryptography==36.0.2
+cryptography==40.0.2
     # via
     #   -r requirements/reporting.in
     #   django-fernet-fields
     #   paramiko
     #   pgpy
     #   pyjwt
     #   pyopenssl
     #   snowflake-connector-python
-django==3.2.15
+django==3.2.19
     # via
     #   -c requirements/constraints.txt
     #   -r requirements/base.in
     #   django-crum
     #   django-fernet-fields
     #   django-filter
     #   django-model-utils
@@ -69,56 +69,56 @@
     #   edx-rbac
 django-crum==0.7.9
     # via
     #   edx-django-utils
     #   edx-rbac
 django-fernet-fields==0.6
     # via -r requirements/base.in
-django-filter==22.1
+django-filter==23.2
     # via -r requirements/base.in
-django-model-utils==4.2.0
+django-model-utils==4.3.1
     # via
     #   -r requirements/base.in
     #   edx-rbac
 django-waffle==3.0.0
     # via
     #   edx-django-utils
     #   edx-drf-extensions
-djangorestframework==3.13.1
+djangorestframework==3.14.0
     # via
     #   drf-jwt
     #   edx-drf-extensions
 docutils==0.16
     # via awscli
 drf-jwt==1.19.2
     # via edx-drf-extensions
-edx-django-utils==5.0.1
+edx-django-utils==5.4.0
     # via
     #   -r requirements/base.in
     #   edx-drf-extensions
     #   edx-rest-api-client
-edx-drf-extensions==8.3.1
+edx-drf-extensions==8.7.0
     # via
     #   -r requirements/base.in
     #   edx-rbac
 edx-opaque-keys==2.3.0
     # via
     #   -r requirements/base.in
     #   edx-drf-extensions
 edx-rbac==1.7.0
     # via -r requirements/base.in
 edx-rest-api-client==5.5.0
     # via -r requirements/base.in
 factory-boy==3.2.1
     # via -r requirements/base.in
-faker==14.2.0
+faker==18.7.0
     # via factory-boy
-filelock==3.8.0
+filelock==3.12.0
     # via snowflake-connector-python
-future==0.18.2
+future==0.18.3
     # via pyjwkest
 idna==3.4
     # via
     #   requests
     #   snowflake-connector-python
 interchange==2021.0.4
     # via py2neo
@@ -126,131 +126,126 @@
     # via
     #   boto3
     #   botocore
 kombu==4.6.11
     # via celery
 monotonic==1.6
     # via py2neo
-newrelic==8.1.0.180
+newrelic==8.8.0
     # via edx-django-utils
 oscrypto==1.3.0
     # via snowflake-connector-python
-packaging==21.3
-    # via py2neo
+packaging==23.1
+    # via
+    #   py2neo
+    #   snowflake-connector-python
 pansi==2020.7.3
     # via py2neo
-paramiko==2.11.0
+paramiko==3.1.0
     # via -r requirements/reporting.in
-pbr==5.10.0
+pbr==5.11.1
     # via stevedore
-pgpy==0.5.4
+pgpy==0.6.0
     # via -r requirements/reporting.in
-psutil==5.9.2
+psutil==5.9.5
     # via edx-django-utils
 py2neo==2021.2.3
     # via -r requirements/reporting.in
-pyasn1==0.4.8
+pyasn1==0.5.0
     # via
     #   pgpy
     #   rsa
 pycparser==2.21
     # via cffi
-pycryptodomex==3.15.0
+pycryptodomex==3.17
     # via
     #   pyjwkest
     #   snowflake-connector-python
-pygments==2.13.0
+pygments==2.15.1
     # via py2neo
 pyjwkest==1.4.2
     # via edx-drf-extensions
-pyjwt[crypto]==2.4.0
+pyjwt[crypto]==2.7.0
     # via
     #   drf-jwt
     #   edx-drf-extensions
     #   edx-rest-api-client
     #   snowflake-connector-python
 pyminizip==0.2.6
     # via -r requirements/reporting.in
-pymongo==3.12.3
+pymongo==3.13.0
     # via edx-opaque-keys
 pynacl==1.5.0
     # via
     #   edx-django-utils
     #   paramiko
-pyopenssl==22.0.0
+pyopenssl==23.1.1
     # via snowflake-connector-python
-pyparsing==3.0.9
-    # via packaging
 python-dateutil==2.8.2
     # via
     #   botocore
     #   edx-drf-extensions
     #   faker
     #   vertica-python
-pytz==2022.2.1
+pytz==2023.3
     # via
     #   celery
     #   django
     #   djangorestframework
     #   interchange
     #   snowflake-connector-python
 pyyaml==5.4.1
     # via awscli
-requests==2.28.1
+requests==2.30.0
     # via
     #   -r requirements/base.in
     #   edx-drf-extensions
     #   edx-rest-api-client
     #   pyjwkest
     #   slumber
     #   snowflake-connector-python
 rsa==4.7.2
     # via awscli
 rules==3.3
     # via -r requirements/base.in
-s3transfer==0.6.0
+s3transfer==0.6.1
     # via
     #   awscli
     #   boto3
 semantic-version==2.10.0
     # via edx-drf-extensions
 six==1.16.0
     # via
     #   edx-drf-extensions
     #   edx-rbac
     #   interchange
     #   pansi
-    #   paramiko
-    #   pgpy
     #   py2neo
     #   pyjwkest
     #   python-dateutil
     #   vertica-python
 slumber==0.7.1
     # via edx-rest-api-client
-snowflake-connector-python==2.7.12
+snowflake-connector-python==3.0.3
     # via -r requirements/reporting.in
-sqlparse==0.4.2
+sqlparse==0.4.4
     # via django
-stevedore==4.0.0
+stevedore==5.1.0
     # via
     #   edx-django-utils
     #   edx-opaque-keys
-typing-extensions==4.3.0
+typing-extensions==4.5.0
     # via snowflake-connector-python
 unicodecsv==0.14.1
     # via -r requirements/reporting.in
-urllib3==1.26.12
+urllib3==1.26.15
     # via
     #   botocore
     #   py2neo
     #   requests
     #   snowflake-connector-python
-vertica-python==1.1.1
+vertica-python==1.3.2
     # via -r requirements/reporting.in
 vine==1.3.0
     # via
     #   amqp
     #   celery
-
-# The following packages are considered to be unsafe in a requirements file:
-# setuptools
```

### Comparing `edx-enterprise-data-4.6.4/requirements/ci.txt` & `edx-enterprise-data-4.6.5/requirements/ci.txt`

 * *Files 20% similar despite different names*

```diff
@@ -1,50 +1,37 @@
 #
-# This file is autogenerated by pip-compile with python 3.8
-# To update, run:
+# This file is autogenerated by pip-compile with Python 3.8
+# by the following command:
 #
 #    make upgrade
 #
-certifi==2022.9.14
-    # via requests
-charset-normalizer==2.1.1
-    # via requests
-codecov==2.1.12
+coverage==7.2.5
     # via -r requirements/ci.in
-coverage==6.4.4
-    # via codecov
 distlib==0.3.6
     # via virtualenv
-filelock==3.8.0
+filelock==3.12.0
     # via
     #   tox
     #   virtualenv
-idna==3.4
-    # via requests
-packaging==21.3
+packaging==23.1
     # via tox
-platformdirs==2.5.2
+platformdirs==3.5.1
     # via virtualenv
 pluggy==1.0.0
     # via tox
 py==1.11.0
     # via tox
-pyparsing==3.0.9
-    # via packaging
-requests==2.28.1
-    # via codecov
 six==1.16.0
     # via tox
 tomli==2.0.1
     # via tox
-tox==3.26.0
+tox==3.28.0
     # via
+    #   -c requirements/constraints.txt
     #   -r requirements/ci.in
     #   tox-battery
 tox-battery==0.5.2
     # via
     #   -c requirements/constraints.txt
     #   -r requirements/ci.in
-urllib3==1.26.12
-    # via requests
-virtualenv==20.16.5
+virtualenv==20.23.0
     # via tox
```

### Comparing `edx-enterprise-data-4.6.4/requirements/constraints.txt` & `edx-enterprise-data-4.6.5/requirements/constraints.txt`

 * *Files 1% similar despite different names*

```diff
@@ -14,7 +14,9 @@
 Django>=3.2,<4.0
 
 # it's experimental, so keep it pinned
 tox-battery==0.5.2
 
 # Constrain until https://github.com/datadriventests/ddt/issues/83 is fixed.
 ddt<1.4.0
+
+tox<4.0.0
```

### Comparing `edx-enterprise-data-4.6.4/requirements/dev.txt` & `edx-enterprise-data-4.6.5/requirements/dev.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,55 +1,55 @@
 #
-# This file is autogenerated by pip-compile with python 3.8
-# To update, run:
+# This file is autogenerated by pip-compile with Python 3.8
+# by the following command:
 #
 #    make upgrade
 #
 amqp==2.6.1
     # via kombu
-asgiref==3.5.2
+asgiref==3.6.0
     # via django
 asn1crypto==1.5.1
     # via
     #   oscrypto
     #   snowflake-connector-python
-astroid==2.12.9
+astroid==2.15.5
     # via
     #   pylint
     #   pylint-celery
-awscli==1.25.74
+awscli==1.27.134
     # via -r requirements/reporting.in
-bcrypt==4.0.0
+bcrypt==4.0.1
     # via paramiko
 billiard==3.6.4.0
     # via celery
-bleach==5.0.1
+bleach==6.0.0
     # via readme-renderer
-boto3==1.24.73
+boto3==1.26.134
     # via -r requirements/reporting.in
-botocore==1.27.73
+botocore==1.29.134
     # via
     #   awscli
     #   boto3
     #   s3transfer
-build==0.8.0
+build==0.10.0
     # via pip-tools
 celery==4.4.7
     # via -r requirements/reporting.in
-certifi==2022.9.14
+certifi==2023.5.7
     # via
     #   py2neo
     #   requests
     #   snowflake-connector-python
 cffi==1.15.1
     # via
     #   cryptography
     #   pynacl
     #   snowflake-connector-python
-chardet==5.0.0
+chardet==5.1.0
     # via diff-cover
 charset-normalizer==2.1.1
     # via
     #   requests
     #   snowflake-connector-python
 click==8.1.3
     # via
@@ -60,33 +60,31 @@
     #   pip-tools
 click-log==0.4.0
     # via edx-lint
 code-annotations==1.3.0
     # via edx-lint
 colorama==0.4.4
     # via awscli
-commonmark==0.9.1
-    # via rich
-cryptography==36.0.2
+cryptography==40.0.2
     # via
     #   -r requirements/reporting.in
     #   django-fernet-fields
     #   paramiko
     #   pgpy
     #   pyjwt
     #   pyopenssl
     #   secretstorage
     #   snowflake-connector-python
-diff-cover==6.5.1
+diff-cover==7.5.0
     # via -r requirements/dev-enterprise_data.in
-dill==0.3.5.1
+dill==0.3.6
     # via pylint
 distlib==0.3.6
     # via virtualenv
-django==3.2.15
+django==3.2.19
     # via
     #   -c requirements/constraints.txt
     #   -r requirements/base.in
     #   django-crum
     #   django-fernet-fields
     #   django-filter
     #   django-model-utils
@@ -98,248 +96,253 @@
     #   edx-rbac
 django-crum==0.7.9
     # via
     #   edx-django-utils
     #   edx-rbac
 django-fernet-fields==0.6
     # via -r requirements/base.in
-django-filter==22.1
+django-filter==23.2
     # via -r requirements/base.in
-django-model-utils==4.2.0
+django-model-utils==4.3.1
     # via
     #   -r requirements/base.in
     #   edx-rbac
 django-waffle==3.0.0
     # via
     #   edx-django-utils
     #   edx-drf-extensions
-djangorestframework==3.13.1
+djangorestframework==3.14.0
     # via
     #   drf-jwt
     #   edx-drf-extensions
 docutils==0.16
     # via
     #   awscli
     #   readme-renderer
 drf-jwt==1.19.2
     # via edx-drf-extensions
-edx-django-utils==5.0.1
+edx-django-utils==5.4.0
     # via
     #   -r requirements/base.in
     #   edx-drf-extensions
     #   edx-rest-api-client
-edx-drf-extensions==8.3.1
+edx-drf-extensions==8.7.0
     # via
     #   -r requirements/base.in
     #   edx-rbac
-edx-i18n-tools==0.9.1
+edx-i18n-tools==0.9.2
     # via -r requirements/dev-enterprise_data.in
-edx-lint==5.2.5
+edx-lint==5.3.4
     # via
     #   -r requirements/dev-enterprise_data.in
     #   -r requirements/quality.in
 edx-opaque-keys==2.3.0
     # via
     #   -r requirements/base.in
     #   edx-drf-extensions
 edx-rbac==1.7.0
     # via -r requirements/base.in
 edx-rest-api-client==5.5.0
     # via -r requirements/base.in
 factory-boy==3.2.1
     # via -r requirements/base.in
-faker==14.2.0
+faker==18.7.0
     # via factory-boy
-filelock==3.8.0
+filelock==3.12.0
     # via
     #   snowflake-connector-python
     #   tox
     #   virtualenv
-future==0.18.2
+future==0.18.3
     # via pyjwkest
 idna==3.4
     # via
     #   requests
     #   snowflake-connector-python
-importlib-metadata==4.12.0
+importlib-metadata==6.6.0
     # via
     #   keyring
     #   twine
+importlib-resources==5.12.0
+    # via keyring
 interchange==2021.0.4
     # via py2neo
-isort==5.10.1
+isort==5.12.0
     # via
     #   -r requirements/quality.in
     #   pylint
-jaraco-classes==3.2.2
+jaraco-classes==3.2.3
     # via keyring
 jeepney==0.8.0
     # via
     #   keyring
     #   secretstorage
 jinja2==3.1.2
     # via
     #   code-annotations
     #   diff-cover
 jmespath==1.0.1
     # via
     #   boto3
     #   botocore
-keyring==23.9.1
+keyring==23.13.1
     # via twine
 kombu==4.6.11
     # via celery
-lazy-object-proxy==1.7.1
+lazy-object-proxy==1.9.0
     # via astroid
-markupsafe==2.1.1
+markdown-it-py==2.2.0
+    # via rich
+markupsafe==2.1.2
     # via jinja2
 mccabe==0.7.0
     # via pylint
+mdurl==0.1.2
+    # via markdown-it-py
 monotonic==1.6
     # via py2neo
-more-itertools==8.14.0
+more-itertools==9.1.0
     # via jaraco-classes
-newrelic==8.1.0.180
+newrelic==8.8.0
     # via edx-django-utils
 oscrypto==1.3.0
     # via snowflake-connector-python
-packaging==21.3
+packaging==23.1
     # via
     #   build
     #   py2neo
+    #   snowflake-connector-python
     #   tox
 pansi==2020.7.3
     # via py2neo
-paramiko==2.11.0
+paramiko==3.1.0
     # via -r requirements/reporting.in
-path==16.4.0
+path==16.6.0
     # via edx-i18n-tools
-pbr==5.10.0
+pbr==5.11.1
     # via stevedore
-pep517==0.13.0
-    # via build
-pgpy==0.5.4
+pgpy==0.6.0
     # via -r requirements/reporting.in
-pip-tools==6.8.0
+pip-tools==6.13.0
     # via -r requirements/dev-enterprise_data.in
-pkginfo==1.8.3
+pkginfo==1.9.6
     # via twine
-platformdirs==2.5.2
+platformdirs==3.5.1
     # via
     #   pylint
     #   virtualenv
 pluggy==1.0.0
     # via
     #   diff-cover
     #   tox
-polib==1.1.1
+polib==1.2.0
     # via edx-i18n-tools
-psutil==5.9.2
+psutil==5.9.5
     # via edx-django-utils
 py==1.11.0
     # via tox
 py2neo==2021.2.3
     # via -r requirements/reporting.in
-pyasn1==0.4.8
+pyasn1==0.5.0
     # via
     #   pgpy
     #   rsa
-pycodestyle==2.9.1
+pycodestyle==2.10.0
     # via -r requirements/quality.in
 pycparser==2.21
     # via cffi
-pycryptodomex==3.15.0
+pycryptodomex==3.17
     # via
     #   pyjwkest
     #   snowflake-connector-python
-pydocstyle==6.1.1
+pydocstyle==6.3.0
     # via -r requirements/quality.in
-pygments==2.13.0
+pygments==2.15.1
     # via
     #   diff-cover
     #   py2neo
     #   readme-renderer
     #   rich
 pyjwkest==1.4.2
     # via edx-drf-extensions
-pyjwt[crypto]==2.4.0
+pyjwt[crypto]==2.7.0
     # via
     #   drf-jwt
     #   edx-drf-extensions
     #   edx-rest-api-client
     #   snowflake-connector-python
-pylint==2.15.2
+pylint==2.17.4
     # via
     #   edx-lint
     #   pylint-celery
     #   pylint-django
     #   pylint-plugin-utils
 pylint-celery==0.3
     # via edx-lint
 pylint-django==2.5.3
     # via edx-lint
-pylint-plugin-utils==0.7
+pylint-plugin-utils==0.8.1
     # via
     #   pylint-celery
     #   pylint-django
 pyminizip==0.2.6
     # via -r requirements/reporting.in
-pymongo==3.12.3
+pymongo==3.13.0
     # via edx-opaque-keys
 pynacl==1.5.0
     # via
     #   edx-django-utils
     #   paramiko
-pyopenssl==22.0.0
+pyopenssl==23.1.1
     # via snowflake-connector-python
-pyparsing==3.0.9
-    # via packaging
+pyproject-hooks==1.0.0
+    # via build
 python-dateutil==2.8.2
     # via
     #   botocore
     #   edx-drf-extensions
     #   faker
     #   vertica-python
-python-slugify==6.1.2
+python-slugify==8.0.1
     # via code-annotations
-pytz==2022.2.1
+pytz==2023.3
     # via
     #   celery
     #   django
     #   djangorestframework
     #   interchange
     #   snowflake-connector-python
 pyyaml==5.4.1
     # via
     #   awscli
     #   code-annotations
     #   edx-i18n-tools
-readme-renderer==37.1
+readme-renderer==37.3
     # via twine
-requests==2.28.1
+requests==2.30.0
     # via
     #   -r requirements/base.in
     #   edx-drf-extensions
     #   edx-rest-api-client
     #   pyjwkest
     #   requests-toolbelt
     #   slumber
     #   snowflake-connector-python
     #   twine
-requests-toolbelt==0.9.1
+requests-toolbelt==1.0.0
     # via twine
 rfc3986==2.0.0
     # via twine
-rich==12.5.1
+rich==13.3.5
     # via twine
 rsa==4.7.2
     # via awscli
 rules==3.3
     # via -r requirements/base.in
-s3transfer==0.6.0
+s3transfer==0.6.1
     # via
     #   awscli
     #   boto3
 secretstorage==3.3.3
     # via keyring
 semantic-version==2.10.0
     # via edx-drf-extensions
@@ -347,86 +350,87 @@
     # via
     #   bleach
     #   edx-drf-extensions
     #   edx-lint
     #   edx-rbac
     #   interchange
     #   pansi
-    #   paramiko
-    #   pgpy
     #   py2neo
     #   pyjwkest
     #   python-dateutil
     #   tox
     #   vertica-python
 slumber==0.7.1
     # via edx-rest-api-client
 snowballstemmer==2.2.0
     # via pydocstyle
-snowflake-connector-python==2.7.12
+snowflake-connector-python==3.0.3
     # via -r requirements/reporting.in
-sqlparse==0.4.2
+sqlparse==0.4.4
     # via django
-stevedore==4.0.0
+stevedore==5.1.0
     # via
     #   code-annotations
     #   edx-django-utils
     #   edx-opaque-keys
-testfixtures==7.0.0
+testfixtures==7.1.0
     # via -r requirements/quality.in
 text-unidecode==1.3
     # via python-slugify
 tomli==2.0.1
     # via
     #   build
-    #   pep517
     #   pylint
+    #   pyproject-hooks
     #   tox
-tomlkit==0.11.4
+tomlkit==0.11.8
     # via pylint
-tox==3.26.0
+tox==3.28.0
     # via
+    #   -c requirements/constraints.txt
     #   -r requirements/dev-enterprise_data.in
     #   tox-battery
 tox-battery==0.5.2
     # via
     #   -c requirements/constraints.txt
     #   -r requirements/dev-enterprise_data.in
-twine==4.0.1
+twine==4.0.2
     # via -r requirements/dev-enterprise_data.in
-typing-extensions==4.3.0
+typing-extensions==4.5.0
     # via
     #   astroid
     #   pylint
     #   rich
     #   snowflake-connector-python
 unicodecsv==0.14.1
     # via -r requirements/reporting.in
-urllib3==1.26.12
+urllib3==1.26.15
     # via
     #   botocore
     #   py2neo
     #   requests
     #   snowflake-connector-python
     #   twine
-vertica-python==1.1.1
+vertica-python==1.3.2
     # via -r requirements/reporting.in
 vine==1.3.0
     # via
     #   amqp
     #   celery
-virtualenv==20.16.5
+virtualenv==20.23.0
     # via tox
 webencodings==0.5.1
     # via bleach
-wheel==0.37.1
+wheel==0.40.0
     # via
     #   -r requirements/dev-enterprise_data.in
     #   pip-tools
-wrapt==1.14.1
+wrapt==1.15.0
     # via astroid
-zipp==3.8.1
-    # via importlib-metadata
+zipp==3.15.0
+    # via
+    #   importlib-metadata
+    #   importlib-resources
 
 # The following packages are considered to be unsafe in a requirements file:
 # pip
 # setuptools
```

### Comparing `edx-enterprise-data-4.6.4/requirements/quality.txt` & `edx-enterprise-data-4.6.5/requirements/quality.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,57 +1,55 @@
 #
-# This file is autogenerated by pip-compile with python 3.8
-# To update, run:
+# This file is autogenerated by pip-compile with Python 3.8
+# by the following command:
 #
 #    make upgrade
 #
 amqp==2.6.1
     # via kombu
-asgiref==3.5.2
+asgiref==3.6.0
     # via django
 asn1crypto==1.5.1
     # via
     #   oscrypto
     #   snowflake-connector-python
-astroid==2.12.9
+astroid==2.15.5
     # via
     #   pylint
     #   pylint-celery
-attrs==22.1.0
-    # via pytest
-awscli==1.25.74
+awscli==1.27.134
     # via -r requirements/reporting.in
-bcrypt==4.0.0
+bcrypt==4.0.1
     # via paramiko
 billiard==3.6.4.0
     # via celery
-bleach==5.0.1
+bleach==6.0.0
     # via readme-renderer
-boto3==1.24.73
+boto3==1.26.134
     # via -r requirements/reporting.in
-botocore==1.27.73
+botocore==1.29.134
     # via
     #   awscli
     #   boto3
     #   s3transfer
-build==0.8.0
+build==0.10.0
     # via pip-tools
 celery==4.4.7
     # via -r requirements/reporting.in
-certifi==2022.9.14
+certifi==2023.5.7
     # via
     #   py2neo
     #   requests
     #   snowflake-connector-python
 cffi==1.15.1
     # via
     #   cryptography
     #   pynacl
     #   snowflake-connector-python
-chardet==5.0.0
+chardet==5.1.0
     # via diff-cover
 charset-normalizer==2.1.1
     # via
     #   requests
     #   snowflake-connector-python
 click==8.1.3
     # via
@@ -62,39 +60,37 @@
     #   pip-tools
 click-log==0.4.0
     # via edx-lint
 code-annotations==1.3.0
     # via edx-lint
 colorama==0.4.4
     # via awscli
-commonmark==0.9.1
-    # via rich
-coverage[toml]==6.4.4
+coverage[toml]==7.2.5
     # via pytest-cov
-cryptography==36.0.2
+cryptography==40.0.2
     # via
     #   -r requirements/reporting.in
     #   django-fernet-fields
     #   paramiko
     #   pgpy
     #   pyjwt
     #   pyopenssl
     #   secretstorage
     #   snowflake-connector-python
 ddt==1.3.1
     # via
     #   -c requirements/constraints.txt
     #   -r requirements/test.in
-diff-cover==6.5.1
+diff-cover==7.5.0
     # via -r requirements/dev-enterprise_data.in
-dill==0.3.5.1
+dill==0.3.6
     # via pylint
 distlib==0.3.6
     # via virtualenv
-django==3.2.15
+django==3.2.19
     # via
     #   -c requirements/constraints.txt
     #   -r requirements/base.in
     #   django-crum
     #   django-fernet-fields
     #   django-filter
     #   django-model-utils
@@ -106,275 +102,281 @@
     #   edx-rbac
 django-crum==0.7.9
     # via
     #   edx-django-utils
     #   edx-rbac
 django-fernet-fields==0.6
     # via -r requirements/base.in
-django-filter==22.1
+django-filter==23.2
     # via -r requirements/base.in
-django-model-utils==4.2.0
+django-model-utils==4.3.1
     # via
     #   -r requirements/base.in
     #   -r requirements/test.in
     #   edx-rbac
 django-waffle==3.0.0
     # via
     #   edx-django-utils
     #   edx-drf-extensions
-djangorestframework==3.13.1
+djangorestframework==3.14.0
     # via
     #   drf-jwt
     #   edx-drf-extensions
 docutils==0.16
     # via
     #   awscli
     #   readme-renderer
 drf-jwt==1.19.2
     # via edx-drf-extensions
-edx-django-utils==5.0.1
+edx-django-utils==5.4.0
     # via
     #   -r requirements/base.in
     #   edx-drf-extensions
     #   edx-rest-api-client
-edx-drf-extensions==8.3.1
+edx-drf-extensions==8.7.0
     # via
     #   -r requirements/base.in
     #   edx-rbac
-edx-i18n-tools==0.9.1
+edx-i18n-tools==0.9.2
     # via -r requirements/dev-enterprise_data.in
-edx-lint==5.2.5
+edx-lint==5.3.4
     # via
     #   -r requirements/dev-enterprise_data.in
     #   -r requirements/quality.in
 edx-opaque-keys==2.3.0
     # via
     #   -r requirements/base.in
     #   edx-drf-extensions
 edx-rbac==1.7.0
     # via -r requirements/base.in
 edx-rest-api-client==5.5.0
     # via -r requirements/base.in
+exceptiongroup==1.1.1
+    # via pytest
 factory-boy==3.2.1
     # via
     #   -r requirements/base.in
     #   -r requirements/test.in
-faker==14.2.0
+faker==18.7.0
     # via factory-boy
-filelock==3.8.0
+filelock==3.12.0
     # via
     #   snowflake-connector-python
     #   tox
     #   virtualenv
 flaky==3.7.0
     # via -r requirements/test.in
 freezegun==1.2.2
     # via -r requirements/test.in
-future==0.18.2
+future==0.18.3
     # via pyjwkest
 idna==3.4
     # via
     #   requests
     #   snowflake-connector-python
-importlib-metadata==4.12.0
+importlib-metadata==6.6.0
     # via
     #   keyring
     #   twine
-iniconfig==1.1.1
+importlib-resources==5.12.0
+    # via keyring
+iniconfig==2.0.0
     # via pytest
 interchange==2021.0.4
     # via py2neo
-isort==5.10.1
+isort==5.12.0
     # via
     #   -r requirements/quality.in
     #   pylint
-jaraco-classes==3.2.2
+jaraco-classes==3.2.3
     # via keyring
 jeepney==0.8.0
     # via
     #   keyring
     #   secretstorage
 jinja2==3.1.2
     # via
     #   code-annotations
     #   diff-cover
 jmespath==1.0.1
     # via
     #   boto3
     #   botocore
-keyring==23.9.1
+keyring==23.13.1
     # via twine
 kombu==4.6.11
     # via celery
-lazy-object-proxy==1.7.1
+lazy-object-proxy==1.9.0
     # via astroid
-markupsafe==2.1.1
+markdown-it-py==2.2.0
+    # via rich
+markupsafe==2.1.2
     # via jinja2
 mccabe==0.7.0
     # via pylint
-mock==4.0.3
+mdurl==0.1.2
+    # via markdown-it-py
+mock==5.0.2
     # via -r requirements/test.in
 monotonic==1.6
     # via py2neo
-more-itertools==8.14.0
+more-itertools==9.1.0
     # via jaraco-classes
-newrelic==8.1.0.180
+newrelic==8.8.0
     # via edx-django-utils
 oscrypto==1.3.0
     # via snowflake-connector-python
-packaging==21.3
+packaging==23.1
     # via
     #   build
     #   py2neo
     #   pytest
+    #   snowflake-connector-python
     #   tox
 pansi==2020.7.3
     # via py2neo
-paramiko==2.11.0
+paramiko==3.1.0
     # via -r requirements/reporting.in
-path==16.4.0
+path==16.6.0
     # via edx-i18n-tools
-pbr==5.10.0
+pbr==5.11.1
     # via stevedore
-pep517==0.13.0
-    # via build
-pgpy==0.5.4
+pgpy==0.6.0
     # via -r requirements/reporting.in
-pip-tools==6.8.0
+pip-tools==6.13.0
     # via -r requirements/dev-enterprise_data.in
-pkginfo==1.8.3
+pkginfo==1.9.6
     # via twine
-platformdirs==2.5.2
+platformdirs==3.5.1
     # via
     #   pylint
     #   virtualenv
 pluggy==1.0.0
     # via
     #   diff-cover
     #   pytest
     #   tox
-polib==1.1.1
+polib==1.2.0
     # via edx-i18n-tools
-psutil==5.9.2
+psutil==5.9.5
     # via edx-django-utils
 py==1.11.0
-    # via
-    #   pytest
-    #   tox
+    # via tox
 py2neo==2021.2.3
     # via -r requirements/reporting.in
-pyasn1==0.4.8
+pyasn1==0.5.0
     # via
     #   pgpy
     #   rsa
-pycodestyle==2.9.1
+pycodestyle==2.10.0
     # via -r requirements/quality.in
 pycparser==2.21
     # via cffi
-pycryptodomex==3.15.0
+pycryptodomex==3.17
     # via
     #   pyjwkest
     #   snowflake-connector-python
-pydocstyle==6.1.1
+pydocstyle==6.3.0
     # via -r requirements/quality.in
-pygments==2.13.0
+pygments==2.15.1
     # via
     #   diff-cover
     #   py2neo
     #   readme-renderer
     #   rich
 pyjwkest==1.4.2
     # via edx-drf-extensions
-pyjwt[crypto]==2.4.0
+pyjwt[crypto]==2.7.0
     # via
     #   drf-jwt
     #   edx-drf-extensions
     #   edx-rest-api-client
     #   snowflake-connector-python
-pylint==2.15.2
+pylint==2.17.4
     # via
     #   edx-lint
     #   pylint-celery
     #   pylint-django
     #   pylint-plugin-utils
 pylint-celery==0.3
     # via edx-lint
 pylint-django==2.5.3
     # via edx-lint
-pylint-plugin-utils==0.7
+pylint-plugin-utils==0.8.1
     # via
     #   pylint-celery
     #   pylint-django
 pyminizip==0.2.6
     # via -r requirements/reporting.in
-pymongo==3.12.3
+pymongo==3.13.0
     # via edx-opaque-keys
 pynacl==1.5.0
     # via
     #   edx-django-utils
     #   paramiko
-pyopenssl==22.0.0
+pyopenssl==23.1.1
     # via snowflake-connector-python
-pyparsing==3.0.9
-    # via packaging
-pytest==7.1.3
+pyproject-hooks==1.0.0
+    # via build
+pytest==7.3.1
     # via
     #   pytest-cov
     #   pytest-django
-pytest-cov==3.0.0
+pytest-cov==4.0.0
     # via -r requirements/test.in
 pytest-django==4.5.2
     # via -r requirements/test.in
 python-dateutil==2.8.2
     # via
     #   botocore
     #   edx-drf-extensions
     #   faker
     #   freezegun
     #   vertica-python
-python-slugify==6.1.2
+python-slugify==8.0.1
     # via code-annotations
-pytz==2022.2.1
+pytz==2023.3
     # via
     #   celery
     #   django
     #   djangorestframework
     #   interchange
     #   snowflake-connector-python
 pyyaml==5.4.1
     # via
     #   awscli
     #   code-annotations
     #   edx-i18n-tools
-readme-renderer==37.1
+    #   responses
+readme-renderer==37.3
     # via twine
-requests==2.28.1
+requests==2.30.0
     # via
     #   -r requirements/base.in
     #   edx-drf-extensions
     #   edx-rest-api-client
     #   pyjwkest
     #   requests-toolbelt
     #   responses
     #   slumber
     #   snowflake-connector-python
     #   twine
-requests-toolbelt==0.9.1
+requests-toolbelt==1.0.0
     # via twine
-responses==0.21.0
+responses==0.23.1
     # via -r requirements/test.in
 rfc3986==2.0.0
     # via twine
-rich==12.5.1
+rich==13.3.5
     # via twine
 rsa==4.7.2
     # via awscli
 rules==3.3
     # via -r requirements/base.in
-s3transfer==0.6.0
+s3transfer==0.6.1
     # via
     #   awscli
     #   boto3
 secretstorage==3.3.3
     # via keyring
 semantic-version==2.10.0
     # via edx-drf-extensions
@@ -382,91 +384,94 @@
     # via
     #   bleach
     #   edx-drf-extensions
     #   edx-lint
     #   edx-rbac
     #   interchange
     #   pansi
-    #   paramiko
-    #   pgpy
     #   py2neo
     #   pyjwkest
     #   python-dateutil
     #   tox
     #   vertica-python
 slumber==0.7.1
     # via edx-rest-api-client
 snowballstemmer==2.2.0
     # via pydocstyle
-snowflake-connector-python==2.7.12
+snowflake-connector-python==3.0.3
     # via -r requirements/reporting.in
-sqlparse==0.4.2
+sqlparse==0.4.4
     # via django
-stevedore==4.0.0
+stevedore==5.1.0
     # via
     #   code-annotations
     #   edx-django-utils
     #   edx-opaque-keys
-testfixtures==7.0.0
+testfixtures==7.1.0
     # via
     #   -r requirements/quality.in
     #   -r requirements/test.in
 text-unidecode==1.3
     # via python-slugify
 tomli==2.0.1
     # via
     #   build
     #   coverage
-    #   pep517
     #   pylint
+    #   pyproject-hooks
     #   pytest
     #   tox
-tomlkit==0.11.4
+tomlkit==0.11.8
     # via pylint
-tox==3.26.0
+tox==3.28.0
     # via
+    #   -c requirements/constraints.txt
     #   -r requirements/dev-enterprise_data.in
     #   tox-battery
 tox-battery==0.5.2
     # via
     #   -c requirements/constraints.txt
     #   -r requirements/dev-enterprise_data.in
-twine==4.0.1
+twine==4.0.2
     # via -r requirements/dev-enterprise_data.in
-typing-extensions==4.3.0
+types-pyyaml==6.0.12.9
+    # via responses
+typing-extensions==4.5.0
     # via
     #   astroid
     #   pylint
     #   rich
     #   snowflake-connector-python
 unicodecsv==0.14.1
     # via -r requirements/reporting.in
-urllib3==1.26.12
+urllib3==1.26.15
     # via
     #   botocore
     #   py2neo
     #   requests
     #   responses
     #   snowflake-connector-python
     #   twine
-vertica-python==1.1.1
+vertica-python==1.3.2
     # via -r requirements/reporting.in
 vine==1.3.0
     # via
     #   amqp
     #   celery
-virtualenv==20.16.5
+virtualenv==20.23.0
     # via tox
 webencodings==0.5.1
     # via bleach
-wheel==0.37.1
+wheel==0.40.0
     # via
     #   -r requirements/dev-enterprise_data.in
     #   pip-tools
-wrapt==1.14.1
+wrapt==1.15.0
     # via astroid
-zipp==3.8.1
-    # via importlib-metadata
+zipp==3.15.0
+    # via
+    #   importlib-metadata
+    #   importlib-resources
 
 # The following packages are considered to be unsafe in a requirements file:
 # pip
 # setuptools
```

### Comparing `edx-enterprise-data-4.6.4/requirements/reporting.in` & `edx-enterprise-data-4.6.5/requirements/reporting.in`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.6.4/requirements/test-master.txt` & `edx-enterprise-data-4.6.5/requirements/test.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,39 +1,37 @@
 #
-# This file is autogenerated by pip-compile with python 3.8
-# To update, run:
+# This file is autogenerated by pip-compile with Python 3.8
+# by the following command:
 #
 #    make upgrade
 #
 amqp==2.6.1
     # via kombu
-asgiref==3.5.2
+asgiref==3.6.0
     # via django
 asn1crypto==1.5.1
     # via
     #   oscrypto
     #   snowflake-connector-python
-attrs==22.1.0
-    # via pytest
-awscli==1.25.74
+awscli==1.27.134
     # via -r requirements/reporting.in
-bcrypt==4.0.0
+bcrypt==4.0.1
     # via paramiko
 billiard==3.6.4.0
     # via celery
-boto3==1.24.73
+boto3==1.26.134
     # via -r requirements/reporting.in
-botocore==1.27.73
+botocore==1.29.134
     # via
     #   awscli
     #   boto3
     #   s3transfer
 celery==4.4.7
     # via -r requirements/reporting.in
-certifi==2022.9.14
+certifi==2023.5.7
     # via
     #   py2neo
     #   requests
     #   snowflake-connector-python
 cffi==1.15.1
     # via
     #   cryptography
@@ -43,33 +41,33 @@
     # via
     #   requests
     #   snowflake-connector-python
 click==8.1.3
     # via edx-django-utils
 colorama==0.4.4
     # via awscli
-coverage[toml]==6.4.4
+coverage[toml]==7.2.5
     # via pytest-cov
-cryptography==36.0.2
+cryptography==40.0.2
     # via
     #   -r requirements/reporting.in
     #   django-fernet-fields
     #   paramiko
     #   pgpy
     #   pyjwt
     #   pyopenssl
     #   snowflake-connector-python
 ddt==1.3.1
     # via
     #   -c requirements/constraints.txt
     #   -r requirements/test.in
+django==3.2.19
     # via
     #   -c requirements/constraints.txt
     #   -r requirements/base.in
-    #   -r requirements/test-master.in
     #   django-crum
     #   django-fernet-fields
     #   django-filter
     #   django-model-utils
     #   djangorestframework
     #   drf-jwt
     #   edx-django-utils
@@ -77,226 +75,222 @@
     #   edx-rbac
 django-crum==0.7.9
     # via
     #   edx-django-utils
     #   edx-rbac
 django-fernet-fields==0.6
     # via -r requirements/base.in
-django-filter==22.1
+django-filter==23.2
     # via -r requirements/base.in
-django-model-utils==4.2.0
+django-model-utils==4.3.1
     # via
     #   -r requirements/base.in
     #   -r requirements/test.in
     #   edx-rbac
 django-waffle==3.0.0
     # via
     #   edx-django-utils
     #   edx-drf-extensions
-djangorestframework==3.13.1
+djangorestframework==3.14.0
     # via
-    #   -r requirements/test-master.in
     #   drf-jwt
     #   edx-drf-extensions
 docutils==0.16
     # via awscli
 drf-jwt==1.19.2
     # via edx-drf-extensions
-edx-django-utils==5.0.1
+edx-django-utils==5.4.0
     # via
     #   -r requirements/base.in
     #   edx-drf-extensions
     #   edx-rest-api-client
-edx-drf-extensions==8.3.1
+edx-drf-extensions==8.7.0
     # via
     #   -r requirements/base.in
-    #   -r requirements/test-master.in
     #   edx-rbac
 edx-opaque-keys==2.3.0
     # via
     #   -r requirements/base.in
     #   edx-drf-extensions
 edx-rbac==1.7.0
     # via -r requirements/base.in
 edx-rest-api-client==5.5.0
     # via -r requirements/base.in
+exceptiongroup==1.1.1
+    # via pytest
 factory-boy==3.2.1
     # via
     #   -r requirements/base.in
     #   -r requirements/test.in
-faker==14.2.0
+faker==18.7.0
     # via factory-boy
-filelock==3.8.0
+filelock==3.12.0
     # via snowflake-connector-python
 flaky==3.7.0
     # via -r requirements/test.in
 freezegun==1.2.2
     # via -r requirements/test.in
-future==0.18.2
+future==0.18.3
     # via pyjwkest
 idna==3.4
     # via
     #   requests
     #   snowflake-connector-python
-iniconfig==1.1.1
+iniconfig==2.0.0
     # via pytest
 interchange==2021.0.4
     # via py2neo
 jmespath==1.0.1
     # via
     #   boto3
     #   botocore
 kombu==4.6.11
     # via celery
-mock==4.0.3
+mock==5.0.2
     # via -r requirements/test.in
 monotonic==1.6
     # via py2neo
-newrelic==8.1.0.180
+newrelic==8.8.0
     # via edx-django-utils
 oscrypto==1.3.0
     # via snowflake-connector-python
-packaging==21.3
+packaging==23.1
     # via
     #   py2neo
     #   pytest
+    #   snowflake-connector-python
 pansi==2020.7.3
     # via py2neo
-paramiko==2.11.0
+paramiko==3.1.0
     # via -r requirements/reporting.in
-pbr==5.10.0
+pbr==5.11.1
     # via stevedore
-pgpy==0.5.4
+pgpy==0.6.0
     # via -r requirements/reporting.in
 pluggy==1.0.0
     # via pytest
-psutil==5.9.2
+psutil==5.9.5
     # via edx-django-utils
-py==1.11.0
-    # via pytest
 py2neo==2021.2.3
     # via -r requirements/reporting.in
-pyasn1==0.4.8
+pyasn1==0.5.0
     # via
     #   pgpy
     #   rsa
 pycparser==2.21
     # via cffi
-pycryptodomex==3.15.0
+pycryptodomex==3.17
     # via
     #   pyjwkest
     #   snowflake-connector-python
-pygments==2.13.0
+pygments==2.15.1
     # via py2neo
 pyjwkest==1.4.2
     # via edx-drf-extensions
-pyjwt[crypto]==2.4.0
+pyjwt[crypto]==2.7.0
     # via
     #   drf-jwt
     #   edx-drf-extensions
     #   edx-rest-api-client
     #   snowflake-connector-python
 pyminizip==0.2.6
     # via -r requirements/reporting.in
-pymongo==3.12.3
+pymongo==3.13.0
     # via edx-opaque-keys
 pynacl==1.5.0
     # via
     #   edx-django-utils
     #   paramiko
-pyopenssl==22.0.0
+pyopenssl==23.1.1
     # via snowflake-connector-python
-pyparsing==3.0.9
-    # via packaging
-pytest==7.1.3
+pytest==7.3.1
     # via
     #   pytest-cov
     #   pytest-django
-pytest-cov==3.0.0
+pytest-cov==4.0.0
     # via -r requirements/test.in
 pytest-django==4.5.2
     # via -r requirements/test.in
 python-dateutil==2.8.2
     # via
     #   botocore
     #   edx-drf-extensions
     #   faker
     #   freezegun
     #   vertica-python
-pytz==2022.2.1
+pytz==2023.3
     # via
     #   celery
     #   django
     #   djangorestframework
     #   interchange
     #   snowflake-connector-python
 pyyaml==5.4.1
-    # via awscli
-requests==2.28.1
+    # via
+    #   awscli
+    #   responses
+requests==2.30.0
     # via
     #   -r requirements/base.in
     #   edx-drf-extensions
     #   edx-rest-api-client
     #   pyjwkest
     #   responses
     #   slumber
     #   snowflake-connector-python
-responses==0.21.0
+responses==0.23.1
     # via -r requirements/test.in
 rsa==4.7.2
     # via awscli
 rules==3.3
     # via -r requirements/base.in
-s3transfer==0.6.0
+s3transfer==0.6.1
     # via
     #   awscli
     #   boto3
 semantic-version==2.10.0
     # via edx-drf-extensions
 six==1.16.0
     # via
     #   edx-drf-extensions
     #   edx-rbac
     #   interchange
     #   pansi
-    #   paramiko
-    #   pgpy
     #   py2neo
     #   pyjwkest
     #   python-dateutil
     #   vertica-python
 slumber==0.7.1
     # via edx-rest-api-client
-snowflake-connector-python==2.7.12
+snowflake-connector-python==3.0.3
     # via -r requirements/reporting.in
-sqlparse==0.4.2
+sqlparse==0.4.4
     # via django
-stevedore==4.0.0
+stevedore==5.1.0
     # via
     #   edx-django-utils
     #   edx-opaque-keys
-testfixtures==7.0.0
+testfixtures==7.1.0
     # via -r requirements/test.in
 tomli==2.0.1
     # via
     #   coverage
     #   pytest
-typing-extensions==4.3.0
+types-pyyaml==6.0.12.9
+    # via responses
+typing-extensions==4.5.0
     # via snowflake-connector-python
 unicodecsv==0.14.1
     # via -r requirements/reporting.in
-urllib3==1.26.12
+urllib3==1.26.15
     # via
     #   botocore
     #   py2neo
     #   requests
     #   responses
     #   snowflake-connector-python
-vertica-python==1.1.1
+vertica-python==1.3.2
     # via -r requirements/reporting.in
 vine==1.3.0
     # via
     #   amqp
     #   celery
-
-# The following packages are considered to be unsafe in a requirements file:
-# setuptools
```

### Comparing `edx-enterprise-data-4.6.4/requirements/test-reporting.txt` & `edx-enterprise-data-4.6.5/requirements/test-reporting.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 #
-# This file is autogenerated by pip-compile with python 3.8
-# To update, run:
+# This file is autogenerated by pip-compile with Python 3.8
+# by the following command:
 #
 #    make upgrade
 #
 amqp==2.6.1
     # via kombu
 asn1crypto==1.5.1
     # via
     #   oscrypto
     #   snowflake-connector-python
 atomicwrites==1.4.1
     # via pytest
-attrs==22.1.0
+attrs==23.1.0
     # via pytest
-awscli==1.25.74
+awscli==1.27.134
     # via -r requirements/reporting.in
-bcrypt==4.0.0
+bcrypt==4.0.1
     # via paramiko
 billiard==3.6.4.0
     # via celery
-boto3==1.24.73
+boto3==1.26.134
     # via -r requirements/reporting.in
-botocore==1.27.73
+botocore==1.29.134
     # via
     #   awscli
     #   boto3
     #   s3transfer
 celery==4.4.7
     # via -r requirements/reporting.in
-certifi==2022.9.14
+certifi==2023.5.7
     # via
     #   py2neo
     #   requests
     #   snowflake-connector-python
 cffi==1.15.1
     # via
     #   cryptography
@@ -41,32 +41,32 @@
     #   snowflake-connector-python
 charset-normalizer==2.1.1
     # via
     #   requests
     #   snowflake-connector-python
 colorama==0.4.4
     # via awscli
-coverage==6.4.4
+coverage==7.2.5
     # via pytest-cov
-cryptography==36.0.2
+cryptography==40.0.2
     # via
     #   -r requirements/reporting.in
     #   paramiko
     #   pgpy
     #   pyopenssl
     #   snowflake-connector-python
 ddt==1.1.2
     # via
     #   -c requirements/constraints.txt
     #   -r requirements/test-reporting.in
 distlib==0.3.6
     # via virtualenv
 docutils==0.16
     # via awscli
-filelock==3.8.0
+filelock==3.12.0
     # via
     #   snowflake-connector-python
     #   tox
     #   virtualenv
 idna==3.4
     # via
     #   requests
@@ -79,130 +79,132 @@
     #   botocore
 kombu==4.6.11
     # via celery
 mock==2.0.0
     # via -r requirements/test-reporting.in
 monotonic==1.6
     # via py2neo
-more-itertools==8.14.0
+more-itertools==9.1.0
     # via pytest
 oscrypto==1.3.0
     # via snowflake-connector-python
-packaging==21.3
+packaging==23.1
     # via
     #   py2neo
+    #   snowflake-connector-python
     #   tox
 pansi==2020.7.3
     # via py2neo
-paramiko==2.11.0
+paramiko==3.1.0
     # via -r requirements/reporting.in
-pbr==5.10.0
+pbr==5.11.1
     # via mock
-pgpy==0.5.4
+pgpy==0.6.0
     # via -r requirements/reporting.in
-platformdirs==2.5.2
+platformdirs==3.5.1
     # via virtualenv
 pluggy==1.0.0
     # via
     #   pytest
     #   tox
 py==1.11.0
     # via
     #   pytest
     #   tox
 py2neo==2021.2.3
     # via -r requirements/reporting.in
-pyasn1==0.4.8
+pyasn1==0.5.0
     # via
     #   pgpy
     #   rsa
 pycparser==2.21
     # via cffi
-pycryptodomex==3.15.0
+pycryptodomex==3.17
     # via snowflake-connector-python
-pygments==2.13.0
+pygments==2.15.1
     # via py2neo
-pyjwt==2.4.0
+pyjwt==2.7.0
     # via snowflake-connector-python
 pyminizip==0.2.6
     # via -r requirements/reporting.in
 pynacl==1.5.0
     # via paramiko
-pyopenssl==22.0.0
+pyopenssl==23.1.1
     # via snowflake-connector-python
-pyparsing==3.0.9
-    # via packaging
 pytest==3.7.1
     # via
     #   -r requirements/test-reporting.in
     #   pytest-cov
 pytest-cov==2.5.1
     # via -r requirements/test-reporting.in
 python-dateutil==2.8.2
     # via
     #   botocore
     #   vertica-python
-pytz==2022.2.1
+pytz==2023.3
     # via
     #   celery
     #   interchange
     #   snowflake-connector-python
 pyyaml==5.4.1
-    # via awscli
-requests==2.28.1
+    # via
+    #   awscli
+    #   responses
+requests==2.30.0
     # via
     #   responses
     #   snowflake-connector-python
-responses==0.21.0
+responses==0.23.1
     # via -r requirements/test-reporting.in
 rsa==4.7.2
     # via awscli
-s3transfer==0.6.0
+s3transfer==0.6.1
     # via
     #   awscli
     #   boto3
 six==1.16.0
     # via
     #   interchange
     #   mock
     #   pansi
-    #   paramiko
-    #   pgpy
     #   py2neo
     #   pytest
     #   python-dateutil
     #   tox
     #   vertica-python
-snowflake-connector-python==2.7.12
+snowflake-connector-python==3.0.3
     # via -r requirements/reporting.in
 tomli==2.0.1
     # via tox
-tox==3.26.0
+tox==3.28.0
     # via
+    #   -c requirements/constraints.txt
     #   -r requirements/test-reporting.in
     #   tox-battery
 tox-battery==0.5.2
     # via
     #   -c requirements/constraints.txt
     #   -r requirements/test-reporting.in
-typing-extensions==4.3.0
+types-pyyaml==6.0.12.9
+    # via responses
+typing-extensions==4.5.0
     # via snowflake-connector-python
 unicodecsv==0.14.1
     # via -r requirements/reporting.in
-urllib3==1.26.12
+urllib3==1.26.15
     # via
     #   botocore
     #   py2neo
     #   requests
     #   responses
     #   snowflake-connector-python
-vertica-python==1.1.1
+vertica-python==1.3.2
     # via -r requirements/reporting.in
 vine==1.3.0
     # via
     #   amqp
     #   celery
-virtualenv==20.16.5
+virtualenv==20.23.0
     # via tox
 
 # The following packages are considered to be unsafe in a requirements file:
 # setuptools
```

### Comparing `edx-enterprise-data-4.6.4/requirements/test.txt` & `edx-enterprise-data-4.6.5/requirements/test-master.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,39 +1,37 @@
 #
-# This file is autogenerated by pip-compile with python 3.8
-# To update, run:
+# This file is autogenerated by pip-compile with Python 3.8
+# by the following command:
 #
 #    make upgrade
 #
 amqp==2.6.1
     # via kombu
-asgiref==3.5.2
+asgiref==3.6.0
     # via django
 asn1crypto==1.5.1
     # via
     #   oscrypto
     #   snowflake-connector-python
-attrs==22.1.0
-    # via pytest
-awscli==1.25.74
+awscli==1.27.134
     # via -r requirements/reporting.in
-bcrypt==4.0.0
+bcrypt==4.0.1
     # via paramiko
 billiard==3.6.4.0
     # via celery
-boto3==1.24.73
+boto3==1.26.134
     # via -r requirements/reporting.in
-botocore==1.27.73
+botocore==1.29.134
     # via
     #   awscli
     #   boto3
     #   s3transfer
 celery==4.4.7
     # via -r requirements/reporting.in
-certifi==2022.9.14
+certifi==2023.5.7
     # via
     #   py2neo
     #   requests
     #   snowflake-connector-python
 cffi==1.15.1
     # via
     #   cryptography
@@ -43,33 +41,33 @@
     # via
     #   requests
     #   snowflake-connector-python
 click==8.1.3
     # via edx-django-utils
 colorama==0.4.4
     # via awscli
-coverage[toml]==6.4.4
+coverage[toml]==7.2.5
     # via pytest-cov
-cryptography==36.0.2
+cryptography==40.0.2
     # via
     #   -r requirements/reporting.in
     #   django-fernet-fields
     #   paramiko
     #   pgpy
     #   pyjwt
     #   pyopenssl
     #   snowflake-connector-python
 ddt==1.3.1
     # via
     #   -c requirements/constraints.txt
     #   -r requirements/test.in
-django==3.2.15
     # via
     #   -c requirements/constraints.txt
     #   -r requirements/base.in
+    #   -r requirements/test-master.in
     #   django-crum
     #   django-fernet-fields
     #   django-filter
     #   django-model-utils
     #   djangorestframework
     #   drf-jwt
     #   edx-django-utils
@@ -77,224 +75,224 @@
     #   edx-rbac
 django-crum==0.7.9
     # via
     #   edx-django-utils
     #   edx-rbac
 django-fernet-fields==0.6
     # via -r requirements/base.in
-django-filter==22.1
+django-filter==23.2
     # via -r requirements/base.in
-django-model-utils==4.2.0
+django-model-utils==4.3.1
     # via
     #   -r requirements/base.in
     #   -r requirements/test.in
     #   edx-rbac
 django-waffle==3.0.0
     # via
     #   edx-django-utils
     #   edx-drf-extensions
-djangorestframework==3.13.1
+djangorestframework==3.14.0
     # via
+    #   -r requirements/test-master.in
     #   drf-jwt
     #   edx-drf-extensions
 docutils==0.16
     # via awscli
 drf-jwt==1.19.2
     # via edx-drf-extensions
-edx-django-utils==5.0.1
+edx-django-utils==5.4.0
     # via
     #   -r requirements/base.in
     #   edx-drf-extensions
     #   edx-rest-api-client
-edx-drf-extensions==8.3.1
+edx-drf-extensions==8.7.0
     # via
     #   -r requirements/base.in
+    #   -r requirements/test-master.in
     #   edx-rbac
 edx-opaque-keys==2.3.0
     # via
     #   -r requirements/base.in
     #   edx-drf-extensions
 edx-rbac==1.7.0
     # via -r requirements/base.in
 edx-rest-api-client==5.5.0
     # via -r requirements/base.in
+exceptiongroup==1.1.1
+    # via pytest
 factory-boy==3.2.1
     # via
     #   -r requirements/base.in
     #   -r requirements/test.in
-faker==14.2.0
+faker==18.7.0
     # via factory-boy
-filelock==3.8.0
+filelock==3.12.0
     # via snowflake-connector-python
 flaky==3.7.0
     # via -r requirements/test.in
 freezegun==1.2.2
     # via -r requirements/test.in
-future==0.18.2
+future==0.18.3
     # via pyjwkest
 idna==3.4
     # via
     #   requests
     #   snowflake-connector-python
-iniconfig==1.1.1
+iniconfig==2.0.0
     # via pytest
 interchange==2021.0.4
     # via py2neo
 jmespath==1.0.1
     # via
     #   boto3
     #   botocore
 kombu==4.6.11
     # via celery
-mock==4.0.3
+mock==5.0.2
     # via -r requirements/test.in
 monotonic==1.6
     # via py2neo
-newrelic==8.1.0.180
+newrelic==8.8.0
     # via edx-django-utils
 oscrypto==1.3.0
     # via snowflake-connector-python
-packaging==21.3
+packaging==23.1
     # via
     #   py2neo
     #   pytest
+    #   snowflake-connector-python
 pansi==2020.7.3
     # via py2neo
-paramiko==2.11.0
+paramiko==3.1.0
     # via -r requirements/reporting.in
-pbr==5.10.0
+pbr==5.11.1
     # via stevedore
-pgpy==0.5.4
+pgpy==0.6.0
     # via -r requirements/reporting.in
 pluggy==1.0.0
     # via pytest
-psutil==5.9.2
+psutil==5.9.5
     # via edx-django-utils
-py==1.11.0
-    # via pytest
 py2neo==2021.2.3
     # via -r requirements/reporting.in
-pyasn1==0.4.8
+pyasn1==0.5.0
     # via
     #   pgpy
     #   rsa
 pycparser==2.21
     # via cffi
-pycryptodomex==3.15.0
+pycryptodomex==3.17
     # via
     #   pyjwkest
     #   snowflake-connector-python
-pygments==2.13.0
+pygments==2.15.1
     # via py2neo
 pyjwkest==1.4.2
     # via edx-drf-extensions
-pyjwt[crypto]==2.4.0
+pyjwt[crypto]==2.7.0
     # via
     #   drf-jwt
     #   edx-drf-extensions
     #   edx-rest-api-client
     #   snowflake-connector-python
 pyminizip==0.2.6
     # via -r requirements/reporting.in
-pymongo==3.12.3
+pymongo==3.13.0
     # via edx-opaque-keys
 pynacl==1.5.0
     # via
     #   edx-django-utils
     #   paramiko
-pyopenssl==22.0.0
+pyopenssl==23.1.1
     # via snowflake-connector-python
-pyparsing==3.0.9
-    # via packaging
-pytest==7.1.3
+pytest==7.3.1
     # via
     #   pytest-cov
     #   pytest-django
-pytest-cov==3.0.0
+pytest-cov==4.0.0
     # via -r requirements/test.in
 pytest-django==4.5.2
     # via -r requirements/test.in
 python-dateutil==2.8.2
     # via
     #   botocore
     #   edx-drf-extensions
     #   faker
     #   freezegun
     #   vertica-python
-pytz==2022.2.1
+pytz==2023.3
     # via
     #   celery
     #   django
     #   djangorestframework
     #   interchange
     #   snowflake-connector-python
 pyyaml==5.4.1
-    # via awscli
-requests==2.28.1
+    # via
+    #   awscli
+    #   responses
+requests==2.30.0
     # via
     #   -r requirements/base.in
     #   edx-drf-extensions
     #   edx-rest-api-client
     #   pyjwkest
     #   responses
     #   slumber
     #   snowflake-connector-python
-responses==0.21.0
+responses==0.23.1
     # via -r requirements/test.in
 rsa==4.7.2
     # via awscli
 rules==3.3
     # via -r requirements/base.in
-s3transfer==0.6.0
+s3transfer==0.6.1
     # via
     #   awscli
     #   boto3
 semantic-version==2.10.0
     # via edx-drf-extensions
 six==1.16.0
     # via
     #   edx-drf-extensions
     #   edx-rbac
     #   interchange
     #   pansi
-    #   paramiko
-    #   pgpy
     #   py2neo
     #   pyjwkest
     #   python-dateutil
     #   vertica-python
 slumber==0.7.1
     # via edx-rest-api-client
-snowflake-connector-python==2.7.12
+snowflake-connector-python==3.0.3
     # via -r requirements/reporting.in
-sqlparse==0.4.2
+sqlparse==0.4.4
     # via django
-stevedore==4.0.0
+stevedore==5.1.0
     # via
     #   edx-django-utils
     #   edx-opaque-keys
-testfixtures==7.0.0
+testfixtures==7.1.0
     # via -r requirements/test.in
 tomli==2.0.1
     # via
     #   coverage
     #   pytest
-typing-extensions==4.3.0
+types-pyyaml==6.0.12.9
+    # via responses
+typing-extensions==4.5.0
     # via snowflake-connector-python
 unicodecsv==0.14.1
     # via -r requirements/reporting.in
-urllib3==1.26.12
+urllib3==1.26.15
     # via
     #   botocore
     #   py2neo
     #   requests
     #   responses
     #   snowflake-connector-python
-vertica-python==1.1.1
+vertica-python==1.3.2
     # via -r requirements/reporting.in
 vine==1.3.0
     # via
     #   amqp
     #   celery
-
-# The following packages are considered to be unsafe in a requirements file:
-# setuptools
```

