# Comparing `tmp/google-cloud-bigtable-2.8.1.tar.gz` & `tmp/google-cloud-bigtable-2.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-cloud-bigtable-2.8.1.tar", last modified: Thu Apr  7 22:36:57 2022, max compression
+gzip compressed data, was "google-cloud-bigtable-2.9.0.tar", last modified: Thu Apr 14 15:53:10 2022, max compression
```

## Comparing `google-cloud-bigtable-2.8.1.tar` & `google-cloud-bigtable-2.9.0.tar`

### file list

```diff
@@ -1,130 +1,130 @@
-drwxr-sr-x   0 root         (0)     1003        0 2022-04-07 22:36:57.070126 google-cloud-bigtable-2.8.1/
--rw-rw-r--   0 root         (0)     1003    11358 2022-04-07 22:34:22.000000 google-cloud-bigtable-2.8.1/LICENSE
--rw-rw-r--   0 root         (0)     1003      860 2022-04-07 22:34:22.000000 google-cloud-bigtable-2.8.1/MANIFEST.in
--rw-r--r--   0 root         (0)     1003     4406 2022-04-07 22:36:57.070126 google-cloud-bigtable-2.8.1/PKG-INFO
--rw-rw-r--   0 root         (0)     1003     3511 2022-04-07 22:34:22.000000 google-cloud-bigtable-2.8.1/README.rst
-drwxr-sr-x   0 root         (0)     1003        0 2022-04-07 22:36:57.050126 google-cloud-bigtable-2.8.1/google/
--rw-rw-r--   0 root         (0)     1003      106 2022-04-07 22:34:22.000000 google-cloud-bigtable-2.8.1/google/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-04-07 22:36:57.050126 google-cloud-bigtable-2.8.1/google/cloud/
--rw-rw-r--   0 root         (0)     1003      106 2022-04-07 22:34:22.000000 google-cloud-bigtable-2.8.1/google/cloud/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-04-07 22:36:57.054126 google-cloud-bigtable-2.8.1/google/cloud/bigtable/
--rw-rw-r--   0 root         (0)     1003      935 2022-04-07 22:34:22.000000 google-cloud-bigtable-2.8.1/google/cloud/bigtable/__init__.py
--rw-rw-r--   0 root         (0)     1003    13172 2022-04-07 22:34:22.000000 google-cloud-bigtable-2.8.1/google/cloud/bigtable/app_profile.py
--rw-rw-r--   0 root         (0)     1003    17578 2022-04-07 22:34:22.000000 google-cloud-bigtable-2.8.1/google/cloud/bigtable/backup.py
--rw-rw-r--   0 root         (0)     1003     5553 2022-04-07 22:34:22.000000 google-cloud-bigtable-2.8.1/google/cloud/bigtable/batcher.py
--rw-rw-r--   0 root         (0)     1003    19705 2022-04-07 22:34:22.000000 google-cloud-bigtable-2.8.1/google/cloud/bigtable/client.py
--rw-rw-r--   0 root         (0)     1003    20527 2022-04-07 22:34:22.000000 google-cloud-bigtable-2.8.1/google/cloud/bigtable/cluster.py
--rw-rw-r--   0 root         (0)     1003    11542 2022-04-07 22:34:22.000000 google-cloud-bigtable-2.8.1/google/cloud/bigtable/column_family.py
--rw-rw-r--   0 root         (0)     1003     2140 2022-04-07 22:34:22.000000 google-cloud-bigtable-2.8.1/google/cloud/bigtable/encryption_info.py
--rw-rw-r--   0 root         (0)     1003     9424 2022-04-07 22:34:22.000000 google-cloud-bigtable-2.8.1/google/cloud/bigtable/enums.py
--rw-rw-r--   0 root         (0)     1003     1807 2022-04-07 22:34:22.000000 google-cloud-bigtable-2.8.1/google/cloud/bigtable/error.py
--rw-rw-r--   0 root         (0)     1003    29601 2022-04-07 22:34:22.000000 google-cloud-bigtable-2.8.1/google/cloud/bigtable/instance.py
--rw-rw-r--   0 root         (0)     1003     9010 2022-04-07 22:34:22.000000 google-cloud-bigtable-2.8.1/google/cloud/bigtable/policy.py
--rw-rw-r--   0 root         (0)     1003       84 2022-04-07 22:34:22.000000 google-cloud-bigtable-2.8.1/google/cloud/bigtable/py.typed
--rw-rw-r--   0 root         (0)     1003    37674 2022-04-07 22:34:22.000000 google-cloud-bigtable-2.8.1/google/cloud/bigtable/row.py
--rw-rw-r--   0 root         (0)     1003    25830 2022-04-07 22:34:22.000000 google-cloud-bigtable-2.8.1/google/cloud/bigtable/row_data.py
--rw-rw-r--   0 root         (0)     1003    28347 2022-04-07 22:34:22.000000 google-cloud-bigtable-2.8.1/google/cloud/bigtable/row_filters.py
--rw-rw-r--   0 root         (0)     1003     7390 2022-04-07 22:34:22.000000 google-cloud-bigtable-2.8.1/google/cloud/bigtable/row_set.py
--rw-rw-r--   0 root         (0)     1003    53684 2022-04-07 22:34:22.000000 google-cloud-bigtable-2.8.1/google/cloud/bigtable/table.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-04-07 22:36:57.054126 google-cloud-bigtable-2.8.1/google/cloud/bigtable_admin_v2/
--rw-rw-r--   0 root         (0)     1003     7176 2022-04-07 22:34:22.000000 google-cloud-bigtable-2.8.1/google/cloud/bigtable_admin_v2/__init__.py
--rw-rw-r--   0 root         (0)     1003    11554 2022-04-07 22:34:22.000000 google-cloud-bigtable-2.8.1/google/cloud/bigtable_admin_v2/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003       88 2022-04-07 22:34:22.000000 google-cloud-bigtable-2.8.1/google/cloud/bigtable_admin_v2/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2022-04-07 22:36:57.054126 google-cloud-bigtable-2.8.1/google/cloud/bigtable_admin_v2/services/
--rw-rw-r--   0 root         (0)     1003      600 2022-04-07 22:34:22.000000 google-cloud-bigtable-2.8.1/google/cloud/bigtable_admin_v2/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-04-07 22:36:57.054126 google-cloud-bigtable-2.8.1/google/cloud/bigtable_admin_v2/services/bigtable_instance_admin/
--rw-rw-r--   0 root         (0)     1003      797 2022-04-07 22:34:22.000000 google-cloud-bigtable-2.8.1/google/cloud/bigtable_admin_v2/services/bigtable_instance_admin/__init__.py
--rw-rw-r--   0 root         (0)     1003    96216 2022-04-07 22:34:22.000000 google-cloud-bigtable-2.8.1/google/cloud/bigtable_admin_v2/services/bigtable_instance_admin/async_client.py
--rw-rw-r--   0 root         (0)     1003   106002 2022-04-07 22:34:22.000000 google-cloud-bigtable-2.8.1/google/cloud/bigtable_admin_v2/services/bigtable_instance_admin/client.py
--rw-rw-r--   0 root         (0)     1003    11323 2022-04-07 22:34:22.000000 google-cloud-bigtable-2.8.1/google/cloud/bigtable_admin_v2/services/bigtable_instance_admin/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-04-07 22:36:57.058126 google-cloud-bigtable-2.8.1/google/cloud/bigtable_admin_v2/services/bigtable_instance_admin/transports/
--rw-rw-r--   0 root         (0)     1003     1265 2022-04-07 22:34:22.000000 google-cloud-bigtable-2.8.1/google/cloud/bigtable_admin_v2/services/bigtable_instance_admin/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003    21383 2022-04-07 22:34:22.000000 google-cloud-bigtable-2.8.1/google/cloud/bigtable_admin_v2/services/bigtable_instance_admin/transports/base.py
--rw-rw-r--   0 root         (0)     1003    37696 2022-04-07 22:34:22.000000 google-cloud-bigtable-2.8.1/google/cloud/bigtable_admin_v2/services/bigtable_instance_admin/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    38638 2022-04-07 22:34:22.000000 google-cloud-bigtable-2.8.1/google/cloud/bigtable_admin_v2/services/bigtable_instance_admin/transports/grpc_asyncio.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-04-07 22:36:57.058126 google-cloud-bigtable-2.8.1/google/cloud/bigtable_admin_v2/services/bigtable_table_admin/
--rw-rw-r--   0 root         (0)     1003      785 2022-04-07 22:34:22.000000 google-cloud-bigtable-2.8.1/google/cloud/bigtable_admin_v2/services/bigtable_table_admin/__init__.py
--rw-rw-r--   0 root         (0)     1003   104108 2022-04-07 22:34:22.000000 google-cloud-bigtable-2.8.1/google/cloud/bigtable_admin_v2/services/bigtable_table_admin/async_client.py
--rw-rw-r--   0 root         (0)     1003   115874 2022-04-07 22:34:22.000000 google-cloud-bigtable-2.8.1/google/cloud/bigtable_admin_v2/services/bigtable_table_admin/client.py
--rw-rw-r--   0 root         (0)     1003    15999 2022-04-07 22:34:22.000000 google-cloud-bigtable-2.8.1/google/cloud/bigtable_admin_v2/services/bigtable_table_admin/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-04-07 22:36:57.058126 google-cloud-bigtable-2.8.1/google/cloud/bigtable_admin_v2/services/bigtable_table_admin/transports/
--rw-rw-r--   0 root         (0)     1003     1238 2022-04-07 22:34:22.000000 google-cloud-bigtable-2.8.1/google/cloud/bigtable_admin_v2/services/bigtable_table_admin/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003    20118 2022-04-07 22:34:22.000000 google-cloud-bigtable-2.8.1/google/cloud/bigtable_admin_v2/services/bigtable_table_admin/transports/base.py
--rw-rw-r--   0 root         (0)     1003    40879 2022-04-07 22:34:22.000000 google-cloud-bigtable-2.8.1/google/cloud/bigtable_admin_v2/services/bigtable_table_admin/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    41793 2022-04-07 22:34:22.000000 google-cloud-bigtable-2.8.1/google/cloud/bigtable_admin_v2/services/bigtable_table_admin/transports/grpc_asyncio.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-04-07 22:36:57.058126 google-cloud-bigtable-2.8.1/google/cloud/bigtable_admin_v2/types/
--rw-rw-r--   0 root         (0)     1003     4525 2022-04-07 22:34:22.000000 google-cloud-bigtable-2.8.1/google/cloud/bigtable_admin_v2/types/__init__.py
--rw-rw-r--   0 root         (0)     1003    25316 2022-04-07 22:34:22.000000 google-cloud-bigtable-2.8.1/google/cloud/bigtable_admin_v2/types/bigtable_instance_admin.py
--rw-rw-r--   0 root         (0)     1003    39244 2022-04-07 22:34:22.000000 google-cloud-bigtable-2.8.1/google/cloud/bigtable_admin_v2/types/bigtable_table_admin.py
--rw-rw-r--   0 root         (0)     1003     1918 2022-04-07 22:34:22.000000 google-cloud-bigtable-2.8.1/google/cloud/bigtable_admin_v2/types/common.py
--rw-rw-r--   0 root         (0)     1003    16134 2022-04-07 22:34:22.000000 google-cloud-bigtable-2.8.1/google/cloud/bigtable_admin_v2/types/instance.py
--rw-rw-r--   0 root         (0)     1003    18420 2022-04-07 22:34:22.000000 google-cloud-bigtable-2.8.1/google/cloud/bigtable_admin_v2/types/table.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-04-07 22:36:57.062126 google-cloud-bigtable-2.8.1/google/cloud/bigtable_v2/
--rw-rw-r--   0 root         (0)     1003     2439 2022-04-07 22:34:22.000000 google-cloud-bigtable-2.8.1/google/cloud/bigtable_v2/__init__.py
--rw-rw-r--   0 root         (0)     1003     2223 2022-04-07 22:34:22.000000 google-cloud-bigtable-2.8.1/google/cloud/bigtable_v2/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003       82 2022-04-07 22:34:22.000000 google-cloud-bigtable-2.8.1/google/cloud/bigtable_v2/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2022-04-07 22:36:57.062126 google-cloud-bigtable-2.8.1/google/cloud/bigtable_v2/services/
--rw-rw-r--   0 root         (0)     1003      600 2022-04-07 22:34:22.000000 google-cloud-bigtable-2.8.1/google/cloud/bigtable_v2/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-04-07 22:36:57.062126 google-cloud-bigtable-2.8.1/google/cloud/bigtable_v2/services/bigtable/
--rw-rw-r--   0 root         (0)     1003      745 2022-04-07 22:34:22.000000 google-cloud-bigtable-2.8.1/google/cloud/bigtable_v2/services/bigtable/__init__.py
--rw-rw-r--   0 root         (0)     1003    41946 2022-04-07 22:34:22.000000 google-cloud-bigtable-2.8.1/google/cloud/bigtable_v2/services/bigtable/async_client.py
--rw-rw-r--   0 root         (0)     1003    54423 2022-04-07 22:34:22.000000 google-cloud-bigtable-2.8.1/google/cloud/bigtable_v2/services/bigtable/client.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-04-07 22:36:57.062126 google-cloud-bigtable-2.8.1/google/cloud/bigtable_v2/services/bigtable/transports/
--rw-rw-r--   0 root         (0)     1003     1140 2022-04-07 22:34:22.000000 google-cloud-bigtable-2.8.1/google/cloud/bigtable_v2/services/bigtable/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     9173 2022-04-07 22:34:22.000000 google-cloud-bigtable-2.8.1/google/cloud/bigtable_v2/services/bigtable/transports/base.py
--rw-rw-r--   0 root         (0)     1003    19326 2022-04-07 22:34:22.000000 google-cloud-bigtable-2.8.1/google/cloud/bigtable_v2/services/bigtable/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    19780 2022-04-07 22:34:22.000000 google-cloud-bigtable-2.8.1/google/cloud/bigtable_v2/services/bigtable/transports/grpc_asyncio.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-04-07 22:36:57.062126 google-cloud-bigtable-2.8.1/google/cloud/bigtable_v2/types/
--rw-rw-r--   0 root         (0)     1003     1789 2022-04-07 22:34:22.000000 google-cloud-bigtable-2.8.1/google/cloud/bigtable_v2/types/__init__.py
--rw-rw-r--   0 root         (0)     1003    20928 2022-04-07 22:34:22.000000 google-cloud-bigtable-2.8.1/google/cloud/bigtable_v2/types/bigtable.py
--rw-rw-r--   0 root         (0)     1003    36953 2022-04-07 22:34:22.000000 google-cloud-bigtable-2.8.1/google/cloud/bigtable_v2/types/data.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-04-07 22:36:57.062126 google-cloud-bigtable-2.8.1/google_cloud_bigtable.egg-info/
--rw-r--r--   0 root         (0)     1003     4406 2022-04-07 22:36:56.000000 google-cloud-bigtable-2.8.1/google_cloud_bigtable.egg-info/PKG-INFO
--rw-r--r--   0 root         (0)     1003     4581 2022-04-07 22:36:56.000000 google-cloud-bigtable-2.8.1/google_cloud_bigtable.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0)     1003        1 2022-04-07 22:36:56.000000 google-cloud-bigtable-2.8.1/google_cloud_bigtable.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0)     1003       20 2022-04-07 22:36:56.000000 google-cloud-bigtable-2.8.1/google_cloud_bigtable.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0)     1003        1 2022-04-07 22:36:56.000000 google-cloud-bigtable-2.8.1/google_cloud_bigtable.egg-info/not-zip-safe
--rw-r--r--   0 root         (0)     1003      186 2022-04-07 22:36:56.000000 google-cloud-bigtable-2.8.1/google_cloud_bigtable.egg-info/requires.txt
--rw-r--r--   0 root         (0)     1003        7 2022-04-07 22:36:56.000000 google-cloud-bigtable-2.8.1/google_cloud_bigtable.egg-info/top_level.txt
-drwxr-sr-x   0 root         (0)     1003        0 2022-04-07 22:36:57.066126 google-cloud-bigtable-2.8.1/scripts/
--rw-rw-r--   0 root         (0)     1003     8432 2022-04-07 22:34:22.000000 google-cloud-bigtable-2.8.1/scripts/fixup_bigtable_admin_v2_keywords.py
--rw-rw-r--   0 root         (0)     1003     6488 2022-04-07 22:34:22.000000 google-cloud-bigtable-2.8.1/scripts/fixup_bigtable_v2_keywords.py
--rw-rw-r--   0 root         (0)     1003       67 2022-04-07 22:36:57.070126 google-cloud-bigtable-2.8.1/setup.cfg
--rw-rw-r--   0 root         (0)     1003     3312 2022-04-07 22:34:22.000000 google-cloud-bigtable-2.8.1/setup.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-04-07 22:36:57.066126 google-cloud-bigtable-2.8.1/tests/
--rw-rw-r--   0 root         (0)     1003      600 2022-04-07 22:34:22.000000 google-cloud-bigtable-2.8.1/tests/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-04-07 22:36:57.066126 google-cloud-bigtable-2.8.1/tests/system/
--rw-rw-r--   0 root         (0)     1003      600 2022-04-07 22:34:22.000000 google-cloud-bigtable-2.8.1/tests/system/__init__.py
--rw-rw-r--   0 root         (0)     1003     1475 2022-04-07 22:34:22.000000 google-cloud-bigtable-2.8.1/tests/system/_helpers.py
--rw-rw-r--   0 root         (0)     1003     5267 2022-04-07 22:34:22.000000 google-cloud-bigtable-2.8.1/tests/system/conftest.py
--rw-rw-r--   0 root         (0)     1003    12486 2022-04-07 22:34:22.000000 google-cloud-bigtable-2.8.1/tests/system/test_data_api.py
--rw-rw-r--   0 root         (0)     1003    26318 2022-04-07 22:34:22.000000 google-cloud-bigtable-2.8.1/tests/system/test_instance_admin.py
--rw-rw-r--   0 root         (0)     1003    12038 2022-04-07 22:34:22.000000 google-cloud-bigtable-2.8.1/tests/system/test_table_admin.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-04-07 22:36:57.070126 google-cloud-bigtable-2.8.1/tests/unit/
--rw-rw-r--   0 root         (0)     1003      600 2022-04-07 22:34:22.000000 google-cloud-bigtable-2.8.1/tests/unit/__init__.py
--rw-rw-r--   0 root         (0)     1003     1040 2022-04-07 22:34:22.000000 google-cloud-bigtable-2.8.1/tests/unit/_testing.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-04-07 22:36:57.070126 google-cloud-bigtable-2.8.1/tests/unit/gapic/
--rw-rw-r--   0 root         (0)     1003      600 2022-04-07 22:34:22.000000 google-cloud-bigtable-2.8.1/tests/unit/gapic/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-04-07 22:36:57.070126 google-cloud-bigtable-2.8.1/tests/unit/gapic/bigtable_admin_v2/
--rw-rw-r--   0 root         (0)     1003      600 2022-04-07 22:34:22.000000 google-cloud-bigtable-2.8.1/tests/unit/gapic/bigtable_admin_v2/__init__.py
--rw-rw-r--   0 root         (0)     1003   252213 2022-04-07 22:34:22.000000 google-cloud-bigtable-2.8.1/tests/unit/gapic/bigtable_admin_v2/test_bigtable_instance_admin.py
--rw-rw-r--   0 root         (0)     1003   261325 2022-04-07 22:34:22.000000 google-cloud-bigtable-2.8.1/tests/unit/gapic/bigtable_admin_v2/test_bigtable_table_admin.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-04-07 22:36:57.070126 google-cloud-bigtable-2.8.1/tests/unit/gapic/bigtable_v2/
--rw-rw-r--   0 root         (0)     1003      600 2022-04-07 22:34:22.000000 google-cloud-bigtable-2.8.1/tests/unit/gapic/bigtable_v2/__init__.py
--rw-rw-r--   0 root         (0)     1003   113709 2022-04-07 22:34:22.000000 google-cloud-bigtable-2.8.1/tests/unit/gapic/bigtable_v2/test_bigtable.py
--rw-rw-r--   0 root         (0)     1003    36953 2022-04-07 22:34:22.000000 google-cloud-bigtable-2.8.1/tests/unit/read-rows-acceptance-test.json
--rw-rw-r--   0 root         (0)     1003    23798 2022-04-07 22:34:22.000000 google-cloud-bigtable-2.8.1/tests/unit/test_app_profile.py
--rw-rw-r--   0 root         (0)     1003    29724 2022-04-07 22:34:22.000000 google-cloud-bigtable-2.8.1/tests/unit/test_backup.py
--rw-rw-r--   0 root         (0)     1003     4350 2022-04-07 22:34:22.000000 google-cloud-bigtable-2.8.1/tests/unit/test_batcher.py
--rw-rw-r--   0 root         (0)     1003    26525 2022-04-07 22:34:22.000000 google-cloud-bigtable-2.8.1/tests/unit/test_client.py
--rw-rw-r--   0 root         (0)     1003    36981 2022-04-07 22:34:22.000000 google-cloud-bigtable-2.8.1/tests/unit/test_cluster.py
--rw-rw-r--   0 root         (0)     1003    20228 2022-04-07 22:34:22.000000 google-cloud-bigtable-2.8.1/tests/unit/test_column_family.py
--rw-rw-r--   0 root         (0)     1003     5157 2022-04-07 22:34:22.000000 google-cloud-bigtable-2.8.1/tests/unit/test_encryption_info.py
--rw-rw-r--   0 root         (0)     1003     2855 2022-04-07 22:34:22.000000 google-cloud-bigtable-2.8.1/tests/unit/test_error.py
--rw-rw-r--   0 root         (0)     1003    31903 2022-04-07 22:34:22.000000 google-cloud-bigtable-2.8.1/tests/unit/test_instance.py
--rw-rw-r--   0 root         (0)     1003     8924 2022-04-07 22:34:22.000000 google-cloud-bigtable-2.8.1/tests/unit/test_policy.py
--rw-rw-r--   0 root         (0)     1003    24763 2022-04-07 22:34:22.000000 google-cloud-bigtable-2.8.1/tests/unit/test_row.py
--rw-rw-r--   0 root         (0)     1003    47982 2022-04-07 22:34:22.000000 google-cloud-bigtable-2.8.1/tests/unit/test_row_data.py
--rw-rw-r--   0 root         (0)     1003    36325 2022-04-07 22:34:22.000000 google-cloud-bigtable-2.8.1/tests/unit/test_row_filters.py
--rw-rw-r--   0 root         (0)     1003     9379 2022-04-07 22:34:22.000000 google-cloud-bigtable-2.8.1/tests/unit/test_row_set.py
--rw-rw-r--   0 root         (0)     1003    70768 2022-04-07 22:34:22.000000 google-cloud-bigtable-2.8.1/tests/unit/test_table.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-04-14 15:53:10.064491 google-cloud-bigtable-2.9.0/
+-rw-rw-r--   0 root         (0)     1003    11358 2022-04-14 15:50:31.000000 google-cloud-bigtable-2.9.0/LICENSE
+-rw-rw-r--   0 root         (0)     1003      860 2022-04-14 15:50:31.000000 google-cloud-bigtable-2.9.0/MANIFEST.in
+-rw-r--r--   0 root         (0)     1003     4406 2022-04-14 15:53:10.064491 google-cloud-bigtable-2.9.0/PKG-INFO
+-rw-rw-r--   0 root         (0)     1003     3511 2022-04-14 15:50:31.000000 google-cloud-bigtable-2.9.0/README.rst
+drwxr-sr-x   0 root         (0)     1003        0 2022-04-14 15:53:10.040479 google-cloud-bigtable-2.9.0/google/
+-rw-rw-r--   0 root         (0)     1003      106 2022-04-14 15:50:31.000000 google-cloud-bigtable-2.9.0/google/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-04-14 15:53:10.040479 google-cloud-bigtable-2.9.0/google/cloud/
+-rw-rw-r--   0 root         (0)     1003      106 2022-04-14 15:50:31.000000 google-cloud-bigtable-2.9.0/google/cloud/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-04-14 15:53:10.044481 google-cloud-bigtable-2.9.0/google/cloud/bigtable/
+-rw-rw-r--   0 root         (0)     1003      935 2022-04-14 15:50:31.000000 google-cloud-bigtable-2.9.0/google/cloud/bigtable/__init__.py
+-rw-rw-r--   0 root         (0)     1003    13885 2022-04-14 15:50:31.000000 google-cloud-bigtable-2.9.0/google/cloud/bigtable/app_profile.py
+-rw-rw-r--   0 root         (0)     1003    17578 2022-04-14 15:50:31.000000 google-cloud-bigtable-2.9.0/google/cloud/bigtable/backup.py
+-rw-rw-r--   0 root         (0)     1003     5553 2022-04-14 15:50:31.000000 google-cloud-bigtable-2.9.0/google/cloud/bigtable/batcher.py
+-rw-rw-r--   0 root         (0)     1003    19705 2022-04-14 15:50:31.000000 google-cloud-bigtable-2.9.0/google/cloud/bigtable/client.py
+-rw-rw-r--   0 root         (0)     1003    20527 2022-04-14 15:50:31.000000 google-cloud-bigtable-2.9.0/google/cloud/bigtable/cluster.py
+-rw-rw-r--   0 root         (0)     1003    11542 2022-04-14 15:50:31.000000 google-cloud-bigtable-2.9.0/google/cloud/bigtable/column_family.py
+-rw-rw-r--   0 root         (0)     1003     2140 2022-04-14 15:50:31.000000 google-cloud-bigtable-2.9.0/google/cloud/bigtable/encryption_info.py
+-rw-rw-r--   0 root         (0)     1003     9424 2022-04-14 15:50:31.000000 google-cloud-bigtable-2.9.0/google/cloud/bigtable/enums.py
+-rw-rw-r--   0 root         (0)     1003     1807 2022-04-14 15:50:31.000000 google-cloud-bigtable-2.9.0/google/cloud/bigtable/error.py
+-rw-rw-r--   0 root         (0)     1003    29966 2022-04-14 15:50:31.000000 google-cloud-bigtable-2.9.0/google/cloud/bigtable/instance.py
+-rw-rw-r--   0 root         (0)     1003     9010 2022-04-14 15:50:31.000000 google-cloud-bigtable-2.9.0/google/cloud/bigtable/policy.py
+-rw-rw-r--   0 root         (0)     1003       84 2022-04-14 15:50:31.000000 google-cloud-bigtable-2.9.0/google/cloud/bigtable/py.typed
+-rw-rw-r--   0 root         (0)     1003    37674 2022-04-14 15:50:31.000000 google-cloud-bigtable-2.9.0/google/cloud/bigtable/row.py
+-rw-rw-r--   0 root         (0)     1003    25830 2022-04-14 15:50:31.000000 google-cloud-bigtable-2.9.0/google/cloud/bigtable/row_data.py
+-rw-rw-r--   0 root         (0)     1003    28347 2022-04-14 15:50:31.000000 google-cloud-bigtable-2.9.0/google/cloud/bigtable/row_filters.py
+-rw-rw-r--   0 root         (0)     1003     7390 2022-04-14 15:50:31.000000 google-cloud-bigtable-2.9.0/google/cloud/bigtable/row_set.py
+-rw-rw-r--   0 root         (0)     1003    53684 2022-04-14 15:50:31.000000 google-cloud-bigtable-2.9.0/google/cloud/bigtable/table.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-04-14 15:53:10.044481 google-cloud-bigtable-2.9.0/google/cloud/bigtable_admin_v2/
+-rw-rw-r--   0 root         (0)     1003     7176 2022-04-14 15:50:31.000000 google-cloud-bigtable-2.9.0/google/cloud/bigtable_admin_v2/__init__.py
+-rw-rw-r--   0 root         (0)     1003    11554 2022-04-14 15:50:31.000000 google-cloud-bigtable-2.9.0/google/cloud/bigtable_admin_v2/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003       88 2022-04-14 15:50:31.000000 google-cloud-bigtable-2.9.0/google/cloud/bigtable_admin_v2/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2022-04-14 15:53:10.044481 google-cloud-bigtable-2.9.0/google/cloud/bigtable_admin_v2/services/
+-rw-rw-r--   0 root         (0)     1003      600 2022-04-14 15:50:31.000000 google-cloud-bigtable-2.9.0/google/cloud/bigtable_admin_v2/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-04-14 15:53:10.044481 google-cloud-bigtable-2.9.0/google/cloud/bigtable_admin_v2/services/bigtable_instance_admin/
+-rw-rw-r--   0 root         (0)     1003      797 2022-04-14 15:50:31.000000 google-cloud-bigtable-2.9.0/google/cloud/bigtable_admin_v2/services/bigtable_instance_admin/__init__.py
+-rw-rw-r--   0 root         (0)     1003    97178 2022-04-14 15:50:31.000000 google-cloud-bigtable-2.9.0/google/cloud/bigtable_admin_v2/services/bigtable_instance_admin/async_client.py
+-rw-rw-r--   0 root         (0)     1003   106955 2022-04-14 15:50:31.000000 google-cloud-bigtable-2.9.0/google/cloud/bigtable_admin_v2/services/bigtable_instance_admin/client.py
+-rw-rw-r--   0 root         (0)     1003    11323 2022-04-14 15:50:31.000000 google-cloud-bigtable-2.9.0/google/cloud/bigtable_admin_v2/services/bigtable_instance_admin/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-04-14 15:53:10.048483 google-cloud-bigtable-2.9.0/google/cloud/bigtable_admin_v2/services/bigtable_instance_admin/transports/
+-rw-rw-r--   0 root         (0)     1003     1265 2022-04-14 15:50:31.000000 google-cloud-bigtable-2.9.0/google/cloud/bigtable_admin_v2/services/bigtable_instance_admin/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003    21462 2022-04-14 15:50:31.000000 google-cloud-bigtable-2.9.0/google/cloud/bigtable_admin_v2/services/bigtable_instance_admin/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    37760 2022-04-14 15:50:31.000000 google-cloud-bigtable-2.9.0/google/cloud/bigtable_admin_v2/services/bigtable_instance_admin/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    38638 2022-04-14 15:50:31.000000 google-cloud-bigtable-2.9.0/google/cloud/bigtable_admin_v2/services/bigtable_instance_admin/transports/grpc_asyncio.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-04-14 15:53:10.048483 google-cloud-bigtable-2.9.0/google/cloud/bigtable_admin_v2/services/bigtable_table_admin/
+-rw-rw-r--   0 root         (0)     1003      785 2022-04-14 15:50:31.000000 google-cloud-bigtable-2.9.0/google/cloud/bigtable_admin_v2/services/bigtable_table_admin/__init__.py
+-rw-rw-r--   0 root         (0)     1003   105031 2022-04-14 15:50:31.000000 google-cloud-bigtable-2.9.0/google/cloud/bigtable_admin_v2/services/bigtable_table_admin/async_client.py
+-rw-rw-r--   0 root         (0)     1003   116797 2022-04-14 15:50:31.000000 google-cloud-bigtable-2.9.0/google/cloud/bigtable_admin_v2/services/bigtable_table_admin/client.py
+-rw-rw-r--   0 root         (0)     1003    15999 2022-04-14 15:50:31.000000 google-cloud-bigtable-2.9.0/google/cloud/bigtable_admin_v2/services/bigtable_table_admin/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-04-14 15:53:10.048483 google-cloud-bigtable-2.9.0/google/cloud/bigtable_admin_v2/services/bigtable_table_admin/transports/
+-rw-rw-r--   0 root         (0)     1003     1238 2022-04-14 15:50:31.000000 google-cloud-bigtable-2.9.0/google/cloud/bigtable_admin_v2/services/bigtable_table_admin/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003    20197 2022-04-14 15:50:31.000000 google-cloud-bigtable-2.9.0/google/cloud/bigtable_admin_v2/services/bigtable_table_admin/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    40943 2022-04-14 15:50:31.000000 google-cloud-bigtable-2.9.0/google/cloud/bigtable_admin_v2/services/bigtable_table_admin/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    41793 2022-04-14 15:50:31.000000 google-cloud-bigtable-2.9.0/google/cloud/bigtable_admin_v2/services/bigtable_table_admin/transports/grpc_asyncio.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-04-14 15:53:10.052485 google-cloud-bigtable-2.9.0/google/cloud/bigtable_admin_v2/types/
+-rw-rw-r--   0 root         (0)     1003     4525 2022-04-14 15:50:31.000000 google-cloud-bigtable-2.9.0/google/cloud/bigtable_admin_v2/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003    25292 2022-04-14 15:50:31.000000 google-cloud-bigtable-2.9.0/google/cloud/bigtable_admin_v2/types/bigtable_instance_admin.py
+-rw-rw-r--   0 root         (0)     1003    39244 2022-04-14 15:50:31.000000 google-cloud-bigtable-2.9.0/google/cloud/bigtable_admin_v2/types/bigtable_table_admin.py
+-rw-rw-r--   0 root         (0)     1003     1918 2022-04-14 15:50:31.000000 google-cloud-bigtable-2.9.0/google/cloud/bigtable_admin_v2/types/common.py
+-rw-rw-r--   0 root         (0)     1003    16084 2022-04-14 15:50:31.000000 google-cloud-bigtable-2.9.0/google/cloud/bigtable_admin_v2/types/instance.py
+-rw-rw-r--   0 root         (0)     1003    18409 2022-04-14 15:50:31.000000 google-cloud-bigtable-2.9.0/google/cloud/bigtable_admin_v2/types/table.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-04-14 15:53:10.052485 google-cloud-bigtable-2.9.0/google/cloud/bigtable_v2/
+-rw-rw-r--   0 root         (0)     1003     2439 2022-04-14 15:50:31.000000 google-cloud-bigtable-2.9.0/google/cloud/bigtable_v2/__init__.py
+-rw-rw-r--   0 root         (0)     1003     2223 2022-04-14 15:50:31.000000 google-cloud-bigtable-2.9.0/google/cloud/bigtable_v2/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003       82 2022-04-14 15:50:31.000000 google-cloud-bigtable-2.9.0/google/cloud/bigtable_v2/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2022-04-14 15:53:10.052485 google-cloud-bigtable-2.9.0/google/cloud/bigtable_v2/services/
+-rw-rw-r--   0 root         (0)     1003      600 2022-04-14 15:50:31.000000 google-cloud-bigtable-2.9.0/google/cloud/bigtable_v2/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-04-14 15:53:10.052485 google-cloud-bigtable-2.9.0/google/cloud/bigtable_v2/services/bigtable/
+-rw-rw-r--   0 root         (0)     1003      745 2022-04-14 15:50:31.000000 google-cloud-bigtable-2.9.0/google/cloud/bigtable_v2/services/bigtable/__init__.py
+-rw-rw-r--   0 root         (0)     1003    41959 2022-04-14 15:50:31.000000 google-cloud-bigtable-2.9.0/google/cloud/bigtable_v2/services/bigtable/async_client.py
+-rw-rw-r--   0 root         (0)     1003    54432 2022-04-14 15:50:31.000000 google-cloud-bigtable-2.9.0/google/cloud/bigtable_v2/services/bigtable/client.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-04-14 15:53:10.052485 google-cloud-bigtable-2.9.0/google/cloud/bigtable_v2/services/bigtable/transports/
+-rw-rw-r--   0 root         (0)     1003     1140 2022-04-14 15:50:31.000000 google-cloud-bigtable-2.9.0/google/cloud/bigtable_v2/services/bigtable/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     9252 2022-04-14 15:50:31.000000 google-cloud-bigtable-2.9.0/google/cloud/bigtable_v2/services/bigtable/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    19390 2022-04-14 15:50:31.000000 google-cloud-bigtable-2.9.0/google/cloud/bigtable_v2/services/bigtable/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    19780 2022-04-14 15:50:31.000000 google-cloud-bigtable-2.9.0/google/cloud/bigtable_v2/services/bigtable/transports/grpc_asyncio.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-04-14 15:53:10.052485 google-cloud-bigtable-2.9.0/google/cloud/bigtable_v2/types/
+-rw-rw-r--   0 root         (0)     1003     1789 2022-04-14 15:50:31.000000 google-cloud-bigtable-2.9.0/google/cloud/bigtable_v2/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003    20928 2022-04-14 15:50:31.000000 google-cloud-bigtable-2.9.0/google/cloud/bigtable_v2/types/bigtable.py
+-rw-rw-r--   0 root         (0)     1003    36953 2022-04-14 15:50:31.000000 google-cloud-bigtable-2.9.0/google/cloud/bigtable_v2/types/data.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-04-14 15:53:10.056487 google-cloud-bigtable-2.9.0/google_cloud_bigtable.egg-info/
+-rw-r--r--   0 root         (0)     1003     4406 2022-04-14 15:53:09.000000 google-cloud-bigtable-2.9.0/google_cloud_bigtable.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0)     1003     4581 2022-04-14 15:53:09.000000 google-cloud-bigtable-2.9.0/google_cloud_bigtable.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0)     1003        1 2022-04-14 15:53:09.000000 google-cloud-bigtable-2.9.0/google_cloud_bigtable.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0)     1003       20 2022-04-14 15:53:09.000000 google-cloud-bigtable-2.9.0/google_cloud_bigtable.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0)     1003        1 2022-04-14 15:53:09.000000 google-cloud-bigtable-2.9.0/google_cloud_bigtable.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0)     1003      187 2022-04-14 15:53:09.000000 google-cloud-bigtable-2.9.0/google_cloud_bigtable.egg-info/requires.txt
+-rw-r--r--   0 root         (0)     1003        7 2022-04-14 15:53:09.000000 google-cloud-bigtable-2.9.0/google_cloud_bigtable.egg-info/top_level.txt
+drwxr-sr-x   0 root         (0)     1003        0 2022-04-14 15:53:10.056487 google-cloud-bigtable-2.9.0/scripts/
+-rw-rw-r--   0 root         (0)     1003     8447 2022-04-14 15:50:31.000000 google-cloud-bigtable-2.9.0/scripts/fixup_bigtable_admin_v2_keywords.py
+-rw-rw-r--   0 root         (0)     1003     6488 2022-04-14 15:50:31.000000 google-cloud-bigtable-2.9.0/scripts/fixup_bigtable_v2_keywords.py
+-rw-rw-r--   0 root         (0)     1003       67 2022-04-14 15:53:10.064491 google-cloud-bigtable-2.9.0/setup.cfg
+-rw-rw-r--   0 root         (0)     1003     3312 2022-04-14 15:50:31.000000 google-cloud-bigtable-2.9.0/setup.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-04-14 15:53:10.056487 google-cloud-bigtable-2.9.0/tests/
+-rw-rw-r--   0 root         (0)     1003      600 2022-04-14 15:50:31.000000 google-cloud-bigtable-2.9.0/tests/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-04-14 15:53:10.056487 google-cloud-bigtable-2.9.0/tests/system/
+-rw-rw-r--   0 root         (0)     1003      600 2022-04-14 15:50:31.000000 google-cloud-bigtable-2.9.0/tests/system/__init__.py
+-rw-rw-r--   0 root         (0)     1003     1475 2022-04-14 15:50:31.000000 google-cloud-bigtable-2.9.0/tests/system/_helpers.py
+-rw-rw-r--   0 root         (0)     1003     5267 2022-04-14 15:50:31.000000 google-cloud-bigtable-2.9.0/tests/system/conftest.py
+-rw-rw-r--   0 root         (0)     1003    12486 2022-04-14 15:50:31.000000 google-cloud-bigtable-2.9.0/tests/system/test_data_api.py
+-rw-rw-r--   0 root         (0)     1003    29686 2022-04-14 15:50:31.000000 google-cloud-bigtable-2.9.0/tests/system/test_instance_admin.py
+-rw-rw-r--   0 root         (0)     1003    12038 2022-04-14 15:50:31.000000 google-cloud-bigtable-2.9.0/tests/system/test_table_admin.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-04-14 15:53:10.060489 google-cloud-bigtable-2.9.0/tests/unit/
+-rw-rw-r--   0 root         (0)     1003      600 2022-04-14 15:50:31.000000 google-cloud-bigtable-2.9.0/tests/unit/__init__.py
+-rw-rw-r--   0 root         (0)     1003     1040 2022-04-14 15:50:31.000000 google-cloud-bigtable-2.9.0/tests/unit/_testing.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-04-14 15:53:10.060489 google-cloud-bigtable-2.9.0/tests/unit/gapic/
+-rw-rw-r--   0 root         (0)     1003      600 2022-04-14 15:50:31.000000 google-cloud-bigtable-2.9.0/tests/unit/gapic/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-04-14 15:53:10.060489 google-cloud-bigtable-2.9.0/tests/unit/gapic/bigtable_admin_v2/
+-rw-rw-r--   0 root         (0)     1003      600 2022-04-14 15:50:31.000000 google-cloud-bigtable-2.9.0/tests/unit/gapic/bigtable_admin_v2/__init__.py
+-rw-rw-r--   0 root         (0)     1003   253502 2022-04-14 15:50:31.000000 google-cloud-bigtable-2.9.0/tests/unit/gapic/bigtable_admin_v2/test_bigtable_instance_admin.py
+-rw-rw-r--   0 root         (0)     1003   262675 2022-04-14 15:50:31.000000 google-cloud-bigtable-2.9.0/tests/unit/gapic/bigtable_admin_v2/test_bigtable_table_admin.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-04-14 15:53:10.064491 google-cloud-bigtable-2.9.0/tests/unit/gapic/bigtable_v2/
+-rw-rw-r--   0 root         (0)     1003      600 2022-04-14 15:50:31.000000 google-cloud-bigtable-2.9.0/tests/unit/gapic/bigtable_v2/__init__.py
+-rw-rw-r--   0 root         (0)     1003   114765 2022-04-14 15:50:31.000000 google-cloud-bigtable-2.9.0/tests/unit/gapic/bigtable_v2/test_bigtable.py
+-rw-rw-r--   0 root         (0)     1003    36953 2022-04-14 15:50:31.000000 google-cloud-bigtable-2.9.0/tests/unit/read-rows-acceptance-test.json
+-rw-rw-r--   0 root         (0)     1003    28863 2022-04-14 15:50:31.000000 google-cloud-bigtable-2.9.0/tests/unit/test_app_profile.py
+-rw-rw-r--   0 root         (0)     1003    29724 2022-04-14 15:50:31.000000 google-cloud-bigtable-2.9.0/tests/unit/test_backup.py
+-rw-rw-r--   0 root         (0)     1003     4350 2022-04-14 15:50:31.000000 google-cloud-bigtable-2.9.0/tests/unit/test_batcher.py
+-rw-rw-r--   0 root         (0)     1003    26525 2022-04-14 15:50:31.000000 google-cloud-bigtable-2.9.0/tests/unit/test_client.py
+-rw-rw-r--   0 root         (0)     1003    36981 2022-04-14 15:50:31.000000 google-cloud-bigtable-2.9.0/tests/unit/test_cluster.py
+-rw-rw-r--   0 root         (0)     1003    20228 2022-04-14 15:50:31.000000 google-cloud-bigtable-2.9.0/tests/unit/test_column_family.py
+-rw-rw-r--   0 root         (0)     1003     5157 2022-04-14 15:50:31.000000 google-cloud-bigtable-2.9.0/tests/unit/test_encryption_info.py
+-rw-rw-r--   0 root         (0)     1003     2855 2022-04-14 15:50:31.000000 google-cloud-bigtable-2.9.0/tests/unit/test_error.py
+-rw-rw-r--   0 root         (0)     1003    31903 2022-04-14 15:50:31.000000 google-cloud-bigtable-2.9.0/tests/unit/test_instance.py
+-rw-rw-r--   0 root         (0)     1003     8924 2022-04-14 15:50:31.000000 google-cloud-bigtable-2.9.0/tests/unit/test_policy.py
+-rw-rw-r--   0 root         (0)     1003    24763 2022-04-14 15:50:31.000000 google-cloud-bigtable-2.9.0/tests/unit/test_row.py
+-rw-rw-r--   0 root         (0)     1003    47982 2022-04-14 15:50:31.000000 google-cloud-bigtable-2.9.0/tests/unit/test_row_data.py
+-rw-rw-r--   0 root         (0)     1003    36325 2022-04-14 15:50:31.000000 google-cloud-bigtable-2.9.0/tests/unit/test_row_filters.py
+-rw-rw-r--   0 root         (0)     1003     9379 2022-04-14 15:50:31.000000 google-cloud-bigtable-2.9.0/tests/unit/test_row_set.py
+-rw-rw-r--   0 root         (0)     1003    70768 2022-04-14 15:50:31.000000 google-cloud-bigtable-2.9.0/tests/unit/test_table.py
```

### Comparing `google-cloud-bigtable-2.8.1/LICENSE` & `google-cloud-bigtable-2.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `google-cloud-bigtable-2.8.1/MANIFEST.in` & `google-cloud-bigtable-2.9.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `google-cloud-bigtable-2.8.1/PKG-INFO` & `google-cloud-bigtable-2.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-bigtable
-Version: 2.8.1
+Version: 2.9.0
 Summary: Google Cloud Bigtable API client library
 Home-page: https://github.com/googleapis/python-bigtable
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `google-cloud-bigtable-2.8.1/README.rst` & `google-cloud-bigtable-2.9.0/README.rst`

 * *Files identical despite different names*

