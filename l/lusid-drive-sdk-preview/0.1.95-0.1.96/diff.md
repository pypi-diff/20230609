# Comparing `tmp/lusid-drive-sdk-preview-0.1.95.tar.gz` & `tmp/lusid-drive-sdk-preview-0.1.96.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/lusid-drive-sdk-preview-0.1.95.tar", last modified: Thu Nov  5 10:09:06 2020, max compression
+gzip compressed data, was "dist/lusid-drive-sdk-preview-0.1.96.tar", last modified: Fri Nov  6 08:29:19 2020, max compression
```

## Comparing `lusid-drive-sdk-preview-0.1.95.tar` & `lusid-drive-sdk-preview-0.1.96.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-11-05 10:09:06.000000 lusid-drive-sdk-preview-0.1.95/
--rw-r--r--   0 root         (0) root         (0)       46 2020-11-05 10:08:19.000000 lusid-drive-sdk-preview-0.1.95/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      352 2020-11-05 10:09:06.000000 lusid-drive-sdk-preview-0.1.95/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-11-05 10:09:06.000000 lusid-drive-sdk-preview-0.1.95/lusid_drive/
--rw-r--r--   0 root         (0) root         (0)     2554 2020-11-05 10:08:19.000000 lusid-drive-sdk-preview-0.1.95/lusid_drive/__init__.py
--rw-r--r--   0 root         (0) root         (0)       23 2020-11-05 10:08:19.000000 lusid-drive-sdk-preview-0.1.95/lusid_drive/__version__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-11-05 10:09:06.000000 lusid-drive-sdk-preview-0.1.95/lusid_drive/api/
--rw-r--r--   0 root         (0) root         (0)      310 2020-11-05 10:08:19.000000 lusid-drive-sdk-preview-0.1.95/lusid_drive/api/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5693 2020-11-05 10:08:19.000000 lusid-drive-sdk-preview-0.1.95/lusid_drive/api/application_metadata_api.py
--rw-r--r--   0 root         (0) root         (0)    33492 2020-11-05 10:08:19.000000 lusid-drive-sdk-preview-0.1.95/lusid_drive/api/files_api.py
--rw-r--r--   0 root         (0) root         (0)    42014 2020-11-05 10:08:19.000000 lusid-drive-sdk-preview-0.1.95/lusid_drive/api/folders_api.py
--rw-r--r--   0 root         (0) root         (0)     6931 2020-11-05 10:08:19.000000 lusid-drive-sdk-preview-0.1.95/lusid_drive/api/search_api.py
--rw-r--r--   0 root         (0) root         (0)    25324 2020-11-05 10:08:19.000000 lusid-drive-sdk-preview-0.1.95/lusid_drive/api_client.py
--rw-r--r--   0 root         (0) root         (0)    10406 2020-11-05 10:08:19.000000 lusid-drive-sdk-preview-0.1.95/lusid_drive/configuration.py
--rw-r--r--   0 root         (0) root         (0)     3829 2020-11-05 10:08:19.000000 lusid-drive-sdk-preview-0.1.95/lusid_drive/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-11-05 10:09:06.000000 lusid-drive-sdk-preview-0.1.95/lusid_drive/models/
--rw-r--r--   0 root         (0) root         (0)     1467 2020-11-05 10:08:19.000000 lusid-drive-sdk-preview-0.1.95/lusid_drive/models/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6046 2020-11-05 10:08:19.000000 lusid-drive-sdk-preview-0.1.95/lusid_drive/models/access_controlled_action.py
--rw-r--r--   0 root         (0) root         (0)     7784 2020-11-05 10:08:19.000000 lusid-drive-sdk-preview-0.1.95/lusid_drive/models/access_controlled_resource.py
--rw-r--r--   0 root         (0) root         (0)     5925 2020-11-05 10:08:19.000000 lusid-drive-sdk-preview-0.1.95/lusid_drive/models/action_id.py
--rw-r--r--   0 root         (0) root         (0)     5118 2020-11-05 10:08:19.000000 lusid-drive-sdk-preview-0.1.95/lusid_drive/models/create_folder.py
--rw-r--r--   0 root         (0) root         (0)     6609 2020-11-05 10:08:19.000000 lusid-drive-sdk-preview-0.1.95/lusid_drive/models/id_selector_definition.py
--rw-r--r--   0 root         (0) root         (0)     7667 2020-11-05 10:08:19.000000 lusid-drive-sdk-preview-0.1.95/lusid_drive/models/identifier_part_schema.py
--rw-r--r--   0 root         (0) root         (0)     5562 2020-11-05 10:08:19.000000 lusid-drive-sdk-preview-0.1.95/lusid_drive/models/link.py
--rw-r--r--   0 root         (0) root         (0)     9303 2020-11-05 10:08:19.000000 lusid-drive-sdk-preview-0.1.95/lusid_drive/models/lusid_problem_details.py
--rw-r--r--   0 root         (0) root         (0)    10491 2020-11-05 10:08:19.000000 lusid-drive-sdk-preview-0.1.95/lusid_drive/models/lusid_validation_problem_details.py
--rw-r--r--   0 root         (0) root         (0)     6732 2020-11-05 10:08:19.000000 lusid-drive-sdk-preview-0.1.95/lusid_drive/models/paged_resource_list_of_storage_object.py
--rw-r--r--   0 root         (0) root         (0)     5164 2020-11-05 10:08:19.000000 lusid-drive-sdk-preview-0.1.95/lusid_drive/models/resource_list_of_access_controlled_resource.py
--rw-r--r--   0 root         (0) root         (0)     5349 2020-11-05 10:08:19.000000 lusid-drive-sdk-preview-0.1.95/lusid_drive/models/search_body.py
--rw-r--r--   0 root         (0) root         (0)    12823 2020-11-05 10:08:19.000000 lusid-drive-sdk-preview-0.1.95/lusid_drive/models/storage_object.py
--rw-r--r--   0 root         (0) root         (0)     5106 2020-11-05 10:08:19.000000 lusid-drive-sdk-preview-0.1.95/lusid_drive/models/update_file.py
--rw-r--r--   0 root         (0) root         (0)     5118 2020-11-05 10:08:19.000000 lusid-drive-sdk-preview-0.1.95/lusid_drive/models/update_folder.py
--rw-r--r--   0 root         (0) root         (0)    12436 2020-11-05 10:08:19.000000 lusid-drive-sdk-preview-0.1.95/lusid_drive/rest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-11-05 10:09:06.000000 lusid-drive-sdk-preview-0.1.95/lusid_drive/tcp/
--rw-r--r--   0 root         (0) root         (0)       99 2020-11-05 10:08:19.000000 lusid-drive-sdk-preview-0.1.95/lusid_drive/tcp/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4970 2020-11-05 10:08:19.000000 lusid-drive-sdk-preview-0.1.95/lusid_drive/tcp/tcp_keep_alive_probes.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-11-05 10:09:06.000000 lusid-drive-sdk-preview-0.1.95/lusid_drive/utilities/
--rw-r--r--   0 root         (0) root         (0)      617 2020-11-05 10:08:19.000000 lusid-drive-sdk-preview-0.1.95/lusid_drive/utilities/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7204 2020-11-05 10:08:19.000000 lusid-drive-sdk-preview-0.1.95/lusid_drive/utilities/api_client_builder.py
--rw-r--r--   0 root         (0) root         (0)     4879 2020-11-05 10:08:19.000000 lusid-drive-sdk-preview-0.1.95/lusid_drive/utilities/api_client_factory.py
--rw-r--r--   0 root         (0) root         (0)     3116 2020-11-05 10:08:19.000000 lusid-drive-sdk-preview-0.1.95/lusid_drive/utilities/api_configuration.py
--rw-r--r--   0 root         (0) root         (0)     3514 2020-11-05 10:08:19.000000 lusid-drive-sdk-preview-0.1.95/lusid_drive/utilities/api_configuration_loader.py
--rw-r--r--   0 root         (0) root         (0)     1019 2020-11-05 10:08:19.000000 lusid-drive-sdk-preview-0.1.95/lusid_drive/utilities/config_keys.json
--rw-r--r--   0 root         (0) root         (0)      862 2020-11-05 10:08:19.000000 lusid-drive-sdk-preview-0.1.95/lusid_drive/utilities/lusid_drive_retry.py
--rw-r--r--   0 root         (0) root         (0)     1725 2020-11-05 10:08:19.000000 lusid-drive-sdk-preview-0.1.95/lusid_drive/utilities/proxy_config.py
--rw-r--r--   0 root         (0) root         (0)     2970 2020-11-05 10:08:19.000000 lusid-drive-sdk-preview-0.1.95/lusid_drive/utilities/refreshing_token.py
--rw-r--r--   0 root         (0) root         (0)      869 2020-11-05 10:08:19.000000 lusid-drive-sdk-preview-0.1.95/lusid_drive/utilities/utility_functions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-11-05 10:09:06.000000 lusid-drive-sdk-preview-0.1.95/lusid_drive_sdk_preview.egg-info/
--rw-r--r--   0 root         (0) root         (0)      352 2020-11-05 10:09:05.000000 lusid-drive-sdk-preview-0.1.95/lusid_drive_sdk_preview.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1735 2020-11-05 10:09:05.000000 lusid-drive-sdk-preview-0.1.95/lusid_drive_sdk_preview.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2020-11-05 10:09:05.000000 lusid-drive-sdk-preview-0.1.95/lusid_drive_sdk_preview.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       84 2020-11-05 10:09:05.000000 lusid-drive-sdk-preview-0.1.95/lusid_drive_sdk_preview.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2020-11-05 10:09:05.000000 lusid-drive-sdk-preview-0.1.95/lusid_drive_sdk_preview.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2020-11-05 10:09:06.000000 lusid-drive-sdk-preview-0.1.95/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2191 2020-11-05 10:08:19.000000 lusid-drive-sdk-preview-0.1.95/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-11-06 08:29:19.000000 lusid-drive-sdk-preview-0.1.96/
+-rw-r--r--   0 root         (0) root         (0)       46 2020-11-06 08:28:47.000000 lusid-drive-sdk-preview-0.1.96/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      352 2020-11-06 08:29:19.000000 lusid-drive-sdk-preview-0.1.96/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-11-06 08:29:19.000000 lusid-drive-sdk-preview-0.1.96/lusid_drive/
+-rw-r--r--   0 root         (0) root         (0)     2554 2020-11-06 08:28:47.000000 lusid-drive-sdk-preview-0.1.96/lusid_drive/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       23 2020-11-06 08:28:47.000000 lusid-drive-sdk-preview-0.1.96/lusid_drive/__version__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-11-06 08:29:19.000000 lusid-drive-sdk-preview-0.1.96/lusid_drive/api/
+-rw-r--r--   0 root         (0) root         (0)      310 2020-11-06 08:28:47.000000 lusid-drive-sdk-preview-0.1.96/lusid_drive/api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5693 2020-11-06 08:28:47.000000 lusid-drive-sdk-preview-0.1.96/lusid_drive/api/application_metadata_api.py
+-rw-r--r--   0 root         (0) root         (0)    33492 2020-11-06 08:28:47.000000 lusid-drive-sdk-preview-0.1.96/lusid_drive/api/files_api.py
+-rw-r--r--   0 root         (0) root         (0)    42014 2020-11-06 08:28:47.000000 lusid-drive-sdk-preview-0.1.96/lusid_drive/api/folders_api.py
+-rw-r--r--   0 root         (0) root         (0)     6931 2020-11-06 08:28:47.000000 lusid-drive-sdk-preview-0.1.96/lusid_drive/api/search_api.py
+-rw-r--r--   0 root         (0) root         (0)    25324 2020-11-06 08:28:47.000000 lusid-drive-sdk-preview-0.1.96/lusid_drive/api_client.py
+-rw-r--r--   0 root         (0) root         (0)    10406 2020-11-06 08:28:47.000000 lusid-drive-sdk-preview-0.1.96/lusid_drive/configuration.py
+-rw-r--r--   0 root         (0) root         (0)     3829 2020-11-06 08:28:47.000000 lusid-drive-sdk-preview-0.1.96/lusid_drive/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-11-06 08:29:19.000000 lusid-drive-sdk-preview-0.1.96/lusid_drive/models/
+-rw-r--r--   0 root         (0) root         (0)     1467 2020-11-06 08:28:47.000000 lusid-drive-sdk-preview-0.1.96/lusid_drive/models/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6046 2020-11-06 08:28:47.000000 lusid-drive-sdk-preview-0.1.96/lusid_drive/models/access_controlled_action.py
+-rw-r--r--   0 root         (0) root         (0)     7784 2020-11-06 08:28:47.000000 lusid-drive-sdk-preview-0.1.96/lusid_drive/models/access_controlled_resource.py
+-rw-r--r--   0 root         (0) root         (0)     5925 2020-11-06 08:28:47.000000 lusid-drive-sdk-preview-0.1.96/lusid_drive/models/action_id.py
+-rw-r--r--   0 root         (0) root         (0)     5118 2020-11-06 08:28:47.000000 lusid-drive-sdk-preview-0.1.96/lusid_drive/models/create_folder.py
+-rw-r--r--   0 root         (0) root         (0)     6609 2020-11-06 08:28:47.000000 lusid-drive-sdk-preview-0.1.96/lusid_drive/models/id_selector_definition.py
+-rw-r--r--   0 root         (0) root         (0)     7667 2020-11-06 08:28:47.000000 lusid-drive-sdk-preview-0.1.96/lusid_drive/models/identifier_part_schema.py
+-rw-r--r--   0 root         (0) root         (0)     5562 2020-11-06 08:28:47.000000 lusid-drive-sdk-preview-0.1.96/lusid_drive/models/link.py
+-rw-r--r--   0 root         (0) root         (0)     9303 2020-11-06 08:28:47.000000 lusid-drive-sdk-preview-0.1.96/lusid_drive/models/lusid_problem_details.py
+-rw-r--r--   0 root         (0) root         (0)    10491 2020-11-06 08:28:47.000000 lusid-drive-sdk-preview-0.1.96/lusid_drive/models/lusid_validation_problem_details.py
+-rw-r--r--   0 root         (0) root         (0)     6732 2020-11-06 08:28:47.000000 lusid-drive-sdk-preview-0.1.96/lusid_drive/models/paged_resource_list_of_storage_object.py
+-rw-r--r--   0 root         (0) root         (0)     5164 2020-11-06 08:28:47.000000 lusid-drive-sdk-preview-0.1.96/lusid_drive/models/resource_list_of_access_controlled_resource.py
+-rw-r--r--   0 root         (0) root         (0)     5349 2020-11-06 08:28:47.000000 lusid-drive-sdk-preview-0.1.96/lusid_drive/models/search_body.py
+-rw-r--r--   0 root         (0) root         (0)    12823 2020-11-06 08:28:47.000000 lusid-drive-sdk-preview-0.1.96/lusid_drive/models/storage_object.py
+-rw-r--r--   0 root         (0) root         (0)     5106 2020-11-06 08:28:47.000000 lusid-drive-sdk-preview-0.1.96/lusid_drive/models/update_file.py
+-rw-r--r--   0 root         (0) root         (0)     5118 2020-11-06 08:28:47.000000 lusid-drive-sdk-preview-0.1.96/lusid_drive/models/update_folder.py
+-rw-r--r--   0 root         (0) root         (0)    12436 2020-11-06 08:28:47.000000 lusid-drive-sdk-preview-0.1.96/lusid_drive/rest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-11-06 08:29:19.000000 lusid-drive-sdk-preview-0.1.96/lusid_drive/tcp/
+-rw-r--r--   0 root         (0) root         (0)       99 2020-11-06 08:28:47.000000 lusid-drive-sdk-preview-0.1.96/lusid_drive/tcp/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4970 2020-11-06 08:28:47.000000 lusid-drive-sdk-preview-0.1.96/lusid_drive/tcp/tcp_keep_alive_probes.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-11-06 08:29:19.000000 lusid-drive-sdk-preview-0.1.96/lusid_drive/utilities/
+-rw-r--r--   0 root         (0) root         (0)      617 2020-11-06 08:28:47.000000 lusid-drive-sdk-preview-0.1.96/lusid_drive/utilities/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7204 2020-11-06 08:28:47.000000 lusid-drive-sdk-preview-0.1.96/lusid_drive/utilities/api_client_builder.py
+-rw-r--r--   0 root         (0) root         (0)     4879 2020-11-06 08:28:47.000000 lusid-drive-sdk-preview-0.1.96/lusid_drive/utilities/api_client_factory.py
+-rw-r--r--   0 root         (0) root         (0)     3116 2020-11-06 08:28:47.000000 lusid-drive-sdk-preview-0.1.96/lusid_drive/utilities/api_configuration.py
+-rw-r--r--   0 root         (0) root         (0)     3514 2020-11-06 08:28:47.000000 lusid-drive-sdk-preview-0.1.96/lusid_drive/utilities/api_configuration_loader.py
+-rw-r--r--   0 root         (0) root         (0)     1019 2020-11-06 08:28:47.000000 lusid-drive-sdk-preview-0.1.96/lusid_drive/utilities/config_keys.json
+-rw-r--r--   0 root         (0) root         (0)      862 2020-11-06 08:28:47.000000 lusid-drive-sdk-preview-0.1.96/lusid_drive/utilities/lusid_drive_retry.py
+-rw-r--r--   0 root         (0) root         (0)     1725 2020-11-06 08:28:47.000000 lusid-drive-sdk-preview-0.1.96/lusid_drive/utilities/proxy_config.py
+-rw-r--r--   0 root         (0) root         (0)     2970 2020-11-06 08:28:47.000000 lusid-drive-sdk-preview-0.1.96/lusid_drive/utilities/refreshing_token.py
+-rw-r--r--   0 root         (0) root         (0)      869 2020-11-06 08:28:47.000000 lusid-drive-sdk-preview-0.1.96/lusid_drive/utilities/utility_functions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-11-06 08:29:19.000000 lusid-drive-sdk-preview-0.1.96/lusid_drive_sdk_preview.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      352 2020-11-06 08:29:19.000000 lusid-drive-sdk-preview-0.1.96/lusid_drive_sdk_preview.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1735 2020-11-06 08:29:19.000000 lusid-drive-sdk-preview-0.1.96/lusid_drive_sdk_preview.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2020-11-06 08:29:19.000000 lusid-drive-sdk-preview-0.1.96/lusid_drive_sdk_preview.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       84 2020-11-06 08:29:19.000000 lusid-drive-sdk-preview-0.1.96/lusid_drive_sdk_preview.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2020-11-06 08:29:19.000000 lusid-drive-sdk-preview-0.1.96/lusid_drive_sdk_preview.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2020-11-06 08:29:19.000000 lusid-drive-sdk-preview-0.1.96/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2191 2020-11-06 08:28:47.000000 lusid-drive-sdk-preview-0.1.96/setup.py
```

### Comparing `lusid-drive-sdk-preview-0.1.95/lusid_drive/__init__.py` & `lusid-drive-sdk-preview-0.1.96/lusid_drive/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,23 +3,23 @@
 # flake8: noqa
 
 """
     FINBOURNE Drive API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.95
+    The version of the OpenAPI document: 0.1.96
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
-__version__ = "0.1.95"
+__version__ = "0.1.96"
 
 # import apis into sdk package
 from lusid_drive.api.application_metadata_api import ApplicationMetadataApi
 from lusid_drive.api.files_api import FilesApi
 from lusid_drive.api.folders_api import FoldersApi
 from lusid_drive.api.search_api import SearchApi
```

### Comparing `lusid-drive-sdk-preview-0.1.95/lusid_drive/api/application_metadata_api.py` & `lusid-drive-sdk-preview-0.1.96/lusid_drive/api/application_metadata_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Drive API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.95
+    The version of the OpenAPI document: 0.1.96
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
@@ -120,15 +120,15 @@
 
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.95'
+        header_params['X-LUSID-SDK-Version'] = '0.1.96'
 
         return self.api_client.call_api(
             '/api/metadata/access/resources', 'GET',
             path_params,
             query_params,
             header_params,
             body=body_params,
```

### Comparing `lusid-drive-sdk-preview-0.1.95/lusid_drive/api/files_api.py` & `lusid-drive-sdk-preview-0.1.96/lusid_drive/api/files_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Drive API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.95
+    The version of the OpenAPI document: 0.1.96
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
@@ -149,15 +149,15 @@
             ['application/octet-stream'])  # noqa: E501
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.95'
+        header_params['X-LUSID-SDK-Version'] = '0.1.96'
 
         return self.api_client.call_api(
             '/api/files', 'POST',
             path_params,
             query_params,
             header_params,
             body=body_params,
@@ -260,15 +260,15 @@
 
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.95'
+        header_params['X-LUSID-SDK-Version'] = '0.1.96'
 
         return self.api_client.call_api(
             '/api/files/{id}', 'DELETE',
             path_params,
             query_params,
             header_params,
             body=body_params,
@@ -371,15 +371,15 @@
 
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.95'
+        header_params['X-LUSID-SDK-Version'] = '0.1.96'
 
         return self.api_client.call_api(
             '/api/files/{id}/contents', 'GET',
             path_params,
             query_params,
             header_params,
             body=body_params,
@@ -482,15 +482,15 @@
 
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.95'
+        header_params['X-LUSID-SDK-Version'] = '0.1.96'
 
         return self.api_client.call_api(
             '/api/files/{id}', 'GET',
             path_params,
             query_params,
             header_params,
             body=body_params,
@@ -600,15 +600,15 @@
             ['application/octet-stream'])  # noqa: E501
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.95'
+        header_params['X-LUSID-SDK-Version'] = '0.1.96'
 
         return self.api_client.call_api(
             '/api/files/{id}/contents', 'PUT',
             path_params,
             query_params,
             header_params,
             body=body_params,
@@ -722,15 +722,15 @@
             ['application/json'])  # noqa: E501
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.95'
+        header_params['X-LUSID-SDK-Version'] = '0.1.96'
 
         return self.api_client.call_api(
             '/api/files/{id}', 'PUT',
             path_params,
             query_params,
             header_params,
             body=body_params,
```

### Comparing `lusid-drive-sdk-preview-0.1.95/lusid_drive/api/folders_api.py` & `lusid-drive-sdk-preview-0.1.96/lusid_drive/api/folders_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Drive API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.95
+    The version of the OpenAPI document: 0.1.96
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
@@ -129,15 +129,15 @@
             ['application/json'])  # noqa: E501
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.95'
+        header_params['X-LUSID-SDK-Version'] = '0.1.96'
 
         return self.api_client.call_api(
             '/api/folders', 'POST',
             path_params,
             query_params,
             header_params,
             body=body_params,
@@ -240,15 +240,15 @@
 
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.95'
+        header_params['X-LUSID-SDK-Version'] = '0.1.96'
 
         return self.api_client.call_api(
             '/api/folders/{id}', 'DELETE',
             path_params,
             query_params,
             header_params,
             body=body_params,
@@ -351,15 +351,15 @@
 
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.95'
+        header_params['X-LUSID-SDK-Version'] = '0.1.96'
 
         return self.api_client.call_api(
             '/api/folders/{id}', 'GET',
             path_params,
             query_params,
             header_params,
             body=body_params,
@@ -483,15 +483,15 @@
 
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.95'
+        header_params['X-LUSID-SDK-Version'] = '0.1.96'
 
         return self.api_client.call_api(
             '/api/folders/{id}/contents', 'GET',
             path_params,
             query_params,
             header_params,
             body=body_params,
@@ -607,15 +607,15 @@
 
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.95'
+        header_params['X-LUSID-SDK-Version'] = '0.1.96'
 
         return self.api_client.call_api(
             '/api/folders', 'GET',
             path_params,
             query_params,
             header_params,
             body=body_params,
@@ -737,15 +737,15 @@
             ['application/json'])  # noqa: E501
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.95'
+        header_params['X-LUSID-SDK-Version'] = '0.1.96'
 
         return self.api_client.call_api(
             '/api/folders/{id}', 'POST',
             path_params,
             query_params,
             header_params,
             body=body_params,
@@ -859,15 +859,15 @@
             ['application/json'])  # noqa: E501
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.95'
+        header_params['X-LUSID-SDK-Version'] = '0.1.96'
 
         return self.api_client.call_api(
             '/api/folders/{id}', 'PUT',
             path_params,
             query_params,
             header_params,
             body=body_params,
```

### Comparing `lusid-drive-sdk-preview-0.1.95/lusid_drive/api/search_api.py` & `lusid-drive-sdk-preview-0.1.96/lusid_drive/api/search_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Drive API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.95
+    The version of the OpenAPI document: 0.1.96
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
@@ -146,15 +146,15 @@
             ['application/json'])  # noqa: E501
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.95'
+        header_params['X-LUSID-SDK-Version'] = '0.1.96'
 
         return self.api_client.call_api(
             '/api/search', 'POST',
             path_params,
             query_params,
             header_params,
             body=body_params,
```

### Comparing `lusid-drive-sdk-preview-0.1.95/lusid_drive/api_client.py` & `lusid-drive-sdk-preview-0.1.96/lusid_drive/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # coding: utf-8
 """
     FINBOURNE Drive API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.95
+    The version of the OpenAPI document: 0.1.96
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 from __future__ import absolute_import
 
 import datetime
@@ -73,15 +73,15 @@
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'OpenAPI-Generator/0.1.95/python'
+        self.user_agent = 'OpenAPI-Generator/0.1.96/python'
 
     def __del__(self):
         if self._pool:
             self._pool.close()
             self._pool.join()
             self._pool = None
```

### Comparing `lusid-drive-sdk-preview-0.1.95/lusid_drive/configuration.py` & `lusid-drive-sdk-preview-0.1.96/lusid_drive/configuration.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Drive API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.95
+    The version of the OpenAPI document: 0.1.96
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
@@ -262,16 +262,16 @@
         """Gets the essential information for debugging.
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
-               "Version of the API: 0.1.95\n"\
-               "SDK Package Version: 0.1.95".\
+               "Version of the API: 0.1.96\n"\
+               "SDK Package Version: 0.1.96".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `lusid-drive-sdk-preview-0.1.95/lusid_drive/exceptions.py` & `lusid-drive-sdk-preview-0.1.96/lusid_drive/exceptions.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Drive API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.95
+    The version of the OpenAPI document: 0.1.96
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import six
```

### Comparing `lusid-drive-sdk-preview-0.1.95/lusid_drive/models/__init__.py` & `lusid-drive-sdk-preview-0.1.96/lusid_drive/models/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # flake8: noqa
 """
     FINBOURNE Drive API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.95