### Comparing `google-cloud-bigtable-2.8.1/google/cloud/bigtable/__init__.py` & `google-cloud-bigtable-2.9.0/google/cloud/bigtable/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigtable-2.8.1/google/cloud/bigtable/app_profile.py` & `google-cloud-bigtable-2.9.0/google/cloud/bigtable/app_profile.py`

 * *Files 16% similar despite different names*

```diff
@@ -55,34 +55,41 @@
                          case for this AppProfile.
 
     :type: cluster_id: str
     :param: cluster_id: (Optional) Unique cluster_id which is only required
                         when routing_policy_type is
                         ROUTING_POLICY_TYPE_SINGLE.
 
+    :type: multi_cluster_ids: list
+    :param: multi_cluster_ids: (Optional) The set of clusters to route to.
+                            The order is ignored; clusters will be tried in order of distance.
+                            If left empty, all clusters are eligible.
+
     :type: allow_transactional_writes: bool
     :param: allow_transactional_writes: (Optional) If true, allow
                                         transactional writes for
                                         ROUTING_POLICY_TYPE_SINGLE.
     """
 
     def __init__(
         self,
         app_profile_id,
         instance,
         routing_policy_type=None,
         description=None,
         cluster_id=None,
+        multi_cluster_ids=None,
         allow_transactional_writes=None,
     ):
         self.app_profile_id = app_profile_id
         self._instance = instance
         self.routing_policy_type = routing_policy_type
         self.description = description
         self.cluster_id = cluster_id
+        self.multi_cluster_ids = multi_cluster_ids
         self.allow_transactional_writes = allow_transactional_writes
 
     @property
     def name(self):
         """AppProfile name used in requests.
 
         .. note::
@@ -180,21 +187,25 @@
     def _update_from_pb(self, app_profile_pb):
         """Refresh self from the server-provided protobuf.
         Helper for :meth:`from_pb` and :meth:`reload`.
         """
         self.routing_policy_type = None
         self.allow_transactional_writes = None
         self.cluster_id = None
-
+        self.multi_cluster_ids = None
         self.description = app_profile_pb.description
 
         routing_policy_type = None
         if app_profile_pb._pb.HasField("multi_cluster_routing_use_any"):
             routing_policy_type = RoutingPolicyType.ANY
             self.allow_transactional_writes = False
+            if app_profile_pb.multi_cluster_routing_use_any.cluster_ids:
+                self.multi_cluster_ids = (
+                    app_profile_pb.multi_cluster_routing_use_any.cluster_ids
+                )
         else:
             routing_policy_type = RoutingPolicyType.SINGLE
             self.cluster_id = app_profile_pb.single_cluster_routing.cluster_id
             self.allow_transactional_writes = (
                 app_profile_pb.single_cluster_routing.allow_transactional_writes
             )
         self.routing_policy_type = routing_policy_type
@@ -211,15 +222,17 @@
             raise ValueError("AppProfile required routing policy.")
 
         single_cluster_routing = None
         multi_cluster_routing_use_any = None
 
         if self.routing_policy_type == RoutingPolicyType.ANY:
             multi_cluster_routing_use_any = (
-                instance.AppProfile.MultiClusterRoutingUseAny()
+                instance.AppProfile.MultiClusterRoutingUseAny(
+                    cluster_ids=self.multi_cluster_ids
+                )
             )
         else:
             single_cluster_routing = instance.AppProfile.SingleClusterRouting(
                 cluster_id=self.cluster_id,
                 allow_transactional_writes=self.allow_transactional_writes,
             )
 
@@ -308,14 +321,15 @@
 
         .. note::
 
             Update any or all of the following values:
             ``routing_policy_type``
             ``description``
             ``cluster_id``
+            ``multi_cluster_ids``
             ``allow_transactional_writes``
 
         For example:
 
         .. literalinclude:: snippets.py
             :start-after: [START bigtable_api_update_app_profile]
             :end-before: [END bigtable_api_update_app_profile]
```