+    The version of the OpenAPI document: 0.1.96
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `lusid-drive-sdk-preview-0.1.95/lusid_drive/models/access_controlled_action.py` & `lusid-drive-sdk-preview-0.1.96/lusid_drive/models/access_controlled_action.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Drive API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.95
+    The version of the OpenAPI document: 0.1.96
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `lusid-drive-sdk-preview-0.1.95/lusid_drive/models/access_controlled_resource.py` & `lusid-drive-sdk-preview-0.1.96/lusid_drive/models/access_controlled_resource.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Drive API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.95
+    The version of the OpenAPI document: 0.1.96
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `lusid-drive-sdk-preview-0.1.95/lusid_drive/models/action_id.py` & `lusid-drive-sdk-preview-0.1.96/lusid_drive/models/action_id.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Drive API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.95
+    The version of the OpenAPI document: 0.1.96
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `lusid-drive-sdk-preview-0.1.95/lusid_drive/models/create_folder.py` & `lusid-drive-sdk-preview-0.1.96/lusid_drive/models/create_folder.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Drive API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.95
+    The version of the OpenAPI document: 0.1.96
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `lusid-drive-sdk-preview-0.1.95/lusid_drive/models/id_selector_definition.py` & `lusid-drive-sdk-preview-0.1.96/lusid_drive/models/id_selector_definition.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Drive API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.95
+    The version of the OpenAPI document: 0.1.96
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `lusid-drive-sdk-preview-0.1.95/lusid_drive/models/identifier_part_schema.py` & `lusid-drive-sdk-preview-0.1.96/lusid_drive/models/identifier_part_schema.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Drive API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.95
+    The version of the OpenAPI document: 0.1.96
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `lusid-drive-sdk-preview-0.1.95/lusid_drive/models/link.py` & `lusid-drive-sdk-preview-0.1.96/lusid_drive/models/link.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Drive API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.95
+    The version of the OpenAPI document: 0.1.96
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `lusid-drive-sdk-preview-0.1.95/lusid_drive/models/lusid_problem_details.py` & `lusid-drive-sdk-preview-0.1.96/lusid_drive/models/lusid_problem_details.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Drive API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.95
+    The version of the OpenAPI document: 0.1.96
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `lusid-drive-sdk-preview-0.1.95/lusid_drive/models/lusid_validation_problem_details.py` & `lusid-drive-sdk-preview-0.1.96/lusid_drive/models/lusid_validation_problem_details.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Drive API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.95
+    The version of the OpenAPI document: 0.1.96
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `lusid-drive-sdk-preview-0.1.95/lusid_drive/models/paged_resource_list_of_storage_object.py` & `lusid-drive-sdk-preview-0.1.96/lusid_drive/models/paged_resource_list_of_storage_object.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Drive API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.95
+    The version of the OpenAPI document: 0.1.96
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `lusid-drive-sdk-preview-0.1.95/lusid_drive/models/resource_list_of_access_controlled_resource.py` & `lusid-drive-sdk-preview-0.1.96/lusid_drive/models/resource_list_of_access_controlled_resource.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Drive API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.95
+    The version of the OpenAPI document: 0.1.96
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `lusid-drive-sdk-preview-0.1.95/lusid_drive/models/search_body.py` & `lusid-drive-sdk-preview-0.1.96/lusid_drive/models/search_body.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Drive API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.95
+    The version of the OpenAPI document: 0.1.96
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `lusid-drive-sdk-preview-0.1.95/lusid_drive/models/storage_object.py` & `lusid-drive-sdk-preview-0.1.96/lusid_drive/models/storage_object.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Drive API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.95
+    The version of the OpenAPI document: 0.1.96
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `lusid-drive-sdk-preview-0.1.95/lusid_drive/models/update_file.py` & `lusid-drive-sdk-preview-0.1.96/lusid_drive/models/update_file.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Drive API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.95
+    The version of the OpenAPI document: 0.1.96
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `lusid-drive-sdk-preview-0.1.95/lusid_drive/models/update_folder.py` & `lusid-drive-sdk-preview-0.1.96/lusid_drive/models/update_folder.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Drive API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.95
+    The version of the OpenAPI document: 0.1.96
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `lusid-drive-sdk-preview-0.1.95/lusid_drive/rest.py` & `lusid-drive-sdk-preview-0.1.96/lusid_drive/rest.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Drive API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.95
+    The version of the OpenAPI document: 0.1.96
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `lusid-drive-sdk-preview-0.1.95/lusid_drive/tcp/tcp_keep_alive_probes.py` & `lusid-drive-sdk-preview-0.1.96/lusid_drive/tcp/tcp_keep_alive_probes.py`

 * *Files identical despite different names*