### Comparing `google-cloud-bigtable-2.8.1/google/cloud/bigtable/backup.py` & `google-cloud-bigtable-2.9.0/google/cloud/bigtable/backup.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigtable-2.8.1/google/cloud/bigtable/batcher.py` & `google-cloud-bigtable-2.9.0/google/cloud/bigtable/batcher.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigtable-2.8.1/google/cloud/bigtable/client.py` & `google-cloud-bigtable-2.9.0/google/cloud/bigtable/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigtable-2.8.1/google/cloud/bigtable/cluster.py` & `google-cloud-bigtable-2.9.0/google/cloud/bigtable/cluster.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigtable-2.8.1/google/cloud/bigtable/column_family.py` & `google-cloud-bigtable-2.9.0/google/cloud/bigtable/column_family.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigtable-2.8.1/google/cloud/bigtable/encryption_info.py` & `google-cloud-bigtable-2.9.0/google/cloud/bigtable/encryption_info.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigtable-2.8.1/google/cloud/bigtable/enums.py` & `google-cloud-bigtable-2.9.0/google/cloud/bigtable/enums.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigtable-2.8.1/google/cloud/bigtable/error.py` & `google-cloud-bigtable-2.9.0/google/cloud/bigtable/error.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigtable-2.8.1/google/cloud/bigtable/instance.py` & `google-cloud-bigtable-2.9.0/google/cloud/bigtable/instance.py`

 * *Files 2% similar despite different names*

```diff
@@ -707,14 +707,15 @@
 
     def app_profile(
         self,
         app_profile_id,
         routing_policy_type=None,
         description=None,
         cluster_id=None,
+        multi_cluster_ids=None,
         allow_transactional_writes=None,
     ):
         """Factory to create AppProfile associated with this instance.
 
         For example:
 
         .. literalinclude:: snippets.py
@@ -738,28 +739,34 @@
                              case for this AppProfile.
 
         :type: cluster_id: str
         :param: cluster_id: (Optional) Unique cluster_id which is only required
                             when routing_policy_type is
                             ROUTING_POLICY_TYPE_SINGLE.
 
+        :type: multi_cluster_ids: list
+        :param: multi_cluster_ids: (Optional) The set of clusters to route to.
+                            The order is ignored; clusters will be tried in order of distance.
+                            If left empty, all clusters are eligible.
+
         :type: allow_transactional_writes: bool
         :param: allow_transactional_writes: (Optional) If true, allow
                                             transactional writes for
                                             ROUTING_POLICY_TYPE_SINGLE.
 
         :rtype: :class:`~google.cloud.bigtable.app_profile.AppProfile>`
         :returns: AppProfile for this instance.
         """
         return AppProfile(
             app_profile_id,
             self,
             routing_policy_type=routing_policy_type,
             description=description,
             cluster_id=cluster_id,
+            multi_cluster_ids=multi_cluster_ids,
             allow_transactional_writes=allow_transactional_writes,
         )
 
     def list_app_profiles(self):
         """Lists information about AppProfiles in an instance.
 
         For example:
```

### Comparing `google-cloud-bigtable-2.8.1/google/cloud/bigtable/policy.py` & `google-cloud-bigtable-2.9.0/google/cloud/bigtable/policy.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigtable-2.8.1/google/cloud/bigtable/row.py` & `google-cloud-bigtable-2.9.0/google/cloud/bigtable/row.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigtable-2.8.1/google/cloud/bigtable/row_data.py` & `google-cloud-bigtable-2.9.0/google/cloud/bigtable/row_data.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigtable-2.8.1/google/cloud/bigtable/row_filters.py` & `google-cloud-bigtable-2.9.0/google/cloud/bigtable/row_filters.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigtable-2.8.1/google/cloud/bigtable/row_set.py` & `google-cloud-bigtable-2.9.0/google/cloud/bigtable/row_set.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigtable-2.8.1/google/cloud/bigtable/table.py` & `google-cloud-bigtable-2.9.0/google/cloud/bigtable/table.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigtable-2.8.1/google/cloud/bigtable_admin_v2/__init__.py` & `google-cloud-bigtable-2.9.0/google/cloud/bigtable_admin_v2/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigtable-2.8.1/google/cloud/bigtable_admin_v2/gapic_metadata.json` & `google-cloud-bigtable-2.9.0/google/cloud/bigtable_admin_v2/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-cloud-bigtable-2.8.1/google/cloud/bigtable_admin_v2/services/__init__.py` & `google-cloud-bigtable-2.9.0/google/cloud/bigtable_admin_v2/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigtable-2.8.1/google/cloud/bigtable_admin_v2/services/bigtable_instance_admin/__init__.py` & `google-cloud-bigtable-2.9.0/google/cloud/bigtable_admin_v2/services/bigtable_instance_admin/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigtable-2.8.1/google/cloud/bigtable_admin_v2/services/bigtable_instance_admin/async_client.py` & `google-cloud-bigtable-2.9.0/google/cloud/bigtable_admin_v2/services/bigtable_instance_admin/async_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 from collections import OrderedDict
 import functools
 import re
-from typing import Dict, Optional, Sequence, Tuple, Type, Union
+from typing import Dict, Mapping, Optional, Sequence, Tuple, Type, Union
 import pkg_resources
 
 from google.api_core.client_options import ClientOptions
 from google.api_core import exceptions as core_exceptions
 from google.api_core import gapic_v1
 from google.api_core import retry as retries
 from google.auth import credentials as ga_credentials  # type: ignore