### Comparing `lusid-drive-sdk-preview-0.1.95/lusid_drive/utilities/__init__.py` & `lusid-drive-sdk-preview-0.1.96/lusid_drive/utilities/__init__.py`

 * *Files identical despite different names*

### Comparing `lusid-drive-sdk-preview-0.1.95/lusid_drive/utilities/api_client_builder.py` & `lusid-drive-sdk-preview-0.1.96/lusid_drive/utilities/api_client_builder.py`

 * *Files identical despite different names*

### Comparing `lusid-drive-sdk-preview-0.1.95/lusid_drive/utilities/api_client_factory.py` & `lusid-drive-sdk-preview-0.1.96/lusid_drive/utilities/api_client_factory.py`

 * *Files identical despite different names*

### Comparing `lusid-drive-sdk-preview-0.1.95/lusid_drive/utilities/api_configuration.py` & `lusid-drive-sdk-preview-0.1.96/lusid_drive/utilities/api_configuration.py`

 * *Files identical despite different names*

### Comparing `lusid-drive-sdk-preview-0.1.95/lusid_drive/utilities/api_configuration_loader.py` & `lusid-drive-sdk-preview-0.1.96/lusid_drive/utilities/api_configuration_loader.py`

 * *Files identical despite different names*

### Comparing `lusid-drive-sdk-preview-0.1.95/lusid_drive/utilities/config_keys.json` & `lusid-drive-sdk-preview-0.1.96/lusid_drive/utilities/config_keys.json`

 * *Files identical despite different names*

### Comparing `lusid-drive-sdk-preview-0.1.95/lusid_drive/utilities/lusid_drive_retry.py` & `lusid-drive-sdk-preview-0.1.96/lusid_drive/utilities/lusid_drive_retry.py`

 * *Files identical despite different names*

### Comparing `lusid-drive-sdk-preview-0.1.95/lusid_drive/utilities/proxy_config.py` & `lusid-drive-sdk-preview-0.1.96/lusid_drive/utilities/proxy_config.py`

 * *Files identical despite different names*

### Comparing `lusid-drive-sdk-preview-0.1.95/lusid_drive/utilities/refreshing_token.py` & `lusid-drive-sdk-preview-0.1.96/lusid_drive/utilities/refreshing_token.py`

 * *Files identical despite different names*

### Comparing `lusid-drive-sdk-preview-0.1.95/lusid_drive/utilities/utility_functions.py` & `lusid-drive-sdk-preview-0.1.96/lusid_drive/utilities/utility_functions.py`

 * *Files identical despite different names*

### Comparing `lusid-drive-sdk-preview-0.1.95/lusid_drive_sdk_preview.egg-info/SOURCES.txt` & `lusid-drive-sdk-preview-0.1.96/lusid_drive_sdk_preview.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lusid-drive-sdk-preview-0.1.95/setup.py` & `lusid-drive-sdk-preview-0.1.96/setup.py`

 * *Files identical despite different names*