@@ -237,15 +237,15 @@
     async def create_instance(
         self,
         request: Union[bigtable_instance_admin.CreateInstanceRequest, dict] = None,
         *,
         parent: str = None,
         instance_id: str = None,
         instance: gba_instance.Instance = None,
-        clusters: Dict[str, gba_instance.Cluster] = None,
+        clusters: Mapping[str, gba_instance.Cluster] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
         timeout: float = None,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> operation_async.AsyncOperation:
         r"""Create an instance within a project.
 
         Note that exactly one of Cluster.serve_nodes and
@@ -277,15 +277,15 @@
             instance (:class:`google.cloud.bigtable_admin_v2.types.Instance`):
                 Required. The instance to create. Fields marked
                 ``OutputOnly`` must be left blank.
 
                 This corresponds to the ``instance`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
-            clusters (Dict[str, gba_instance.Cluster]):
+            clusters (:class:`Mapping[str, google.cloud.bigtable_admin_v2.types.Cluster]`):
                 Required. The clusters to be created within the
                 instance, mapped by desired cluster ID, e.g., just
                 ``mycluster`` rather than
                 ``projects/myproject/instances/myinstance/clusters/mycluster``.
                 Fields marked ``OutputOnly`` must be left blank.
                 Currently, at most four clusters can be specified.
 
@@ -1868,69 +1868,75 @@
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
             google.iam.v1.policy_pb2.Policy:
-                Defines an Identity and Access Management (IAM) policy. It is used to
-                   specify access control policies for Cloud Platform
-                   resources.
+                An Identity and Access Management (IAM) policy, which specifies access
+                   controls for Google Cloud resources.
 
                    A Policy is a collection of bindings. A binding binds
-                   one or more members to a single role. Members can be
-                   user accounts, service accounts, Google groups, and
-                   domains (such as G Suite). A role is a named list of
-                   permissions (defined by IAM or configured by users).
-                   A binding can optionally specify a condition, which
-                   is a logic expression that further constrains the
-                   role binding based on attributes about the request
-                   and/or target resource.
+                   one or more members, or principals, to a single role.
+                   Principals can be user accounts, service accounts,
+                   Google groups, and domains (such as G Suite). A role
+                   is a named list of permissions; each role can be an
+                   IAM predefined role or a user-created custom role.
+
+                   For some types of Google Cloud resources, a binding
+                   can also specify a condition, which is a logical
+                   expression that allows access to a resource only if
+                   the expression evaluates to true. A condition can add
+                   constraints based on attributes of the request, the
+                   resource, or both. To learn which resources support
+                   conditions in their IAM policies, see the [IAM
+                   documentation](\ https://cloud.google.com/iam/help/conditions/resource-policies).
 
-                   **JSON Example**
+                   **JSON example:**
 
                       {
                          "bindings": [
                             {
                                "role":
                                "roles/resourcemanager.organizationAdmin",
                                "members": [ "user:mike@example.com",
                                "group:admins@example.com",
                                "domain:google.com",
                                "serviceAccount:my-project-id@appspot.gserviceaccount.com"
                                ]
 
                             }, { "role":
                             "roles/resourcemanager.organizationViewer",
-                            "members": ["user:eve@example.com"],
+                            "members": [ "user:eve@example.com" ],
                             "condition": { "title": "expirable access",
                             "description": "Does not grant access after
                             Sep 2020", "expression": "request.time <
                             timestamp('2020-10-01T00:00:00.000Z')", } }
 
-                         ]
+                         ], "etag": "BwWWja0YfJA=", "version": 3
 
                       }
 
-                   **YAML Example**
+                   **YAML example:**
 
                       bindings: - members: - user:\ mike@example.com -
                       group:\ admins@example.com - domain:google.com -
                       serviceAccount:\ my-project-id@appspot.gserviceaccount.com
                       role: roles/resourcemanager.organizationAdmin -
                       members: - user:\ eve@example.com role:
                       roles/resourcemanager.organizationViewer
                       condition: title: expirable access description:
                       Does not grant access after Sep 2020 expression:
                       request.time <
-                      timestamp('2020-10-01T00:00:00.000Z')
+                      timestamp('2020-10-01T00:00:00.000Z') etag:
+                      BwWWja0YfJA= version: 3
 
                    For a description of IAM and its features, see the
-                   [IAM developer's
-                   guide](\ https://cloud.google.com/iam/docs).
+                   [IAM
+                   documentation](\ https://cloud.google.com/iam/docs/).
 
         """
         # Create or coerce a protobuf request object.
         # Quick check: If we got a request object, we should *not* have
         # gotten any keyword arguments that map to the request.
         has_flattened_params = any([resource])
         if request is not None and has_flattened_params:
@@ -2012,69 +2018,75 @@
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
             google.iam.v1.policy_pb2.Policy:
-                Defines an Identity and Access Management (IAM) policy. It is used to
-                   specify access control policies for Cloud Platform
-                   resources.
+                An Identity and Access Management (IAM) policy, which specifies access
+                   controls for Google Cloud resources.
 
                    A Policy is a collection of bindings. A binding binds
-                   one or more members to a single role. Members can be
-                   user accounts, service accounts, Google groups, and
-                   domains (such as G Suite). A role is a named list of
-                   permissions (defined by IAM or configured by users).
-                   A binding can optionally specify a condition, which
-                   is a logic expression that further constrains the
-                   role binding based on attributes about the request
-                   and/or target resource.
+                   one or more members, or principals, to a single role.
+                   Principals can be user accounts, service accounts,
+                   Google groups, and domains (such as G Suite). A role
+                   is a named list of permissions; each role can be an
+                   IAM predefined role or a user-created custom role.
+
+                   For some types of Google Cloud resources, a binding
+                   can also specify a condition, which is a logical
+                   expression that allows access to a resource only if
+                   the expression evaluates to true. A condition can add
+                   constraints based on attributes of the request, the
+                   resource, or both. To learn which resources support
+                   conditions in their IAM policies, see the [IAM
+                   documentation](\ https://cloud.google.com/iam/help/conditions/resource-policies).
 
-                   **JSON Example**
+                   **JSON example:**
 
                       {
                          "bindings": [
                             {
                                "role":
                                "roles/resourcemanager.organizationAdmin",
                                "members": [ "user:mike@example.com",
                                "group:admins@example.com",
                                "domain:google.com",
                                "serviceAccount:my-project-id@appspot.gserviceaccount.com"
                                ]
 
                             }, { "role":
                             "roles/resourcemanager.organizationViewer",
-                            "members": ["user:eve@example.com"],
+                            "members": [ "user:eve@example.com" ],
                             "condition": { "title": "expirable access",
                             "description": "Does not grant access after
                             Sep 2020", "expression": "request.time <
                             timestamp('2020-10-01T00:00:00.000Z')", } }
 
-                         ]
+                         ], "etag": "BwWWja0YfJA=", "version": 3
 
                       }
 
-                   **YAML Example**
+                   **YAML example:**
 
                       bindings: - members: - user:\ mike@example.com -
                       group:\ admins@example.com - domain:google.com -
                       serviceAccount:\ my-project-id@appspot.gserviceaccount.com
                       role: roles/resourcemanager.organizationAdmin -
                       members: - user:\ eve@example.com role:
                       roles/resourcemanager.organizationViewer
                       condition: title: expirable access description:
                       Does not grant access after Sep 2020 expression:
                       request.time <
-                      timestamp('2020-10-01T00:00:00.000Z')
+                      timestamp('2020-10-01T00:00:00.000Z') etag:
+                      BwWWja0YfJA= version: 3
 
                    For a description of IAM and its features, see the
-                   [IAM developer's
-                   guide](\ https://cloud.google.com/iam/docs).
+                   [IAM
+                   documentation](\ https://cloud.google.com/iam/docs/).
 
         """
         # Create or coerce a protobuf request object.
         # Quick check: If we got a request object, we should *not* have
         # gotten any keyword arguments that map to the request.
         has_flattened_params = any([resource])
         if request is not None and has_flattened_params:
```

### Comparing `google-cloud-bigtable-2.8.1/google/cloud/bigtable_admin_v2/services/bigtable_instance_admin/client.py` & `google-cloud-bigtable-2.9.0/google/cloud/bigtable_admin_v2/services/bigtable_instance_admin/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 from collections import OrderedDict
 import os
 import re
-from typing import Dict, Optional, Sequence, Tuple, Type, Union
+from typing import Dict, Mapping, Optional, Sequence, Tuple, Type, Union
 import pkg_resources
 
 from google.api_core import client_options as client_options_lib
 from google.api_core import exceptions as core_exceptions
 from google.api_core import gapic_v1
 from google.api_core import retry as retries
 from google.auth import credentials as ga_credentials  # type: ignore
@@ -553,15 +553,15 @@
     def create_instance(
         self,
         request: Union[bigtable_instance_admin.CreateInstanceRequest, dict] = None,
         *,
         parent: str = None,
         instance_id: str = None,
         instance: gba_instance.Instance = None,
-        clusters: Dict[str, gba_instance.Cluster] = None,
+        clusters: Mapping[str, gba_instance.Cluster] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
         timeout: float = None,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> operation.Operation:
         r"""Create an instance within a project.
 
         Note that exactly one of Cluster.serve_nodes and
@@ -593,15 +593,15 @@
             instance (google.cloud.bigtable_admin_v2.types.Instance):
                 Required. The instance to create. Fields marked
                 ``OutputOnly`` must be left blank.
 
                 This corresponds to the ``instance`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
-            clusters (Dict[str, gba_instance.Cluster]):
+            clusters (Mapping[str, google.cloud.bigtable_admin_v2.types.Cluster]):
                 Required. The clusters to be created within the
                 instance, mapped by desired cluster ID, e.g., just
                 ``mycluster`` rather than
                 ``projects/myproject/instances/myinstance/clusters/mycluster``.
                 Fields marked ``OutputOnly`` must be left blank.
                 Currently, at most four clusters can be specified.
 
@@ -2077,69 +2077,75 @@
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
             google.iam.v1.policy_pb2.Policy:
-                Defines an Identity and Access Management (IAM) policy. It is used to
-                   specify access control policies for Cloud Platform
-                   resources.
+                An Identity and Access Management (IAM) policy, which specifies access
+                   controls for Google Cloud resources.
 
                    A Policy is a collection of bindings. A binding binds
-                   one or more members to a single role. Members can be
-                   user accounts, service accounts, Google groups, and
-                   domains (such as G Suite). A role is a named list of
-                   permissions (defined by IAM or configured by users).
-                   A binding can optionally specify a condition, which
-                   is a logic expression that further constrains the
-                   role binding based on attributes about the request
-                   and/or target resource.
+                   one or more members, or principals, to a single role.
+                   Principals can be user accounts, service accounts,
+                   Google groups, and domains (such as G Suite). A role
+                   is a named list of permissions; each role can be an
+                   IAM predefined role or a user-created custom role.
+
+                   For some types of Google Cloud resources, a binding
+                   can also specify a condition, which is a logical
+                   expression that allows access to a resource only if
+                   the expression evaluates to true. A condition can add
+                   constraints based on attributes of the request, the
+                   resource, or both. To learn which resources support
+                   conditions in their IAM policies, see the [IAM
+                   documentation](\ https://cloud.google.com/iam/help/conditions/resource-policies).
 
-                   **JSON Example**
+                   **JSON example:**
 
                       {
                          "bindings": [
                             {
                                "role":
                                "roles/resourcemanager.organizationAdmin",
                                "members": [ "user:mike@example.com",
                                "group:admins@example.com",
                                "domain:google.com",
                                "serviceAccount:my-project-id@appspot.gserviceaccount.com"
                                ]
 
                             }, { "role":
                             "roles/resourcemanager.organizationViewer",
-                            "members": ["user:eve@example.com"],
+                            "members": [ "user:eve@example.com" ],
                             "condition": { "title": "expirable access",
                             "description": "Does not grant access after
                             Sep 2020", "expression": "request.time <
                             timestamp('2020-10-01T00:00:00.000Z')", } }
 
-                         ]
+                         ], "etag": "BwWWja0YfJA=", "version": 3
 
                       }
 
-                   **YAML Example**
+                   **YAML example:**
 
                       bindings: - members: - user:\ mike@example.com -
                       group:\ admins@example.com - domain:google.com -
                       serviceAccount:\ my-project-id@appspot.gserviceaccount.com
                       role: roles/resourcemanager.organizationAdmin -
                       members: - user:\ eve@example.com role:
                       roles/resourcemanager.organizationViewer
                       condition: title: expirable access description:
                       Does not grant access after Sep 2020 expression:
                       request.time <
-                      timestamp('2020-10-01T00:00:00.000Z')
+                      timestamp('2020-10-01T00:00:00.000Z') etag:
+                      BwWWja0YfJA= version: 3
 
                    For a description of IAM and its features, see the
-                   [IAM developer's
-                   guide](\ https://cloud.google.com/iam/docs).
+                   [IAM
+                   documentation](\ https://cloud.google.com/iam/docs/).
 
         """
         # Create or coerce a protobuf request object.
         # Quick check: If we got a request object, we should *not* have
         # gotten any keyword arguments that map to the request.
         has_flattened_params = any([resource])
         if request is not None and has_flattened_params:
@@ -2208,69 +2214,75 @@
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
             google.iam.v1.policy_pb2.Policy:
-                Defines an Identity and Access Management (IAM) policy. It is used to
-                   specify access control policies for Cloud Platform
-                   resources.
+                An Identity and Access Management (IAM) policy, which specifies access
+                   controls for Google Cloud resources.
 
                    A Policy is a collection of bindings. A binding binds
-                   one or more members to a single role. Members can be
-                   user accounts, service accounts, Google groups, and
-                   domains (such as G Suite). A role is a named list of
-                   permissions (defined by IAM or configured by users).
-                   A binding can optionally specify a condition, which
-                   is a logic expression that further constrains the
-                   role binding based on attributes about the request
-                   and/or target resource.
+                   one or more members, or principals, to a single role.
+                   Principals can be user accounts, service accounts,
+                   Google groups, and domains (such as G Suite). A role
+                   is a named list of permissions; each role can be an
+                   IAM predefined role or a user-created custom role.
+
+                   For some types of Google Cloud resources, a binding
+                   can also specify a condition, which is a logical
+                   expression that allows access to a resource only if
+                   the expression evaluates to true. A condition can add
+                   constraints based on attributes of the request, the
+                   resource, or both. To learn which resources support
+                   conditions in their IAM policies, see the [IAM
+                   documentation](\ https://cloud.google.com/iam/help/conditions/resource-policies).
 
-                   **JSON Example**
+                   **JSON example:**
 
                       {
                          "bindings": [
                             {
                                "role":
                                "roles/resourcemanager.organizationAdmin",
                                "members": [ "user:mike@example.com",
                                "group:admins@example.com",
                                "domain:google.com",
                                "serviceAccount:my-project-id@appspot.gserviceaccount.com"
                                ]
 
                             }, { "role":
                             "roles/resourcemanager.organizationViewer",
-                            "members": ["user:eve@example.com"],
+                            "members": [ "user:eve@example.com" ],
                             "condition": { "title": "expirable access",
                             "description": "Does not grant access after
                             Sep 2020", "expression": "request.time <
                             timestamp('2020-10-01T00:00:00.000Z')", } }
 
-                         ]
+                         ], "etag": "BwWWja0YfJA=", "version": 3
 
                       }
 
-                   **YAML Example**
+                   **YAML example:**
 
                       bindings: - members: - user:\ mike@example.com -
                       group:\ admins@example.com - domain:google.com -
                       serviceAccount:\ my-project-id@appspot.gserviceaccount.com
                       role: roles/resourcemanager.organizationAdmin -
                       members: - user:\ eve@example.com role:
                       roles/resourcemanager.organizationViewer
                       condition: title: expirable access description:
                       Does not grant access after Sep 2020 expression:
                       request.time <
-                      timestamp('2020-10-01T00:00:00.000Z')
+                      timestamp('2020-10-01T00:00:00.000Z') etag:
+                      BwWWja0YfJA= version: 3
 
                    For a description of IAM and its features, see the
-                   [IAM developer's
-                   guide](\ https://cloud.google.com/iam/docs).
+                   [IAM
+                   documentation](\ https://cloud.google.com/iam/docs/).
 
         """
         # Create or coerce a protobuf request object.
         # Quick check: If we got a request object, we should *not* have
         # gotten any keyword arguments that map to the request.
         has_flattened_params = any([resource])
         if request is not None and has_flattened_params:
```

### Comparing `google-cloud-bigtable-2.8.1/google/cloud/bigtable_admin_v2/services/bigtable_instance_admin/pagers.py` & `google-cloud-bigtable-2.9.0/google/cloud/bigtable_admin_v2/services/bigtable_instance_admin/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigtable-2.8.1/google/cloud/bigtable_admin_v2/services/bigtable_instance_admin/transports/__init__.py` & `google-cloud-bigtable-2.9.0/google/cloud/bigtable_admin_v2/services/bigtable_instance_admin/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigtable-2.8.1/google/cloud/bigtable_admin_v2/services/bigtable_instance_admin/transports/base.py` & `google-cloud-bigtable-2.9.0/google/cloud/bigtable_admin_v2/services/bigtable_instance_admin/transports/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -90,14 +90,15 @@
                 The client info used to send a user-agent string along with
                 API requests. If ``None``, then default info will be used.
                 Generally, you only need to set this if you're developing
                 your own client library.
             always_use_jwt_access (Optional[bool]): Whether self signed JWT should
                 be used for service account credentials.
         """
+
         # Save the hostname. Default to port 443 (HTTPS) if none is specified.
         if ":" not in host:
             host += ":443"
         self._host = host
 
         scopes_kwargs = {"scopes": scopes, "default_scopes": self.AUTH_SCOPES}
 
@@ -594,9 +595,13 @@
         Union[
             bigtable_instance_admin.ListHotTabletsResponse,
             Awaitable[bigtable_instance_admin.ListHotTabletsResponse],
         ],
     ]:
         raise NotImplementedError()
 
+    @property
+    def kind(self) -> str:
+        raise NotImplementedError()
+
 
 __all__ = ("BigtableInstanceAdminTransport",)
```

### Comparing `google-cloud-bigtable-2.8.1/google/cloud/bigtable_admin_v2/services/bigtable_instance_admin/transports/grpc.py` & `google-cloud-bigtable-2.9.0/google/cloud/bigtable_admin_v2/services/bigtable_instance_admin/transports/grpc.py`

 * *Files 1% similar despite different names*

```diff
@@ -858,9 +858,13 @@
                 response_deserializer=bigtable_instance_admin.ListHotTabletsResponse.deserialize,
             )
         return self._stubs["list_hot_tablets"]
 
     def close(self):
         self.grpc_channel.close()
 
+    @property
+    def kind(self) -> str:
+        return "grpc"
+
 
 __all__ = ("BigtableInstanceAdminGrpcTransport",)
```

### Comparing `google-cloud-bigtable-2.8.1/google/cloud/bigtable_admin_v2/services/bigtable_instance_admin/transports/grpc_asyncio.py` & `google-cloud-bigtable-2.9.0/google/cloud/bigtable_admin_v2/services/bigtable_instance_admin/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigtable-2.8.1/google/cloud/bigtable_admin_v2/services/bigtable_table_admin/__init__.py` & `google-cloud-bigtable-2.9.0/google/cloud/bigtable_admin_v2/services/bigtable_table_admin/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigtable-2.8.1/google/cloud/bigtable_admin_v2/services/bigtable_table_admin/async_client.py` & `google-cloud-bigtable-2.9.0/google/cloud/bigtable_admin_v2/services/bigtable_table_admin/async_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 from collections import OrderedDict
 import functools
 import re
-from typing import Dict, Optional, Sequence, Tuple, Type, Union
+from typing import Dict, Mapping, Optional, Sequence, Tuple, Type, Union
 import pkg_resources
 
 from google.api_core.client_options import ClientOptions
 from google.api_core import exceptions as core_exceptions
 from google.api_core import gapic_v1
 from google.api_core import retry as retries
 from google.auth import credentials as ga_credentials  # type: ignore
@@ -2083,69 +2083,75 @@
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
             google.iam.v1.policy_pb2.Policy:
-                Defines an Identity and Access Management (IAM) policy. It is used to
-                   specify access control policies for Cloud Platform
-                   resources.
+                An Identity and Access Management (IAM) policy, which specifies access
+                   controls for Google Cloud resources.
 
                    A Policy is a collection of bindings. A binding binds
-                   one or more members to a single role. Members can be
-                   user accounts, service accounts, Google groups, and
-                   domains (such as G Suite). A role is a named list of
-                   permissions (defined by IAM or configured by users).
-                   A binding can optionally specify a condition, which
-                   is a logic expression that further constrains the
-                   role binding based on attributes about the request
-                   and/or target resource.
+                   one or more members, or principals, to a single role.
+                   Principals can be user accounts, service accounts,
+                   Google groups, and domains (such as G Suite). A role
+                   is a named list of permissions; each role can be an
+                   IAM predefined role or a user-created custom role.
+
+                   For some types of Google Cloud resources, a binding
+                   can also specify a condition, which is a logical
+                   expression that allows access to a resource only if
+                   the expression evaluates to true. A condition can add
+                   constraints based on attributes of the request, the
+                   resource, or both. To learn which resources support
+                   conditions in their IAM policies, see the [IAM
+                   documentation](\ https://cloud.google.com/iam/help/conditions/resource-policies).
 
-                   **JSON Example**
+                   **JSON example:**
 
                       {
                          "bindings": [
                             {
                                "role":
                                "roles/resourcemanager.organizationAdmin",
                                "members": [ "user:mike@example.com",
                                "group:admins@example.com",
                                "domain:google.com",
                                "serviceAccount:my-project-id@appspot.gserviceaccount.com"
                                ]
 
                             }, { "role":
                             "roles/resourcemanager.organizationViewer",
-                            "members": ["user:eve@example.com"],
+                            "members": [ "user:eve@example.com" ],
                             "condition": { "title": "expirable access",
                             "description": "Does not grant access after
                             Sep 2020", "expression": "request.time <
                             timestamp('2020-10-01T00:00:00.000Z')", } }
 
-                         ]
+                         ], "etag": "BwWWja0YfJA=", "version": 3
 
                       }
 
-                   **YAML Example**
+                   **YAML example:**
 
                       bindings: - members: - user:\ mike@example.com -
                       group:\ admins@example.com - domain:google.com -
                       serviceAccount:\ my-project-id@appspot.gserviceaccount.com
                       role: roles/resourcemanager.organizationAdmin -
                       members: - user:\ eve@example.com role:
                       roles/resourcemanager.organizationViewer
                       condition: title: expirable access description:
                       Does not grant access after Sep 2020 expression:
                       request.time <
-                      timestamp('2020-10-01T00:00:00.000Z')
+                      timestamp('2020-10-01T00:00:00.000Z') etag:
+                      BwWWja0YfJA= version: 3
 
                    For a description of IAM and its features, see the
-                   [IAM developer's
-                   guide](\ https://cloud.google.com/iam/docs).
+                   [IAM
+                   documentation](\ https://cloud.google.com/iam/docs/).
 
         """
         # Create or coerce a protobuf request object.
         # Quick check: If we got a request object, we should *not* have
         # gotten any keyword arguments that map to the request.
         has_flattened_params = any([resource])
         if request is not None and has_flattened_params:
@@ -2227,69 +2233,75 @@
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
             google.iam.v1.policy_pb2.Policy:
-                Defines an Identity and Access Management (IAM) policy. It is used to
-                   specify access control policies for Cloud Platform
-                   resources.
+                An Identity and Access Management (IAM) policy, which specifies access
+                   controls for Google Cloud resources.
 
                    A Policy is a collection of bindings. A binding binds
-                   one or more members to a single role. Members can be
-                   user accounts, service accounts, Google groups, and
-                   domains (such as G Suite). A role is a named list of
-                   permissions (defined by IAM or configured by users).
-                   A binding can optionally specify a condition, which
-                   is a logic expression that further constrains the
-                   role binding based on attributes about the request
-                   and/or target resource.
+                   one or more members, or principals, to a single role.
+                   Principals can be user accounts, service accounts,
+                   Google groups, and domains (such as G Suite). A role
+                   is a named list of permissions; each role can be an
+                   IAM predefined role or a user-created custom role.
+
+                   For some types of Google Cloud resources, a binding
+                   can also specify a condition, which is a logical
+                   expression that allows access to a resource only if
+                   the expression evaluates to true. A condition can add
+                   constraints based on attributes of the request, the
+                   resource, or both. To learn which resources support
+                   conditions in their IAM policies, see the [IAM
+                   documentation](\ https://cloud.google.com/iam/help/conditions/resource-policies).
 
-                   **JSON Example**
+                   **JSON example:**
 
                       {
                          "bindings": [
                             {
                                "role":
                                "roles/resourcemanager.organizationAdmin",
                                "members": [ "user:mike@example.com",
                                "group:admins@example.com",
                                "domain:google.com",
                                "serviceAccount:my-project-id@appspot.gserviceaccount.com"
                                ]
 
                             }, { "role":
                             "roles/resourcemanager.organizationViewer",
-                            "members": ["user:eve@example.com"],
+                            "members": [ "user:eve@example.com" ],
                             "condition": { "title": "expirable access",
                             "description": "Does not grant access after
                             Sep 2020", "expression": "request.time <
                             timestamp('2020-10-01T00:00:00.000Z')", } }
 
-                         ]
+                         ], "etag": "BwWWja0YfJA=", "version": 3
 
                       }
 
-                   **YAML Example**
+                   **YAML example:**
 
                       bindings: - members: - user:\ mike@example.com -
                       group:\ admins@example.com - domain:google.com -
                       serviceAccount:\ my-project-id@appspot.gserviceaccount.com
                       role: roles/resourcemanager.organizationAdmin -
                       members: - user:\ eve@example.com role:
                       roles/resourcemanager.organizationViewer
                       condition: title: expirable access description:
                       Does not grant access after Sep 2020 expression:
                       request.time <
-                      timestamp('2020-10-01T00:00:00.000Z')
+                      timestamp('2020-10-01T00:00:00.000Z') etag:
+                      BwWWja0YfJA= version: 3
 
                    For a description of IAM and its features, see the
-                   [IAM developer's
-                   guide](\ https://cloud.google.com/iam/docs).
+                   [IAM
+                   documentation](\ https://cloud.google.com/iam/docs/).
 
         """
         # Create or coerce a protobuf request object.
         # Quick check: If we got a request object, we should *not* have
         # gotten any keyword arguments that map to the request.
         has_flattened_params = any([resource])
         if request is not None and has_flattened_params:
```

### Comparing `google-cloud-bigtable-2.8.1/google/cloud/bigtable_admin_v2/services/bigtable_table_admin/client.py` & `google-cloud-bigtable-2.9.0/google/cloud/bigtable_admin_v2/services/bigtable_table_admin/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 from collections import OrderedDict
 import os
 import re
-from typing import Dict, Optional, Sequence, Tuple, Type, Union
+from typing import Dict, Mapping, Optional, Sequence, Tuple, Type, Union
 import pkg_resources
 
 from google.api_core import client_options as client_options_lib
 from google.api_core import exceptions as core_exceptions
 from google.api_core import gapic_v1
 from google.api_core import retry as retries
 from google.auth import credentials as ga_credentials  # type: ignore
@@ -2333,69 +2333,75 @@
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
             google.iam.v1.policy_pb2.Policy:
-                Defines an Identity and Access Management (IAM) policy. It is used to
-                   specify access control policies for Cloud Platform
-                   resources.
+                An Identity and Access Management (IAM) policy, which specifies access
+                   controls for Google Cloud resources.
 
                    A Policy is a collection of bindings. A binding binds
-                   one or more members to a single role. Members can be
-                   user accounts, service accounts, Google groups, and
-                   domains (such as G Suite). A role is a named list of
-                   permissions (defined by IAM or configured by users).
-                   A binding can optionally specify a condition, which
-                   is a logic expression that further constrains the
-                   role binding based on attributes about the request
-                   and/or target resource.
+                   one or more members, or principals, to a single role.
+                   Principals can be user accounts, service accounts,
+                   Google groups, and domains (such as G Suite). A role
+                   is a named list of permissions; each role can be an
+                   IAM predefined role or a user-created custom role.
+
+                   For some types of Google Cloud resources, a binding
+                   can also specify a condition, which is a logical
+                   expression that allows access to a resource only if
+                   the expression evaluates to true. A condition can add
+                   constraints based on attributes of the request, the
+                   resource, or both. To learn which resources support
+                   conditions in their IAM policies, see the [IAM
+                   documentation](\ https://cloud.google.com/iam/help/conditions/resource-policies).
 
-                   **JSON Example**
+                   **JSON example:**
 
                       {
                          "bindings": [
                             {
                                "role":
                                "roles/resourcemanager.organizationAdmin",
                                "members": [ "user:mike@example.com",
                                "group:admins@example.com",
                                "domain:google.com",
                                "serviceAccount:my-project-id@appspot.gserviceaccount.com"
                                ]
 
                             }, { "role":
                             "roles/resourcemanager.organizationViewer",
-                            "members": ["user:eve@example.com"],
+                            "members": [ "user:eve@example.com" ],
                             "condition": { "title": "expirable access",
                             "description": "Does not grant access after
                             Sep 2020", "expression": "request.time <
                             timestamp('2020-10-01T00:00:00.000Z')", } }
 
-                         ]
+                         ], "etag": "BwWWja0YfJA=", "version": 3
 
                       }
 
-                   **YAML Example**
+                   **YAML example:**
 
                       bindings: - members: - user:\ mike@example.com -
                       group:\ admins@example.com - domain:google.com -
                       serviceAccount:\ my-project-id@appspot.gserviceaccount.com
                       role: roles/resourcemanager.organizationAdmin -
                       members: - user:\ eve@example.com role:
                       roles/resourcemanager.organizationViewer
                       condition: title: expirable access description:
                       Does not grant access after Sep 2020 expression:
                       request.time <
-                      timestamp('2020-10-01T00:00:00.000Z')
+                      timestamp('2020-10-01T00:00:00.000Z') etag:
+                      BwWWja0YfJA= version: 3
 
                    For a description of IAM and its features, see the
-                   [IAM developer's
-                   guide](\ https://cloud.google.com/iam/docs).
+                   [IAM
+                   documentation](\ https://cloud.google.com/iam/docs/).
 
         """
         # Create or coerce a protobuf request object.
         # Quick check: If we got a request object, we should *not* have
         # gotten any keyword arguments that map to the request.
         has_flattened_params = any([resource])
         if request is not None and has_flattened_params:
@@ -2464,69 +2470,75 @@
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
             google.iam.v1.policy_pb2.Policy:
-                Defines an Identity and Access Management (IAM) policy. It is used to
-                   specify access control policies for Cloud Platform
-                   resources.
+                An Identity and Access Management (IAM) policy, which specifies access
+                   controls for Google Cloud resources.
 
                    A Policy is a collection of bindings. A binding binds
-                   one or more members to a single role. Members can be
-                   user accounts, service accounts, Google groups, and
-                   domains (such as G Suite). A role is a named list of
-                   permissions (defined by IAM or configured by users).
-                   A binding can optionally specify a condition, which
-                   is a logic expression that further constrains the
-                   role binding based on attributes about the request
-                   and/or target resource.
+                   one or more members, or principals, to a single role.
+                   Principals can be user accounts, service accounts,
+                   Google groups, and domains (such as G Suite). A role
+                   is a named list of permissions; each role can be an
+                   IAM predefined role or a user-created custom role.
+
+                   For some types of Google Cloud resources, a binding
+                   can also specify a condition, which is a logical
+                   expression that allows access to a resource only if
+                   the expression evaluates to true. A condition can add
+                   constraints based on attributes of the request, the
+                   resource, or both. To learn which resources support
+                   conditions in their IAM policies, see the [IAM
+                   documentation](\ https://cloud.google.com/iam/help/conditions/resource-policies).
 
-                   **JSON Example**
+                   **JSON example:**
 
                       {
                          "bindings": [
                             {
                                "role":
                                "roles/resourcemanager.organizationAdmin",
                                "members": [ "user:mike@example.com",
                                "group:admins@example.com",
                                "domain:google.com",
                                "serviceAccount:my-project-id@appspot.gserviceaccount.com"
                                ]
 
                             }, { "role":
                             "roles/resourcemanager.organizationViewer",
-                            "members": ["user:eve@example.com"],
+                            "members": [ "user:eve@example.com" ],
                             "condition": { "title": "expirable access",
                             "description": "Does not grant access after
                             Sep 2020", "expression": "request.time <
                             timestamp('2020-10-01T00:00:00.000Z')", } }
 
-                         ]
+                         ], "etag": "BwWWja0YfJA=", "version": 3
 
                       }
 
-                   **YAML Example**
+                   **YAML example:**
 
                       bindings: - members: - user:\ mike@example.com -
                       group:\ admins@example.com - domain:google.com -
                       serviceAccount:\ my-project-id@appspot.gserviceaccount.com
                       role: roles/resourcemanager.organizationAdmin -
                       members: - user:\ eve@example.com role:
                       roles/resourcemanager.organizationViewer
                       condition: title: expirable access description:
                       Does not grant access after Sep 2020 expression:
                       request.time <
-                      timestamp('2020-10-01T00:00:00.000Z')
+                      timestamp('2020-10-01T00:00:00.000Z') etag:
+                      BwWWja0YfJA= version: 3
 
                    For a description of IAM and its features, see the
-                   [IAM developer's
-                   guide](\ https://cloud.google.com/iam/docs).
+                   [IAM
+                   documentation](\ https://cloud.google.com/iam/docs/).
 
         """
         # Create or coerce a protobuf request object.
         # Quick check: If we got a request object, we should *not* have
         # gotten any keyword arguments that map to the request.
         has_flattened_params = any([resource])
         if request is not None and has_flattened_params:
```

### Comparing `google-cloud-bigtable-2.8.1/google/cloud/bigtable_admin_v2/services/bigtable_table_admin/pagers.py` & `google-cloud-bigtable-2.9.0/google/cloud/bigtable_admin_v2/services/bigtable_table_admin/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigtable-2.8.1/google/cloud/bigtable_admin_v2/services/bigtable_table_admin/transports/__init__.py` & `google-cloud-bigtable-2.9.0/google/cloud/bigtable_admin_v2/services/bigtable_table_admin/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigtable-2.8.1/google/cloud/bigtable_admin_v2/services/bigtable_table_admin/transports/base.py` & `google-cloud-bigtable-2.9.0/google/cloud/bigtable_admin_v2/services/bigtable_table_admin/transports/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -90,14 +90,15 @@
                 The client info used to send a user-agent string along with
                 API requests. If ``None``, then default info will be used.
                 Generally, you only need to set this if you're developing
                 your own client library.
             always_use_jwt_access (Optional[bool]): Whether self signed JWT should
                 be used for service account credentials.
         """
+
         # Save the hostname. Default to port 443 (HTTPS) if none is specified.
         if ":" not in host:
             host += ":443"
         self._host = host
 
         scopes_kwargs = {"scopes": scopes, "default_scopes": self.AUTH_SCOPES}
 
@@ -572,9 +573,13 @@
         Union[
             iam_policy_pb2.TestIamPermissionsResponse,
             Awaitable[iam_policy_pb2.TestIamPermissionsResponse],
         ],
     ]:
         raise NotImplementedError()
 
+    @property
+    def kind(self) -> str:
+        raise NotImplementedError()
+
 
 __all__ = ("BigtableTableAdminTransport",)
```

### Comparing `google-cloud-bigtable-2.8.1/google/cloud/bigtable_admin_v2/services/bigtable_table_admin/transports/grpc.py` & `google-cloud-bigtable-2.9.0/google/cloud/bigtable_admin_v2/services/bigtable_table_admin/transports/grpc.py`

 * *Files 0% similar despite different names*

```diff
@@ -921,9 +921,13 @@
                 response_deserializer=iam_policy_pb2.TestIamPermissionsResponse.FromString,
             )
         return self._stubs["test_iam_permissions"]
 
     def close(self):
         self.grpc_channel.close()
 
+    @property
+    def kind(self) -> str:
+        return "grpc"
+
 
 __all__ = ("BigtableTableAdminGrpcTransport",)
```

### Comparing `google-cloud-bigtable-2.8.1/google/cloud/bigtable_admin_v2/services/bigtable_table_admin/transports/grpc_asyncio.py` & `google-cloud-bigtable-2.9.0/google/cloud/bigtable_admin_v2/services/bigtable_table_admin/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigtable-2.8.1/google/cloud/bigtable_admin_v2/types/__init__.py` & `google-cloud-bigtable-2.9.0/google/cloud/bigtable_admin_v2/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigtable-2.8.1/google/cloud/bigtable_admin_v2/types/bigtable_instance_admin.py` & `google-cloud-bigtable-2.9.0/google/cloud/bigtable_admin_v2/types/bigtable_instance_admin.py`

 * *Files 0% similar despite different names*

```diff
@@ -64,15 +64,15 @@
         instance_id (str):
             Required. The ID to be used when referring to the new
             instance within its project, e.g., just ``myinstance``
             rather than ``projects/myproject/instances/myinstance``.
         instance (google.cloud.bigtable_admin_v2.types.Instance):
             Required. The instance to create. Fields marked
             ``OutputOnly`` must be left blank.
-        clusters (Sequence[google.cloud.bigtable_admin_v2.types.CreateInstanceRequest.ClustersEntry]):
+        clusters (Mapping[str, google.cloud.bigtable_admin_v2.types.Cluster]):
             Required. The clusters to be created within the instance,
             mapped by desired cluster ID, e.g., just ``mycluster``
             rather than
             ``projects/myproject/instances/myinstance/clusters/mycluster``.
             Fields marked ``OutputOnly`` must be left blank. Currently,
             at most four clusters can be specified.
     """
```

### Comparing `google-cloud-bigtable-2.8.1/google/cloud/bigtable_admin_v2/types/bigtable_table_admin.py` & `google-cloud-bigtable-2.9.0/google/cloud/bigtable_admin_v2/types/bigtable_table_admin.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigtable-2.8.1/google/cloud/bigtable_admin_v2/types/common.py` & `google-cloud-bigtable-2.9.0/google/cloud/bigtable_admin_v2/types/common.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigtable-2.8.1/google/cloud/bigtable_admin_v2/types/instance.py` & `google-cloud-bigtable-2.9.0/google/cloud/bigtable_admin_v2/types/instance.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,15 +47,15 @@
             instance as it appears in UIs. Can be changed at
             any time, but should be kept globally unique to
             avoid confusion.
         state (google.cloud.bigtable_admin_v2.types.Instance.State):
             (``OutputOnly``) The current state of the instance.
         type_ (google.cloud.bigtable_admin_v2.types.Instance.Type):
             The type of the instance. Defaults to ``PRODUCTION``.
-        labels (Sequence[google.cloud.bigtable_admin_v2.types.Instance.LabelsEntry]):
+        labels (Mapping[str, str]):
             Labels are a flexible and lightweight mechanism for
             organizing cloud resources into groups that reflect a
             customer's organizational needs and deployment strategies.
             They can be used to filter resources and aggregate metrics.
 
             -  Label keys must be between 1 and 63 characters long and
                must conform to the regular expression:
```

### Comparing `google-cloud-bigtable-2.8.1/google/cloud/bigtable_admin_v2/types/table.py` & `google-cloud-bigtable-2.9.0/google/cloud/bigtable_admin_v2/types/table.py`

 * *Files 2% similar despite different names*

```diff
@@ -77,22 +77,22 @@
 
     Attributes:
         name (str):
             The unique name of the table. Values are of the form
             ``projects/{project}/instances/{instance}/tables/[_a-zA-Z0-9][-_.a-zA-Z0-9]*``.
             Views: ``NAME_ONLY``, ``SCHEMA_VIEW``, ``REPLICATION_VIEW``,
             ``FULL``
-        cluster_states (Sequence[google.cloud.bigtable_admin_v2.types.Table.ClusterStatesEntry]):
+        cluster_states (Mapping[str, google.cloud.bigtable_admin_v2.types.Table.ClusterState]):
             Output only. Map from cluster ID to per-cluster table state.
             If it could not be determined whether or not the table has
             data in a particular cluster (for example, if its zone is
             unavailable), then there will be an entry for the cluster
             with UNKNOWN ``replication_status``. Views:
             ``REPLICATION_VIEW``, ``ENCRYPTION_VIEW``, ``FULL``
-        column_families (Sequence[google.cloud.bigtable_admin_v2.types.Table.ColumnFamiliesEntry]):
+        column_families (Mapping[str, google.cloud.bigtable_admin_v2.types.ColumnFamily]):
             (``CreationOnly``) The column families configured for this
             table, mapped by column family ID. Views: ``SCHEMA_VIEW``,
             ``FULL``
         granularity (google.cloud.bigtable_admin_v2.types.Table.TimestampGranularity):
             (``CreationOnly``) The granularity (i.e. ``MILLIS``) at
             which timestamps are stored in this table. Timestamps not
             matching the granularity will be rejected. If unspecified at
```

### Comparing `google-cloud-bigtable-2.8.1/google/cloud/bigtable_v2/__init__.py` & `google-cloud-bigtable-2.9.0/google/cloud/bigtable_v2/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigtable-2.8.1/google/cloud/bigtable_v2/gapic_metadata.json` & `google-cloud-bigtable-2.9.0/google/cloud/bigtable_v2/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-cloud-bigtable-2.8.1/google/cloud/bigtable_v2/services/__init__.py` & `google-cloud-bigtable-2.9.0/google/cloud/bigtable_v2/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigtable-2.8.1/google/cloud/bigtable_v2/services/bigtable/__init__.py` & `google-cloud-bigtable-2.9.0/google/cloud/bigtable_v2/services/bigtable/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigtable-2.8.1/google/cloud/bigtable_v2/services/bigtable/async_client.py` & `google-cloud-bigtable-2.9.0/google/cloud/bigtable_v2/services/bigtable/async_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 # limitations under the License.
 #
 from collections import OrderedDict
 import functools
 import re
 from typing import (
     Dict,
+    Mapping,
     Optional,
     AsyncIterable,
     Awaitable,
     Sequence,
     Tuple,
     Type,
     Union,
```

### Comparing `google-cloud-bigtable-2.8.1/google/cloud/bigtable_v2/services/bigtable/client.py` & `google-cloud-bigtable-2.9.0/google/cloud/bigtable_v2/services/bigtable/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 from collections import OrderedDict
 import os
 import re
-from typing import Dict, Optional, Iterable, Sequence, Tuple, Type, Union
+from typing import Dict, Mapping, Optional, Iterable, Sequence, Tuple, Type, Union
 import pkg_resources
 
 from google.api_core import client_options as client_options_lib
 from google.api_core import exceptions as core_exceptions
 from google.api_core import gapic_v1
 from google.api_core import retry as retries
 from google.auth import credentials as ga_credentials  # type: ignore
```

### Comparing `google-cloud-bigtable-2.8.1/google/cloud/bigtable_v2/services/bigtable/transports/__init__.py` & `google-cloud-bigtable-2.9.0/google/cloud/bigtable_v2/services/bigtable/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigtable-2.8.1/google/cloud/bigtable_v2/services/bigtable/transports/base.py` & `google-cloud-bigtable-2.9.0/google/cloud/bigtable_v2/services/bigtable/transports/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -83,14 +83,15 @@
                 The client info used to send a user-agent string along with
                 API requests. If ``None``, then default info will be used.
                 Generally, you only need to set this if you're developing
                 your own client library.
             always_use_jwt_access (Optional[bool]): Whether self signed JWT should
                 be used for service account credentials.
         """
+
         # Save the hostname. Default to port 443 (HTTPS) if none is specified.
         if ":" not in host:
             host += ":443"
         self._host = host
 
         scopes_kwargs = {"scopes": scopes, "default_scopes": self.AUTH_SCOPES}
 
@@ -250,9 +251,13 @@
         Union[
             bigtable.ReadModifyWriteRowResponse,
             Awaitable[bigtable.ReadModifyWriteRowResponse],
         ],
     ]:
         raise NotImplementedError()
 
+    @property
+    def kind(self) -> str:
+        raise NotImplementedError()
+
 
 __all__ = ("BigtableTransport",)
```

### Comparing `google-cloud-bigtable-2.8.1/google/cloud/bigtable_v2/services/bigtable/transports/grpc.py` & `google-cloud-bigtable-2.9.0/google/cloud/bigtable_v2/services/bigtable/transports/grpc.py`

 * *Files 1% similar despite different names*

```diff
@@ -434,9 +434,13 @@
                 response_deserializer=bigtable.ReadModifyWriteRowResponse.deserialize,
             )
         return self._stubs["read_modify_write_row"]
 
     def close(self):
         self.grpc_channel.close()
 
+    @property
+    def kind(self) -> str:
+        return "grpc"
+
 
 __all__ = ("BigtableGrpcTransport",)
```

### Comparing `google-cloud-bigtable-2.8.1/google/cloud/bigtable_v2/services/bigtable/transports/grpc_asyncio.py` & `google-cloud-bigtable-2.9.0/google/cloud/bigtable_v2/services/bigtable/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigtable-2.8.1/google/cloud/bigtable_v2/types/__init__.py` & `google-cloud-bigtable-2.9.0/google/cloud/bigtable_v2/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigtable-2.8.1/google/cloud/bigtable_v2/types/bigtable.py` & `google-cloud-bigtable-2.9.0/google/cloud/bigtable_v2/types/bigtable.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigtable-2.8.1/google/cloud/bigtable_v2/types/data.py` & `google-cloud-bigtable-2.9.0/google/cloud/bigtable_v2/types/data.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigtable-2.8.1/google_cloud_bigtable.egg-info/PKG-INFO` & `google-cloud-bigtable-2.9.0/google_cloud_bigtable.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-bigtable
-Version: 2.8.1
+Version: 2.9.0
 Summary: Google Cloud Bigtable API client library
 Home-page: https://github.com/googleapis/python-bigtable
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `google-cloud-bigtable-2.8.1/google_cloud_bigtable.egg-info/SOURCES.txt` & `google-cloud-bigtable-2.9.0/google_cloud_bigtable.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `google-cloud-bigtable-2.8.1/scripts/fixup_bigtable_admin_v2_keywords.py` & `google-cloud-bigtable-2.9.0/scripts/fixup_bigtable_admin_v2_keywords.py`

 * *Files 0% similar despite different names*

```diff
@@ -68,15 +68,15 @@
         'list_instances': ('parent', 'page_token', ),
         'list_snapshots': ('parent', 'page_size', 'page_token', ),
         'list_tables': ('parent', 'view', 'page_size', 'page_token', ),
         'modify_column_families': ('name', 'modifications', ),
         'partial_update_cluster': ('cluster', 'update_mask', ),
         'partial_update_instance': ('instance', 'update_mask', ),
         'restore_table': ('parent', 'table_id', 'backup', ),
-        'set_iam_policy': ('resource', 'policy', ),
+        'set_iam_policy': ('resource', 'policy', 'update_mask', ),
         'snapshot_table': ('name', 'cluster', 'snapshot_id', 'ttl', 'description', ),
         'test_iam_permissions': ('resource', 'permissions', ),
         'update_app_profile': ('app_profile', 'update_mask', 'ignore_warnings', ),
         'update_backup': ('backup', 'update_mask', ),
         'update_cluster': ('name', 'location', 'state', 'serve_nodes', 'cluster_config', 'default_storage_type', 'encryption_config', ),
         'update_instance': ('display_name', 'name', 'state', 'type_', 'labels', 'create_time', ),
     }
```

### Comparing `google-cloud-bigtable-2.8.1/scripts/fixup_bigtable_v2_keywords.py` & `google-cloud-bigtable-2.9.0/scripts/fixup_bigtable_v2_keywords.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigtable-2.8.1/setup.py` & `google-cloud-bigtable-2.9.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,30 +18,30 @@
 import setuptools
 
 
 # Package metadata.
 
 name = "google-cloud-bigtable"
 description = "Google Cloud Bigtable API client library"
-version = "2.8.1"
+version = "2.9.0"
 # Should be one of:
 # 'Development Status :: 3 - Alpha'
 # 'Development Status :: 4 - Beta'
 # 'Development Status :: 5 - Production/Stable'
 release_status = "Development Status :: 5 - Production/Stable"
 dependencies = [
     # NOTE: Maintainers, please do not require google-api-core>=2.x.x
     # Until this issue is closed
     # https://github.com/googleapis/google-cloud-python/issues/10566
     "google-api-core[grpc] >= 1.31.5, <3.0.0dev,!=2.0.*,!=2.1.*,!=2.2.*,!=2.3.0",
     # NOTE: Maintainers, please do not require google-api-core>=2.x.x
     # Until this issue is closed
     # https://github.com/googleapis/google-cloud-python/issues/10566
     "google-cloud-core >= 1.4.1, <3.0.0dev",
-    "grpc-google-iam-v1 >= 0.12.3, < 0.13dev",
+    "grpc-google-iam-v1 >= 0.12.4, <1.0.0dev",
     "proto-plus >= 1.18.0",
 ]
 extras = {"libcst": "libcst >= 0.2.5"}
 
 
 # Setup boilerplate below this line.
```

### Comparing `google-cloud-bigtable-2.8.1/tests/__init__.py` & `google-cloud-bigtable-2.9.0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigtable-2.8.1/tests/system/__init__.py` & `google-cloud-bigtable-2.9.0/tests/system/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigtable-2.8.1/tests/system/_helpers.py` & `google-cloud-bigtable-2.9.0/tests/system/_helpers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigtable-2.8.1/tests/system/conftest.py` & `google-cloud-bigtable-2.9.0/tests/system/conftest.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigtable-2.8.1/tests/system/test_data_api.py` & `google-cloud-bigtable-2.9.0/tests/system/test_data_api.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigtable-2.8.1/tests/system/test_instance_admin.py` & `google-cloud-bigtable-2.9.0/tests/system/test_instance_admin.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,40 +20,43 @@
 
 def _create_app_profile_helper(
     app_profile_id,
     instance,
     routing_policy_type,
     description=None,
     cluster_id=None,
+    multi_cluster_ids=None,
     allow_transactional_writes=None,
     ignore_warnings=None,
 ):
 
     app_profile = instance.app_profile(
         app_profile_id=app_profile_id,
         routing_policy_type=routing_policy_type,
         description=description,
         cluster_id=cluster_id,
+        multi_cluster_ids=multi_cluster_ids,
         allow_transactional_writes=allow_transactional_writes,
     )
     assert app_profile.allow_transactional_writes == allow_transactional_writes
 
     app_profile.create(ignore_warnings=ignore_warnings)
 
     # Load a different app_profile objec form the server and
-    # verrify that it is the same
+    # verify that it is the same
     alt_app_profile = instance.app_profile(app_profile_id)
     alt_app_profile.reload()
 
     app_profile.app_profile_id == alt_app_profile.app_profile_id
     app_profile.routing_policy_type == routing_policy_type
     alt_app_profile.routing_policy_type == routing_policy_type
     app_profile.description == alt_app_profile.description
     assert not app_profile.allow_transactional_writes
     assert not alt_app_profile.allow_transactional_writes
+    assert app_profile.multi_cluster_ids == alt_app_profile.multi_cluster_ids
 
     return app_profile
 
 
 def _list_app_profiles_helper(instance, expected_app_profile_ids):
     app_profiles = instance.list_app_profiles()
     found = [app_prof.app_profile_id for app_prof in app_profiles]
@@ -63,34 +66,37 @@
 
 def _modify_app_profile_helper(
     app_profile_id,
     instance,
     routing_policy_type,
     description=None,
     cluster_id=None,
+    multi_cluster_ids=None,
     allow_transactional_writes=None,
     ignore_warnings=None,
 ):
     app_profile = instance.app_profile(
         app_profile_id=app_profile_id,
         routing_policy_type=routing_policy_type,
         description=description,
         cluster_id=cluster_id,
+        multi_cluster_ids=multi_cluster_ids,
         allow_transactional_writes=allow_transactional_writes,
     )
 
     operation = app_profile.update(ignore_warnings=ignore_warnings)
     operation.result(timeout=60)
 
     alt_profile = instance.app_profile(app_profile_id)
     alt_profile.reload()
 
     assert alt_profile.description == description
     assert alt_profile.routing_policy_type == routing_policy_type
     assert alt_profile.cluster_id == cluster_id
+    assert alt_profile.multi_cluster_ids == multi_cluster_ids
     assert alt_profile.allow_transactional_writes == allow_transactional_writes
 
 
 def _delete_app_profile_helper(app_profile):
     assert app_profile.exists()
     app_profile.delete(ignore_warnings=True)
     assert not app_profile.exists()
@@ -391,14 +397,107 @@
     )
 
     # Test delete app profiles
     for app_profile in app_profiles_to_delete:
         _delete_app_profile_helper(app_profile)
 
 
+def test_instance_create_app_profile_create_with_multi_cluster_ids(
+    admin_client,
+    unique_suffix,
+    admin_instance_populated,
+    admin_cluster,
+    location_id,
+    instance_labels,
+    instances_to_delete,
+    skip_on_emulator,
+):
+    alt_instance_id = f"dif{unique_suffix}"
+    instance = admin_client.instance(
+        alt_instance_id,
+        instance_type=enums.Instance.Type.PRODUCTION,
+        labels=instance_labels,
+    )
+
+    serve_nodes = 1
+
+    alt_cluster_id_1 = f"{alt_instance_id}-c1"
+    cluster_1 = instance.cluster(
+        alt_cluster_id_1,
+        location_id=location_id,
+        serve_nodes=serve_nodes,
+        default_storage_type=enums.StorageType.HDD,
+    )
+
+    alt_cluster_id_2 = f"{alt_instance_id}-c2"
+    location_id_2 = "us-central1-f"
+    cluster_2 = instance.cluster(
+        alt_cluster_id_2,
+        location_id=location_id_2,
+        serve_nodes=serve_nodes,
+        default_storage_type=enums.StorageType.HDD,
+    )
+    operation = instance.create(clusters=[cluster_1, cluster_2])
+    instances_to_delete.append(instance)
+    operation.result(timeout=240)  # Ensure the operation completes.
+
+    # Create a new instance and make sure it is the same.
+    instance_alt = admin_client.instance(alt_instance_id)
+    instance_alt.reload()
+
+    assert instance == instance_alt
+    assert instance.display_name == instance_alt.display_name
+    assert instance.type_ == instance_alt.type_
+
+    clusters, failed_locations = instance_alt.list_clusters()
+    assert failed_locations == []
+    alt_cluster_1, alt_cluster_2 = sorted(clusters, key=lambda x: x.name)
+
+    assert cluster_1.location_id == alt_cluster_1.location_id
+    assert cluster_2.location_id == alt_cluster_2.location_id
+
+    # Test create app profile with multi_cluster_routing policy
+    app_profiles_to_delete = []
+    description = "routing policy-multi"
+    app_profile_id_1 = "app_profile_id_1"
+    routing = enums.RoutingPolicyType.ANY
+
+    multi_cluster_ids = [alt_cluster_id_1, alt_cluster_id_2]
+    app_profile_1 = _create_app_profile_helper(
+        app_profile_id_1,
+        instance,
+        routing_policy_type=routing,
+        description=description,
+        ignore_warnings=True,
+        multi_cluster_ids=multi_cluster_ids,
+    )
+    assert len(app_profile_1.multi_cluster_ids) == len(multi_cluster_ids)
+    assert app_profile_1.multi_cluster_ids == multi_cluster_ids
+
+    # remove a cluster from the multi_cluster_ids
+    app_profile_1.multi_cluster_ids.pop()
+    app_profile_1.update()
+
+    assert len(app_profile_1.multi_cluster_ids) == 1
+    assert app_profile_1.multi_cluster_ids == [alt_cluster_id_1]
+
+    # add a cluster from the multi_cluster_ids
+    app_profile_1.multi_cluster_ids.append(alt_cluster_id_2)
+    app_profile_1.update()
+
+    assert len(app_profile_1.multi_cluster_ids) == 2
+    assert app_profile_1.multi_cluster_ids == [alt_cluster_id_1, alt_cluster_id_2]
+
+    app_profiles_to_delete.append(app_profile_1)
+
+    # # Test delete app profiles
+    for app_profile in app_profiles_to_delete:
+        _delete_app_profile_helper(app_profile)
+
+
 def test_instance_create_w_two_clusters_cmek(
     admin_client,
     unique_suffix,
     admin_instance_populated,
     admin_cluster,
     location_id,
     instance_labels,
```

### Comparing `google-cloud-bigtable-2.8.1/tests/system/test_table_admin.py` & `google-cloud-bigtable-2.9.0/tests/system/test_table_admin.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigtable-2.8.1/tests/unit/__init__.py` & `google-cloud-bigtable-2.9.0/tests/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigtable-2.8.1/tests/unit/_testing.py` & `google-cloud-bigtable-2.9.0/tests/unit/_testing.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigtable-2.8.1/tests/unit/gapic/__init__.py` & `google-cloud-bigtable-2.9.0/tests/unit/gapic/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigtable-2.8.1/tests/unit/gapic/bigtable_admin_v2/__init__.py` & `google-cloud-bigtable-2.9.0/tests/unit/gapic/bigtable_admin_v2/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigtable-2.8.1/tests/unit/gapic/bigtable_admin_v2/test_bigtable_instance_admin.py` & `google-cloud-bigtable-2.9.0/tests/unit/gapic/bigtable_admin_v2/test_bigtable_instance_admin.py`

 * *Files 1% similar despite different names*

```diff
@@ -100,32 +100,34 @@
     assert (
         BigtableInstanceAdminClient._get_default_mtls_endpoint(non_googleapi)
         == non_googleapi
     )
 
 
 @pytest.mark.parametrize(
-    "client_class",
+    "client_class,transport_name",
     [
-        BigtableInstanceAdminClient,
-        BigtableInstanceAdminAsyncClient,
+        (BigtableInstanceAdminClient, "grpc"),
+        (BigtableInstanceAdminAsyncClient, "grpc_asyncio"),
     ],
 )
-def test_bigtable_instance_admin_client_from_service_account_info(client_class):
+def test_bigtable_instance_admin_client_from_service_account_info(
+    client_class, transport_name
+):
     creds = ga_credentials.AnonymousCredentials()
     with mock.patch.object(
         service_account.Credentials, "from_service_account_info"
     ) as factory:
         factory.return_value = creds
         info = {"valid": True}
-        client = client_class.from_service_account_info(info)
+        client = client_class.from_service_account_info(info, transport=transport_name)
         assert client.transport._credentials == creds
         assert isinstance(client, client_class)
 
-        assert client.transport._host == "bigtableadmin.googleapis.com:443"
+        assert client.transport._host == ("bigtableadmin.googleapis.com:443")
 
 
 @pytest.mark.parametrize(
     "transport_class,transport_name",
     [
         (transports.BigtableInstanceAdminGrpcTransport, "grpc"),
         (transports.BigtableInstanceAdminGrpcAsyncIOTransport, "grpc_asyncio"),
@@ -146,35 +148,41 @@
     ) as use_jwt:
         creds = service_account.Credentials(None, None, None)
         transport = transport_class(credentials=creds, always_use_jwt_access=False)
         use_jwt.assert_not_called()
 
 
 @pytest.mark.parametrize(
-    "client_class",
+    "client_class,transport_name",
     [
-        BigtableInstanceAdminClient,
-        BigtableInstanceAdminAsyncClient,
+        (BigtableInstanceAdminClient, "grpc"),
+        (BigtableInstanceAdminAsyncClient, "grpc_asyncio"),
     ],
 )
-def test_bigtable_instance_admin_client_from_service_account_file(client_class):
+def test_bigtable_instance_admin_client_from_service_account_file(
+    client_class, transport_name
+):
     creds = ga_credentials.AnonymousCredentials()
     with mock.patch.object(
         service_account.Credentials, "from_service_account_file"
     ) as factory:
         factory.return_value = creds
-        client = client_class.from_service_account_file("dummy/file/path.json")
+        client = client_class.from_service_account_file(
+            "dummy/file/path.json", transport=transport_name
+        )
         assert client.transport._credentials == creds
         assert isinstance(client, client_class)
 
-        client = client_class.from_service_account_json("dummy/file/path.json")
+        client = client_class.from_service_account_json(
+            "dummy/file/path.json", transport=transport_name
+        )
         assert client.transport._credentials == creds
         assert isinstance(client, client_class)
 
-        assert client.transport._host == "bigtableadmin.googleapis.com:443"
+        assert client.transport._host == ("bigtableadmin.googleapis.com:443")
 
 
 def test_bigtable_instance_admin_client_get_transport_class():
     transport = BigtableInstanceAdminClient.get_transport_class()
     available_transports = [
         transports.BigtableInstanceAdminGrpcTransport,
     ]
@@ -4306,15 +4314,15 @@
             RuntimeError,
         )
         async_pager = await client.list_app_profiles(
             request={},
         )
         assert async_pager.next_page_token == "abc"
         responses = []
-        async for response in async_pager:
+        async for response in async_pager:  # pragma: no branch
             responses.append(response)
 
         assert len(responses) == 6
         assert all(isinstance(i, instance.AppProfile) for i in responses)
 
 
 @pytest.mark.asyncio
@@ -4354,15 +4362,17 @@
                     instance.AppProfile(),
                     instance.AppProfile(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (await client.list_app_profiles(request={})).pages:
+        async for page_ in (
+            await client.list_app_profiles(request={})
+        ).pages:  # pragma: no branch
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
@@ -5259,14 +5269,15 @@
     with mock.patch.object(type(client.transport.set_iam_policy), "__call__") as call:
         # Designate an appropriate return value for the call.
         call.return_value = policy_pb2.Policy()
         response = client.set_iam_policy(
             request={
                 "resource": "resource_value",
                 "policy": policy_pb2.Policy(version=774),
+                "update_mask": field_mask_pb2.FieldMask(paths=["paths_value"]),
             }
         )
         call.assert_called()
 
 
 def test_set_iam_policy_flattened():
     client = BigtableInstanceAdminClient(
@@ -5987,15 +5998,15 @@
             RuntimeError,
         )
         async_pager = await client.list_hot_tablets(
             request={},
         )
         assert async_pager.next_page_token == "abc"
         responses = []
-        async for response in async_pager:
+        async for response in async_pager:  # pragma: no branch
             responses.append(response)
 
         assert len(responses) == 6
         assert all(isinstance(i, instance.HotTablet) for i in responses)
 
 
 @pytest.mark.asyncio
@@ -6033,15 +6044,17 @@
                     instance.HotTablet(),
                     instance.HotTablet(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (await client.list_hot_tablets(request={})).pages:
+        async for page_ in (
+            await client.list_hot_tablets(request={})
+        ).pages:  # pragma: no branch
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 def test_credentials_transport_error():
     # It is an error to provide credentials and a transport instance.
@@ -6130,14 +6143,27 @@
     # Test default credentials are used if not provided.
     with mock.patch.object(google.auth, "default") as adc:
         adc.return_value = (ga_credentials.AnonymousCredentials(), None)
         transport_class()
         adc.assert_called_once()
 
 
+@pytest.mark.parametrize(
+    "transport_name",
+    [
+        "grpc",
+    ],
+)
+def test_transport_kind(transport_name):
+    transport = BigtableInstanceAdminClient.get_transport_class(transport_name)(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
+    assert transport.kind == transport_name
+
+
 def test_transport_grpc_default():
     # A client should use the gRPC transport by default.
     client = BigtableInstanceAdminClient(
         credentials=ga_credentials.AnonymousCredentials(),
     )
     assert isinstance(
         client.transport,
@@ -6197,14 +6223,22 @@
         transport.close()
 
     # Additionally, the LRO client (a property) should
     # also raise NotImplementedError
     with pytest.raises(NotImplementedError):
         transport.operations_client
 
+    # Catch all for all remaining methods and properties
+    remainder = [
+        "kind",
+    ]
+    for r in remainder:
+        with pytest.raises(NotImplementedError):
+            getattr(transport, r)()
+
 
 def test_bigtable_instance_admin_base_transport_with_credentials_file():
     # Instantiate the base transport with a credentials file
     with mock.patch.object(
         google.auth, "load_credentials_from_file", autospec=True
     ) as load_creds, mock.patch(
         "google.cloud.bigtable_admin_v2.services.bigtable_instance_admin.transports.BigtableInstanceAdminTransport._prep_wrapped_messages"
@@ -6378,32 +6412,48 @@
             )
             expected_cert, expected_key = client_cert_source_callback()
             mock_ssl_cred.assert_called_once_with(
                 certificate_chain=expected_cert, private_key=expected_key
             )
 
 
-def test_bigtable_instance_admin_host_no_port():
+@pytest.mark.parametrize(
+    "transport_name",
+    [
+        "grpc",
+        "grpc_asyncio",
+    ],
+)
+def test_bigtable_instance_admin_host_no_port(transport_name):
     client = BigtableInstanceAdminClient(
         credentials=ga_credentials.AnonymousCredentials(),
         client_options=client_options.ClientOptions(
             api_endpoint="bigtableadmin.googleapis.com"
         ),
+        transport=transport_name,
     )
-    assert client.transport._host == "bigtableadmin.googleapis.com:443"
+    assert client.transport._host == ("bigtableadmin.googleapis.com:443")
 
 
-def test_bigtable_instance_admin_host_with_port():
+@pytest.mark.parametrize(
+    "transport_name",
+    [
+        "grpc",
+        "grpc_asyncio",
+    ],
+)
+def test_bigtable_instance_admin_host_with_port(transport_name):
     client = BigtableInstanceAdminClient(
         credentials=ga_credentials.AnonymousCredentials(),
         client_options=client_options.ClientOptions(
             api_endpoint="bigtableadmin.googleapis.com:8000"
         ),
+        transport=transport_name,
     )
-    assert client.transport._host == "bigtableadmin.googleapis.com:8000"
+    assert client.transport._host == ("bigtableadmin.googleapis.com:8000")
 
 
 def test_bigtable_instance_admin_grpc_transport_channel():
     channel = grpc.secure_channel("http://localhost/", grpc.local_channel_credentials())
 
     # Check that channel is used if provided.
     transport = transports.BigtableInstanceAdminGrpcTransport(
```

### Comparing `google-cloud-bigtable-2.8.1/tests/unit/gapic/bigtable_admin_v2/test_bigtable_table_admin.py` & `google-cloud-bigtable-2.9.0/tests/unit/gapic/bigtable_admin_v2/test_bigtable_table_admin.py`

 * *Files 2% similar despite different names*

```diff
@@ -102,32 +102,34 @@
     assert (
         BigtableTableAdminClient._get_default_mtls_endpoint(non_googleapi)
         == non_googleapi
     )
 
 
 @pytest.mark.parametrize(
-    "client_class",
+    "client_class,transport_name",
     [
-        BigtableTableAdminClient,
-        BigtableTableAdminAsyncClient,
+        (BigtableTableAdminClient, "grpc"),
+        (BigtableTableAdminAsyncClient, "grpc_asyncio"),
     ],
 )
-def test_bigtable_table_admin_client_from_service_account_info(client_class):
+def test_bigtable_table_admin_client_from_service_account_info(
+    client_class, transport_name
+):
     creds = ga_credentials.AnonymousCredentials()
     with mock.patch.object(
         service_account.Credentials, "from_service_account_info"
     ) as factory:
         factory.return_value = creds
         info = {"valid": True}
-        client = client_class.from_service_account_info(info)
+        client = client_class.from_service_account_info(info, transport=transport_name)
         assert client.transport._credentials == creds
         assert isinstance(client, client_class)
 
-        assert client.transport._host == "bigtableadmin.googleapis.com:443"
+        assert client.transport._host == ("bigtableadmin.googleapis.com:443")
 
 
 @pytest.mark.parametrize(
     "transport_class,transport_name",
     [
         (transports.BigtableTableAdminGrpcTransport, "grpc"),
         (transports.BigtableTableAdminGrpcAsyncIOTransport, "grpc_asyncio"),
@@ -148,35 +150,41 @@
     ) as use_jwt:
         creds = service_account.Credentials(None, None, None)
         transport = transport_class(credentials=creds, always_use_jwt_access=False)
         use_jwt.assert_not_called()
 
 
 @pytest.mark.parametrize(
-    "client_class",
+    "client_class,transport_name",
     [
-        BigtableTableAdminClient,
-        BigtableTableAdminAsyncClient,
+        (BigtableTableAdminClient, "grpc"),
+        (BigtableTableAdminAsyncClient, "grpc_asyncio"),
     ],
 )
-def test_bigtable_table_admin_client_from_service_account_file(client_class):
+def test_bigtable_table_admin_client_from_service_account_file(
+    client_class, transport_name
+):
     creds = ga_credentials.AnonymousCredentials()
     with mock.patch.object(
         service_account.Credentials, "from_service_account_file"
     ) as factory:
         factory.return_value = creds
-        client = client_class.from_service_account_file("dummy/file/path.json")
+        client = client_class.from_service_account_file(
+            "dummy/file/path.json", transport=transport_name
+        )
         assert client.transport._credentials == creds
         assert isinstance(client, client_class)
 
-        client = client_class.from_service_account_json("dummy/file/path.json")
+        client = client_class.from_service_account_json(
+            "dummy/file/path.json", transport=transport_name
+        )
         assert client.transport._credentials == creds
         assert isinstance(client, client_class)
 
-        assert client.transport._host == "bigtableadmin.googleapis.com:443"
+        assert client.transport._host == ("bigtableadmin.googleapis.com:443")
 
 
 def test_bigtable_table_admin_client_get_transport_class():
     transport = BigtableTableAdminClient.get_transport_class()
     available_transports = [
         transports.BigtableTableAdminGrpcTransport,
     ]
@@ -1555,15 +1563,15 @@
             RuntimeError,
         )
         async_pager = await client.list_tables(
             request={},
         )
         assert async_pager.next_page_token == "abc"
         responses = []
-        async for response in async_pager:
+        async for response in async_pager:  # pragma: no branch
             responses.append(response)
 
         assert len(responses) == 6
         assert all(isinstance(i, table.Table) for i in responses)
 
 
 @pytest.mark.asyncio
@@ -1601,15 +1609,17 @@
                     table.Table(),
                     table.Table(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (await client.list_tables(request={})).pages:
+        async for page_ in (
+            await client.list_tables(request={})
+        ).pages:  # pragma: no branch
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
@@ -3847,15 +3857,15 @@
             RuntimeError,
         )
         async_pager = await client.list_snapshots(
             request={},
         )
         assert async_pager.next_page_token == "abc"
         responses = []
-        async for response in async_pager:
+        async for response in async_pager:  # pragma: no branch
             responses.append(response)
 
         assert len(responses) == 6
         assert all(isinstance(i, table.Snapshot) for i in responses)
 
 
 @pytest.mark.asyncio
@@ -3893,15 +3903,17 @@
                     table.Snapshot(),
                     table.Snapshot(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (await client.list_snapshots(request={})).pages:
+        async for page_ in (
+            await client.list_snapshots(request={})
+        ).pages:  # pragma: no branch
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
@@ -5446,15 +5458,15 @@
             RuntimeError,
         )
         async_pager = await client.list_backups(
             request={},
         )
         assert async_pager.next_page_token == "abc"
         responses = []
-        async for response in async_pager:
+        async for response in async_pager:  # pragma: no branch
             responses.append(response)
 
         assert len(responses) == 6
         assert all(isinstance(i, table.Backup) for i in responses)
 
 
 @pytest.mark.asyncio
@@ -5492,15 +5504,17 @@
                     table.Backup(),
                     table.Backup(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (await client.list_backups(request={})).pages:
+        async for page_ in (
+            await client.list_backups(request={})
+        ).pages:  # pragma: no branch
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
@@ -6056,14 +6070,15 @@
     with mock.patch.object(type(client.transport.set_iam_policy), "__call__") as call:
         # Designate an appropriate return value for the call.
         call.return_value = policy_pb2.Policy()
         response = client.set_iam_policy(
             request={
                 "resource": "resource_value",
                 "policy": policy_pb2.Policy(version=774),
+                "update_mask": field_mask_pb2.FieldMask(paths=["paths_value"]),
             }
         )
         call.assert_called()
 
 
 def test_set_iam_policy_flattened():
     client = BigtableTableAdminClient(
@@ -6508,14 +6523,27 @@
     # Test default credentials are used if not provided.
     with mock.patch.object(google.auth, "default") as adc:
         adc.return_value = (ga_credentials.AnonymousCredentials(), None)
         transport_class()
         adc.assert_called_once()
 
 
+@pytest.mark.parametrize(
+    "transport_name",
+    [
+        "grpc",
+    ],
+)
+def test_transport_kind(transport_name):
+    transport = BigtableTableAdminClient.get_transport_class(transport_name)(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
+    assert transport.kind == transport_name
+
+
 def test_transport_grpc_default():
     # A client should use the gRPC transport by default.
     client = BigtableTableAdminClient(
         credentials=ga_credentials.AnonymousCredentials(),
     )
     assert isinstance(
         client.transport,
@@ -6576,14 +6604,22 @@
         transport.close()
 
     # Additionally, the LRO client (a property) should
     # also raise NotImplementedError
     with pytest.raises(NotImplementedError):
         transport.operations_client
 
+    # Catch all for all remaining methods and properties
+    remainder = [
+        "kind",
+    ]
+    for r in remainder:
+        with pytest.raises(NotImplementedError):
+            getattr(transport, r)()
+
 
 def test_bigtable_table_admin_base_transport_with_credentials_file():
     # Instantiate the base transport with a credentials file
     with mock.patch.object(
         google.auth, "load_credentials_from_file", autospec=True
     ) as load_creds, mock.patch(
         "google.cloud.bigtable_admin_v2.services.bigtable_table_admin.transports.BigtableTableAdminTransport._prep_wrapped_messages"
@@ -6751,32 +6787,48 @@
             )
             expected_cert, expected_key = client_cert_source_callback()
             mock_ssl_cred.assert_called_once_with(
                 certificate_chain=expected_cert, private_key=expected_key
             )
 
 
-def test_bigtable_table_admin_host_no_port():
+@pytest.mark.parametrize(
+    "transport_name",
+    [
+        "grpc",
+        "grpc_asyncio",
+    ],
+)
+def test_bigtable_table_admin_host_no_port(transport_name):
     client = BigtableTableAdminClient(
         credentials=ga_credentials.AnonymousCredentials(),
         client_options=client_options.ClientOptions(
             api_endpoint="bigtableadmin.googleapis.com"
         ),
+        transport=transport_name,
     )
-    assert client.transport._host == "bigtableadmin.googleapis.com:443"
+    assert client.transport._host == ("bigtableadmin.googleapis.com:443")
 
 
-def test_bigtable_table_admin_host_with_port():
+@pytest.mark.parametrize(
+    "transport_name",
+    [
+        "grpc",
+        "grpc_asyncio",
+    ],
+)
+def test_bigtable_table_admin_host_with_port(transport_name):
     client = BigtableTableAdminClient(
         credentials=ga_credentials.AnonymousCredentials(),
         client_options=client_options.ClientOptions(
             api_endpoint="bigtableadmin.googleapis.com:8000"
         ),
+        transport=transport_name,
     )
-    assert client.transport._host == "bigtableadmin.googleapis.com:8000"
+    assert client.transport._host == ("bigtableadmin.googleapis.com:8000")
 
 
 def test_bigtable_table_admin_grpc_transport_channel():
     channel = grpc.secure_channel("http://localhost/", grpc.local_channel_credentials())
 
     # Check that channel is used if provided.
     transport = transports.BigtableTableAdminGrpcTransport(
```

### Comparing `google-cloud-bigtable-2.8.1/tests/unit/gapic/bigtable_v2/__init__.py` & `google-cloud-bigtable-2.9.0/tests/unit/gapic/bigtable_v2/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigtable-2.8.1/tests/unit/gapic/bigtable_v2/test_bigtable.py` & `google-cloud-bigtable-2.9.0/tests/unit/gapic/bigtable_v2/test_bigtable.py`

 * *Files 1% similar despite different names*

```diff
@@ -76,32 +76,32 @@
         BigtableClient._get_default_mtls_endpoint(sandbox_mtls_endpoint)
         == sandbox_mtls_endpoint
     )
     assert BigtableClient._get_default_mtls_endpoint(non_googleapi) == non_googleapi
 
 
 @pytest.mark.parametrize(
-    "client_class",
+    "client_class,transport_name",
     [
-        BigtableClient,
-        BigtableAsyncClient,
+        (BigtableClient, "grpc"),
+        (BigtableAsyncClient, "grpc_asyncio"),
     ],
 )
-def test_bigtable_client_from_service_account_info(client_class):
+def test_bigtable_client_from_service_account_info(client_class, transport_name):
     creds = ga_credentials.AnonymousCredentials()
     with mock.patch.object(
         service_account.Credentials, "from_service_account_info"
     ) as factory:
         factory.return_value = creds
         info = {"valid": True}
-        client = client_class.from_service_account_info(info)
+        client = client_class.from_service_account_info(info, transport=transport_name)
         assert client.transport._credentials == creds
         assert isinstance(client, client_class)
 
-        assert client.transport._host == "bigtable.googleapis.com:443"
+        assert client.transport._host == ("bigtable.googleapis.com:443")
 
 
 @pytest.mark.parametrize(
     "transport_class,transport_name",
     [
         (transports.BigtableGrpcTransport, "grpc"),
         (transports.BigtableGrpcAsyncIOTransport, "grpc_asyncio"),
@@ -122,35 +122,39 @@
     ) as use_jwt:
         creds = service_account.Credentials(None, None, None)
         transport = transport_class(credentials=creds, always_use_jwt_access=False)
         use_jwt.assert_not_called()
 
 
 @pytest.mark.parametrize(
-    "client_class",
+    "client_class,transport_name",
     [
-        BigtableClient,
-        BigtableAsyncClient,
+        (BigtableClient, "grpc"),
+        (BigtableAsyncClient, "grpc_asyncio"),
     ],
 )
-def test_bigtable_client_from_service_account_file(client_class):
+def test_bigtable_client_from_service_account_file(client_class, transport_name):
     creds = ga_credentials.AnonymousCredentials()
     with mock.patch.object(
         service_account.Credentials, "from_service_account_file"
     ) as factory:
         factory.return_value = creds
-        client = client_class.from_service_account_file("dummy/file/path.json")
+        client = client_class.from_service_account_file(
+            "dummy/file/path.json", transport=transport_name
+        )
         assert client.transport._credentials == creds
         assert isinstance(client, client_class)
 
-        client = client_class.from_service_account_json("dummy/file/path.json")
+        client = client_class.from_service_account_json(
+            "dummy/file/path.json", transport=transport_name
+        )
         assert client.transport._credentials == creds
         assert isinstance(client, client_class)
 
-        assert client.transport._host == "bigtable.googleapis.com:443"
+        assert client.transport._host == ("bigtable.googleapis.com:443")
 
 
 def test_bigtable_client_get_transport_class():
     transport = BigtableClient.get_transport_class()
     available_transports = [
         transports.BigtableGrpcTransport,
     ]
@@ -2481,14 +2485,27 @@
     # Test default credentials are used if not provided.
     with mock.patch.object(google.auth, "default") as adc:
         adc.return_value = (ga_credentials.AnonymousCredentials(), None)
         transport_class()
         adc.assert_called_once()
 
 
+@pytest.mark.parametrize(
+    "transport_name",
+    [
+        "grpc",
+    ],
+)
+def test_transport_kind(transport_name):
+    transport = BigtableClient.get_transport_class(transport_name)(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
+    assert transport.kind == transport_name
+
+
 def test_transport_grpc_default():
     # A client should use the gRPC transport by default.
     client = BigtableClient(
         credentials=ga_credentials.AnonymousCredentials(),
     )
     assert isinstance(
         client.transport,
@@ -2529,14 +2546,22 @@
     for method in methods:
         with pytest.raises(NotImplementedError):
             getattr(transport, method)(request=object())
 
     with pytest.raises(NotImplementedError):
         transport.close()
 
+    # Catch all for all remaining methods and properties
+    remainder = [
+        "kind",
+    ]
+    for r in remainder:
+        with pytest.raises(NotImplementedError):
+            getattr(transport, r)()
+
 
 def test_bigtable_base_transport_with_credentials_file():
     # Instantiate the base transport with a credentials file
     with mock.patch.object(
         google.auth, "load_credentials_from_file", autospec=True
     ) as load_creds, mock.patch(
         "google.cloud.bigtable_v2.services.bigtable.transports.BigtableTransport._prep_wrapped_messages"
@@ -2699,32 +2724,48 @@
             )
             expected_cert, expected_key = client_cert_source_callback()
             mock_ssl_cred.assert_called_once_with(
                 certificate_chain=expected_cert, private_key=expected_key
             )
 
 
-def test_bigtable_host_no_port():
+@pytest.mark.parametrize(
+    "transport_name",
+    [
+        "grpc",
+        "grpc_asyncio",
+    ],
+)
+def test_bigtable_host_no_port(transport_name):
     client = BigtableClient(
         credentials=ga_credentials.AnonymousCredentials(),
         client_options=client_options.ClientOptions(
             api_endpoint="bigtable.googleapis.com"
         ),
+        transport=transport_name,
     )
-    assert client.transport._host == "bigtable.googleapis.com:443"
+    assert client.transport._host == ("bigtable.googleapis.com:443")
 
 
-def test_bigtable_host_with_port():
+@pytest.mark.parametrize(
+    "transport_name",
+    [
+        "grpc",
+        "grpc_asyncio",
+    ],
+)
+def test_bigtable_host_with_port(transport_name):
     client = BigtableClient(
         credentials=ga_credentials.AnonymousCredentials(),
         client_options=client_options.ClientOptions(
             api_endpoint="bigtable.googleapis.com:8000"
         ),
+        transport=transport_name,
     )
-    assert client.transport._host == "bigtable.googleapis.com:8000"
+    assert client.transport._host == ("bigtable.googleapis.com:8000")
 
 
 def test_bigtable_grpc_transport_channel():
     channel = grpc.secure_channel("http://localhost/", grpc.local_channel_credentials())
 
     # Check that channel is used if provided.
     transport = transports.BigtableGrpcTransport(
```

### Comparing `google-cloud-bigtable-2.8.1/tests/unit/read-rows-acceptance-test.json` & `google-cloud-bigtable-2.9.0/tests/unit/read-rows-acceptance-test.json`

 * *Files identical despite different names*

### Comparing `google-cloud-bigtable-2.8.1/tests/unit/test_app_profile.py` & `google-cloud-bigtable-2.9.0/tests/unit/test_app_profile.py`

 * *Files 11% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 PROJECT = "project"
 INSTANCE_ID = "instance-id"
 APP_PROFILE_ID = "app-profile-id"
 APP_PROFILE_NAME = "projects/{}/instances/{}/appProfiles/{}".format(
     PROJECT, INSTANCE_ID, APP_PROFILE_ID
 )
 CLUSTER_ID = "cluster-id"
+CLUSTER_ID_2 = "cluster-id-2"
 OP_ID = 8765
 OP_NAME = "operations/projects/{}/instances/{}/appProfiles/{}/operations/{}".format(
     PROJECT, INSTANCE_ID, APP_PROFILE_ID, OP_ID
 )
 
 
 def _make_app_profile(*args, **kwargs):
@@ -50,14 +51,15 @@
 
     app_profile = _make_app_profile(APP_PROFILE_ID, instance)
     assert isinstance(app_profile, AppProfile)
     assert app_profile._instance == instance
     assert app_profile.routing_policy_type is None
     assert app_profile.description is None
     assert app_profile.cluster_id is None
+    assert app_profile.multi_cluster_ids is None
     assert app_profile.allow_transactional_writes is None
 
 
 def test_app_profile_constructor_explicit():
     from google.cloud.bigtable.enums import RoutingPolicyType
 
     ANY = RoutingPolicyType.ANY
@@ -88,17 +90,40 @@
     assert app_profile1.routing_policy_type == ANY
     assert app_profile1.description == DESCRIPTION_1
     assert app_profile2.app_profile_id == APP_PROFILE_ID_2
     assert app_profile2._instance is instance
     assert app_profile2.routing_policy_type == SINGLE
     assert app_profile2.description == DESCRIPTION_2
     assert app_profile2.cluster_id == CLUSTER_ID
+    assert app_profile2.multi_cluster_ids is None
     assert app_profile2.allow_transactional_writes == ALLOW_WRITES
 
 
+def test_app_profile_constructor_multi_cluster_ids():
+    from google.cloud.bigtable.enums import RoutingPolicyType
+
+    ANY = RoutingPolicyType.ANY
+    DESCRIPTION_1 = "routing policy any"
+    client = _Client(PROJECT)
+    instance = _Instance(INSTANCE_ID, client)
+
+    app_profile1 = _make_app_profile(
+        APP_PROFILE_ID,
+        instance,
+        routing_policy_type=ANY,
+        description=DESCRIPTION_1,
+        multi_cluster_ids=[CLUSTER_ID, CLUSTER_ID_2],
+    )
+    assert app_profile1.app_profile_id == APP_PROFILE_ID
+    assert app_profile1._instance is instance
+    assert app_profile1.routing_policy_type == ANY
+    assert app_profile1.description == DESCRIPTION_1
+    assert app_profile1.multi_cluster_ids == [CLUSTER_ID, CLUSTER_ID_2]
+
+
 def test_app_profile_name():
     credentials = _make_credentials()
     client = _make_client(project=PROJECT, credentials=credentials, admin=True)
     instance = _Instance(INSTANCE_ID, client)
 
     app_profile = _make_app_profile(APP_PROFILE_ID, instance)
     assert app_profile.name == APP_PROFILE_NAME
@@ -143,63 +168,96 @@
     from google.cloud.bigtable_admin_v2.types import instance as data_v2_pb2
     from google.cloud.bigtable.app_profile import AppProfile
     from google.cloud.bigtable.enums import RoutingPolicyType
 
     client = _Client(PROJECT)
     instance = _Instance(INSTANCE_ID, client)
 
-    desctiption = "routing any"
+    description = "routing any"
     routing = RoutingPolicyType.ANY
     multi_cluster_routing_use_any = data_v2_pb2.AppProfile.MultiClusterRoutingUseAny()
 
     app_profile_pb = data_v2_pb2.AppProfile(
         name=APP_PROFILE_NAME,
-        description=desctiption,
+        description=description,
         multi_cluster_routing_use_any=multi_cluster_routing_use_any,
     )
 
     app_profile = AppProfile.from_pb(app_profile_pb, instance)
     assert isinstance(app_profile, AppProfile)
     assert app_profile._instance is instance
     assert app_profile.app_profile_id == APP_PROFILE_ID
-    assert app_profile.description == desctiption
+    assert app_profile.description == description
     assert app_profile.routing_policy_type == routing
     assert app_profile.cluster_id is None
+    assert app_profile.multi_cluster_ids is None
     assert app_profile.allow_transactional_writes is False
 
 
+def test_app_profile_from_pb_success_w_routing_any_multi_cluster_ids():
+    from google.cloud.bigtable_admin_v2.types import instance as data_v2_pb2
+    from google.cloud.bigtable.app_profile import AppProfile
+    from google.cloud.bigtable.enums import RoutingPolicyType
+
+    client = _Client(PROJECT)
+    instance = _Instance(INSTANCE_ID, client)
+
+    description = "routing any"
+    routing = RoutingPolicyType.ANY
+    multi_cluster_routing_use_any = data_v2_pb2.AppProfile.MultiClusterRoutingUseAny(
+        cluster_ids=[CLUSTER_ID, CLUSTER_ID_2]
+    )
+
+    app_profile_pb = data_v2_pb2.AppProfile(
+        name=APP_PROFILE_NAME,
+        description=description,
+        multi_cluster_routing_use_any=multi_cluster_routing_use_any,
+    )
+
+    app_profile = AppProfile.from_pb(app_profile_pb, instance)
+    assert isinstance(app_profile, AppProfile)
+    assert app_profile._instance is instance
+    assert app_profile.app_profile_id == APP_PROFILE_ID
+    assert app_profile.description == description
+    assert app_profile.routing_policy_type == routing
+    assert app_profile.cluster_id is None
+    assert app_profile.allow_transactional_writes is False
+    assert app_profile.multi_cluster_ids == [CLUSTER_ID, CLUSTER_ID_2]
+
+
 def test_app_profile_from_pb_success_w_routing_single():
     from google.cloud.bigtable_admin_v2.types import instance as data_v2_pb2
     from google.cloud.bigtable.app_profile import AppProfile
     from google.cloud.bigtable.enums import RoutingPolicyType
 
     client = _Client(PROJECT)
     instance = _Instance(INSTANCE_ID, client)
 
-    desctiption = "routing single"
+    description = "routing single"
     allow_transactional_writes = True
     routing = RoutingPolicyType.SINGLE
     single_cluster_routing = data_v2_pb2.AppProfile.SingleClusterRouting(
         cluster_id=CLUSTER_ID,
         allow_transactional_writes=allow_transactional_writes,
     )
 
     app_profile_pb = data_v2_pb2.AppProfile(
         name=APP_PROFILE_NAME,
-        description=desctiption,
+        description=description,
         single_cluster_routing=single_cluster_routing,
     )
 
     app_profile = AppProfile.from_pb(app_profile_pb, instance)
     assert isinstance(app_profile, AppProfile)
     assert app_profile._instance is instance
     assert app_profile.app_profile_id == APP_PROFILE_ID
-    assert app_profile.description == desctiption
+    assert app_profile.description == description
     assert app_profile.routing_policy_type == routing
     assert app_profile.cluster_id == CLUSTER_ID
+    assert app_profile.multi_cluster_ids is None
     assert app_profile.allow_transactional_writes == allow_transactional_writes
 
 
 def test_app_profile_from_pb_w_bad_app_profile_name():
     from google.cloud.bigtable_admin_v2.types import instance as data_v2_pb2
     from google.cloud.bigtable.app_profile import AppProfile
 
@@ -286,22 +344,24 @@
     # Create expected_result.
     expected_result = None  # reload() has no return value.
 
     # Check app_profile config values before.
     assert app_profile.routing_policy_type == routing
     assert app_profile.description == description
     assert app_profile.cluster_id is None
+    assert app_profile.multi_cluster_ids is None
     assert app_profile.allow_transactional_writes is None
 
     # Perform the method and check the result.
     result = app_profile.reload()
     assert result == expected_result
     assert app_profile.routing_policy_type == RoutingPolicyType.SINGLE
     assert app_profile.description == description_from_server
     assert app_profile.cluster_id == cluster_id_from_server
+    assert app_profile.multi_cluster_ids is None
     assert app_profile.allow_transactional_writes == allow_transactional_writes
 
 
 def test_app_profile_exists():
     from google.cloud.bigtable_admin_v2.services.bigtable_instance_admin import (
         BigtableInstanceAdminClient,
     )
@@ -390,14 +450,15 @@
     assert isinstance(result, AppProfile)
     assert result.app_profile_id == APP_PROFILE_ID
     assert result._instance is instance
     assert result.routing_policy_type == routing
     assert result.description == description
     assert result.allow_transactional_writes is False
     assert result.cluster_id is None
+    assert result.multi_cluster_ids is None
 
 
 def test_app_profile_create_w_routing_single():
     from google.cloud.bigtable_admin_v2.services.bigtable_instance_admin import (
         BigtableInstanceAdminClient,
     )
     from google.cloud.bigtable.app_profile import AppProfile
@@ -450,14 +511,15 @@
     assert isinstance(result, AppProfile)
     assert result.app_profile_id == APP_PROFILE_ID
     assert result._instance is instance
     assert result.routing_policy_type == routing
     assert result.description == description
     assert result.allow_transactional_writes == allow_writes
     assert result.cluster_id == CLUSTER_ID
+    assert result.multi_cluster_ids is None
 
 
 def test_app_profile_create_w_wrong_routing_policy():
     credentials = _make_credentials()
     client = _make_client(project=PROJECT, credentials=credentials, admin=True)
     instance = client.instance(INSTANCE_ID)
     app_profile = _make_app_profile(APP_PROFILE_ID, instance, routing_policy_type=None)
@@ -494,14 +556,90 @@
     )
 
     # Create response_pb
     metadata = messages_v2_pb2.UpdateAppProfileMetadata()
     type_url = "type.googleapis.com/{}".format(
         messages_v2_pb2.UpdateAppProfileMetadata._meta._pb.DESCRIPTOR.full_name
     )
+    response_pb = operations_pb2.Operation(
+        name=OP_NAME,
+        metadata=Any(type_url=type_url, value=metadata._pb.SerializeToString()),
+    )
+
+    # Patch the stub used by the API method.
+    instance_api = mock.create_autospec(BigtableInstanceAdminClient)
+    # Mock api calls
+    instance_api.app_profile_path.return_value = (
+        "projects/project/instances/instance-id/appProfiles/app-profile-id"
+    )
+
+    client._instance_admin_client = instance_api
+
+    # Perform the method and check the result.
+    ignore_warnings = True
+    expected_request_update_mask = field_mask_pb2.FieldMask(
+        paths=["description", "single_cluster_routing"]
+    )
+
+    expected_request = {
+        "request": {
+            "app_profile": app_profile._to_pb(),
+            "update_mask": expected_request_update_mask,
+            "ignore_warnings": ignore_warnings,
+        }
+    }
+
+    instance_api.update_app_profile.return_value = response_pb
+    app_profile._instance._client._instance_admin_client = instance_api
+    result = app_profile.update(ignore_warnings=ignore_warnings)
+    actual_request = client._instance_admin_client.update_app_profile.call_args_list[
+        0
+    ].kwargs
+
+    assert actual_request == expected_request
+    assert (
+        result.metadata.type_url
+        == "type.googleapis.com/google.bigtable.admin.v2.UpdateAppProfileMetadata"
+    )
+
+
+def test_app_profile_update_w_routing_any_multi_cluster_ids():
+    from google.longrunning import operations_pb2
+    from google.protobuf.any_pb2 import Any
+    from google.cloud.bigtable_admin_v2.types import (
+        bigtable_instance_admin as messages_v2_pb2,
+    )
+    from google.cloud.bigtable.enums import RoutingPolicyType
+    from google.cloud.bigtable_admin_v2.services.bigtable_instance_admin import (
+        BigtableInstanceAdminClient,
+    )
+    from google.protobuf import field_mask_pb2
+
+    credentials = _make_credentials()
+    client = _make_client(project=PROJECT, credentials=credentials, admin=True)
+    instance = client.instance(INSTANCE_ID)
+
+    routing = RoutingPolicyType.SINGLE
+    description = "to routing policy single"
+    allow_writes = True
+    app_profile = _make_app_profile(
+        APP_PROFILE_ID,
+        instance,
+        routing_policy_type=routing,
+        description=description,
+        cluster_id=CLUSTER_ID,
+        allow_transactional_writes=allow_writes,
+        multi_cluster_ids=[CLUSTER_ID, CLUSTER_ID_2],
+    )
+
+    # Create response_pb
+    metadata = messages_v2_pb2.UpdateAppProfileMetadata()
+    type_url = "type.googleapis.com/{}".format(
+        messages_v2_pb2.UpdateAppProfileMetadata._meta._pb.DESCRIPTOR.full_name
+    )
     response_pb = operations_pb2.Operation(
         name=OP_NAME,
         metadata=Any(type_url=type_url, value=metadata._pb.SerializeToString()),
     )
 
     # Patch the stub used by the API method.
     instance_api = mock.create_autospec(BigtableInstanceAdminClient)
```

### Comparing `google-cloud-bigtable-2.8.1/tests/unit/test_backup.py` & `google-cloud-bigtable-2.9.0/tests/unit/test_backup.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigtable-2.8.1/tests/unit/test_batcher.py` & `google-cloud-bigtable-2.9.0/tests/unit/test_batcher.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigtable-2.8.1/tests/unit/test_client.py` & `google-cloud-bigtable-2.9.0/tests/unit/test_client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigtable-2.8.1/tests/unit/test_cluster.py` & `google-cloud-bigtable-2.9.0/tests/unit/test_cluster.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigtable-2.8.1/tests/unit/test_column_family.py` & `google-cloud-bigtable-2.9.0/tests/unit/test_column_family.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigtable-2.8.1/tests/unit/test_encryption_info.py` & `google-cloud-bigtable-2.9.0/tests/unit/test_encryption_info.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigtable-2.8.1/tests/unit/test_error.py` & `google-cloud-bigtable-2.9.0/tests/unit/test_error.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigtable-2.8.1/tests/unit/test_instance.py` & `google-cloud-bigtable-2.9.0/tests/unit/test_instance.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigtable-2.8.1/tests/unit/test_policy.py` & `google-cloud-bigtable-2.9.0/tests/unit/test_policy.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigtable-2.8.1/tests/unit/test_row.py` & `google-cloud-bigtable-2.9.0/tests/unit/test_row.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigtable-2.8.1/tests/unit/test_row_data.py` & `google-cloud-bigtable-2.9.0/tests/unit/test_row_data.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigtable-2.8.1/tests/unit/test_row_filters.py` & `google-cloud-bigtable-2.9.0/tests/unit/test_row_filters.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigtable-2.8.1/tests/unit/test_row_set.py` & `google-cloud-bigtable-2.9.0/tests/unit/test_row_set.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigtable-2.8.1/tests/unit/test_table.py` & `google-cloud-bigtable-2.9.0/tests/unit/test_table.py`

 * *Files identical despite different names*

