# Comparing `tmp/klaviyo-api-2.0.1.tar.gz` & `tmp/klaviyo-api-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "klaviyo-api-2.0.1.tar", last modified: Tue May 30 20:18:45 2023, max compression
+gzip compressed data, was "klaviyo-api-2.0.2.tar", last modified: Fri Jun  9 19:11:08 2023, max compression
```

## Comparing `klaviyo-api-2.0.1.tar` & `klaviyo-api-2.0.2.tar`

### file list

```diff
@@ -1,282 +1,252 @@
-drwxr-xr-x   0 local      (503) staff       (20)        0 2023-05-30 20:18:45.932567 klaviyo-api-2.0.1/
--rw-r--r--   0 local      (503) staff       (20)     1063 2023-05-30 20:18:37.000000 klaviyo-api-2.0.1/LICENSE
--rw-r--r--   0 local      (503) staff       (20)    53409 2023-05-30 20:18:45.932790 klaviyo-api-2.0.1/PKG-INFO
--rw-r--r--   0 local      (503) staff       (20)    52892 2023-05-30 20:18:37.000000 klaviyo-api-2.0.1/README.md
--rw-r--r--   0 local      (503) staff       (20)      103 2023-05-30 20:18:37.000000 klaviyo-api-2.0.1/pyproject.toml
--rw-r--r--   0 local      (503) staff       (20)      801 2023-05-30 20:18:45.933422 klaviyo-api-2.0.1/setup.cfg
-drwxr-xr-x   0 local      (503) staff       (20)        0 2023-05-30 20:18:45.740355 klaviyo-api-2.0.1/src/
-drwxr-xr-x   0 local      (503) staff       (20)        0 2023-05-30 20:18:45.744953 klaviyo-api-2.0.1/src/klaviyo_api/
--rw-r--r--   0 local      (503) staff       (20)      130 2023-05-30 20:18:37.000000 klaviyo-api-2.0.1/src/klaviyo_api/__init__.py
--rw-r--r--   0 local      (503) staff       (20)      501 2023-05-30 20:18:37.000000 klaviyo-api-2.0.1/src/klaviyo_api/custom_retry.py
--rw-r--r--   0 local      (503) staff       (20)    25983 2023-05-30 20:18:36.000000 klaviyo-api-2.0.1/src/klaviyo_api/wrapper.py
-drwxr-xr-x   0 local      (503) staff       (20)        0 2023-05-30 20:18:45.747154 klaviyo-api-2.0.1/src/klaviyo_api.egg-info/
--rw-r--r--   0 local      (503) staff       (20)    53409 2023-05-30 20:18:45.000000 klaviyo-api-2.0.1/src/klaviyo_api.egg-info/PKG-INFO
--rw-r--r--   0 local      (503) staff       (20)    16572 2023-05-30 20:18:45.000000 klaviyo-api-2.0.1/src/klaviyo_api.egg-info/SOURCES.txt
--rw-r--r--   0 local      (503) staff       (20)        1 2023-05-30 20:18:45.000000 klaviyo-api-2.0.1/src/klaviyo_api.egg-info/dependency_links.txt
--rw-r--r--   0 local      (503) staff       (20)      119 2023-05-30 20:18:45.000000 klaviyo-api-2.0.1/src/klaviyo_api.egg-info/requires.txt
--rw-r--r--   0 local      (503) staff       (20)       27 2023-05-30 20:18:45.000000 klaviyo-api-2.0.1/src/klaviyo_api.egg-info/top_level.txt
-drwxr-xr-x   0 local      (503) staff       (20)        0 2023-05-30 20:18:45.750729 klaviyo-api-2.0.1/src/openapi_client/
--rw-r--r--   0 local      (503) staff       (20)      788 2023-05-30 20:18:36.000000 klaviyo-api-2.0.1/src/openapi_client/__init__.py
-drwxr-xr-x   0 local      (503) staff       (20)        0 2023-05-30 20:18:45.759585 klaviyo-api-2.0.1/src/openapi_client/api/
--rw-r--r--   0 local      (503) staff       (20)      220 2023-05-30 20:18:36.000000 klaviyo-api-2.0.1/src/openapi_client/api/__init__.py
--rw-r--r--   0 local      (503) staff       (20)   108410 2023-05-30 20:18:35.000000 klaviyo-api-2.0.1/src/openapi_client/api/campaigns_api.py
--rw-r--r--   0 local      (503) staff       (20)   351426 2023-05-30 20:18:35.000000 klaviyo-api-2.0.1/src/openapi_client/api/catalogs_api.py
--rw-r--r--   0 local      (503) staff       (20)    19405 2023-05-30 20:18:35.000000 klaviyo-api-2.0.1/src/openapi_client/api/client_api.py
--rw-r--r--   0 local      (503) staff       (20)     7236 2023-05-30 20:18:35.000000 klaviyo-api-2.0.1/src/openapi_client/api/data_privacy_api.py
--rw-r--r--   0 local      (503) staff       (20)    58131 2023-05-30 20:18:35.000000 klaviyo-api-2.0.1/src/openapi_client/api/events_api.py
--rw-r--r--   0 local      (503) staff       (20)   106404 2023-05-30 20:18:35.000000 klaviyo-api-2.0.1/src/openapi_client/api/flows_api.py
--rw-r--r--   0 local      (503) staff       (20)    70579 2023-05-30 20:18:35.000000 klaviyo-api-2.0.1/src/openapi_client/api/lists_api.py
--rw-r--r--   0 local      (503) staff       (20)    21644 2023-05-30 20:18:35.000000 klaviyo-api-2.0.1/src/openapi_client/api/metrics_api.py
--rw-r--r--   0 local      (503) staff       (20)    87637 2023-05-30 20:18:35.000000 klaviyo-api-2.0.1/src/openapi_client/api/profiles_api.py
--rw-r--r--   0 local      (503) staff       (20)    48387 2023-05-30 20:18:35.000000 klaviyo-api-2.0.1/src/openapi_client/api/segments_api.py
--rw-r--r--   0 local      (503) staff       (20)   147862 2023-05-30 20:18:35.000000 klaviyo-api-2.0.1/src/openapi_client/api/tags_api.py
--rw-r--r--   0 local      (503) staff       (20)    42674 2023-05-30 20:18:35.000000 klaviyo-api-2.0.1/src/openapi_client/api/templates_api.py
--rw-r--r--   0 local      (503) staff       (20)    39451 2023-05-30 20:18:36.000000 klaviyo-api-2.0.1/src/openapi_client/api_client.py
-drwxr-xr-x   0 local      (503) staff       (20)        0 2023-05-30 20:18:45.760182 klaviyo-api-2.0.1/src/openapi_client/apis/
--rw-r--r--   0 local      (503) staff       (20)     1084 2023-05-30 20:18:36.000000 klaviyo-api-2.0.1/src/openapi_client/apis/__init__.py
--rw-r--r--   0 local      (503) staff       (20)    17158 2023-05-30 20:18:36.000000 klaviyo-api-2.0.1/src/openapi_client/configuration.py
--rw-r--r--   0 local      (503) staff       (20)     5120 2023-05-30 20:18:36.000000 klaviyo-api-2.0.1/src/openapi_client/exceptions.py
-drwxr-xr-x   0 local      (503) staff       (20)        0 2023-05-30 20:18:45.931737 klaviyo-api-2.0.1/src/openapi_client/model/
--rw-r--r--   0 local      (503) staff       (20)      348 2023-05-30 20:18:36.000000 klaviyo-api-2.0.1/src/openapi_client/model/__init__.py
--rw-r--r--   0 local      (503) staff       (20)    11834 2023-05-30 20:18:33.000000 klaviyo-api-2.0.1/src/openapi_client/model/audiences_sub_object.py
--rw-r--r--   0 local      (503) staff       (20)    11849 2023-05-30 20:18:33.000000 klaviyo-api-2.0.1/src/openapi_client/model/campaign_clone_query.py
--rw-r--r--   0 local      (503) staff       (20)    12354 2023-05-30 20:18:33.000000 klaviyo-api-2.0.1/src/openapi_client/model/campaign_clone_query_resource_object.py
--rw-r--r--   0 local      (503) staff       (20)    11954 2023-05-30 20:18:33.000000 klaviyo-api-2.0.1/src/openapi_client/model/campaign_clone_query_resource_object_attributes.py
--rw-r--r--   0 local      (503) staff       (20)    11859 2023-05-30 20:18:33.000000 klaviyo-api-2.0.1/src/openapi_client/model/campaign_create_query.py
--rw-r--r--   0 local      (503) staff       (20)    12364 2023-05-30 20:18:33.000000 klaviyo-api-2.0.1/src/openapi_client/model/campaign_create_query_resource_object.py
--rw-r--r--   0 local      (503) staff       (20)    13914 2023-05-30 20:18:33.000000 klaviyo-api-2.0.1/src/openapi_client/model/campaign_create_query_resource_object_attributes.py
--rw-r--r--   0 local      (503) staff       (20)    11633 2023-05-30 20:18:33.000000 klaviyo-api-2.0.1/src/openapi_client/model/campaign_enum.py
--rw-r--r--   0 local      (503) staff       (20)    12011 2023-05-30 20:18:33.000000 klaviyo-api-2.0.1/src/openapi_client/model/campaign_message_assign_template_query.py
--rw-r--r--   0 local      (503) staff       (20)    12566 2023-05-30 20:18:33.000000 klaviyo-api-2.0.1/src/openapi_client/model/campaign_message_assign_template_query_resource_object.py
--rw-r--r--   0 local      (503) staff       (20)    12055 2023-05-30 20:18:33.000000 klaviyo-api-2.0.1/src/openapi_client/model/campaign_message_assign_template_query_resource_object_attributes.py
--rw-r--r--   0 local      (503) staff       (20)    11750 2023-05-30 20:18:33.000000 klaviyo-api-2.0.1/src/openapi_client/model/campaign_message_enum.py
--rw-r--r--   0 local      (503) staff       (20)    12001 2023-05-30 20:18:33.000000 klaviyo-api-2.0.1/src/openapi_client/model/campaign_message_partial_update_query.py
--rw-r--r--   0 local      (503) staff       (20)    12786 2023-05-30 20:18:33.000000 klaviyo-api-2.0.1/src/openapi_client/model/campaign_message_partial_update_query_resource_object.py
--rw-r--r--   0 local      (503) staff       (20)    12109 2023-05-30 20:18:33.000000 klaviyo-api-2.0.1/src/openapi_client/model/campaign_message_partial_update_query_resource_object_attributes.py
--rw-r--r--   0 local      (503) staff       (20)    11930 2023-05-30 20:18:33.000000 klaviyo-api-2.0.1/src/openapi_client/model/campaign_partial_update_query.py
--rw-r--r--   0 local      (503) staff       (20)    12667 2023-05-30 20:18:33.000000 klaviyo-api-2.0.1/src/openapi_client/model/campaign_partial_update_query_resource_object.py
--rw-r--r--   0 local      (503) staff       (20)    13373 2023-05-30 20:18:33.000000 klaviyo-api-2.0.1/src/openapi_client/model/campaign_partial_update_query_resource_object_attributes.py
--rw-r--r--   0 local      (503) staff       (20)    11942 2023-05-30 20:18:33.000000 klaviyo-api-2.0.1/src/openapi_client/model/campaign_recipient_estimation_enum.py
--rw-r--r--   0 local      (503) staff       (20)    12082 2023-05-30 20:18:33.000000 klaviyo-api-2.0.1/src/openapi_client/model/campaign_recipient_estimation_job_create_query.py
--rw-r--r--   0 local      (503) staff       (20)    12744 2023-05-30 20:18:33.000000 klaviyo-api-2.0.1/src/openapi_client/model/campaign_recipient_estimation_job_create_query_resource_object.py
--rw-r--r--   0 local      (503) staff       (20)    11768 2023-05-30 20:18:33.000000 klaviyo-api-2.0.1/src/openapi_client/model/campaign_recipient_estimation_job_create_query_resource_object_attributes.py
--rw-r--r--   0 local      (503) staff       (20)    11999 2023-05-30 20:18:33.000000 klaviyo-api-2.0.1/src/openapi_client/model/campaign_recipient_estimation_job_enum.py
--rw-r--r--   0 local      (503) staff       (20)    11931 2023-05-30 20:18:33.000000 klaviyo-api-2.0.1/src/openapi_client/model/campaign_send_job_create_query.py
--rw-r--r--   0 local      (503) staff       (20)    12487 2023-05-30 20:18:33.000000 klaviyo-api-2.0.1/src/openapi_client/model/campaign_send_job_create_query_resource_object.py
--rw-r--r--   0 local      (503) staff       (20)    11675 2023-05-30 20:18:33.000000 klaviyo-api-2.0.1/src/openapi_client/model/campaign_send_job_create_query_resource_object_attributes.py
--rw-r--r--   0 local      (503) staff       (20)    11762 2023-05-30 20:18:33.000000 klaviyo-api-2.0.1/src/openapi_client/model/campaign_send_job_enum.py
--rw-r--r--   0 local      (503) staff       (20)    12002 2023-05-30 20:18:33.000000 klaviyo-api-2.0.1/src/openapi_client/model/campaign_send_job_partial_update_query.py
--rw-r--r--   0 local      (503) staff       (20)    12848 2023-05-30 20:18:33.000000 klaviyo-api-2.0.1/src/openapi_client/model/campaign_send_job_partial_update_query_resource_object.py
--rw-r--r--   0 local      (503) staff       (20)    11850 2023-05-30 20:18:33.000000 klaviyo-api-2.0.1/src/openapi_client/model/campaign_send_job_partial_update_query_resource_object_attributes.py
--rw-r--r--   0 local      (503) staff       (20)    11981 2023-05-30 20:18:33.000000 klaviyo-api-2.0.1/src/openapi_client/model/catalog_category_bulk_create_job_enum.py
--rw-r--r--   0 local      (503) staff       (20)    11981 2023-05-30 20:18:33.000000 klaviyo-api-2.0.1/src/openapi_client/model/catalog_category_bulk_delete_job_enum.py
--rw-r--r--   0 local      (503) staff       (20)    11981 2023-05-30 20:18:33.000000 klaviyo-api-2.0.1/src/openapi_client/model/catalog_category_bulk_update_job_enum.py
--rw-r--r--   0 local      (503) staff       (20)    12022 2023-05-30 20:18:33.000000 klaviyo-api-2.0.1/src/openapi_client/model/catalog_category_create_job_create_query.py
--rw-r--r--   0 local      (503) staff       (20)    12671 2023-05-30 20:18:33.000000 klaviyo-api-2.0.1/src/openapi_client/model/catalog_category_create_job_create_query_resource_object.py
--rw-r--r--   0 local      (503) staff       (20)    12179 2023-05-30 20:18:33.000000 klaviyo-api-2.0.1/src/openapi_client/model/catalog_category_create_job_create_query_resource_object_attributes.py
--rw-r--r--   0 local      (503) staff       (20)    11930 2023-05-30 20:18:33.000000 klaviyo-api-2.0.1/src/openapi_client/model/catalog_category_create_query.py
--rw-r--r--   0 local      (503) staff       (20)    13136 2023-05-30 20:18:33.000000 klaviyo-api-2.0.1/src/openapi_client/model/catalog_category_create_query_resource_object.py
--rw-r--r--   0 local      (503) staff       (20)    13243 2023-05-30 20:18:33.000000 klaviyo-api-2.0.1/src/openapi_client/model/catalog_category_create_query_resource_object_attributes.py
--rw-r--r--   0 local      (503) staff       (20)    12022 2023-05-30 20:18:33.000000 klaviyo-api-2.0.1/src/openapi_client/model/catalog_category_delete_job_create_query.py
--rw-r--r--   0 local      (503) staff       (20)    12671 2023-05-30 20:18:33.000000 klaviyo-api-2.0.1/src/openapi_client/model/catalog_category_delete_job_create_query_resource_object.py
--rw-r--r--   0 local      (503) staff       (20)    12179 2023-05-30 20:18:33.000000 klaviyo-api-2.0.1/src/openapi_client/model/catalog_category_delete_job_create_query_resource_object_attributes.py
--rw-r--r--   0 local      (503) staff       (20)    12422 2023-05-30 20:18:33.000000 klaviyo-api-2.0.1/src/openapi_client/model/catalog_category_delete_query_resource_object.py
--rw-r--r--   0 local      (503) staff       (20)    11750 2023-05-30 20:18:33.000000 klaviyo-api-2.0.1/src/openapi_client/model/catalog_category_enum.py
--rw-r--r--   0 local      (503) staff       (20)    12114 2023-05-30 20:18:34.000000 klaviyo-api-2.0.1/src/openapi_client/model/catalog_category_item_op.py
--rw-r--r--   0 local      (503) staff       (20)    12022 2023-05-30 20:18:34.000000 klaviyo-api-2.0.1/src/openapi_client/model/catalog_category_update_job_create_query.py
--rw-r--r--   0 local      (503) staff       (20)    12671 2023-05-30 20:18:34.000000 klaviyo-api-2.0.1/src/openapi_client/model/catalog_category_update_job_create_query_resource_object.py
--rw-r--r--   0 local      (503) staff       (20)    12179 2023-05-30 20:18:34.000000 klaviyo-api-2.0.1/src/openapi_client/model/catalog_category_update_job_create_query_resource_object_attributes.py
--rw-r--r--   0 local      (503) staff       (20)    11930 2023-05-30 20:18:34.000000 klaviyo-api-2.0.1/src/openapi_client/model/catalog_category_update_query.py
--rw-r--r--   0 local      (503) staff       (20)    13736 2023-05-30 20:18:34.000000 klaviyo-api-2.0.1/src/openapi_client/model/catalog_category_update_query_resource_object.py
--rw-r--r--   0 local      (503) staff       (20)    11663 2023-05-30 20:18:34.000000 klaviyo-api-2.0.1/src/openapi_client/model/catalog_category_update_query_resource_object_attributes.py
--rw-r--r--   0 local      (503) staff       (20)    12102 2023-05-30 20:18:34.000000 klaviyo-api-2.0.1/src/openapi_client/model/catalog_category_update_query_resource_object_relationships.py
--rw-r--r--   0 local      (503) staff       (20)    12225 2023-05-30 20:18:34.000000 klaviyo-api-2.0.1/src/openapi_client/model/catalog_category_update_query_resource_object_relationships_items.py
--rw-r--r--   0 local      (503) staff       (20)    12137 2023-05-30 20:18:34.000000 klaviyo-api-2.0.1/src/openapi_client/model/catalog_category_update_query_resource_object_relationships_items_data_inner.py
--rw-r--r--   0 local      (503) staff       (20)    11921 2023-05-30 20:18:34.000000 klaviyo-api-2.0.1/src/openapi_client/model/catalog_item_bulk_create_job_enum.py
--rw-r--r--   0 local      (503) staff       (20)    11921 2023-05-30 20:18:34.000000 klaviyo-api-2.0.1/src/openapi_client/model/catalog_item_bulk_delete_job_enum.py
--rw-r--r--   0 local      (503) staff       (20)    11921 2023-05-30 20:18:34.000000 klaviyo-api-2.0.1/src/openapi_client/model/catalog_item_bulk_update_job_enum.py
--rw-r--r--   0 local      (503) staff       (20)    12121 2023-05-30 20:18:34.000000 klaviyo-api-2.0.1/src/openapi_client/model/catalog_item_category_op.py
--rw-r--r--   0 local      (503) staff       (20)    11982 2023-05-30 20:18:34.000000 klaviyo-api-2.0.1/src/openapi_client/model/catalog_item_create_job_create_query.py
--rw-r--r--   0 local      (503) staff       (20)    12603 2023-05-30 20:18:34.000000 klaviyo-api-2.0.1/src/openapi_client/model/catalog_item_create_job_create_query_resource_object.py
--rw-r--r--   0 local      (503) staff       (20)    12074 2023-05-30 20:18:34.000000 klaviyo-api-2.0.1/src/openapi_client/model/catalog_item_create_job_create_query_resource_object_attributes.py
--rw-r--r--   0 local      (503) staff       (20)    11890 2023-05-30 20:18:34.000000 klaviyo-api-2.0.1/src/openapi_client/model/catalog_item_create_query.py
--rw-r--r--   0 local      (503) staff       (20)    13040 2023-05-30 20:18:34.000000 klaviyo-api-2.0.1/src/openapi_client/model/catalog_item_create_query_resource_object.py
--rw-r--r--   0 local      (503) staff       (20)    17029 2023-05-30 20:18:34.000000 klaviyo-api-2.0.1/src/openapi_client/model/catalog_item_create_query_resource_object_attributes.py
--rw-r--r--   0 local      (503) staff       (20)    12122 2023-05-30 20:18:34.000000 klaviyo-api-2.0.1/src/openapi_client/model/catalog_item_create_query_resource_object_relationships.py
--rw-r--r--   0 local      (503) staff       (20)    12235 2023-05-30 20:18:34.000000 klaviyo-api-2.0.1/src/openapi_client/model/catalog_item_create_query_resource_object_relationships_categories.py
--rw-r--r--   0 local      (503) staff       (20)    12172 2023-05-30 20:18:34.000000 klaviyo-api-2.0.1/src/openapi_client/model/catalog_item_create_query_resource_object_relationships_categories_data_inner.py
--rw-r--r--   0 local      (503) staff       (20)    11982 2023-05-30 20:18:34.000000 klaviyo-api-2.0.1/src/openapi_client/model/catalog_item_delete_job_create_query.py
--rw-r--r--   0 local      (503) staff       (20)    12603 2023-05-30 20:18:34.000000 klaviyo-api-2.0.1/src/openapi_client/model/catalog_item_delete_job_create_query_resource_object.py
--rw-r--r--   0 local      (503) staff       (20)    12074 2023-05-30 20:18:34.000000 klaviyo-api-2.0.1/src/openapi_client/model/catalog_item_delete_job_create_query_resource_object_attributes.py
--rw-r--r--   0 local      (503) staff       (20)    12374 2023-05-30 20:18:34.000000 klaviyo-api-2.0.1/src/openapi_client/model/catalog_item_delete_query_resource_object.py
--rw-r--r--   0 local      (503) staff       (20)    11690 2023-05-30 20:18:34.000000 klaviyo-api-2.0.1/src/openapi_client/model/catalog_item_enum.py
--rw-r--r--   0 local      (503) staff       (20)    11982 2023-05-30 20:18:34.000000 klaviyo-api-2.0.1/src/openapi_client/model/catalog_item_update_job_create_query.py
--rw-r--r--   0 local      (503) staff       (20)    12603 2023-05-30 20:18:34.000000 klaviyo-api-2.0.1/src/openapi_client/model/catalog_item_update_job_create_query_resource_object.py
--rw-r--r--   0 local      (503) staff       (20)    12074 2023-05-30 20:18:34.000000 klaviyo-api-2.0.1/src/openapi_client/model/catalog_item_update_job_create_query_resource_object_attributes.py
--rw-r--r--   0 local      (503) staff       (20)    11890 2023-05-30 20:18:34.000000 klaviyo-api-2.0.1/src/openapi_client/model/catalog_item_update_query.py
--rw-r--r--   0 local      (503) staff       (20)    13632 2023-05-30 20:18:34.000000 klaviyo-api-2.0.1/src/openapi_client/model/catalog_item_update_query_resource_object.py
--rw-r--r--   0 local      (503) staff       (20)    15281 2023-05-30 20:18:34.000000 klaviyo-api-2.0.1/src/openapi_client/model/catalog_item_update_query_resource_object_attributes.py
--rw-r--r--   0 local      (503) staff       (20)    12792 2023-05-30 20:18:34.000000 klaviyo-api-2.0.1/src/openapi_client/model/catalog_job_error_payload.py
--rw-r--r--   0 local      (503) staff       (20)    11966 2023-05-30 20:18:34.000000 klaviyo-api-2.0.1/src/openapi_client/model/catalog_variant_bulk_create_job_enum.py
--rw-r--r--   0 local      (503) staff       (20)    11966 2023-05-30 20:18:34.000000 klaviyo-api-2.0.1/src/openapi_client/model/catalog_variant_bulk_delete_job_enum.py
--rw-r--r--   0 local      (503) staff       (20)    11966 2023-05-30 20:18:34.000000 klaviyo-api-2.0.1/src/openapi_client/model/catalog_variant_bulk_update_job_enum.py
--rw-r--r--   0 local      (503) staff       (20)    12012 2023-05-30 20:18:34.000000 klaviyo-api-2.0.1/src/openapi_client/model/catalog_variant_create_job_create_query.py
--rw-r--r--   0 local      (503) staff       (20)    12654 2023-05-30 20:18:34.000000 klaviyo-api-2.0.1/src/openapi_client/model/catalog_variant_create_job_create_query_resource_object.py
--rw-r--r--   0 local      (503) staff       (20)    12143 2023-05-30 20:18:34.000000 klaviyo-api-2.0.1/src/openapi_client/model/catalog_variant_create_job_create_query_resource_object_attributes.py
--rw-r--r--   0 local      (503) staff       (20)    11920 2023-05-30 20:18:34.000000 klaviyo-api-2.0.1/src/openapi_client/model/catalog_variant_create_query.py
--rw-r--r--   0 local      (503) staff       (20)    13119 2023-05-30 20:18:34.000000 klaviyo-api-2.0.1/src/openapi_client/model/catalog_variant_create_query_resource_object.py
--rw-r--r--   0 local      (503) staff       (20)    19026 2023-05-30 20:18:34.000000 klaviyo-api-2.0.1/src/openapi_client/model/catalog_variant_create_query_resource_object_attributes.py
--rw-r--r--   0 local      (503) staff       (20)    12012 2023-05-30 20:18:34.000000 klaviyo-api-2.0.1/src/openapi_client/model/catalog_variant_delete_job_create_query.py
--rw-r--r--   0 local      (503) staff       (20)    12654 2023-05-30 20:18:34.000000 klaviyo-api-2.0.1/src/openapi_client/model/catalog_variant_delete_job_create_query_resource_object.py
--rw-r--r--   0 local      (503) staff       (20)    12143 2023-05-30 20:18:34.000000 klaviyo-api-2.0.1/src/openapi_client/model/catalog_variant_delete_job_create_query_resource_object_attributes.py
--rw-r--r--   0 local      (503) staff       (20)    12410 2023-05-30 20:18:34.000000 klaviyo-api-2.0.1/src/openapi_client/model/catalog_variant_delete_query_resource_object.py
--rw-r--r--   0 local      (503) staff       (20)    11735 2023-05-30 20:18:34.000000 klaviyo-api-2.0.1/src/openapi_client/model/catalog_variant_enum.py
--rw-r--r--   0 local      (503) staff       (20)    12012 2023-05-30 20:18:34.000000 klaviyo-api-2.0.1/src/openapi_client/model/catalog_variant_update_job_create_query.py
--rw-r--r--   0 local      (503) staff       (20)    12654 2023-05-30 20:18:34.000000 klaviyo-api-2.0.1/src/openapi_client/model/catalog_variant_update_job_create_query_resource_object.py
--rw-r--r--   0 local      (503) staff       (20)    12143 2023-05-30 20:18:34.000000 klaviyo-api-2.0.1/src/openapi_client/model/catalog_variant_update_job_create_query_resource_object_attributes.py
--rw-r--r--   0 local      (503) staff       (20)    11920 2023-05-30 20:18:34.000000 klaviyo-api-2.0.1/src/openapi_client/model/catalog_variant_update_query.py
--rw-r--r--   0 local      (503) staff       (20)    13066 2023-05-30 20:18:34.000000 klaviyo-api-2.0.1/src/openapi_client/model/catalog_variant_update_query_resource_object.py
--rw-r--r--   0 local      (503) staff       (20)    17148 2023-05-30 20:18:34.000000 klaviyo-api-2.0.1/src/openapi_client/model/catalog_variant_update_query_resource_object_attributes.py
--rw-r--r--   0 local      (503) staff       (20)    12224 2023-05-30 20:18:34.000000 klaviyo-api-2.0.1/src/openapi_client/model/collection_links.py
--rw-r--r--   0 local      (503) staff       (20)    13057 2023-05-30 20:18:34.000000 klaviyo-api-2.0.1/src/openapi_client/model/content_sub_object.py
--rw-r--r--   0 local      (503) staff       (20)    12002 2023-05-30 20:18:34.000000 klaviyo-api-2.0.1/src/openapi_client/model/data_privacy_create_deletion_job_query.py
--rw-r--r--   0 local      (503) staff       (20)    12608 2023-05-30 20:18:34.000000 klaviyo-api-2.0.1/src/openapi_client/model/data_privacy_create_deletion_job_query_resource_object.py
--rw-r--r--   0 local      (503) staff       (20)    12449 2023-05-30 20:18:34.000000 klaviyo-api-2.0.1/src/openapi_client/model/data_privacy_create_deletion_job_query_resource_object_attributes.py
--rw-r--r--   0 local      (503) staff       (20)    11879 2023-05-30 20:18:34.000000 klaviyo-api-2.0.1/src/openapi_client/model/data_privacy_deletion_job_enum.py
--rw-r--r--   0 local      (503) staff       (20)    11685 2023-05-30 20:18:34.000000 klaviyo-api-2.0.1/src/openapi_client/model/email_channel.py
--rw-r--r--   0 local      (503) staff       (20)    14791 2023-05-30 20:18:34.000000 klaviyo-api-2.0.1/src/openapi_client/model/email_marketing.py
--rw-r--r--   0 local      (503) staff       (20)    12468 2023-05-30 20:18:34.000000 klaviyo-api-2.0.1/src/openapi_client/model/email_marketing_list_suppression.py
--rw-r--r--   0 local      (503) staff       (20)    12135 2023-05-30 20:18:34.000000 klaviyo-api-2.0.1/src/openapi_client/model/email_marketing_suppression.py
--rw-r--r--   0 local      (503) staff       (20)    12321 2023-05-30 20:18:34.000000 klaviyo-api-2.0.1/src/openapi_client/model/email_message_content.py
--rw-r--r--   0 local      (503) staff       (20)    12694 2023-05-30 20:18:34.000000 klaviyo-api-2.0.1/src/openapi_client/model/email_tracking_options.py
--rw-r--r--   0 local      (503) staff       (20)    11790 2023-05-30 20:18:34.000000 klaviyo-api-2.0.1/src/openapi_client/model/error_source.py
--rw-r--r--   0 local      (503) staff       (20)    11829 2023-05-30 20:18:34.000000 klaviyo-api-2.0.1/src/openapi_client/model/event_create_query.py
--rw-r--r--   0 local      (503) staff       (20)    12313 2023-05-30 20:18:34.000000 klaviyo-api-2.0.1/src/openapi_client/model/event_create_query_resource_object.py
--rw-r--r--   0 local      (503) staff       (20)    17076 2023-05-30 20:18:34.000000 klaviyo-api-2.0.1/src/openapi_client/model/event_create_query_resource_object_attributes.py
--rw-r--r--   0 local      (503) staff       (20)    11588 2023-05-30 20:18:34.000000 klaviyo-api-2.0.1/src/openapi_client/model/event_enum.py
--rw-r--r--   0 local      (503) staff       (20)    11675 2023-05-30 20:18:34.000000 klaviyo-api-2.0.1/src/openapi_client/model/flow_action_enum.py
--rw-r--r--   0 local      (503) staff       (20)    11573 2023-05-30 20:18:34.000000 klaviyo-api-2.0.1/src/openapi_client/model/flow_enum.py
--rw-r--r--   0 local      (503) staff       (20)    11690 2023-05-30 20:18:34.000000 klaviyo-api-2.0.1/src/openapi_client/model/flow_message_enum.py
--rw-r--r--   0 local      (503) staff       (20)    11819 2023-05-30 20:18:34.000000 klaviyo-api-2.0.1/src/openapi_client/model/flow_update_query.py
--rw-r--r--   0 local      (503) staff       (20)    12538 2023-05-30 20:18:34.000000 klaviyo-api-2.0.1/src/openapi_client/model/flow_update_query_resource_object.py
--rw-r--r--   0 local      (503) staff       (20)    11764 2023-05-30 20:18:34.000000 klaviyo-api-2.0.1/src/openapi_client/model/flow_update_query_resource_object_attributes.py
--rw-r--r--   0 local      (503) staff       (20)    11999 2023-05-30 20:18:34.000000 klaviyo-api-2.0.1/src/openapi_client/model/get_create_variants_jobs5_xx_response.py
--rw-r--r--   0 local      (503) staff       (20)    12816 2023-05-30 20:18:34.000000 klaviyo-api-2.0.1/src/openapi_client/model/get_create_variants_jobs5_xx_response_errors_inner.py
--rw-r--r--   0 local      (503) staff       (20)    11775 2023-05-30 20:18:34.000000 klaviyo-api-2.0.1/src/openapi_client/model/get_create_variants_jobs5_xx_response_errors_inner_source.py
--rw-r--r--   0 local      (503) staff       (20)    11819 2023-05-30 20:18:34.000000 klaviyo-api-2.0.1/src/openapi_client/model/list_create_query.py
--rw-r--r--   0 local      (503) staff       (20)    12296 2023-05-30 20:18:34.000000 klaviyo-api-2.0.1/src/openapi_client/model/list_create_query_resource_object.py
--rw-r--r--   0 local      (503) staff       (20)    11668 2023-05-30 20:18:34.000000 klaviyo-api-2.0.1/src/openapi_client/model/list_create_query_resource_object_attributes.py
--rw-r--r--   0 local      (503) staff       (20)    11573 2023-05-30 20:18:34.000000 klaviyo-api-2.0.1/src/openapi_client/model/list_enum.py
--rw-r--r--   0 local      (503) staff       (20)    11831 2023-05-30 20:18:34.000000 klaviyo-api-2.0.1/src/openapi_client/model/list_members_add_query.py
--rw-r--r--   0 local      (503) staff       (20)    11980 2023-05-30 20:18:34.000000 klaviyo-api-2.0.1/src/openapi_client/model/list_members_add_query_data_inner.py
--rw-r--r--   0 local      (503) staff       (20)    11840 2023-05-30 20:18:34.000000 klaviyo-api-2.0.1/src/openapi_client/model/list_members_delete_query.py
--rw-r--r--   0 local      (503) staff       (20)    11890 2023-05-30 20:18:34.000000 klaviyo-api-2.0.1/src/openapi_client/model/list_partial_update_query.py
--rw-r--r--   0 local      (503) staff       (20)    12625 2023-05-30 20:18:34.000000 klaviyo-api-2.0.1/src/openapi_client/model/list_partial_update_query_resource_object.py
--rw-r--r--   0 local      (503) staff       (20)    11750 2023-05-30 20:18:34.000000 klaviyo-api-2.0.1/src/openapi_client/model/metric_aggregate_enum.py
--rw-r--r--   0 local      (503) staff       (20)    11869 2023-05-30 20:18:34.000000 klaviyo-api-2.0.1/src/openapi_client/model/metric_aggregate_query.py
--rw-r--r--   0 local      (503) staff       (20)    12424 2023-05-30 20:18:34.000000 klaviyo-api-2.0.1/src/openapi_client/model/metric_aggregate_query_resource_object.py
--rw-r--r--   0 local      (503) staff       (20)    21013 2023-05-30 20:18:34.000000 klaviyo-api-2.0.1/src/openapi_client/model/metric_aggregate_query_resource_object_attributes.py
--rw-r--r--   0 local      (503) staff       (20)    12259 2023-05-30 20:18:34.000000 klaviyo-api-2.0.1/src/openapi_client/model/metric_aggregate_row_dto.py
--rw-r--r--   0 local      (503) staff       (20)    11996 2023-05-30 20:18:34.000000 klaviyo-api-2.0.1/src/openapi_client/model/metric_create_query.py
--rw-r--r--   0 local      (503) staff       (20)    11603 2023-05-30 20:18:34.000000 klaviyo-api-2.0.1/src/openapi_client/model/metric_enum.py
--rw-r--r--   0 local      (503) staff       (20)    11495 2023-05-30 20:18:34.000000 klaviyo-api-2.0.1/src/openapi_client/model/object_links.py
--rw-r--r--   0 local      (503) staff       (20)    11910 2023-05-30 20:18:34.000000 klaviyo-api-2.0.1/src/openapi_client/model/onsite_profile_create_query.py
--rw-r--r--   0 local      (503) staff       (20)    12758 2023-05-30 20:18:34.000000 klaviyo-api-2.0.1/src/openapi_client/model/onsite_profile_create_query_resource_object.py
--rw-r--r--   0 local      (503) staff       (20)    15425 2023-05-30 20:18:34.000000 klaviyo-api-2.0.1/src/openapi_client/model/onsite_profile_create_query_resource_object_attributes.py
--rw-r--r--   0 local      (503) staff       (20)    11894 2023-05-30 20:18:34.000000 klaviyo-api-2.0.1/src/openapi_client/model/onsite_profile_meta.py
--rw-r--r--   0 local      (503) staff       (20)    13575 2023-05-30 20:18:34.000000 klaviyo-api-2.0.1/src/openapi_client/model/onsite_profile_meta_identifiers.py
--rw-r--r--   0 local      (503) staff       (20)    11960 2023-05-30 20:18:34.000000 klaviyo-api-2.0.1/src/openapi_client/model/onsite_subscription_create_query.py
--rw-r--r--   0 local      (503) staff       (20)    12493 2023-05-30 20:18:34.000000 klaviyo-api-2.0.1/src/openapi_client/model/onsite_subscription_create_query_resource_object.py
--rw-r--r--   0 local      (503) staff       (20)    13508 2023-05-30 20:18:34.000000 klaviyo-api-2.0.1/src/openapi_client/model/onsite_subscription_create_query_resource_object_attributes.py
--rw-r--r--   0 local      (503) staff       (20)    14569 2023-05-30 20:18:34.000000 klaviyo-api-2.0.1/src/openapi_client/model/predictive_analytics.py
--rw-r--r--   0 local      (503) staff       (20)    11765 2023-05-30 20:18:34.000000 klaviyo-api-2.0.1/src/openapi_client/model/profile_aggregate_enum.py
--rw-r--r--   0 local      (503) staff       (20)    11849 2023-05-30 20:18:34.000000 klaviyo-api-2.0.1/src/openapi_client/model/profile_create_query.py
--rw-r--r--   0 local      (503) staff       (20)    12347 2023-05-30 20:18:34.000000 klaviyo-api-2.0.1/src/openapi_client/model/profile_create_query_resource_object.py
--rw-r--r--   0 local      (503) staff       (20)    15156 2023-05-30 20:18:34.000000 klaviyo-api-2.0.1/src/openapi_client/model/profile_create_query_resource_object_attributes.py
--rw-r--r--   0 local      (503) staff       (20)    11618 2023-05-30 20:18:34.000000 klaviyo-api-2.0.1/src/openapi_client/model/profile_enum.py
--rw-r--r--   0 local      (503) staff       (20)    13961 2023-05-30 20:18:34.000000 klaviyo-api-2.0.1/src/openapi_client/model/profile_location.py
--rw-r--r--   0 local      (503) staff       (20)    11301 2023-05-30 20:18:34.000000 klaviyo-api-2.0.1/src/openapi_client/model/profile_location_latitude.py
--rw-r--r--   0 local      (503) staff       (20)    11304 2023-05-30 20:18:34.000000 klaviyo-api-2.0.1/src/openapi_client/model/profile_location_longitude.py
--rw-r--r--   0 local      (503) staff       (20)    11920 2023-05-30 20:18:34.000000 klaviyo-api-2.0.1/src/openapi_client/model/profile_partial_update_query.py
--rw-r--r--   0 local      (503) staff       (20)    12725 2023-05-30 20:18:34.000000 klaviyo-api-2.0.1/src/openapi_client/model/profile_partial_update_query_resource_object.py
--rw-r--r--   0 local      (503) staff       (20)    12041 2023-05-30 20:18:34.000000 klaviyo-api-2.0.1/src/openapi_client/model/profile_subscription_bulk_create_job_enum.py
--rw-r--r--   0 local      (503) staff       (20)    12026 2023-05-30 20:18:34.000000 klaviyo-api-2.0.1/src/openapi_client/model/profile_suppression_bulk_create_job_enum.py
--rw-r--r--   0 local      (503) staff       (20)    12071 2023-05-30 20:18:34.000000 klaviyo-api-2.0.1/src/openapi_client/model/profile_unsubscription_bulk_create_job_enum.py
--rw-r--r--   0 local      (503) staff       (20)    12056 2023-05-30 20:18:34.000000 klaviyo-api-2.0.1/src/openapi_client/model/profile_unsuppression_bulk_create_job_enum.py
--rw-r--r--   0 local      (503) staff       (20)    11618 2023-05-30 20:18:34.000000 klaviyo-api-2.0.1/src/openapi_client/model/segment_enum.py
--rw-r--r--   0 local      (503) staff       (20)    11920 2023-05-30 20:18:34.000000 klaviyo-api-2.0.1/src/openapi_client/model/segment_partial_update_query.py
--rw-r--r--   0 local      (503) staff       (20)    12586 2023-05-30 20:18:34.000000 klaviyo-api-2.0.1/src/openapi_client/model/segment_partial_update_query_resource_object.py
--rw-r--r--   0 local      (503) staff       (20)    11632 2023-05-30 20:18:34.000000 klaviyo-api-2.0.1/src/openapi_client/model/segment_partial_update_query_resource_object_attributes.py
--rw-r--r--   0 local      (503) staff       (20)    11956 2023-05-30 20:18:34.000000 klaviyo-api-2.0.1/src/openapi_client/model/send_options.py
--rw-r--r--   0 local      (503) staff       (20)    11612 2023-05-30 20:18:34.000000 klaviyo-api-2.0.1/src/openapi_client/model/send_options_sub_object.py
--rw-r--r--   0 local      (503) staff       (20)    13115 2023-05-30 20:18:34.000000 klaviyo-api-2.0.1/src/openapi_client/model/send_strategy_sub_object.py
--rw-r--r--   0 local      (503) staff       (20)    12019 2023-05-30 20:18:34.000000 klaviyo-api-2.0.1/src/openapi_client/model/send_time_sub_object.py
--rw-r--r--   0 local      (503) staff       (20)    11665 2023-05-30 20:18:34.000000 klaviyo-api-2.0.1/src/openapi_client/model/sms_channel.py
--rw-r--r--   0 local      (503) staff       (20)    12982 2023-05-30 20:18:34.000000 klaviyo-api-2.0.1/src/openapi_client/model/sms_marketing.py
--rw-r--r--   0 local      (503) staff       (20)    11704 2023-05-30 20:18:34.000000 klaviyo-api-2.0.1/src/openapi_client/model/sms_message_content.py
--rw-r--r--   0 local      (503) staff       (20)    12566 2023-05-30 20:18:34.000000 klaviyo-api-2.0.1/src/openapi_client/model/sms_render_options.py
--rw-r--r--   0 local      (503) staff       (20)    12005 2023-05-30 20:18:34.000000 klaviyo-api-2.0.1/src/openapi_client/model/sms_tracking_options.py
--rw-r--r--   0 local      (503) staff       (20)    12702 2023-05-30 20:18:34.000000 klaviyo-api-2.0.1/src/openapi_client/model/static_schedule_options.py
--rw-r--r--   0 local      (503) staff       (20)    11547 2023-05-30 20:18:34.000000 klaviyo-api-2.0.1/src/openapi_client/model/sto_schedule_options.py
--rw-r--r--   0 local      (503) staff       (20)    12979 2023-05-30 20:18:34.000000 klaviyo-api-2.0.1/src/openapi_client/model/subscription.py
--rw-r--r--   0 local      (503) staff       (20)    12200 2023-05-30 20:18:34.000000 klaviyo-api-2.0.1/src/openapi_client/model/subscription_channels.py
--rw-r--r--   0 local      (503) staff       (20)    11991 2023-05-30 20:18:34.000000 klaviyo-api-2.0.1/src/openapi_client/model/subscription_create_job_create_query.py
--rw-r--r--   0 local      (503) staff       (20)    12668 2023-05-30 20:18:35.000000 klaviyo-api-2.0.1/src/openapi_client/model/subscription_create_job_create_query_resource_object.py
--rw-r--r--   0 local      (503) staff       (20)    12750 2023-05-30 20:18:35.000000 klaviyo-api-2.0.1/src/openapi_client/model/subscription_create_job_create_query_resource_object_attributes.py
--rw-r--r--   0 local      (503) staff       (20)    11693 2023-05-30 20:18:35.000000 klaviyo-api-2.0.1/src/openapi_client/model/subscription_enum.py
--rw-r--r--   0 local      (503) staff       (20)    11949 2023-05-30 20:18:35.000000 klaviyo-api-2.0.1/src/openapi_client/model/subscriptions.py
--rw-r--r--   0 local      (503) staff       (20)    11598 2023-05-30 20:18:35.000000 klaviyo-api-2.0.1/src/openapi_client/model/suppression.py
--rw-r--r--   0 local      (503) staff       (20)    11981 2023-05-30 20:18:35.000000 klaviyo-api-2.0.1/src/openapi_client/model/suppression_create_job_create_query.py
--rw-r--r--   0 local      (503) staff       (20)    12651 2023-05-30 20:18:35.000000 klaviyo-api-2.0.1/src/openapi_client/model/suppression_create_job_create_query_resource_object.py
--rw-r--r--   0 local      (503) staff       (20)    11983 2023-05-30 20:18:35.000000 klaviyo-api-2.0.1/src/openapi_client/model/suppression_create_job_create_query_resource_object_attributes.py
--rw-r--r--   0 local      (503) staff       (20)    11770 2023-05-30 20:18:35.000000 klaviyo-api-2.0.1/src/openapi_client/model/tag_campaign_op.py
--rw-r--r--   0 local      (503) staff       (20)    11970 2023-05-30 20:18:35.000000 klaviyo-api-2.0.1/src/openapi_client/model/tag_campaign_op_data_inner.py
--rw-r--r--   0 local      (503) staff       (20)    11809 2023-05-30 20:18:35.000000 klaviyo-api-2.0.1/src/openapi_client/model/tag_create_query.py
--rw-r--r--   0 local      (503) staff       (20)    12279 2023-05-30 20:18:35.000000 klaviyo-api-2.0.1/src/openapi_client/model/tag_create_query_resource_object.py
--rw-r--r--   0 local      (503) staff       (20)    12174 2023-05-30 20:18:35.000000 klaviyo-api-2.0.1/src/openapi_client/model/tag_create_query_resource_object_attributes.py
--rw-r--r--   0 local      (503) staff       (20)    11558 2023-05-30 20:18:35.000000 klaviyo-api-2.0.1/src/openapi_client/model/tag_enum.py
--rw-r--r--   0 local      (503) staff       (20)    11730 2023-05-30 20:18:35.000000 klaviyo-api-2.0.1/src/openapi_client/model/tag_flow_op.py
--rw-r--r--   0 local      (503) staff       (20)    11926 2023-05-30 20:18:35.000000 klaviyo-api-2.0.1/src/openapi_client/model/tag_flow_op_data_inner.py
--rw-r--r--   0 local      (503) staff       (20)    11860 2023-05-30 20:18:35.000000 klaviyo-api-2.0.1/src/openapi_client/model/tag_group_create_query.py
--rw-r--r--   0 local      (503) staff       (20)    12366 2023-05-30 20:18:35.000000 klaviyo-api-2.0.1/src/openapi_client/model/tag_group_create_query_resource_object.py
--rw-r--r--   0 local      (503) staff       (20)    11858 2023-05-30 20:18:35.000000 klaviyo-api-2.0.1/src/openapi_client/model/tag_group_create_query_resource_object_attributes.py
--rw-r--r--   0 local      (503) staff       (20)    11645 2023-05-30 20:18:35.000000 klaviyo-api-2.0.1/src/openapi_client/model/tag_group_enum.py
--rw-r--r--   0 local      (503) staff       (20)    11860 2023-05-30 20:18:35.000000 klaviyo-api-2.0.1/src/openapi_client/model/tag_group_update_query.py
--rw-r--r--   0 local      (503) staff       (20)    12568 2023-05-30 20:18:35.000000 klaviyo-api-2.0.1/src/openapi_client/model/tag_group_update_query_resource_object.py
--rw-r--r--   0 local      (503) staff       (20)    11881 2023-05-30 20:18:35.000000 klaviyo-api-2.0.1/src/openapi_client/model/tag_group_update_query_resource_object_attributes.py
--rw-r--r--   0 local      (503) staff       (20)    11730 2023-05-30 20:18:35.000000 klaviyo-api-2.0.1/src/openapi_client/model/tag_list_op.py
--rw-r--r--   0 local      (503) staff       (20)    11926 2023-05-30 20:18:35.000000 klaviyo-api-2.0.1/src/openapi_client/model/tag_list_op_data_inner.py
--rw-r--r--   0 local      (503) staff       (20)    11760 2023-05-30 20:18:35.000000 klaviyo-api-2.0.1/src/openapi_client/model/tag_segment_op.py
--rw-r--r--   0 local      (503) staff       (20)    11959 2023-05-30 20:18:35.000000 klaviyo-api-2.0.1/src/openapi_client/model/tag_segment_op_data_inner.py
--rw-r--r--   0 local      (503) staff       (20)    11809 2023-05-30 20:18:35.000000 klaviyo-api-2.0.1/src/openapi_client/model/tag_update_query.py
--rw-r--r--   0 local      (503) staff       (20)    12469 2023-05-30 20:18:35.000000 klaviyo-api-2.0.1/src/openapi_client/model/tag_update_query_resource_object.py
--rw-r--r--   0 local      (503) staff       (20)    11625 2023-05-30 20:18:35.000000 klaviyo-api-2.0.1/src/openapi_client/model/tag_update_query_resource_object_attributes.py
--rw-r--r--   0 local      (503) staff       (20)    11849 2023-05-30 20:18:35.000000 klaviyo-api-2.0.1/src/openapi_client/model/template_clone_query.py
--rw-r--r--   0 local      (503) staff       (20)    12354 2023-05-30 20:18:35.000000 klaviyo-api-2.0.1/src/openapi_client/model/template_clone_query_resource_object.py
--rw-r--r--   0 local      (503) staff       (20)    12223 2023-05-30 20:18:35.000000 klaviyo-api-2.0.1/src/openapi_client/model/template_clone_query_resource_object_attributes.py
--rw-r--r--   0 local      (503) staff       (20)    11859 2023-05-30 20:18:35.000000 klaviyo-api-2.0.1/src/openapi_client/model/template_create_query.py
--rw-r--r--   0 local      (503) staff       (20)    12364 2023-05-30 20:18:35.000000 klaviyo-api-2.0.1/src/openapi_client/model/template_create_query_resource_object.py
--rw-r--r--   0 local      (503) staff       (20)    12887 2023-05-30 20:18:35.000000 klaviyo-api-2.0.1/src/openapi_client/model/template_create_query_resource_object_attributes.py
--rw-r--r--   0 local      (503) staff       (20)    11633 2023-05-30 20:18:35.000000 klaviyo-api-2.0.1/src/openapi_client/model/template_enum.py
--rw-r--r--   0 local      (503) staff       (20)    11859 2023-05-30 20:18:35.000000 klaviyo-api-2.0.1/src/openapi_client/model/template_render_query.py
--rw-r--r--   0 local      (503) staff       (20)    12364 2023-05-30 20:18:35.000000 klaviyo-api-2.0.1/src/openapi_client/model/template_render_query_resource_object.py
--rw-r--r--   0 local      (503) staff       (20)    12898 2023-05-30 20:18:35.000000 klaviyo-api-2.0.1/src/openapi_client/model/template_render_query_resource_object_attributes.py
--rw-r--r--   0 local      (503) staff       (20)    11859 2023-05-30 20:18:35.000000 klaviyo-api-2.0.1/src/openapi_client/model/template_update_query.py
--rw-r--r--   0 local      (503) staff       (20)    12570 2023-05-30 20:18:35.000000 klaviyo-api-2.0.1/src/openapi_client/model/template_update_query_resource_object.py
--rw-r--r--   0 local      (503) staff       (20)    12475 2023-05-30 20:18:35.000000 klaviyo-api-2.0.1/src/openapi_client/model/template_update_query_resource_object_attributes.py
--rw-r--r--   0 local      (503) staff       (20)    11879 2023-05-30 20:18:35.000000 klaviyo-api-2.0.1/src/openapi_client/model/test_api_analytics_sample_enum.py
--rw-r--r--   0 local      (503) staff       (20)    11645 2023-05-30 20:18:35.000000 klaviyo-api-2.0.1/src/openapi_client/model/test_list_enum.py
--rw-r--r--   0 local      (503) staff       (20)    12184 2023-05-30 20:18:35.000000 klaviyo-api-2.0.1/src/openapi_client/model/throttled_schedule_options.py
--rw-r--r--   0 local      (503) staff       (20)    13204 2023-05-30 20:18:35.000000 klaviyo-api-2.0.1/src/openapi_client/model/tracking_options_sub_object.py
--rw-r--r--   0 local      (503) staff       (20)    12011 2023-05-30 20:18:35.000000 klaviyo-api-2.0.1/src/openapi_client/model/unsubscription_create_job_create_query.py
--rw-r--r--   0 local      (503) staff       (20)    12702 2023-05-30 20:18:35.000000 klaviyo-api-2.0.1/src/openapi_client/model/unsubscription_create_job_create_query_resource_object.py
--rw-r--r--   0 local      (503) staff       (20)    12305 2023-05-30 20:18:35.000000 klaviyo-api-2.0.1/src/openapi_client/model/unsubscription_create_job_create_query_resource_object_attributes.py
--rw-r--r--   0 local      (503) staff       (20)    12001 2023-05-30 20:18:35.000000 klaviyo-api-2.0.1/src/openapi_client/model/unsuppression_create_job_create_query.py
--rw-r--r--   0 local      (503) staff       (20)    12685 2023-05-30 20:18:35.000000 klaviyo-api-2.0.1/src/openapi_client/model/unsuppression_create_job_create_query_resource_object.py
--rw-r--r--   0 local      (503) staff       (20)    11989 2023-05-30 20:18:35.000000 klaviyo-api-2.0.1/src/openapi_client/model/unsuppression_create_job_create_query_resource_object_attributes.py
--rw-r--r--   0 local      (503) staff       (20)    11689 2023-05-30 20:18:35.000000 klaviyo-api-2.0.1/src/openapi_client/model/utm_param_info.py
--rw-r--r--   0 local      (503) staff       (20)    11845 2023-05-30 20:18:35.000000 klaviyo-api-2.0.1/src/openapi_client/model/utm_params_sub_object.py
--rw-r--r--   0 local      (503) staff       (20)    82630 2023-05-30 20:18:36.000000 klaviyo-api-2.0.1/src/openapi_client/model_utils.py
-drwxr-xr-x   0 local      (503) staff       (20)        0 2023-05-30 20:18:45.932219 klaviyo-api-2.0.1/src/openapi_client/models/
--rw-r--r--   0 local      (503) staff       (20)    24813 2023-05-30 20:18:36.000000 klaviyo-api-2.0.1/src/openapi_client/models/__init__.py
--rw-r--r--   0 local      (503) staff       (20)    14324 2023-05-30 20:18:36.000000 klaviyo-api-2.0.1/src/openapi_client/rest.py
+drwxr-xr-x   0 local      (503) staff       (20)        0 2023-06-09 19:11:08.222437 klaviyo-api-2.0.2/
+-rw-r--r--   0 local      (503) staff       (20)     1063 2023-06-09 19:10:53.000000 klaviyo-api-2.0.2/LICENSE
+-rw-r--r--   0 local      (503) staff       (20)    55411 2023-06-09 19:11:08.223169 klaviyo-api-2.0.2/PKG-INFO
+-rw-r--r--   0 local      (503) staff       (20)    54894 2023-06-09 19:10:53.000000 klaviyo-api-2.0.2/README.md
+-rw-r--r--   0 local      (503) staff       (20)      103 2023-06-09 19:10:53.000000 klaviyo-api-2.0.2/pyproject.toml
+-rw-r--r--   0 local      (503) staff       (20)      801 2023-06-09 19:11:08.224583 klaviyo-api-2.0.2/setup.cfg
+drwxr-xr-x   0 local      (503) staff       (20)        0 2023-06-09 19:11:07.979222 klaviyo-api-2.0.2/src/
+drwxr-xr-x   0 local      (503) staff       (20)        0 2023-06-09 19:11:07.984390 klaviyo-api-2.0.2/src/klaviyo_api/
+-rw-r--r--   0 local      (503) staff       (20)      130 2023-06-09 19:10:53.000000 klaviyo-api-2.0.2/src/klaviyo_api/__init__.py
+-rw-r--r--   0 local      (503) staff       (20)      501 2023-06-09 19:10:53.000000 klaviyo-api-2.0.2/src/klaviyo_api/custom_retry.py
+-rw-r--r--   0 local      (503) staff       (20)    25983 2023-06-09 19:10:52.000000 klaviyo-api-2.0.2/src/klaviyo_api/wrapper.py
+drwxr-xr-x   0 local      (503) staff       (20)        0 2023-06-09 19:11:07.988615 klaviyo-api-2.0.2/src/klaviyo_api.egg-info/
+-rw-r--r--   0 local      (503) staff       (20)    55411 2023-06-09 19:11:07.000000 klaviyo-api-2.0.2/src/klaviyo_api.egg-info/PKG-INFO
+-rw-r--r--   0 local      (503) staff       (20)    15129 2023-06-09 19:11:07.000000 klaviyo-api-2.0.2/src/klaviyo_api.egg-info/SOURCES.txt
+-rw-r--r--   0 local      (503) staff       (20)        1 2023-06-09 19:11:07.000000 klaviyo-api-2.0.2/src/klaviyo_api.egg-info/dependency_links.txt
+-rw-r--r--   0 local      (503) staff       (20)      119 2023-06-09 19:11:07.000000 klaviyo-api-2.0.2/src/klaviyo_api.egg-info/requires.txt
+-rw-r--r--   0 local      (503) staff       (20)       27 2023-06-09 19:11:07.000000 klaviyo-api-2.0.2/src/klaviyo_api.egg-info/top_level.txt
+drwxr-xr-x   0 local      (503) staff       (20)        0 2023-06-09 19:11:07.994296 klaviyo-api-2.0.2/src/openapi_client/
+-rw-r--r--   0 local      (503) staff       (20)      788 2023-06-09 19:10:53.000000 klaviyo-api-2.0.2/src/openapi_client/__init__.py
+drwxr-xr-x   0 local      (503) staff       (20)        0 2023-06-09 19:11:08.008558 klaviyo-api-2.0.2/src/openapi_client/api/
+-rw-r--r--   0 local      (503) staff       (20)      220 2023-06-09 19:10:53.000000 klaviyo-api-2.0.2/src/openapi_client/api/__init__.py
+-rw-r--r--   0 local      (503) staff       (20)   108410 2023-06-09 19:10:51.000000 klaviyo-api-2.0.2/src/openapi_client/api/campaigns_api.py
+-rw-r--r--   0 local      (503) staff       (20)   351426 2023-06-09 19:10:51.000000 klaviyo-api-2.0.2/src/openapi_client/api/catalogs_api.py
+-rw-r--r--   0 local      (503) staff       (20)    19728 2023-06-09 19:10:51.000000 klaviyo-api-2.0.2/src/openapi_client/api/client_api.py
+-rw-r--r--   0 local      (503) staff       (20)     7236 2023-06-09 19:10:51.000000 klaviyo-api-2.0.2/src/openapi_client/api/data_privacy_api.py
+-rw-r--r--   0 local      (503) staff       (20)    58131 2023-06-09 19:10:51.000000 klaviyo-api-2.0.2/src/openapi_client/api/events_api.py
+-rw-r--r--   0 local      (503) staff       (20)   108931 2023-06-09 19:10:51.000000 klaviyo-api-2.0.2/src/openapi_client/api/flows_api.py
+-rw-r--r--   0 local      (503) staff       (20)    70516 2023-06-09 19:10:51.000000 klaviyo-api-2.0.2/src/openapi_client/api/lists_api.py
+-rw-r--r--   0 local      (503) staff       (20)    21844 2023-06-09 19:10:51.000000 klaviyo-api-2.0.2/src/openapi_client/api/metrics_api.py
+-rw-r--r--   0 local      (503) staff       (20)    86332 2023-06-09 19:10:51.000000 klaviyo-api-2.0.2/src/openapi_client/api/profiles_api.py
+-rw-r--r--   0 local      (503) staff       (20)    48324 2023-06-09 19:10:51.000000 klaviyo-api-2.0.2/src/openapi_client/api/segments_api.py
+-rw-r--r--   0 local      (503) staff       (20)   147862 2023-06-09 19:10:51.000000 klaviyo-api-2.0.2/src/openapi_client/api/tags_api.py
+-rw-r--r--   0 local      (503) staff       (20)    42670 2023-06-09 19:10:51.000000 klaviyo-api-2.0.2/src/openapi_client/api/templates_api.py
+-rw-r--r--   0 local      (503) staff       (20)    39451 2023-06-09 19:10:53.000000 klaviyo-api-2.0.2/src/openapi_client/api_client.py
+drwxr-xr-x   0 local      (503) staff       (20)        0 2023-06-09 19:11:08.009513 klaviyo-api-2.0.2/src/openapi_client/apis/
+-rw-r--r--   0 local      (503) staff       (20)     1084 2023-06-09 19:10:53.000000 klaviyo-api-2.0.2/src/openapi_client/apis/__init__.py
+-rw-r--r--   0 local      (503) staff       (20)    17158 2023-06-09 19:10:53.000000 klaviyo-api-2.0.2/src/openapi_client/configuration.py
+-rw-r--r--   0 local      (503) staff       (20)     5120 2023-06-09 19:10:53.000000 klaviyo-api-2.0.2/src/openapi_client/exceptions.py
+drwxr-xr-x   0 local      (503) staff       (20)        0 2023-06-09 19:11:08.220023 klaviyo-api-2.0.2/src/openapi_client/model/
+-rw-r--r--   0 local      (503) staff       (20)      348 2023-06-09 19:10:53.000000 klaviyo-api-2.0.2/src/openapi_client/model/__init__.py
+-rw-r--r--   0 local      (503) staff       (20)    11834 2023-06-09 19:10:48.000000 klaviyo-api-2.0.2/src/openapi_client/model/audiences_sub_object.py
+-rw-r--r--   0 local      (503) staff       (20)    11849 2023-06-09 19:10:48.000000 klaviyo-api-2.0.2/src/openapi_client/model/campaign_clone_query.py
+-rw-r--r--   0 local      (503) staff       (20)    12354 2023-06-09 19:10:48.000000 klaviyo-api-2.0.2/src/openapi_client/model/campaign_clone_query_resource_object.py
+-rw-r--r--   0 local      (503) staff       (20)    11954 2023-06-09 19:10:48.000000 klaviyo-api-2.0.2/src/openapi_client/model/campaign_clone_query_resource_object_attributes.py
+-rw-r--r--   0 local      (503) staff       (20)    11859 2023-06-09 19:10:48.000000 klaviyo-api-2.0.2/src/openapi_client/model/campaign_create_query.py
+-rw-r--r--   0 local      (503) staff       (20)    12364 2023-06-09 19:10:48.000000 klaviyo-api-2.0.2/src/openapi_client/model/campaign_create_query_resource_object.py
+-rw-r--r--   0 local      (503) staff       (20)    13914 2023-06-09 19:10:48.000000 klaviyo-api-2.0.2/src/openapi_client/model/campaign_create_query_resource_object_attributes.py
+-rw-r--r--   0 local      (503) staff       (20)    11633 2023-06-09 19:10:48.000000 klaviyo-api-2.0.2/src/openapi_client/model/campaign_enum.py
+-rw-r--r--   0 local      (503) staff       (20)    12011 2023-06-09 19:10:48.000000 klaviyo-api-2.0.2/src/openapi_client/model/campaign_message_assign_template_query.py
+-rw-r--r--   0 local      (503) staff       (20)    12566 2023-06-09 19:10:48.000000 klaviyo-api-2.0.2/src/openapi_client/model/campaign_message_assign_template_query_resource_object.py
+-rw-r--r--   0 local      (503) staff       (20)    12055 2023-06-09 19:10:48.000000 klaviyo-api-2.0.2/src/openapi_client/model/campaign_message_assign_template_query_resource_object_attributes.py
+-rw-r--r--   0 local      (503) staff       (20)    11750 2023-06-09 19:10:48.000000 klaviyo-api-2.0.2/src/openapi_client/model/campaign_message_enum.py
+-rw-r--r--   0 local      (503) staff       (20)    12001 2023-06-09 19:10:48.000000 klaviyo-api-2.0.2/src/openapi_client/model/campaign_message_partial_update_query.py
+-rw-r--r--   0 local      (503) staff       (20)    12786 2023-06-09 19:10:48.000000 klaviyo-api-2.0.2/src/openapi_client/model/campaign_message_partial_update_query_resource_object.py
+-rw-r--r--   0 local      (503) staff       (20)    12109 2023-06-09 19:10:48.000000 klaviyo-api-2.0.2/src/openapi_client/model/campaign_message_partial_update_query_resource_object_attributes.py
+-rw-r--r--   0 local      (503) staff       (20)    11930 2023-06-09 19:10:48.000000 klaviyo-api-2.0.2/src/openapi_client/model/campaign_partial_update_query.py
+-rw-r--r--   0 local      (503) staff       (20)    12667 2023-06-09 19:10:48.000000 klaviyo-api-2.0.2/src/openapi_client/model/campaign_partial_update_query_resource_object.py
+-rw-r--r--   0 local      (503) staff       (20)    13373 2023-06-09 19:10:48.000000 klaviyo-api-2.0.2/src/openapi_client/model/campaign_partial_update_query_resource_object_attributes.py
+-rw-r--r--   0 local      (503) staff       (20)    12082 2023-06-09 19:10:48.000000 klaviyo-api-2.0.2/src/openapi_client/model/campaign_recipient_estimation_job_create_query.py
+-rw-r--r--   0 local      (503) staff       (20)    12744 2023-06-09 19:10:48.000000 klaviyo-api-2.0.2/src/openapi_client/model/campaign_recipient_estimation_job_create_query_resource_object.py
+-rw-r--r--   0 local      (503) staff       (20)    11768 2023-06-09 19:10:48.000000 klaviyo-api-2.0.2/src/openapi_client/model/campaign_recipient_estimation_job_create_query_resource_object_attributes.py
+-rw-r--r--   0 local      (503) staff       (20)    11999 2023-06-09 19:10:48.000000 klaviyo-api-2.0.2/src/openapi_client/model/campaign_recipient_estimation_job_enum.py
+-rw-r--r--   0 local      (503) staff       (20)    11931 2023-06-09 19:10:48.000000 klaviyo-api-2.0.2/src/openapi_client/model/campaign_send_job_create_query.py
+-rw-r--r--   0 local      (503) staff       (20)    12487 2023-06-09 19:10:48.000000 klaviyo-api-2.0.2/src/openapi_client/model/campaign_send_job_create_query_resource_object.py
+-rw-r--r--   0 local      (503) staff       (20)    11675 2023-06-09 19:10:48.000000 klaviyo-api-2.0.2/src/openapi_client/model/campaign_send_job_create_query_resource_object_attributes.py
+-rw-r--r--   0 local      (503) staff       (20)    11762 2023-06-09 19:10:48.000000 klaviyo-api-2.0.2/src/openapi_client/model/campaign_send_job_enum.py
+-rw-r--r--   0 local      (503) staff       (20)    12002 2023-06-09 19:10:48.000000 klaviyo-api-2.0.2/src/openapi_client/model/campaign_send_job_partial_update_query.py
+-rw-r--r--   0 local      (503) staff       (20)    12848 2023-06-09 19:10:48.000000 klaviyo-api-2.0.2/src/openapi_client/model/campaign_send_job_partial_update_query_resource_object.py
+-rw-r--r--   0 local      (503) staff       (20)    11850 2023-06-09 19:10:48.000000 klaviyo-api-2.0.2/src/openapi_client/model/campaign_send_job_partial_update_query_resource_object_attributes.py
+-rw-r--r--   0 local      (503) staff       (20)    11981 2023-06-09 19:10:48.000000 klaviyo-api-2.0.2/src/openapi_client/model/catalog_category_bulk_create_job_enum.py
+-rw-r--r--   0 local      (503) staff       (20)    11981 2023-06-09 19:10:48.000000 klaviyo-api-2.0.2/src/openapi_client/model/catalog_category_bulk_delete_job_enum.py
+-rw-r--r--   0 local      (503) staff       (20)    11981 2023-06-09 19:10:48.000000 klaviyo-api-2.0.2/src/openapi_client/model/catalog_category_bulk_update_job_enum.py
+-rw-r--r--   0 local      (503) staff       (20)    12022 2023-06-09 19:10:48.000000 klaviyo-api-2.0.2/src/openapi_client/model/catalog_category_create_job_create_query.py
+-rw-r--r--   0 local      (503) staff       (20)    12671 2023-06-09 19:10:48.000000 klaviyo-api-2.0.2/src/openapi_client/model/catalog_category_create_job_create_query_resource_object.py
+-rw-r--r--   0 local      (503) staff       (20)    12179 2023-06-09 19:10:48.000000 klaviyo-api-2.0.2/src/openapi_client/model/catalog_category_create_job_create_query_resource_object_attributes.py
+-rw-r--r--   0 local      (503) staff       (20)    11930 2023-06-09 19:10:48.000000 klaviyo-api-2.0.2/src/openapi_client/model/catalog_category_create_query.py
+-rw-r--r--   0 local      (503) staff       (20)    13136 2023-06-09 19:10:48.000000 klaviyo-api-2.0.2/src/openapi_client/model/catalog_category_create_query_resource_object.py
+-rw-r--r--   0 local      (503) staff       (20)    13243 2023-06-09 19:10:48.000000 klaviyo-api-2.0.2/src/openapi_client/model/catalog_category_create_query_resource_object_attributes.py
+-rw-r--r--   0 local      (503) staff       (20)    12022 2023-06-09 19:10:49.000000 klaviyo-api-2.0.2/src/openapi_client/model/catalog_category_delete_job_create_query.py
+-rw-r--r--   0 local      (503) staff       (20)    12671 2023-06-09 19:10:49.000000 klaviyo-api-2.0.2/src/openapi_client/model/catalog_category_delete_job_create_query_resource_object.py
+-rw-r--r--   0 local      (503) staff       (20)    12179 2023-06-09 19:10:49.000000 klaviyo-api-2.0.2/src/openapi_client/model/catalog_category_delete_job_create_query_resource_object_attributes.py
+-rw-r--r--   0 local      (503) staff       (20)    12422 2023-06-09 19:10:49.000000 klaviyo-api-2.0.2/src/openapi_client/model/catalog_category_delete_query_resource_object.py
+-rw-r--r--   0 local      (503) staff       (20)    11750 2023-06-09 19:10:49.000000 klaviyo-api-2.0.2/src/openapi_client/model/catalog_category_enum.py
+-rw-r--r--   0 local      (503) staff       (20)    12114 2023-06-09 19:10:49.000000 klaviyo-api-2.0.2/src/openapi_client/model/catalog_category_item_op.py
+-rw-r--r--   0 local      (503) staff       (20)    12022 2023-06-09 19:10:49.000000 klaviyo-api-2.0.2/src/openapi_client/model/catalog_category_update_job_create_query.py
+-rw-r--r--   0 local      (503) staff       (20)    12671 2023-06-09 19:10:49.000000 klaviyo-api-2.0.2/src/openapi_client/model/catalog_category_update_job_create_query_resource_object.py
+-rw-r--r--   0 local      (503) staff       (20)    12179 2023-06-09 19:10:49.000000 klaviyo-api-2.0.2/src/openapi_client/model/catalog_category_update_job_create_query_resource_object_attributes.py
+-rw-r--r--   0 local      (503) staff       (20)    11930 2023-06-09 19:10:49.000000 klaviyo-api-2.0.2/src/openapi_client/model/catalog_category_update_query.py
+-rw-r--r--   0 local      (503) staff       (20)    13736 2023-06-09 19:10:49.000000 klaviyo-api-2.0.2/src/openapi_client/model/catalog_category_update_query_resource_object.py
+-rw-r--r--   0 local      (503) staff       (20)    11663 2023-06-09 19:10:49.000000 klaviyo-api-2.0.2/src/openapi_client/model/catalog_category_update_query_resource_object_attributes.py
+-rw-r--r--   0 local      (503) staff       (20)    12102 2023-06-09 19:10:49.000000 klaviyo-api-2.0.2/src/openapi_client/model/catalog_category_update_query_resource_object_relationships.py
+-rw-r--r--   0 local      (503) staff       (20)    12225 2023-06-09 19:10:49.000000 klaviyo-api-2.0.2/src/openapi_client/model/catalog_category_update_query_resource_object_relationships_items.py
+-rw-r--r--   0 local      (503) staff       (20)    12137 2023-06-09 19:10:49.000000 klaviyo-api-2.0.2/src/openapi_client/model/catalog_category_update_query_resource_object_relationships_items_data_inner.py
+-rw-r--r--   0 local      (503) staff       (20)    11921 2023-06-09 19:10:49.000000 klaviyo-api-2.0.2/src/openapi_client/model/catalog_item_bulk_create_job_enum.py
+-rw-r--r--   0 local      (503) staff       (20)    11921 2023-06-09 19:10:49.000000 klaviyo-api-2.0.2/src/openapi_client/model/catalog_item_bulk_delete_job_enum.py
+-rw-r--r--   0 local      (503) staff       (20)    11921 2023-06-09 19:10:49.000000 klaviyo-api-2.0.2/src/openapi_client/model/catalog_item_bulk_update_job_enum.py
+-rw-r--r--   0 local      (503) staff       (20)    12121 2023-06-09 19:10:49.000000 klaviyo-api-2.0.2/src/openapi_client/model/catalog_item_category_op.py
+-rw-r--r--   0 local      (503) staff       (20)    11982 2023-06-09 19:10:49.000000 klaviyo-api-2.0.2/src/openapi_client/model/catalog_item_create_job_create_query.py
+-rw-r--r--   0 local      (503) staff       (20)    12603 2023-06-09 19:10:49.000000 klaviyo-api-2.0.2/src/openapi_client/model/catalog_item_create_job_create_query_resource_object.py
+-rw-r--r--   0 local      (503) staff       (20)    12074 2023-06-09 19:10:49.000000 klaviyo-api-2.0.2/src/openapi_client/model/catalog_item_create_job_create_query_resource_object_attributes.py
+-rw-r--r--   0 local      (503) staff       (20)    11890 2023-06-09 19:10:49.000000 klaviyo-api-2.0.2/src/openapi_client/model/catalog_item_create_query.py
+-rw-r--r--   0 local      (503) staff       (20)    13040 2023-06-09 19:10:49.000000 klaviyo-api-2.0.2/src/openapi_client/model/catalog_item_create_query_resource_object.py
+-rw-r--r--   0 local      (503) staff       (20)    17029 2023-06-09 19:10:49.000000 klaviyo-api-2.0.2/src/openapi_client/model/catalog_item_create_query_resource_object_attributes.py
+-rw-r--r--   0 local      (503) staff       (20)    12122 2023-06-09 19:10:49.000000 klaviyo-api-2.0.2/src/openapi_client/model/catalog_item_create_query_resource_object_relationships.py
+-rw-r--r--   0 local      (503) staff       (20)    12235 2023-06-09 19:10:49.000000 klaviyo-api-2.0.2/src/openapi_client/model/catalog_item_create_query_resource_object_relationships_categories.py
+-rw-r--r--   0 local      (503) staff       (20)    12172 2023-06-09 19:10:49.000000 klaviyo-api-2.0.2/src/openapi_client/model/catalog_item_create_query_resource_object_relationships_categories_data_inner.py
+-rw-r--r--   0 local      (503) staff       (20)    11982 2023-06-09 19:10:49.000000 klaviyo-api-2.0.2/src/openapi_client/model/catalog_item_delete_job_create_query.py
+-rw-r--r--   0 local      (503) staff       (20)    12603 2023-06-09 19:10:49.000000 klaviyo-api-2.0.2/src/openapi_client/model/catalog_item_delete_job_create_query_resource_object.py
+-rw-r--r--   0 local      (503) staff       (20)    12074 2023-06-09 19:10:49.000000 klaviyo-api-2.0.2/src/openapi_client/model/catalog_item_delete_job_create_query_resource_object_attributes.py
+-rw-r--r--   0 local      (503) staff       (20)    12374 2023-06-09 19:10:49.000000 klaviyo-api-2.0.2/src/openapi_client/model/catalog_item_delete_query_resource_object.py
+-rw-r--r--   0 local      (503) staff       (20)    11690 2023-06-09 19:10:49.000000 klaviyo-api-2.0.2/src/openapi_client/model/catalog_item_enum.py
+-rw-r--r--   0 local      (503) staff       (20)    11982 2023-06-09 19:10:49.000000 klaviyo-api-2.0.2/src/openapi_client/model/catalog_item_update_job_create_query.py
+-rw-r--r--   0 local      (503) staff       (20)    12603 2023-06-09 19:10:49.000000 klaviyo-api-2.0.2/src/openapi_client/model/catalog_item_update_job_create_query_resource_object.py
+-rw-r--r--   0 local      (503) staff       (20)    12074 2023-06-09 19:10:49.000000 klaviyo-api-2.0.2/src/openapi_client/model/catalog_item_update_job_create_query_resource_object_attributes.py
+-rw-r--r--   0 local      (503) staff       (20)    11890 2023-06-09 19:10:49.000000 klaviyo-api-2.0.2/src/openapi_client/model/catalog_item_update_query.py
+-rw-r--r--   0 local      (503) staff       (20)    13632 2023-06-09 19:10:49.000000 klaviyo-api-2.0.2/src/openapi_client/model/catalog_item_update_query_resource_object.py
+-rw-r--r--   0 local      (503) staff       (20)    15281 2023-06-09 19:10:49.000000 klaviyo-api-2.0.2/src/openapi_client/model/catalog_item_update_query_resource_object_attributes.py
+-rw-r--r--   0 local      (503) staff       (20)    11966 2023-06-09 19:10:49.000000 klaviyo-api-2.0.2/src/openapi_client/model/catalog_variant_bulk_create_job_enum.py
+-rw-r--r--   0 local      (503) staff       (20)    11966 2023-06-09 19:10:49.000000 klaviyo-api-2.0.2/src/openapi_client/model/catalog_variant_bulk_delete_job_enum.py
+-rw-r--r--   0 local      (503) staff       (20)    11966 2023-06-09 19:10:49.000000 klaviyo-api-2.0.2/src/openapi_client/model/catalog_variant_bulk_update_job_enum.py
+-rw-r--r--   0 local      (503) staff       (20)    12012 2023-06-09 19:10:49.000000 klaviyo-api-2.0.2/src/openapi_client/model/catalog_variant_create_job_create_query.py
+-rw-r--r--   0 local      (503) staff       (20)    12654 2023-06-09 19:10:49.000000 klaviyo-api-2.0.2/src/openapi_client/model/catalog_variant_create_job_create_query_resource_object.py
+-rw-r--r--   0 local      (503) staff       (20)    12143 2023-06-09 19:10:49.000000 klaviyo-api-2.0.2/src/openapi_client/model/catalog_variant_create_job_create_query_resource_object_attributes.py
+-rw-r--r--   0 local      (503) staff       (20)    11920 2023-06-09 19:10:49.000000 klaviyo-api-2.0.2/src/openapi_client/model/catalog_variant_create_query.py
+-rw-r--r--   0 local      (503) staff       (20)    13119 2023-06-09 19:10:49.000000 klaviyo-api-2.0.2/src/openapi_client/model/catalog_variant_create_query_resource_object.py
+-rw-r--r--   0 local      (503) staff       (20)    19026 2023-06-09 19:10:49.000000 klaviyo-api-2.0.2/src/openapi_client/model/catalog_variant_create_query_resource_object_attributes.py
+-rw-r--r--   0 local      (503) staff       (20)    12012 2023-06-09 19:10:49.000000 klaviyo-api-2.0.2/src/openapi_client/model/catalog_variant_delete_job_create_query.py
+-rw-r--r--   0 local      (503) staff       (20)    12654 2023-06-09 19:10:49.000000 klaviyo-api-2.0.2/src/openapi_client/model/catalog_variant_delete_job_create_query_resource_object.py
+-rw-r--r--   0 local      (503) staff       (20)    12143 2023-06-09 19:10:49.000000 klaviyo-api-2.0.2/src/openapi_client/model/catalog_variant_delete_job_create_query_resource_object_attributes.py
+-rw-r--r--   0 local      (503) staff       (20)    12410 2023-06-09 19:10:49.000000 klaviyo-api-2.0.2/src/openapi_client/model/catalog_variant_delete_query_resource_object.py
+-rw-r--r--   0 local      (503) staff       (20)    11735 2023-06-09 19:10:49.000000 klaviyo-api-2.0.2/src/openapi_client/model/catalog_variant_enum.py
+-rw-r--r--   0 local      (503) staff       (20)    12012 2023-06-09 19:10:49.000000 klaviyo-api-2.0.2/src/openapi_client/model/catalog_variant_update_job_create_query.py
+-rw-r--r--   0 local      (503) staff       (20)    12654 2023-06-09 19:10:49.000000 klaviyo-api-2.0.2/src/openapi_client/model/catalog_variant_update_job_create_query_resource_object.py
+-rw-r--r--   0 local      (503) staff       (20)    12143 2023-06-09 19:10:49.000000 klaviyo-api-2.0.2/src/openapi_client/model/catalog_variant_update_job_create_query_resource_object_attributes.py
+-rw-r--r--   0 local      (503) staff       (20)    11920 2023-06-09 19:10:49.000000 klaviyo-api-2.0.2/src/openapi_client/model/catalog_variant_update_query.py
+-rw-r--r--   0 local      (503) staff       (20)    13066 2023-06-09 19:10:49.000000 klaviyo-api-2.0.2/src/openapi_client/model/catalog_variant_update_query_resource_object.py
+-rw-r--r--   0 local      (503) staff       (20)    17148 2023-06-09 19:10:49.000000 klaviyo-api-2.0.2/src/openapi_client/model/catalog_variant_update_query_resource_object_attributes.py
+-rw-r--r--   0 local      (503) staff       (20)    13057 2023-06-09 19:10:49.000000 klaviyo-api-2.0.2/src/openapi_client/model/content_sub_object.py
+-rw-r--r--   0 local      (503) staff       (20)    12002 2023-06-09 19:10:49.000000 klaviyo-api-2.0.2/src/openapi_client/model/data_privacy_create_deletion_job_query.py
+-rw-r--r--   0 local      (503) staff       (20)    12608 2023-06-09 19:10:49.000000 klaviyo-api-2.0.2/src/openapi_client/model/data_privacy_create_deletion_job_query_resource_object.py
+-rw-r--r--   0 local      (503) staff       (20)    12449 2023-06-09 19:10:49.000000 klaviyo-api-2.0.2/src/openapi_client/model/data_privacy_create_deletion_job_query_resource_object_attributes.py
+-rw-r--r--   0 local      (503) staff       (20)    11879 2023-06-09 19:10:49.000000 klaviyo-api-2.0.2/src/openapi_client/model/data_privacy_deletion_job_enum.py
+-rw-r--r--   0 local      (503) staff       (20)    11829 2023-06-09 19:10:49.000000 klaviyo-api-2.0.2/src/openapi_client/model/event_create_query.py
+-rw-r--r--   0 local      (503) staff       (20)    12313 2023-06-09 19:10:49.000000 klaviyo-api-2.0.2/src/openapi_client/model/event_create_query_resource_object.py
+-rw-r--r--   0 local      (503) staff       (20)    17076 2023-06-09 19:10:49.000000 klaviyo-api-2.0.2/src/openapi_client/model/event_create_query_resource_object_attributes.py
+-rw-r--r--   0 local      (503) staff       (20)    11588 2023-06-09 19:10:49.000000 klaviyo-api-2.0.2/src/openapi_client/model/event_enum.py
+-rw-r--r--   0 local      (503) staff       (20)    11573 2023-06-09 19:10:49.000000 klaviyo-api-2.0.2/src/openapi_client/model/flow_enum.py
+-rw-r--r--   0 local      (503) staff       (20)    11819 2023-06-09 19:10:49.000000 klaviyo-api-2.0.2/src/openapi_client/model/flow_update_query.py
+-rw-r--r--   0 local      (503) staff       (20)    12538 2023-06-09 19:10:49.000000 klaviyo-api-2.0.2/src/openapi_client/model/flow_update_query_resource_object.py
+-rw-r--r--   0 local      (503) staff       (20)    11764 2023-06-09 19:10:50.000000 klaviyo-api-2.0.2/src/openapi_client/model/flow_update_query_resource_object_attributes.py
+-rw-r--r--   0 local      (503) staff       (20)    11999 2023-06-09 19:10:50.000000 klaviyo-api-2.0.2/src/openapi_client/model/get_create_variants_jobs5_xx_response.py
+-rw-r--r--   0 local      (503) staff       (20)    12816 2023-06-09 19:10:50.000000 klaviyo-api-2.0.2/src/openapi_client/model/get_create_variants_jobs5_xx_response_errors_inner.py
+-rw-r--r--   0 local      (503) staff       (20)    11775 2023-06-09 19:10:50.000000 klaviyo-api-2.0.2/src/openapi_client/model/get_create_variants_jobs5_xx_response_errors_inner_source.py
+-rw-r--r--   0 local      (503) staff       (20)    11819 2023-06-09 19:10:50.000000 klaviyo-api-2.0.2/src/openapi_client/model/list_create_query.py
+-rw-r--r--   0 local      (503) staff       (20)    12296 2023-06-09 19:10:50.000000 klaviyo-api-2.0.2/src/openapi_client/model/list_create_query_resource_object.py
+-rw-r--r--   0 local      (503) staff       (20)    11668 2023-06-09 19:10:50.000000 klaviyo-api-2.0.2/src/openapi_client/model/list_create_query_resource_object_attributes.py
+-rw-r--r--   0 local      (503) staff       (20)    11573 2023-06-09 19:10:50.000000 klaviyo-api-2.0.2/src/openapi_client/model/list_enum.py
+-rw-r--r--   0 local      (503) staff       (20)    11831 2023-06-09 19:10:50.000000 klaviyo-api-2.0.2/src/openapi_client/model/list_members_add_query.py
+-rw-r--r--   0 local      (503) staff       (20)    11980 2023-06-09 19:10:50.000000 klaviyo-api-2.0.2/src/openapi_client/model/list_members_add_query_data_inner.py
+-rw-r--r--   0 local      (503) staff       (20)    11840 2023-06-09 19:10:50.000000 klaviyo-api-2.0.2/src/openapi_client/model/list_members_delete_query.py
+-rw-r--r--   0 local      (503) staff       (20)    11890 2023-06-09 19:10:50.000000 klaviyo-api-2.0.2/src/openapi_client/model/list_partial_update_query.py
+-rw-r--r--   0 local      (503) staff       (20)    12625 2023-06-09 19:10:50.000000 klaviyo-api-2.0.2/src/openapi_client/model/list_partial_update_query_resource_object.py
+-rw-r--r--   0 local      (503) staff       (20)    11750 2023-06-09 19:10:50.000000 klaviyo-api-2.0.2/src/openapi_client/model/metric_aggregate_enum.py
+-rw-r--r--   0 local      (503) staff       (20)    11869 2023-06-09 19:10:50.000000 klaviyo-api-2.0.2/src/openapi_client/model/metric_aggregate_query.py
+-rw-r--r--   0 local      (503) staff       (20)    12424 2023-06-09 19:10:50.000000 klaviyo-api-2.0.2/src/openapi_client/model/metric_aggregate_query_resource_object.py
+-rw-r--r--   0 local      (503) staff       (20)    21013 2023-06-09 19:10:50.000000 klaviyo-api-2.0.2/src/openapi_client/model/metric_aggregate_query_resource_object_attributes.py
+-rw-r--r--   0 local      (503) staff       (20)    11996 2023-06-09 19:10:50.000000 klaviyo-api-2.0.2/src/openapi_client/model/metric_create_query.py
+-rw-r--r--   0 local      (503) staff       (20)    11910 2023-06-09 19:10:50.000000 klaviyo-api-2.0.2/src/openapi_client/model/onsite_profile_create_query.py
+-rw-r--r--   0 local      (503) staff       (20)    12408 2023-06-09 19:10:50.000000 klaviyo-api-2.0.2/src/openapi_client/model/onsite_profile_create_query_resource_object.py
+-rw-r--r--   0 local      (503) staff       (20)    15425 2023-06-09 19:10:50.000000 klaviyo-api-2.0.2/src/openapi_client/model/onsite_profile_create_query_resource_object_attributes.py
+-rw-r--r--   0 local      (503) staff       (20)    11960 2023-06-09 19:10:50.000000 klaviyo-api-2.0.2/src/openapi_client/model/onsite_subscription_create_query.py
+-rw-r--r--   0 local      (503) staff       (20)    12493 2023-06-09 19:10:50.000000 klaviyo-api-2.0.2/src/openapi_client/model/onsite_subscription_create_query_resource_object.py
+-rw-r--r--   0 local      (503) staff       (20)    13508 2023-06-09 19:10:50.000000 klaviyo-api-2.0.2/src/openapi_client/model/onsite_subscription_create_query_resource_object_attributes.py
+-rw-r--r--   0 local      (503) staff       (20)    11849 2023-06-09 19:10:50.000000 klaviyo-api-2.0.2/src/openapi_client/model/profile_create_query.py
+-rw-r--r--   0 local      (503) staff       (20)    12347 2023-06-09 19:10:50.000000 klaviyo-api-2.0.2/src/openapi_client/model/profile_create_query_resource_object.py
+-rw-r--r--   0 local      (503) staff       (20)    15156 2023-06-09 19:10:50.000000 klaviyo-api-2.0.2/src/openapi_client/model/profile_create_query_resource_object_attributes.py
+-rw-r--r--   0 local      (503) staff       (20)    11618 2023-06-09 19:10:50.000000 klaviyo-api-2.0.2/src/openapi_client/model/profile_enum.py
+-rw-r--r--   0 local      (503) staff       (20)    13961 2023-06-09 19:10:50.000000 klaviyo-api-2.0.2/src/openapi_client/model/profile_location.py
+-rw-r--r--   0 local      (503) staff       (20)    11301 2023-06-09 19:10:50.000000 klaviyo-api-2.0.2/src/openapi_client/model/profile_location_latitude.py
+-rw-r--r--   0 local      (503) staff       (20)    11304 2023-06-09 19:10:50.000000 klaviyo-api-2.0.2/src/openapi_client/model/profile_location_longitude.py
+-rw-r--r--   0 local      (503) staff       (20)    11920 2023-06-09 19:10:50.000000 klaviyo-api-2.0.2/src/openapi_client/model/profile_partial_update_query.py
+-rw-r--r--   0 local      (503) staff       (20)    12725 2023-06-09 19:10:50.000000 klaviyo-api-2.0.2/src/openapi_client/model/profile_partial_update_query_resource_object.py
+-rw-r--r--   0 local      (503) staff       (20)    12041 2023-06-09 19:10:50.000000 klaviyo-api-2.0.2/src/openapi_client/model/profile_subscription_bulk_create_job_enum.py
+-rw-r--r--   0 local      (503) staff       (20)    12026 2023-06-09 19:10:50.000000 klaviyo-api-2.0.2/src/openapi_client/model/profile_suppression_bulk_create_job_enum.py
+-rw-r--r--   0 local      (503) staff       (20)    12071 2023-06-09 19:10:50.000000 klaviyo-api-2.0.2/src/openapi_client/model/profile_unsubscription_bulk_create_job_enum.py
+-rw-r--r--   0 local      (503) staff       (20)    12056 2023-06-09 19:10:50.000000 klaviyo-api-2.0.2/src/openapi_client/model/profile_unsuppression_bulk_create_job_enum.py
+-rw-r--r--   0 local      (503) staff       (20)    11618 2023-06-09 19:10:50.000000 klaviyo-api-2.0.2/src/openapi_client/model/segment_enum.py
+-rw-r--r--   0 local      (503) staff       (20)    11920 2023-06-09 19:10:50.000000 klaviyo-api-2.0.2/src/openapi_client/model/segment_partial_update_query.py
+-rw-r--r--   0 local      (503) staff       (20)    12586 2023-06-09 19:10:50.000000 klaviyo-api-2.0.2/src/openapi_client/model/segment_partial_update_query_resource_object.py
+-rw-r--r--   0 local      (503) staff       (20)    11632 2023-06-09 19:10:50.000000 klaviyo-api-2.0.2/src/openapi_client/model/segment_partial_update_query_resource_object_attributes.py
+-rw-r--r--   0 local      (503) staff       (20)    11612 2023-06-09 19:10:50.000000 klaviyo-api-2.0.2/src/openapi_client/model/send_options_sub_object.py
+-rw-r--r--   0 local      (503) staff       (20)    13115 2023-06-09 19:10:50.000000 klaviyo-api-2.0.2/src/openapi_client/model/send_strategy_sub_object.py
+-rw-r--r--   0 local      (503) staff       (20)    12702 2023-06-09 19:10:50.000000 klaviyo-api-2.0.2/src/openapi_client/model/static_schedule_options.py
+-rw-r--r--   0 local      (503) staff       (20)    11547 2023-06-09 19:10:50.000000 klaviyo-api-2.0.2/src/openapi_client/model/sto_schedule_options.py
+-rw-r--r--   0 local      (503) staff       (20)    12979 2023-06-09 19:10:50.000000 klaviyo-api-2.0.2/src/openapi_client/model/subscription.py
+-rw-r--r--   0 local      (503) staff       (20)    12200 2023-06-09 19:10:50.000000 klaviyo-api-2.0.2/src/openapi_client/model/subscription_channels.py
+-rw-r--r--   0 local      (503) staff       (20)    11991 2023-06-09 19:10:50.000000 klaviyo-api-2.0.2/src/openapi_client/model/subscription_create_job_create_query.py
+-rw-r--r--   0 local      (503) staff       (20)    12668 2023-06-09 19:10:50.000000 klaviyo-api-2.0.2/src/openapi_client/model/subscription_create_job_create_query_resource_object.py
+-rw-r--r--   0 local      (503) staff       (20)    12750 2023-06-09 19:10:50.000000 klaviyo-api-2.0.2/src/openapi_client/model/subscription_create_job_create_query_resource_object_attributes.py
+-rw-r--r--   0 local      (503) staff       (20)    11693 2023-06-09 19:10:50.000000 klaviyo-api-2.0.2/src/openapi_client/model/subscription_enum.py
+-rw-r--r--   0 local      (503) staff       (20)    11598 2023-06-09 19:10:50.000000 klaviyo-api-2.0.2/src/openapi_client/model/suppression.py
+-rw-r--r--   0 local      (503) staff       (20)    11981 2023-06-09 19:10:50.000000 klaviyo-api-2.0.2/src/openapi_client/model/suppression_create_job_create_query.py
+-rw-r--r--   0 local      (503) staff       (20)    12651 2023-06-09 19:10:50.000000 klaviyo-api-2.0.2/src/openapi_client/model/suppression_create_job_create_query_resource_object.py
+-rw-r--r--   0 local      (503) staff       (20)    11983 2023-06-09 19:10:50.000000 klaviyo-api-2.0.2/src/openapi_client/model/suppression_create_job_create_query_resource_object_attributes.py
+-rw-r--r--   0 local      (503) staff       (20)    11770 2023-06-09 19:10:50.000000 klaviyo-api-2.0.2/src/openapi_client/model/tag_campaign_op.py
+-rw-r--r--   0 local      (503) staff       (20)    11970 2023-06-09 19:10:50.000000 klaviyo-api-2.0.2/src/openapi_client/model/tag_campaign_op_data_inner.py
+-rw-r--r--   0 local      (503) staff       (20)    11809 2023-06-09 19:10:50.000000 klaviyo-api-2.0.2/src/openapi_client/model/tag_create_query.py
+-rw-r--r--   0 local      (503) staff       (20)    12279 2023-06-09 19:10:50.000000 klaviyo-api-2.0.2/src/openapi_client/model/tag_create_query_resource_object.py
+-rw-r--r--   0 local      (503) staff       (20)    12174 2023-06-09 19:10:50.000000 klaviyo-api-2.0.2/src/openapi_client/model/tag_create_query_resource_object_attributes.py
+-rw-r--r--   0 local      (503) staff       (20)    11558 2023-06-09 19:10:50.000000 klaviyo-api-2.0.2/src/openapi_client/model/tag_enum.py
+-rw-r--r--   0 local      (503) staff       (20)    11730 2023-06-09 19:10:50.000000 klaviyo-api-2.0.2/src/openapi_client/model/tag_flow_op.py
+-rw-r--r--   0 local      (503) staff       (20)    11926 2023-06-09 19:10:50.000000 klaviyo-api-2.0.2/src/openapi_client/model/tag_flow_op_data_inner.py
+-rw-r--r--   0 local      (503) staff       (20)    11860 2023-06-09 19:10:50.000000 klaviyo-api-2.0.2/src/openapi_client/model/tag_group_create_query.py
+-rw-r--r--   0 local      (503) staff       (20)    12366 2023-06-09 19:10:50.000000 klaviyo-api-2.0.2/src/openapi_client/model/tag_group_create_query_resource_object.py
+-rw-r--r--   0 local      (503) staff       (20)    11858 2023-06-09 19:10:50.000000 klaviyo-api-2.0.2/src/openapi_client/model/tag_group_create_query_resource_object_attributes.py
+-rw-r--r--   0 local      (503) staff       (20)    11645 2023-06-09 19:10:50.000000 klaviyo-api-2.0.2/src/openapi_client/model/tag_group_enum.py
+-rw-r--r--   0 local      (503) staff       (20)    11860 2023-06-09 19:10:50.000000 klaviyo-api-2.0.2/src/openapi_client/model/tag_group_update_query.py
+-rw-r--r--   0 local      (503) staff       (20)    12568 2023-06-09 19:10:50.000000 klaviyo-api-2.0.2/src/openapi_client/model/tag_group_update_query_resource_object.py
+-rw-r--r--   0 local      (503) staff       (20)    11881 2023-06-09 19:10:50.000000 klaviyo-api-2.0.2/src/openapi_client/model/tag_group_update_query_resource_object_attributes.py
+-rw-r--r--   0 local      (503) staff       (20)    11730 2023-06-09 19:10:50.000000 klaviyo-api-2.0.2/src/openapi_client/model/tag_list_op.py
+-rw-r--r--   0 local      (503) staff       (20)    11926 2023-06-09 19:10:50.000000 klaviyo-api-2.0.2/src/openapi_client/model/tag_list_op_data_inner.py
+-rw-r--r--   0 local      (503) staff       (20)    11760 2023-06-09 19:10:50.000000 klaviyo-api-2.0.2/src/openapi_client/model/tag_segment_op.py
+-rw-r--r--   0 local      (503) staff       (20)    11959 2023-06-09 19:10:50.000000 klaviyo-api-2.0.2/src/openapi_client/model/tag_segment_op_data_inner.py
+-rw-r--r--   0 local      (503) staff       (20)    11809 2023-06-09 19:10:50.000000 klaviyo-api-2.0.2/src/openapi_client/model/tag_update_query.py
+-rw-r--r--   0 local      (503) staff       (20)    12469 2023-06-09 19:10:50.000000 klaviyo-api-2.0.2/src/openapi_client/model/tag_update_query_resource_object.py
+-rw-r--r--   0 local      (503) staff       (20)    11625 2023-06-09 19:10:50.000000 klaviyo-api-2.0.2/src/openapi_client/model/tag_update_query_resource_object_attributes.py
+-rw-r--r--   0 local      (503) staff       (20)    11849 2023-06-09 19:10:50.000000 klaviyo-api-2.0.2/src/openapi_client/model/template_clone_query.py
+-rw-r--r--   0 local      (503) staff       (20)    12354 2023-06-09 19:10:50.000000 klaviyo-api-2.0.2/src/openapi_client/model/template_clone_query_resource_object.py
+-rw-r--r--   0 local      (503) staff       (20)    12223 2023-06-09 19:10:50.000000 klaviyo-api-2.0.2/src/openapi_client/model/template_clone_query_resource_object_attributes.py
+-rw-r--r--   0 local      (503) staff       (20)    11859 2023-06-09 19:10:50.000000 klaviyo-api-2.0.2/src/openapi_client/model/template_create_query.py
+-rw-r--r--   0 local      (503) staff       (20)    12364 2023-06-09 19:10:50.000000 klaviyo-api-2.0.2/src/openapi_client/model/template_create_query_resource_object.py
+-rw-r--r--   0 local      (503) staff       (20)    12887 2023-06-09 19:10:50.000000 klaviyo-api-2.0.2/src/openapi_client/model/template_create_query_resource_object_attributes.py
+-rw-r--r--   0 local      (503) staff       (20)    11633 2023-06-09 19:10:50.000000 klaviyo-api-2.0.2/src/openapi_client/model/template_enum.py
+-rw-r--r--   0 local      (503) staff       (20)    11859 2023-06-09 19:10:50.000000 klaviyo-api-2.0.2/src/openapi_client/model/template_render_query.py
+-rw-r--r--   0 local      (503) staff       (20)    12364 2023-06-09 19:10:50.000000 klaviyo-api-2.0.2/src/openapi_client/model/template_render_query_resource_object.py
+-rw-r--r--   0 local      (503) staff       (20)    12898 2023-06-09 19:10:50.000000 klaviyo-api-2.0.2/src/openapi_client/model/template_render_query_resource_object_attributes.py
+-rw-r--r--   0 local      (503) staff       (20)    11859 2023-06-09 19:10:50.000000 klaviyo-api-2.0.2/src/openapi_client/model/template_update_query.py
+-rw-r--r--   0 local      (503) staff       (20)    12570 2023-06-09 19:10:50.000000 klaviyo-api-2.0.2/src/openapi_client/model/template_update_query_resource_object.py
+-rw-r--r--   0 local      (503) staff       (20)    12475 2023-06-09 19:10:50.000000 klaviyo-api-2.0.2/src/openapi_client/model/template_update_query_resource_object_attributes.py
+-rw-r--r--   0 local      (503) staff       (20)    12184 2023-06-09 19:10:50.000000 klaviyo-api-2.0.2/src/openapi_client/model/throttled_schedule_options.py
+-rw-r--r--   0 local      (503) staff       (20)    13204 2023-06-09 19:10:50.000000 klaviyo-api-2.0.2/src/openapi_client/model/tracking_options_sub_object.py
+-rw-r--r--   0 local      (503) staff       (20)    12011 2023-06-09 19:10:50.000000 klaviyo-api-2.0.2/src/openapi_client/model/unsubscription_create_job_create_query.py
+-rw-r--r--   0 local      (503) staff       (20)    12702 2023-06-09 19:10:50.000000 klaviyo-api-2.0.2/src/openapi_client/model/unsubscription_create_job_create_query_resource_object.py
+-rw-r--r--   0 local      (503) staff       (20)    12305 2023-06-09 19:10:50.000000 klaviyo-api-2.0.2/src/openapi_client/model/unsubscription_create_job_create_query_resource_object_attributes.py
+-rw-r--r--   0 local      (503) staff       (20)    12001 2023-06-09 19:10:50.000000 klaviyo-api-2.0.2/src/openapi_client/model/unsuppression_create_job_create_query.py
+-rw-r--r--   0 local      (503) staff       (20)    12685 2023-06-09 19:10:50.000000 klaviyo-api-2.0.2/src/openapi_client/model/unsuppression_create_job_create_query_resource_object.py
+-rw-r--r--   0 local      (503) staff       (20)    11989 2023-06-09 19:10:50.000000 klaviyo-api-2.0.2/src/openapi_client/model/unsuppression_create_job_create_query_resource_object_attributes.py
+-rw-r--r--   0 local      (503) staff       (20)    11845 2023-06-09 19:10:50.000000 klaviyo-api-2.0.2/src/openapi_client/model/utm_params_sub_object.py
+-rw-r--r--   0 local      (503) staff       (20)    82630 2023-06-09 19:10:53.000000 klaviyo-api-2.0.2/src/openapi_client/model_utils.py
+drwxr-xr-x   0 local      (503) staff       (20)        0 2023-06-09 19:11:08.221569 klaviyo-api-2.0.2/src/openapi_client/models/
+-rw-r--r--   0 local      (503) staff       (20)    22673 2023-06-09 19:10:53.000000 klaviyo-api-2.0.2/src/openapi_client/models/__init__.py
+-rw-r--r--   0 local      (503) staff       (20)    14324 2023-06-09 19:10:53.000000 klaviyo-api-2.0.2/src/openapi_client/rest.py
```

### Comparing `klaviyo-api-2.0.1/LICENSE` & `klaviyo-api-2.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.1/PKG-INFO` & `klaviyo-api-2.0.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,10 @@
-Metadata-Version: 2.1
-Name: klaviyo-api
-Version: 2.0.1
-Summary: Klaviyo Python SDK
-Home-page: https://github.com/klaviyo/klaviyo-api-python
-Author: Klaviyo Developers
-Author-email: developers@klaviyo.com
-Project-URL: API Docs, https://developers.klaviyo.com/en/reference/api_overview
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Klaviyo Python SDK
 
-- SDK version: 2.0.1
+- SDK version: 2.0.2
 - API revision: 2023-02-22
 
 ## Helpful Resources
 
 - [API Reference](https://developers.klaviyo.com/en/v2023-02-22/reference)
 - [API Guides](https://developers.klaviyo.com/en/v2023-02-22/docs)
 - [Postman Workspace](https://www.postman.com/klaviyo/workspace/klaviyo-developers)
@@ -118,14 +103,81 @@
 
 ### Example request
 
 ```python
 klaviyo.Metrics.get_metrics() 
 ```
 
+### Use Case Examples
+
+#### How to use filtering, sorting, and spare fieldset JSON API features
+
+**Use Case**: Get events associated with a specific metric, then return just the event properties sorted by oldest to newest datetime.
+
+```python
+klaviyo.Events.get_events(
+    fields_event=['event_properties'], 
+    filter="equals(metric_id,\"aBc123\")", 
+    sort='-datetime'
+    )
+```
+
+NOTE: the filter param values need to be url-encoded
+
+#### How to filter based on datetime
+
+**Use Case**: Get profiles that have been updated between two datetimes.
+
+```python
+klaviyo.Profiles.get_profiles(
+    filter='less-than(updated,2023-04-26T00:00:00Z),greater-than(updated,2023-04-19T00:00:00Z)'
+    )
+```
+
+#### How to use pagination and the page[size] param
+
+**Use Case**: Use cursor-based pagination to get the next 20 profile records.
+
+```python
+klaviyo.Profiles.get_profiles(
+    page_cursor="https://a.klaviyo.com/api/profiles/?page%5Bcursor%5D=bmV4dDo6aWQ6OjAxRjNaWk5ITlRYMUtFVEhQMzJTUzRBN0ZY",
+    page_size=20
+)
+```
+
+NOTE: This page cursor value is exactly what is returned in the `self`/`next`/`prev` response values
+
+#### How to add additional information to your API response via additional-fields and the `includes` parameter
+
+**Use Case**: Get a specific profile, return an additional predictive analytics field, and also return the list objects associated with the profile.
+
+```python
+klaviyo.Profiles.get_profile(
+    '01GDDKASAP8TKDDA2GRZDSVP4H', 
+    additional_fields_profile=['predictive_analytics'], 
+    include=['lists']
+)
+```
+
+#### How to use our relationship endpoints to see related resources
+
+**Use Case**: Get all list memberships for a profile with the given `profile_id`.
+
+```python
+klaviyo.Profiles.get_profile_relationships_lists('01GDDKASAP8TKDDA2GRZDSVP4H')
+```
+
+#### How to see what Klaviyo objects are associated with a specific tag
+
+**Use Case**: Get all campaigns associated with the given `tag_id`.
+
+```python
+klaviyo.Tags.get_tag_relationships_campaigns('9c8db7a0-5ab5-4e3c-9a37-a3224fd14382')
+```
+
 ## Error Handling
 
 This SDK throws an `ApiException` error when the server returns a non-`2XX` response. 
 
 An `ApiException` consists of the following attributes:
 
 * `status` : `int`
@@ -1507,17 +1559,18 @@
 # action_id | str
 
 ## Keyword Arguments
 
 # fields_flow_message | [str]
 # filter | str
 # page_cursor | str
+# page_size | int
 # sort | str
 
-klaviyo.Flows.get_flow_action_messages(action_id, fields_flow_message=fields_flow_message, filter=filter, page_cursor=page_cursor, sort=sort)
+klaviyo.Flows.get_flow_action_messages(action_id, fields_flow_message=fields_flow_message, filter=filter, page_cursor=page_cursor, page_size=page_size, sort=sort)
 ```
 
 
 
 
 #### [Get Flow Action Relationships Flow](https://developers.klaviyo.com/en/v2023-02-22/reference/get_flow_action_relationships_flow)
 
@@ -1539,17 +1592,18 @@
 
 # id | str
 
 ## Keyword Arguments
 
 # filter | str
 # page_cursor | str
+# page_size | int
 # sort | str
 
-klaviyo.Flows.get_flow_action_relationships_messages(id, filter=filter, page_cursor=page_cursor, sort=sort)
+klaviyo.Flows.get_flow_action_relationships_messages(id, filter=filter, page_cursor=page_cursor, page_size=page_size, sort=sort)
 ```
 
 
 
 
 #### [Get Flow Actions For Flow](https://developers.klaviyo.com/en/v2023-02-22/reference/get_flow_flow_actions)
 
@@ -1559,17 +1613,18 @@
 # flow_id | str
 
 ## Keyword Arguments
 
 # fields_flow_action | [str]
 # filter | str
 # page_cursor | str
+# page_size | int
 # sort | str
 
-klaviyo.Flows.get_flow_flow_actions(flow_id, fields_flow_action=fields_flow_action, filter=filter, page_cursor=page_cursor, sort=sort)
+klaviyo.Flows.get_flow_flow_actions(flow_id, fields_flow_action=fields_flow_action, filter=filter, page_cursor=page_cursor, page_size=page_size, sort=sort)
 ```
 
 
 
 
 #### [Get Flow Message](https://developers.klaviyo.com/en/v2023-02-22/reference/get_flow_message)
 
@@ -1626,17 +1681,18 @@
 ## Positional Arguments
 
 # id | str
 
 ## Keyword Arguments
 
 # filter | str
+# page_size | int
 # sort | str
 
-klaviyo.Flows.get_flow_relationships_flow_actions(id, filter=filter, sort=sort)
+klaviyo.Flows.get_flow_relationships_flow_actions(id, filter=filter, page_size=page_size, sort=sort)
 ```
 
 
 
 
 #### [Get Flow Relationships Tags](https://developers.klaviyo.com/en/v2023-02-22/reference/get_flow_relationships_tags)
 
@@ -1675,17 +1731,18 @@
 ## Keyword Arguments
 
 # fields_flow_action | [str]
 # fields_flow | [str]
 # filter | str
 # include | [str]
 # page_cursor | str
+# page_size | int
 # sort | str
 
-klaviyo.Flows.get_flows(fields_flow_action=fields_flow_action, fields_flow=fields_flow, filter=filter, include=include, page_cursor=page_cursor, sort=sort)
+klaviyo.Flows.get_flows(fields_flow_action=fields_flow_action, fields_flow=fields_flow, filter=filter, include=include, page_cursor=page_cursor, page_size=page_size, sort=sort)
 ```
 
 
 
 
 #### [Update Flow Status](https://developers.klaviyo.com/en/v2023-02-22/reference/update_flow)
 
@@ -1931,19 +1988,15 @@
 #### [Create Profile](https://developers.klaviyo.com/en/v2023-02-22/reference/create_profile)
 
 ```python
 ## Positional Arguments
 
 # body | dict
 
-## Keyword Arguments
-
-# additional_fields_profile | [str]
-
-klaviyo.Profiles.create_profile(body, additional_fields_profile=additional_fields_profile)
+klaviyo.Profiles.create_profile(body)
 ```
 
 
 
 
 #### [Get Profile](https://developers.klaviyo.com/en/v2023-02-22/reference/get_profile)
 
@@ -2032,18 +2085,18 @@
 
 ## Keyword Arguments
 
 # additional_fields_profile | [str]
 # fields_profile | [str]
 # filter | str
 # page_cursor | str
-# sort | str
 # page_size | int
+# sort | str
 
-klaviyo.Profiles.get_profiles(additional_fields_profile=additional_fields_profile, fields_profile=fields_profile, filter=filter, page_cursor=page_cursor, sort=sort, page_size=page_size)
+klaviyo.Profiles.get_profiles(additional_fields_profile=additional_fields_profile, fields_profile=fields_profile, filter=filter, page_cursor=page_cursor, page_size=page_size, sort=sort)
 ```
 
 
 
 
 #### [Subscribe Profiles](https://developers.klaviyo.com/en/v2023-02-22/reference/subscribe_profiles)
 
@@ -2101,19 +2154,15 @@
 
 ```python
 ## Positional Arguments
 
 # id | str
 # body | dict
 
-## Keyword Arguments
-
-# additional_fields_profile | [str]
-
-klaviyo.Profiles.update_profile(id, body, additional_fields_profile=additional_fields_profile)
+klaviyo.Profiles.update_profile(id, body)
 ```
 
 
 
 
 
 
@@ -2748,8 +2797,8 @@
 4. There is no need to pass in your private `api_key` for any operations, as it is defined upon client instantiation; public key is still required where applicable. However, you can pass in an optional `api_key` kwarg to override the client private key for a specific call (REMINDER: don't do this client-side).
 
 ## Namespace
 
 In the interest of making the SDK Pythonic, we made the following namespace changes *relative* to the language agnostic resources up top (API Docs, Guides, etc).
 
 - Resource names use Title + Snake Casing, (e.g. `Data_Privacy`)
-- function names and parameter names use snake case (e.g. `get_metrics`, and `profile_id`)
+- function names and parameter names use snake case (e.g. `get_metrics`, and `profile_id`)
```

### Comparing `klaviyo-api-2.0.1/README.md` & `klaviyo-api-2.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,25 @@
+Metadata-Version: 2.1
+Name: klaviyo-api
+Version: 2.0.2
+Summary: Klaviyo Python SDK
+Home-page: https://github.com/klaviyo/klaviyo-api-python
+Author: Klaviyo Developers
+Author-email: developers@klaviyo.com
+Project-URL: API Docs, https://developers.klaviyo.com/en/reference/api_overview
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # Klaviyo Python SDK
 
-- SDK version: 2.0.1
+- SDK version: 2.0.2
 - API revision: 2023-02-22
 
 ## Helpful Resources
 
 - [API Reference](https://developers.klaviyo.com/en/v2023-02-22/reference)
 - [API Guides](https://developers.klaviyo.com/en/v2023-02-22/docs)
 - [Postman Workspace](https://www.postman.com/klaviyo/workspace/klaviyo-developers)
@@ -103,14 +118,81 @@
 
 ### Example request
 
 ```python
 klaviyo.Metrics.get_metrics() 
 ```
 
+### Use Case Examples
+
+#### How to use filtering, sorting, and spare fieldset JSON API features
+
+**Use Case**: Get events associated with a specific metric, then return just the event properties sorted by oldest to newest datetime.
+
+```python
+klaviyo.Events.get_events(
+    fields_event=['event_properties'], 
+    filter="equals(metric_id,\"aBc123\")", 
+    sort='-datetime'
+    )
+```
+
+NOTE: the filter param values need to be url-encoded
+
+#### How to filter based on datetime
+
+**Use Case**: Get profiles that have been updated between two datetimes.
+
+```python
+klaviyo.Profiles.get_profiles(
+    filter='less-than(updated,2023-04-26T00:00:00Z),greater-than(updated,2023-04-19T00:00:00Z)'
+    )
+```
+
+#### How to use pagination and the page[size] param
+
+**Use Case**: Use cursor-based pagination to get the next 20 profile records.
+
+```python
+klaviyo.Profiles.get_profiles(
+    page_cursor="https://a.klaviyo.com/api/profiles/?page%5Bcursor%5D=bmV4dDo6aWQ6OjAxRjNaWk5ITlRYMUtFVEhQMzJTUzRBN0ZY",
+    page_size=20
+)
+```
+
+NOTE: This page cursor value is exactly what is returned in the `self`/`next`/`prev` response values
+
+#### How to add additional information to your API response via additional-fields and the `includes` parameter
+
+**Use Case**: Get a specific profile, return an additional predictive analytics field, and also return the list objects associated with the profile.
+
+```python
+klaviyo.Profiles.get_profile(
+    '01GDDKASAP8TKDDA2GRZDSVP4H', 
+    additional_fields_profile=['predictive_analytics'], 
+    include=['lists']
+)
+```
+
+#### How to use our relationship endpoints to see related resources
+
+**Use Case**: Get all list memberships for a profile with the given `profile_id`.
+
+```python
+klaviyo.Profiles.get_profile_relationships_lists('01GDDKASAP8TKDDA2GRZDSVP4H')
+```
+
+#### How to see what Klaviyo objects are associated with a specific tag
+
+**Use Case**: Get all campaigns associated with the given `tag_id`.
+
+```python
+klaviyo.Tags.get_tag_relationships_campaigns('9c8db7a0-5ab5-4e3c-9a37-a3224fd14382')
+```
+
 ## Error Handling
 
 This SDK throws an `ApiException` error when the server returns a non-`2XX` response. 
 
 An `ApiException` consists of the following attributes:
 
 * `status` : `int`
@@ -1492,17 +1574,18 @@
 # action_id | str
 
 ## Keyword Arguments
 
 # fields_flow_message | [str]
 # filter | str
 # page_cursor | str
+# page_size | int
 # sort | str
 
-klaviyo.Flows.get_flow_action_messages(action_id, fields_flow_message=fields_flow_message, filter=filter, page_cursor=page_cursor, sort=sort)
+klaviyo.Flows.get_flow_action_messages(action_id, fields_flow_message=fields_flow_message, filter=filter, page_cursor=page_cursor, page_size=page_size, sort=sort)
 ```
 
 
 
 
 #### [Get Flow Action Relationships Flow](https://developers.klaviyo.com/en/v2023-02-22/reference/get_flow_action_relationships_flow)
 
@@ -1524,17 +1607,18 @@
 
 # id | str
 
 ## Keyword Arguments
 
 # filter | str
 # page_cursor | str
+# page_size | int
 # sort | str
 
-klaviyo.Flows.get_flow_action_relationships_messages(id, filter=filter, page_cursor=page_cursor, sort=sort)
+klaviyo.Flows.get_flow_action_relationships_messages(id, filter=filter, page_cursor=page_cursor, page_size=page_size, sort=sort)
 ```
 
 
 
 
 #### [Get Flow Actions For Flow](https://developers.klaviyo.com/en/v2023-02-22/reference/get_flow_flow_actions)
 
@@ -1544,17 +1628,18 @@
 # flow_id | str
 
 ## Keyword Arguments
 
 # fields_flow_action | [str]
 # filter | str
 # page_cursor | str
+# page_size | int
 # sort | str
 
-klaviyo.Flows.get_flow_flow_actions(flow_id, fields_flow_action=fields_flow_action, filter=filter, page_cursor=page_cursor, sort=sort)
+klaviyo.Flows.get_flow_flow_actions(flow_id, fields_flow_action=fields_flow_action, filter=filter, page_cursor=page_cursor, page_size=page_size, sort=sort)
 ```
 
 
 
 
 #### [Get Flow Message](https://developers.klaviyo.com/en/v2023-02-22/reference/get_flow_message)
 
@@ -1611,17 +1696,18 @@
 ## Positional Arguments
 
 # id | str
 
 ## Keyword Arguments
 
 # filter | str
+# page_size | int
 # sort | str
 
-klaviyo.Flows.get_flow_relationships_flow_actions(id, filter=filter, sort=sort)
+klaviyo.Flows.get_flow_relationships_flow_actions(id, filter=filter, page_size=page_size, sort=sort)
 ```
 
 
 
 
 #### [Get Flow Relationships Tags](https://developers.klaviyo.com/en/v2023-02-22/reference/get_flow_relationships_tags)
 
@@ -1660,17 +1746,18 @@
 ## Keyword Arguments
 
 # fields_flow_action | [str]
 # fields_flow | [str]
 # filter | str
 # include | [str]
 # page_cursor | str
+# page_size | int
 # sort | str
 
-klaviyo.Flows.get_flows(fields_flow_action=fields_flow_action, fields_flow=fields_flow, filter=filter, include=include, page_cursor=page_cursor, sort=sort)
+klaviyo.Flows.get_flows(fields_flow_action=fields_flow_action, fields_flow=fields_flow, filter=filter, include=include, page_cursor=page_cursor, page_size=page_size, sort=sort)
 ```
 
 
 
 
 #### [Update Flow Status](https://developers.klaviyo.com/en/v2023-02-22/reference/update_flow)
 
@@ -1916,19 +2003,15 @@
 #### [Create Profile](https://developers.klaviyo.com/en/v2023-02-22/reference/create_profile)
 
 ```python
 ## Positional Arguments
 
 # body | dict
 
-## Keyword Arguments
-
-# additional_fields_profile | [str]
-
-klaviyo.Profiles.create_profile(body, additional_fields_profile=additional_fields_profile)
+klaviyo.Profiles.create_profile(body)
 ```
 
 
 
 
 #### [Get Profile](https://developers.klaviyo.com/en/v2023-02-22/reference/get_profile)
 
@@ -2017,18 +2100,18 @@
 
 ## Keyword Arguments
 
 # additional_fields_profile | [str]
 # fields_profile | [str]
 # filter | str
 # page_cursor | str
-# sort | str
 # page_size | int
+# sort | str
 
-klaviyo.Profiles.get_profiles(additional_fields_profile=additional_fields_profile, fields_profile=fields_profile, filter=filter, page_cursor=page_cursor, sort=sort, page_size=page_size)
+klaviyo.Profiles.get_profiles(additional_fields_profile=additional_fields_profile, fields_profile=fields_profile, filter=filter, page_cursor=page_cursor, page_size=page_size, sort=sort)
 ```
 
 
 
 
 #### [Subscribe Profiles](https://developers.klaviyo.com/en/v2023-02-22/reference/subscribe_profiles)
 
@@ -2086,19 +2169,15 @@
 
 ```python
 ## Positional Arguments
 
 # id | str
 # body | dict
 
-## Keyword Arguments
-
-# additional_fields_profile | [str]
-
-klaviyo.Profiles.update_profile(id, body, additional_fields_profile=additional_fields_profile)
+klaviyo.Profiles.update_profile(id, body)
 ```
 
 
 
 
 
 
@@ -2733,8 +2812,8 @@
 4. There is no need to pass in your private `api_key` for any operations, as it is defined upon client instantiation; public key is still required where applicable. However, you can pass in an optional `api_key` kwarg to override the client private key for a specific call (REMINDER: don't do this client-side).
 
 ## Namespace
 
 In the interest of making the SDK Pythonic, we made the following namespace changes *relative* to the language agnostic resources up top (API Docs, Guides, etc).
 
 - Resource names use Title + Snake Casing, (e.g. `Data_Privacy`)
-- function names and parameter names use snake case (e.g. `get_metrics`, and `profile_id`)
+- function names and parameter names use snake case (e.g. `get_metrics`, and `profile_id`)
```

### Comparing `klaviyo-api-2.0.1/setup.cfg` & `klaviyo-api-2.0.2/setup.cfg`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = klaviyo-api
-version = 2.0.1
+version = 2.0.2
 author = Klaviyo Developers
 author_email = developers@klaviyo.com
 description = Klaviyo Python SDK
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/klaviyo/klaviyo-api-python
 project_urls =
```

### Comparing `klaviyo-api-2.0.1/src/klaviyo_api/wrapper.py` & `klaviyo-api-2.0.2/src/klaviyo_api/wrapper.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.1/src/klaviyo_api.egg-info/PKG-INFO` & `klaviyo-api-2.0.2/src/klaviyo_api.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: klaviyo-api
-Version: 2.0.1
+Version: 2.0.2
 Summary: Klaviyo Python SDK
 Home-page: https://github.com/klaviyo/klaviyo-api-python
 Author: Klaviyo Developers
 Author-email: developers@klaviyo.com
 Project-URL: API Docs, https://developers.klaviyo.com/en/reference/api_overview
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Klaviyo Python SDK
 
-- SDK version: 2.0.1
+- SDK version: 2.0.2
 - API revision: 2023-02-22
 
 ## Helpful Resources
 
 - [API Reference](https://developers.klaviyo.com/en/v2023-02-22/reference)
 - [API Guides](https://developers.klaviyo.com/en/v2023-02-22/docs)
 - [Postman Workspace](https://www.postman.com/klaviyo/workspace/klaviyo-developers)
@@ -118,14 +118,81 @@
 
 ### Example request
 
 ```python
 klaviyo.Metrics.get_metrics() 
 ```
 
+### Use Case Examples
+
+#### How to use filtering, sorting, and spare fieldset JSON API features
+
+**Use Case**: Get events associated with a specific metric, then return just the event properties sorted by oldest to newest datetime.
+
+```python
+klaviyo.Events.get_events(
+    fields_event=['event_properties'], 
+    filter="equals(metric_id,\"aBc123\")", 
+    sort='-datetime'
+    )
+```
+
+NOTE: the filter param values need to be url-encoded
+
+#### How to filter based on datetime
+
+**Use Case**: Get profiles that have been updated between two datetimes.
+
+```python
+klaviyo.Profiles.get_profiles(
+    filter='less-than(updated,2023-04-26T00:00:00Z),greater-than(updated,2023-04-19T00:00:00Z)'
+    )
+```
+
+#### How to use pagination and the page[size] param
+
+**Use Case**: Use cursor-based pagination to get the next 20 profile records.
+
+```python
+klaviyo.Profiles.get_profiles(
+    page_cursor="https://a.klaviyo.com/api/profiles/?page%5Bcursor%5D=bmV4dDo6aWQ6OjAxRjNaWk5ITlRYMUtFVEhQMzJTUzRBN0ZY",
+    page_size=20
+)
+```
+
+NOTE: This page cursor value is exactly what is returned in the `self`/`next`/`prev` response values
+
+#### How to add additional information to your API response via additional-fields and the `includes` parameter
+
+**Use Case**: Get a specific profile, return an additional predictive analytics field, and also return the list objects associated with the profile.
+
+```python
+klaviyo.Profiles.get_profile(
+    '01GDDKASAP8TKDDA2GRZDSVP4H', 
+    additional_fields_profile=['predictive_analytics'], 
+    include=['lists']
+)
+```
+
+#### How to use our relationship endpoints to see related resources
+
+**Use Case**: Get all list memberships for a profile with the given `profile_id`.
+
+```python
+klaviyo.Profiles.get_profile_relationships_lists('01GDDKASAP8TKDDA2GRZDSVP4H')
+```
+
+#### How to see what Klaviyo objects are associated with a specific tag
+
+**Use Case**: Get all campaigns associated with the given `tag_id`.
+
+```python
+klaviyo.Tags.get_tag_relationships_campaigns('9c8db7a0-5ab5-4e3c-9a37-a3224fd14382')
+```
+
 ## Error Handling
 
 This SDK throws an `ApiException` error when the server returns a non-`2XX` response. 
 
 An `ApiException` consists of the following attributes:
 
 * `status` : `int`
@@ -1507,17 +1574,18 @@
 # action_id | str
 
 ## Keyword Arguments
 
 # fields_flow_message | [str]
 # filter | str
 # page_cursor | str
+# page_size | int
 # sort | str
 
-klaviyo.Flows.get_flow_action_messages(action_id, fields_flow_message=fields_flow_message, filter=filter, page_cursor=page_cursor, sort=sort)
+klaviyo.Flows.get_flow_action_messages(action_id, fields_flow_message=fields_flow_message, filter=filter, page_cursor=page_cursor, page_size=page_size, sort=sort)
 ```
 
 
 
 
 #### [Get Flow Action Relationships Flow](https://developers.klaviyo.com/en/v2023-02-22/reference/get_flow_action_relationships_flow)
 
@@ -1539,17 +1607,18 @@
 
 # id | str
 
 ## Keyword Arguments
 
 # filter | str
 # page_cursor | str
+# page_size | int
 # sort | str
 
-klaviyo.Flows.get_flow_action_relationships_messages(id, filter=filter, page_cursor=page_cursor, sort=sort)
+klaviyo.Flows.get_flow_action_relationships_messages(id, filter=filter, page_cursor=page_cursor, page_size=page_size, sort=sort)
 ```
 
 
 
 
 #### [Get Flow Actions For Flow](https://developers.klaviyo.com/en/v2023-02-22/reference/get_flow_flow_actions)
 
@@ -1559,17 +1628,18 @@
 # flow_id | str
 
 ## Keyword Arguments
 
 # fields_flow_action | [str]
 # filter | str
 # page_cursor | str
+# page_size | int
 # sort | str
 
-klaviyo.Flows.get_flow_flow_actions(flow_id, fields_flow_action=fields_flow_action, filter=filter, page_cursor=page_cursor, sort=sort)
+klaviyo.Flows.get_flow_flow_actions(flow_id, fields_flow_action=fields_flow_action, filter=filter, page_cursor=page_cursor, page_size=page_size, sort=sort)
 ```
 
 
 
 
 #### [Get Flow Message](https://developers.klaviyo.com/en/v2023-02-22/reference/get_flow_message)
 
@@ -1626,17 +1696,18 @@
 ## Positional Arguments
 
 # id | str
 
 ## Keyword Arguments
 
 # filter | str
+# page_size | int
 # sort | str
 
-klaviyo.Flows.get_flow_relationships_flow_actions(id, filter=filter, sort=sort)
+klaviyo.Flows.get_flow_relationships_flow_actions(id, filter=filter, page_size=page_size, sort=sort)
 ```
 
 
 
 
 #### [Get Flow Relationships Tags](https://developers.klaviyo.com/en/v2023-02-22/reference/get_flow_relationships_tags)
 
@@ -1675,17 +1746,18 @@
 ## Keyword Arguments
 
 # fields_flow_action | [str]
 # fields_flow | [str]
 # filter | str
 # include | [str]
 # page_cursor | str
+# page_size | int
 # sort | str
 
-klaviyo.Flows.get_flows(fields_flow_action=fields_flow_action, fields_flow=fields_flow, filter=filter, include=include, page_cursor=page_cursor, sort=sort)
+klaviyo.Flows.get_flows(fields_flow_action=fields_flow_action, fields_flow=fields_flow, filter=filter, include=include, page_cursor=page_cursor, page_size=page_size, sort=sort)
 ```
 
 
 
 
 #### [Update Flow Status](https://developers.klaviyo.com/en/v2023-02-22/reference/update_flow)
 
@@ -1931,19 +2003,15 @@
 #### [Create Profile](https://developers.klaviyo.com/en/v2023-02-22/reference/create_profile)
 
 ```python
 ## Positional Arguments
 
 # body | dict
 
-## Keyword Arguments
-
-# additional_fields_profile | [str]
-
-klaviyo.Profiles.create_profile(body, additional_fields_profile=additional_fields_profile)
+klaviyo.Profiles.create_profile(body)
 ```
 
 
 
 
 #### [Get Profile](https://developers.klaviyo.com/en/v2023-02-22/reference/get_profile)
 
@@ -2032,18 +2100,18 @@
 
 ## Keyword Arguments
 
 # additional_fields_profile | [str]
 # fields_profile | [str]
 # filter | str
 # page_cursor | str
-# sort | str
 # page_size | int
+# sort | str
 
-klaviyo.Profiles.get_profiles(additional_fields_profile=additional_fields_profile, fields_profile=fields_profile, filter=filter, page_cursor=page_cursor, sort=sort, page_size=page_size)
+klaviyo.Profiles.get_profiles(additional_fields_profile=additional_fields_profile, fields_profile=fields_profile, filter=filter, page_cursor=page_cursor, page_size=page_size, sort=sort)
 ```
 
 
 
 
 #### [Subscribe Profiles](https://developers.klaviyo.com/en/v2023-02-22/reference/subscribe_profiles)
 
@@ -2101,19 +2169,15 @@
 
 ```python
 ## Positional Arguments
 
 # id | str
 # body | dict
 
-## Keyword Arguments
-
-# additional_fields_profile | [str]
-
-klaviyo.Profiles.update_profile(id, body, additional_fields_profile=additional_fields_profile)
+klaviyo.Profiles.update_profile(id, body)
 ```
```

### Comparing `klaviyo-api-2.0.1/src/klaviyo_api.egg-info/SOURCES.txt` & `klaviyo-api-2.0.2/src/klaviyo_api.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -45,15 +45,14 @@
 src/openapi_client/model/campaign_message_enum.py
 src/openapi_client/model/campaign_message_partial_update_query.py
 src/openapi_client/model/campaign_message_partial_update_query_resource_object.py
 src/openapi_client/model/campaign_message_partial_update_query_resource_object_attributes.py
 src/openapi_client/model/campaign_partial_update_query.py
 src/openapi_client/model/campaign_partial_update_query_resource_object.py
 src/openapi_client/model/campaign_partial_update_query_resource_object_attributes.py
-src/openapi_client/model/campaign_recipient_estimation_enum.py
 src/openapi_client/model/campaign_recipient_estimation_job_create_query.py
 src/openapi_client/model/campaign_recipient_estimation_job_create_query_resource_object.py
 src/openapi_client/model/campaign_recipient_estimation_job_create_query_resource_object_attributes.py
 src/openapi_client/model/campaign_recipient_estimation_job_enum.py
 src/openapi_client/model/campaign_send_job_create_query.py
 src/openapi_client/model/campaign_send_job_create_query_resource_object.py
 src/openapi_client/model/campaign_send_job_create_query_resource_object_attributes.py
@@ -105,15 +104,14 @@
 src/openapi_client/model/catalog_item_enum.py
 src/openapi_client/model/catalog_item_update_job_create_query.py
 src/openapi_client/model/catalog_item_update_job_create_query_resource_object.py
 src/openapi_client/model/catalog_item_update_job_create_query_resource_object_attributes.py
 src/openapi_client/model/catalog_item_update_query.py
 src/openapi_client/model/catalog_item_update_query_resource_object.py
 src/openapi_client/model/catalog_item_update_query_resource_object_attributes.py
-src/openapi_client/model/catalog_job_error_payload.py
 src/openapi_client/model/catalog_variant_bulk_create_job_enum.py
 src/openapi_client/model/catalog_variant_bulk_delete_job_enum.py
 src/openapi_client/model/catalog_variant_bulk_update_job_enum.py
 src/openapi_client/model/catalog_variant_create_job_create_query.py
 src/openapi_client/model/catalog_variant_create_job_create_query_resource_object.py
 src/openapi_client/model/catalog_variant_create_job_create_query_resource_object_attributes.py
 src/openapi_client/model/catalog_variant_create_query.py
@@ -126,34 +124,24 @@
 src/openapi_client/model/catalog_variant_enum.py
 src/openapi_client/model/catalog_variant_update_job_create_query.py
 src/openapi_client/model/catalog_variant_update_job_create_query_resource_object.py
 src/openapi_client/model/catalog_variant_update_job_create_query_resource_object_attributes.py
 src/openapi_client/model/catalog_variant_update_query.py
 src/openapi_client/model/catalog_variant_update_query_resource_object.py
 src/openapi_client/model/catalog_variant_update_query_resource_object_attributes.py
-src/openapi_client/model/collection_links.py
 src/openapi_client/model/content_sub_object.py
 src/openapi_client/model/data_privacy_create_deletion_job_query.py
 src/openapi_client/model/data_privacy_create_deletion_job_query_resource_object.py
 src/openapi_client/model/data_privacy_create_deletion_job_query_resource_object_attributes.py
 src/openapi_client/model/data_privacy_deletion_job_enum.py
-src/openapi_client/model/email_channel.py
-src/openapi_client/model/email_marketing.py
-src/openapi_client/model/email_marketing_list_suppression.py
-src/openapi_client/model/email_marketing_suppression.py
-src/openapi_client/model/email_message_content.py
-src/openapi_client/model/email_tracking_options.py
-src/openapi_client/model/error_source.py
 src/openapi_client/model/event_create_query.py
 src/openapi_client/model/event_create_query_resource_object.py
 src/openapi_client/model/event_create_query_resource_object_attributes.py
 src/openapi_client/model/event_enum.py
-src/openapi_client/model/flow_action_enum.py
 src/openapi_client/model/flow_enum.py
-src/openapi_client/model/flow_message_enum.py
 src/openapi_client/model/flow_update_query.py
 src/openapi_client/model/flow_update_query_resource_object.py
 src/openapi_client/model/flow_update_query_resource_object_attributes.py
 src/openapi_client/model/get_create_variants_jobs5_xx_response.py
 src/openapi_client/model/get_create_variants_jobs5_xx_response_errors_inner.py
 src/openapi_client/model/get_create_variants_jobs5_xx_response_errors_inner_source.py
 src/openapi_client/model/list_create_query.py
@@ -165,28 +153,21 @@
 src/openapi_client/model/list_members_delete_query.py
 src/openapi_client/model/list_partial_update_query.py
 src/openapi_client/model/list_partial_update_query_resource_object.py
 src/openapi_client/model/metric_aggregate_enum.py
 src/openapi_client/model/metric_aggregate_query.py
 src/openapi_client/model/metric_aggregate_query_resource_object.py
 src/openapi_client/model/metric_aggregate_query_resource_object_attributes.py
-src/openapi_client/model/metric_aggregate_row_dto.py
 src/openapi_client/model/metric_create_query.py
-src/openapi_client/model/metric_enum.py
-src/openapi_client/model/object_links.py
 src/openapi_client/model/onsite_profile_create_query.py
 src/openapi_client/model/onsite_profile_create_query_resource_object.py
 src/openapi_client/model/onsite_profile_create_query_resource_object_attributes.py
-src/openapi_client/model/onsite_profile_meta.py
-src/openapi_client/model/onsite_profile_meta_identifiers.py
 src/openapi_client/model/onsite_subscription_create_query.py
 src/openapi_client/model/onsite_subscription_create_query_resource_object.py
 src/openapi_client/model/onsite_subscription_create_query_resource_object_attributes.py
-src/openapi_client/model/predictive_analytics.py
-src/openapi_client/model/profile_aggregate_enum.py
 src/openapi_client/model/profile_create_query.py
 src/openapi_client/model/profile_create_query_resource_object.py
 src/openapi_client/model/profile_create_query_resource_object_attributes.py
 src/openapi_client/model/profile_enum.py
 src/openapi_client/model/profile_location.py
 src/openapi_client/model/profile_location_latitude.py
 src/openapi_client/model/profile_location_longitude.py
@@ -196,32 +177,24 @@
 src/openapi_client/model/profile_suppression_bulk_create_job_enum.py
 src/openapi_client/model/profile_unsubscription_bulk_create_job_enum.py
 src/openapi_client/model/profile_unsuppression_bulk_create_job_enum.py
 src/openapi_client/model/segment_enum.py
 src/openapi_client/model/segment_partial_update_query.py
 src/openapi_client/model/segment_partial_update_query_resource_object.py
 src/openapi_client/model/segment_partial_update_query_resource_object_attributes.py
-src/openapi_client/model/send_options.py
 src/openapi_client/model/send_options_sub_object.py
 src/openapi_client/model/send_strategy_sub_object.py
-src/openapi_client/model/send_time_sub_object.py
-src/openapi_client/model/sms_channel.py
-src/openapi_client/model/sms_marketing.py
-src/openapi_client/model/sms_message_content.py
-src/openapi_client/model/sms_render_options.py
-src/openapi_client/model/sms_tracking_options.py
 src/openapi_client/model/static_schedule_options.py
 src/openapi_client/model/sto_schedule_options.py
 src/openapi_client/model/subscription.py
 src/openapi_client/model/subscription_channels.py
 src/openapi_client/model/subscription_create_job_create_query.py
 src/openapi_client/model/subscription_create_job_create_query_resource_object.py
 src/openapi_client/model/subscription_create_job_create_query_resource_object_attributes.py
 src/openapi_client/model/subscription_enum.py
-src/openapi_client/model/subscriptions.py
 src/openapi_client/model/suppression.py
 src/openapi_client/model/suppression_create_job_create_query.py
 src/openapi_client/model/suppression_create_job_create_query_resource_object.py
 src/openapi_client/model/suppression_create_job_create_query_resource_object_attributes.py
 src/openapi_client/model/tag_campaign_op.py
 src/openapi_client/model/tag_campaign_op_data_inner.py
 src/openapi_client/model/tag_create_query.py
@@ -253,20 +226,17 @@
 src/openapi_client/model/template_enum.py
 src/openapi_client/model/template_render_query.py
 src/openapi_client/model/template_render_query_resource_object.py
 src/openapi_client/model/template_render_query_resource_object_attributes.py
 src/openapi_client/model/template_update_query.py
 src/openapi_client/model/template_update_query_resource_object.py
 src/openapi_client/model/template_update_query_resource_object_attributes.py
-src/openapi_client/model/test_api_analytics_sample_enum.py
-src/openapi_client/model/test_list_enum.py
 src/openapi_client/model/throttled_schedule_options.py
 src/openapi_client/model/tracking_options_sub_object.py
 src/openapi_client/model/unsubscription_create_job_create_query.py
 src/openapi_client/model/unsubscription_create_job_create_query_resource_object.py
 src/openapi_client/model/unsubscription_create_job_create_query_resource_object_attributes.py
 src/openapi_client/model/unsuppression_create_job_create_query.py
 src/openapi_client/model/unsuppression_create_job_create_query_resource_object.py
 src/openapi_client/model/unsuppression_create_job_create_query_resource_object_attributes.py
-src/openapi_client/model/utm_param_info.py
 src/openapi_client/model/utm_params_sub_object.py
 src/openapi_client/models/__init__.py
```

### Comparing `klaviyo-api-2.0.1/src/openapi_client/__init__.py` & `klaviyo-api-2.0.2/src/openapi_client/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
     The version of the OpenAPI document: 2023-02-22
     Contact: developers@klaviyo.com
     Generated by: https://openapi-generator.tech
 """
 
 
-__version__ = "2.0.1"
+__version__ = "2.0.2"
 
 # import ApiClient
 from openapi_client.api_client import ApiClient
 
 # import Configuration
 from openapi_client.configuration import Configuration
```

### Comparing `klaviyo-api-2.0.1/src/openapi_client/api/campaigns_api.py` & `klaviyo-api-2.0.2/src/openapi_client/api/campaigns_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1154,15 +1154,15 @@
     def create_campaign(
         self,
         campaign_create_query,
         **kwargs
     ):
         """Create Campaign  # noqa: E501
 
-        Creates a campaign given a set of parameters, then returns it.<br><br>*Rate limits*:<br>Burst: `10/s`<br>Steady: `150/m`  **Scopes:** `Campaigns Write`  # noqa: E501
+        Creates a campaign given a set of parameters, then returns it.<br><br>*Rate limits*:<br>Burst: `10/s`<br>Steady: `150/m`  **Scopes:** `campaigns:write`  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.create_campaign(campaign_create_query, async_req=True)
         >>> result = thread.get()
 
         Args:
@@ -1237,15 +1237,15 @@
     def create_campaign_clone(
         self,
         campaign_clone_query,
         **kwargs
     ):
         """Create Campaign Clone  # noqa: E501
 
-        Clones an existing campaign, returning a new campaign based on the original with a new ID and name.<br><br>*Rate limits*:<br>Burst: `10/s`<br>Steady: `150/m`  **Scopes:** `Campaigns Write`  # noqa: E501
+        Clones an existing campaign, returning a new campaign based on the original with a new ID and name.<br><br>*Rate limits*:<br>Burst: `10/s`<br>Steady: `150/m`  **Scopes:** `campaigns:write`  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.create_campaign_clone(campaign_clone_query, async_req=True)
         >>> result = thread.get()
 
         Args:
@@ -1320,15 +1320,15 @@
     def create_campaign_message_assign_template(
         self,
         campaign_message_assign_template_query,
         **kwargs
     ):
         """Assign Campaign Message Template  # noqa: E501
 
-        Creates a non-reusable version of the template and assigns it to the message.<br><br>*Rate limits*:<br>Burst: `10/s`<br>Steady: `150/m`  **Scopes:** `Campaigns Write`  # noqa: E501
+        Creates a non-reusable version of the template and assigns it to the message.<br><br>*Rate limits*:<br>Burst: `10/s`<br>Steady: `150/m`  **Scopes:** `campaigns:write`  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.create_campaign_message_assign_template(campaign_message_assign_template_query, async_req=True)
         >>> result = thread.get()
 
         Args:
@@ -1403,15 +1403,15 @@
     def create_campaign_recipient_estimation_job(
         self,
         campaign_recipient_estimation_job_create_query,
         **kwargs
     ):
         """Create Campaign Recipient Estimation Job  # noqa: E501
 
-        Trigger an asynchronous job to update the estimated number of recipients for the given campaign ID. Use the `Get Campaign Recipient Estimation Job` endpoint to retrieve the status of this estimation job. Use the `Get Campaign Recipient Estimation` endpoint to retrieve the estimated recipient count for a given campaign.<br><br>*Rate limits*:<br>Burst: `10/s`<br>Steady: `150/m`  **Scopes:** `Campaigns Write`  # noqa: E501
+        Trigger an asynchronous job to update the estimated number of recipients for the given campaign ID. Use the `Get Campaign Recipient Estimation Job` endpoint to retrieve the status of this estimation job. Use the `Get Campaign Recipient Estimation` endpoint to retrieve the estimated recipient count for a given campaign.<br><br>*Rate limits*:<br>Burst: `10/s`<br>Steady: `150/m`  **Scopes:** `campaigns:write`  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.create_campaign_recipient_estimation_job(campaign_recipient_estimation_job_create_query, async_req=True)
         >>> result = thread.get()
 
         Args:
@@ -1486,15 +1486,15 @@
     def create_campaign_send_job(
         self,
         campaign_send_job_create_query,
         **kwargs
     ):
         """Create Campaign Send Job  # noqa: E501
 
-        Trigger a campaign to send asynchronously<br><br>*Rate limits*:<br>Burst: `10/s`<br>Steady: `150/m`  **Scopes:** `Campaigns Write`  # noqa: E501
+        Trigger a campaign to send asynchronously<br><br>*Rate limits*:<br>Burst: `10/s`<br>Steady: `150/m`  **Scopes:** `campaigns:write`  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.create_campaign_send_job(campaign_send_job_create_query, async_req=True)
         >>> result = thread.get()
 
         Args:
@@ -1569,15 +1569,15 @@
     def delete_campaign(
         self,
         id,
         **kwargs
     ):
         """Delete Campaign  # noqa: E501
 
-        Delete a campaign with the given campaign ID.<br><br>*Rate limits*:<br>Burst: `10/s`<br>Steady: `150/m`  **Scopes:** `Campaigns Write`  # noqa: E501
+        Delete a campaign with the given campaign ID.<br><br>*Rate limits*:<br>Burst: `10/s`<br>Steady: `150/m`  **Scopes:** `campaigns:write`  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.delete_campaign(id, async_req=True)
         >>> result = thread.get()
 
         Args:
@@ -1652,15 +1652,15 @@
     def get_campaign(
         self,
         id,
         **kwargs
     ):
         """Get Campaign  # noqa: E501
 
-        Returns a specific campaign based on a required id.<br><br>*Rate limits*:<br>Burst: `10/s`<br>Steady: `150/m`  **Scopes:** `Campaigns Read`  # noqa: E501
+        Returns a specific campaign based on a required id.<br><br>*Rate limits*:<br>Burst: `10/s`<br>Steady: `150/m`  **Scopes:** `campaigns:read`  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.get_campaign(id, async_req=True)
         >>> result = thread.get()
 
         Args:
@@ -1738,15 +1738,15 @@
     def get_campaign_message(
         self,
         id,
         **kwargs
     ):
         """Get Campaign Message  # noqa: E501
 
-        Returns a specific message based on a required id.<br><br>*Rate limits*:<br>Burst: `10/s`<br>Steady: `150/m`  **Scopes:** `Campaigns Read`  # noqa: E501
+        Returns a specific message based on a required id.<br><br>*Rate limits*:<br>Burst: `10/s`<br>Steady: `150/m`  **Scopes:** `campaigns:read`  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.get_campaign_message(id, async_req=True)
         >>> result = thread.get()
 
         Args:
@@ -1822,15 +1822,15 @@
     def get_campaign_recipient_estimation(
         self,
         id,
         **kwargs
     ):
         """Get Campaign Recipient Estimation  # noqa: E501
 
-        Get the estimated recipient count for a campaign with the provided campaign ID. You can refresh this count by using the `Create Campaign Recipient Estimation Job` endpoint.<br><br>*Rate limits*:<br>Burst: `10/s`<br>Steady: `150/m`  **Scopes:** `Campaigns Read`  # noqa: E501
+        Get the estimated recipient count for a campaign with the provided campaign ID. You can refresh this count by using the `Create Campaign Recipient Estimation Job` endpoint.<br><br>*Rate limits*:<br>Burst: `10/s`<br>Steady: `150/m`  **Scopes:** `campaigns:read`  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.get_campaign_recipient_estimation(id, async_req=True)
         >>> result = thread.get()
 
         Args:
@@ -1906,15 +1906,15 @@
     def get_campaign_recipient_estimation_job(
         self,
         id,
         **kwargs
     ):
         """Get Campaign Recipient Estimation Job  # noqa: E501
 
-        Retrieve the status of a recipient estimation job triggered with the `Create Campaign Recipient Estimation Job` endpoint.<br><br>*Rate limits*:<br>Burst: `10/s`<br>Steady: `150/m`  **Scopes:** `Campaigns Read`  # noqa: E501
+        Retrieve the status of a recipient estimation job triggered with the `Create Campaign Recipient Estimation Job` endpoint.<br><br>*Rate limits*:<br>Burst: `10/s`<br>Steady: `150/m`  **Scopes:** `campaigns:read`  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.get_campaign_recipient_estimation_job(id, async_req=True)
         >>> result = thread.get()
 
         Args:
@@ -1990,15 +1990,15 @@
     def get_campaign_relationships_tags(
         self,
         id,
         **kwargs
     ):
         """Get Campaign Relationships Tags  # noqa: E501
 
-        Returns the IDs of all tags associated with the given campaign.<br><br>*Rate limits*:<br>Burst: `3/s`<br>Steady: `60/m`  **Scopes:** `Campaigns Read` `Tags Read`  # noqa: E501
+        Returns the IDs of all tags associated with the given campaign.<br><br>*Rate limits*:<br>Burst: `3/s`<br>Steady: `60/m`  **Scopes:** `campaigns:read` `tags:read`  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.get_campaign_relationships_tags(id, async_req=True)
         >>> result = thread.get()
 
         Args:
@@ -2073,15 +2073,15 @@
     def get_campaign_send_job(
         self,
         id,
         **kwargs
     ):
         """Get Campaign Send Job  # noqa: E501
 
-        Get a campaign send job<br><br>*Rate limits*:<br>Burst: `10/s`<br>Steady: `150/m`  **Scopes:** `Campaigns Read`  # noqa: E501
+        Get a campaign send job<br><br>*Rate limits*:<br>Burst: `10/s`<br>Steady: `150/m`  **Scopes:** `campaigns:read`  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.get_campaign_send_job(id, async_req=True)
         >>> result = thread.get()
 
         Args:
@@ -2157,15 +2157,15 @@
     def get_campaign_tags(
         self,
         campaign_id,
         **kwargs
     ):
         """Get Campaign Tags  # noqa: E501
 
-        Return all tags that belong to the given campaign.<br><br>*Rate limits*:<br>Burst: `3/s`<br>Steady: `60/m`  **Scopes:** `Campaigns Read` `Tags Read`  # noqa: E501
+        Return all tags that belong to the given campaign.<br><br>*Rate limits*:<br>Burst: `3/s`<br>Steady: `60/m`  **Scopes:** `campaigns:read` `tags:read`  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.get_campaign_tags(campaign_id, async_req=True)
         >>> result = thread.get()
 
         Args:
@@ -2240,15 +2240,15 @@
 
     def get_campaigns(
         self,
         **kwargs
     ):
         """Get Campaigns  # noqa: E501
 
-        Returns some or all campaigns based on [optional] filters<br><br>*Rate limits*:<br>Burst: `10/s`<br>Steady: `150/m`  **Scopes:** `Campaigns Read`  # noqa: E501
+        Returns some or all campaigns based on [optional] filters<br><br>*Rate limits*:<br>Burst: `10/s`<br>Steady: `150/m`  **Scopes:** `campaigns:read`  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.get_campaigns(async_req=True)
         >>> result = thread.get()
 
 
@@ -2326,15 +2326,15 @@
         self,
         id,
         campaign_partial_update_query,
         **kwargs
     ):
         """Update Campaign  # noqa: E501
 
-        Update a campaign with the given campaign ID.<br><br>*Rate limits*:<br>Burst: `10/s`<br>Steady: `150/m`  **Scopes:** `Campaigns Write`  # noqa: E501
+        Update a campaign with the given campaign ID.<br><br>*Rate limits*:<br>Burst: `10/s`<br>Steady: `150/m`  **Scopes:** `campaigns:write`  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.update_campaign(id, campaign_partial_update_query, async_req=True)
         >>> result = thread.get()
 
         Args:
@@ -2413,15 +2413,15 @@
         self,
         id,
         campaign_message_partial_update_query,
         **kwargs
     ):
         """Update Campaign Message  # noqa: E501
 
-        Update a campaign message<br><br>*Rate limits*:<br>Burst: `10/s`<br>Steady: `150/m`  **Scopes:** `Campaigns Write`  # noqa: E501
+        Update a campaign message<br><br>*Rate limits*:<br>Burst: `10/s`<br>Steady: `150/m`  **Scopes:** `campaigns:write`  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.update_campaign_message(id, campaign_message_partial_update_query, async_req=True)
         >>> result = thread.get()
 
         Args:
@@ -2500,15 +2500,15 @@
         self,
         id,
         campaign_send_job_partial_update_query,
         **kwargs
     ):
         """Update Campaign Send Job  # noqa: E501
 
-        Permanently cancel the campaign, setting the status to CANCELED or revert the campaign, setting the status back to DRAFT<br><br>*Rate limits*:<br>Burst: `10/s`<br>Steady: `150/m`  **Scopes:** `Campaigns Write`  # noqa: E501
+        Permanently cancel the campaign, setting the status to CANCELED or revert the campaign, setting the status back to DRAFT<br><br>*Rate limits*:<br>Burst: `10/s`<br>Steady: `150/m`  **Scopes:** `campaigns:write`  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.update_campaign_send_job(id, campaign_send_job_partial_update_query, async_req=True)
         >>> result = thread.get()
 
         Args:
```

### Comparing `klaviyo-api-2.0.1/src/openapi_client/api/catalogs_api.py` & `klaviyo-api-2.0.2/src/openapi_client/api/catalogs_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -3793,15 +3793,15 @@
     def create_catalog_category(
         self,
         catalog_category_create_query,
         **kwargs
     ):
         """Create Catalog Category  # noqa: E501
 
-        Create a new catalog category.<br><br>*Rate limits*:<br>Burst: `75/s`<br>Steady: `700/m`  **Scopes:** `Catalogs Write`  # noqa: E501
+        Create a new catalog category.<br><br>*Rate limits*:<br>Burst: `75/s`<br>Steady: `700/m`  **Scopes:** `catalogs:write`  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.create_catalog_category(catalog_category_create_query, async_req=True)
         >>> result = thread.get()
 
         Args:
@@ -3877,15 +3877,15 @@
         self,
         id,
         catalog_category_item_op,
         **kwargs
     ):
         """Create Catalog Category Relationships Items  # noqa: E501
 
-        Create a new item relationship for the given category ID.<br><br>*Rate limits*:<br>Burst: `75/s`<br>Steady: `700/m`  **Scopes:** `Catalogs Write`  # noqa: E501
+        Create a new item relationship for the given category ID.<br><br>*Rate limits*:<br>Burst: `75/s`<br>Steady: `700/m`  **Scopes:** `catalogs:write`  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.create_catalog_category_relationships_items(id, catalog_category_item_op, async_req=True)
         >>> result = thread.get()
 
         Args:
@@ -3963,15 +3963,15 @@
     def create_catalog_item(
         self,
         catalog_item_create_query,
         **kwargs
     ):
         """Create Catalog Item  # noqa: E501
 
-        Create a new catalog item.<br><br>*Rate limits*:<br>Burst: `75/s`<br>Steady: `700/m`  **Scopes:** `Catalogs Write`  # noqa: E501
+        Create a new catalog item.<br><br>*Rate limits*:<br>Burst: `75/s`<br>Steady: `700/m`  **Scopes:** `catalogs:write`  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.create_catalog_item(catalog_item_create_query, async_req=True)
         >>> result = thread.get()
 
         Args:
@@ -4047,15 +4047,15 @@
         self,
         id,
         catalog_item_category_op,
         **kwargs
     ):
         """Create Catalog Item Relationships Categories  # noqa: E501
 
-        Create a new catalog category relationship for the given item ID.<br><br>*Rate limits*:<br>Burst: `75/s`<br>Steady: `700/m`  **Scopes:** `Catalogs Write`  # noqa: E501
+        Create a new catalog category relationship for the given item ID.<br><br>*Rate limits*:<br>Burst: `75/s`<br>Steady: `700/m`  **Scopes:** `catalogs:write`  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.create_catalog_item_relationships_categories(id, catalog_item_category_op, async_req=True)
         >>> result = thread.get()
 
         Args:
@@ -4133,15 +4133,15 @@
     def create_catalog_variant(
         self,
         catalog_variant_create_query,
         **kwargs
     ):
         """Create Catalog Variant  # noqa: E501
 
-        Create a new variant for a related catalog item.<br><br>*Rate limits*:<br>Burst: `75/s`<br>Steady: `700/m`  **Scopes:** `Catalogs Write`  # noqa: E501
+        Create a new variant for a related catalog item.<br><br>*Rate limits*:<br>Burst: `75/s`<br>Steady: `700/m`  **Scopes:** `catalogs:write`  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.create_catalog_variant(catalog_variant_create_query, async_req=True)
         >>> result = thread.get()
 
         Args:
@@ -4216,15 +4216,15 @@
     def delete_catalog_category(
         self,
         id,
         **kwargs
     ):
         """Delete Catalog Category  # noqa: E501
 
-        Delete a catalog category using the given category ID.<br><br>*Rate limits*:<br>Burst: `75/s`<br>Steady: `700/m`  **Scopes:** `Catalogs Write`  # noqa: E501
+        Delete a catalog category using the given category ID.<br><br>*Rate limits*:<br>Burst: `75/s`<br>Steady: `700/m`  **Scopes:** `catalogs:write`  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.delete_catalog_category(id, async_req=True)
         >>> result = thread.get()
 
         Args:
@@ -4300,15 +4300,15 @@
         self,
         id,
         catalog_category_item_op,
         **kwargs
     ):
         """Delete Catalog Category Relationships Items  # noqa: E501
 
-        Delete item relationships for the given category ID.<br><br>*Rate limits*:<br>Burst: `75/s`<br>Steady: `700/m`  **Scopes:** `Catalogs Write`  # noqa: E501
+        Delete item relationships for the given category ID.<br><br>*Rate limits*:<br>Burst: `75/s`<br>Steady: `700/m`  **Scopes:** `catalogs:write`  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.delete_catalog_category_relationships_items(id, catalog_category_item_op, async_req=True)
         >>> result = thread.get()
 
         Args:
@@ -4386,15 +4386,15 @@
     def delete_catalog_item(
         self,
         id,
         **kwargs
     ):
         """Delete Catalog Item  # noqa: E501
 
-        Delete a catalog item with the given item ID.<br><br>*Rate limits*:<br>Burst: `75/s`<br>Steady: `700/m`  **Scopes:** `Catalogs Write`  # noqa: E501
+        Delete a catalog item with the given item ID.<br><br>*Rate limits*:<br>Burst: `75/s`<br>Steady: `700/m`  **Scopes:** `catalogs:write`  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.delete_catalog_item(id, async_req=True)
         >>> result = thread.get()
 
         Args:
@@ -4470,15 +4470,15 @@
         self,
         id,
         catalog_item_category_op,
         **kwargs
     ):
         """Delete Catalog Item Relationships Categories  # noqa: E501
 
-        Delete catalog category relationships for the given item ID.<br><br>*Rate limits*:<br>Burst: `75/s`<br>Steady: `700/m`  **Scopes:** `Catalogs Write`  # noqa: E501
+        Delete catalog category relationships for the given item ID.<br><br>*Rate limits*:<br>Burst: `75/s`<br>Steady: `700/m`  **Scopes:** `catalogs:write`  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.delete_catalog_item_relationships_categories(id, catalog_item_category_op, async_req=True)
         >>> result = thread.get()
 
         Args:
@@ -4556,15 +4556,15 @@
     def delete_catalog_variant(
         self,
         id,
         **kwargs
     ):
         """Delete Catalog Variant  # noqa: E501
 
-        Delete a catalog item variant with the given variant ID.<br><br>*Rate limits*:<br>Burst: `75/s`<br>Steady: `700/m`  **Scopes:** `Catalogs Write`  # noqa: E501
+        Delete a catalog item variant with the given variant ID.<br><br>*Rate limits*:<br>Burst: `75/s`<br>Steady: `700/m`  **Scopes:** `catalogs:write`  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.delete_catalog_variant(id, async_req=True)
         >>> result = thread.get()
 
         Args:
@@ -4638,15 +4638,15 @@
 
     def get_catalog_categories(
         self,
         **kwargs
     ):
         """Get Catalog Categories  # noqa: E501
 
-        Get all catalog categories in an account. Catalog categories can be sorted by the following fields, in ascending and descending order: `created` Returns a maximum of 100 categories per request.<br><br>*Rate limits*:<br>Burst: `350/s`<br>Steady: `3500/m`  **Scopes:** `Catalogs Read`  # noqa: E501
+        Get all catalog categories in an account. Catalog categories can be sorted by the following fields, in ascending and descending order: `created` Returns a maximum of 100 categories per request.<br><br>*Rate limits*:<br>Burst: `350/s`<br>Steady: `3500/m`  **Scopes:** `catalogs:read`  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.get_catalog_categories(async_req=True)
         >>> result = thread.get()
 
 
@@ -4721,15 +4721,15 @@
     def get_catalog_category(
         self,
         id,
         **kwargs
     ):
         """Get Catalog Category  # noqa: E501
 
-        Get a catalog category with the given category ID.<br><br>*Rate limits*:<br>Burst: `350/s`<br>Steady: `3500/m`  **Scopes:** `Catalogs Read`  # noqa: E501
+        Get a catalog category with the given category ID.<br><br>*Rate limits*:<br>Burst: `350/s`<br>Steady: `3500/m`  **Scopes:** `catalogs:read`  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.get_catalog_category(id, async_req=True)
         >>> result = thread.get()
 
         Args:
@@ -4805,15 +4805,15 @@
     def get_catalog_category_items(
         self,
         category_id,
         **kwargs
     ):
         """Get Catalog Category Items  # noqa: E501
 
-        Get all items in a category with the given category ID. Items can be sorted by the following fields, in ascending and descending order: `created` Include parameters can be provided to get the following related resource data: `variants` Returns a maximum of 100 items per request.<br><br>*Rate limits*:<br>Burst: `350/s`<br>Steady: `3500/m`  **Scopes:** `Catalogs Read`  # noqa: E501
+        Get all items in a category with the given category ID. Items can be sorted by the following fields, in ascending and descending order: `created` Include parameters can be provided to get the following related resource data: `variants` Returns a maximum of 100 items per request.<br><br>*Rate limits*:<br>Burst: `350/s`<br>Steady: `3500/m`  **Scopes:** `catalogs:read`  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.get_catalog_category_items(category_id, async_req=True)
         >>> result = thread.get()
 
         Args:
@@ -4894,15 +4894,15 @@
     def get_catalog_category_relationships_items(
         self,
         id,
         **kwargs
     ):
         """Get Catalog Category Relationships Items  # noqa: E501
 
-        Get all items in the given category ID. Returns a maximum of 100 items per request.<br><br>*Rate limits*:<br>Burst: `350/s`<br>Steady: `3500/m`  **Scopes:** `Catalogs Read`  # noqa: E501
+        Get all items in the given category ID. Returns a maximum of 100 items per request.<br><br>*Rate limits*:<br>Burst: `350/s`<br>Steady: `3500/m`  **Scopes:** `catalogs:read`  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.get_catalog_category_relationships_items(id, async_req=True)
         >>> result = thread.get()
 
         Args:
@@ -4978,15 +4978,15 @@
     def get_catalog_item(
         self,
         id,
         **kwargs
     ):
         """Get Catalog Item  # noqa: E501
 
-        Get a specific catalog item with the given item ID. Include parameters can be provided to get the following related resource data: `variants`<br><br>*Rate limits*:<br>Burst: `350/s`<br>Steady: `3500/m`  **Scopes:** `Catalogs Read`  # noqa: E501
+        Get a specific catalog item with the given item ID. Include parameters can be provided to get the following related resource data: `variants`<br><br>*Rate limits*:<br>Burst: `350/s`<br>Steady: `3500/m`  **Scopes:** `catalogs:read`  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.get_catalog_item(id, async_req=True)
         >>> result = thread.get()
 
         Args:
@@ -5064,15 +5064,15 @@
     def get_catalog_item_categories(
         self,
         item_id,
         **kwargs
     ):
         """Get Catalog Item Categories  # noqa: E501
 
-        Get all catalog categories that an item with the given item ID is in. Catalog categories can be sorted by the following fields, in ascending and descending order: `created` Returns a maximum of 100 categories per request.<br><br>*Rate limits*:<br>Burst: `350/s`<br>Steady: `3500/m`  **Scopes:** `Catalogs Read`  # noqa: E501
+        Get all catalog categories that an item with the given item ID is in. Catalog categories can be sorted by the following fields, in ascending and descending order: `created` Returns a maximum of 100 categories per request.<br><br>*Rate limits*:<br>Burst: `350/s`<br>Steady: `3500/m`  **Scopes:** `catalogs:read`  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.get_catalog_item_categories(item_id, async_req=True)
         >>> result = thread.get()
 
         Args:
@@ -5151,15 +5151,15 @@
     def get_catalog_item_relationships_categories(
         self,
         id,
         **kwargs
     ):
         """Get Catalog Item Relationships Categories  # noqa: E501
 
-        Get all catalog categories that a particular item is in. Returns a maximum of 100 categories per request.<br><br>*Rate limits*:<br>Burst: `350/s`<br>Steady: `3500/m`  **Scopes:** `Catalogs Read`  # noqa: E501
+        Get all catalog categories that a particular item is in. Returns a maximum of 100 categories per request.<br><br>*Rate limits*:<br>Burst: `350/s`<br>Steady: `3500/m`  **Scopes:** `catalogs:read`  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.get_catalog_item_relationships_categories(id, async_req=True)
         >>> result = thread.get()
 
         Args:
@@ -5235,15 +5235,15 @@
     def get_catalog_item_variants(
         self,
         item_id,
         **kwargs
     ):
         """Get Catalog Item Variants  # noqa: E501
 
-        Get all variants related to the given item ID. Variants can be sorted by the following fields, in ascending and descending order: `created` Returns a maximum of 100 variants per request.<br><br>*Rate limits*:<br>Burst: `350/s`<br>Steady: `3500/m`  **Scopes:** `Catalogs Read`  # noqa: E501
+        Get all variants related to the given item ID. Variants can be sorted by the following fields, in ascending and descending order: `created` Returns a maximum of 100 variants per request.<br><br>*Rate limits*:<br>Burst: `350/s`<br>Steady: `3500/m`  **Scopes:** `catalogs:read`  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.get_catalog_item_variants(item_id, async_req=True)
         >>> result = thread.get()
 
         Args:
@@ -5321,15 +5321,15 @@
 
     def get_catalog_items(
         self,
         **kwargs
     ):
         """Get Catalog Items  # noqa: E501
 
-        Get all catalog items in an account. Catalog items can be sorted by the following fields, in ascending and descending order: `created` Include parameters can be provided to get the following related resource data: `variants` Returns a maximum of 100 items per request.<br><br>*Rate limits*:<br>Burst: `350/s`<br>Steady: `3500/m`  **Scopes:** `Catalogs Read`  # noqa: E501
+        Get all catalog items in an account. Catalog items can be sorted by the following fields, in ascending and descending order: `created` Include parameters can be provided to get the following related resource data: `variants` Returns a maximum of 100 items per request.<br><br>*Rate limits*:<br>Burst: `350/s`<br>Steady: `3500/m`  **Scopes:** `catalogs:read`  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.get_catalog_items(async_req=True)
         >>> result = thread.get()
 
 
@@ -5406,15 +5406,15 @@
     def get_catalog_variant(
         self,
         id,
         **kwargs
     ):
         """Get Catalog Variant  # noqa: E501
 
-        Get a catalog item variant with the given variant ID.<br><br>*Rate limits*:<br>Burst: `350/s`<br>Steady: `3500/m`  **Scopes:** `Catalogs Read`  # noqa: E501
+        Get a catalog item variant with the given variant ID.<br><br>*Rate limits*:<br>Burst: `350/s`<br>Steady: `3500/m`  **Scopes:** `catalogs:read`  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.get_catalog_variant(id, async_req=True)
         >>> result = thread.get()
 
         Args:
@@ -5489,15 +5489,15 @@
 
     def get_catalog_variants(
         self,
         **kwargs
     ):
         """Get Catalog Variants  # noqa: E501
 
-        Get all variants in an account. Variants can be sorted by the following fields, in ascending and descending order: `created` Returns a maximum of 100 variants per request.<br><br>*Rate limits*:<br>Burst: `350/s`<br>Steady: `3500/m`  **Scopes:** `Catalogs Read`  # noqa: E501
+        Get all variants in an account. Variants can be sorted by the following fields, in ascending and descending order: `created` Returns a maximum of 100 variants per request.<br><br>*Rate limits*:<br>Burst: `350/s`<br>Steady: `3500/m`  **Scopes:** `catalogs:read`  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.get_catalog_variants(async_req=True)
         >>> result = thread.get()
 
 
@@ -5572,15 +5572,15 @@
     def get_create_categories_job(
         self,
         job_id,
         **kwargs
     ):
         """Get Create Categories Job  # noqa: E501
 
-        Get a catalog category bulk create job with the given job ID. An `include` parameter can be provided to get the following related resource data: `categories`.<br><br>*Rate limits*:<br>Burst: `350/s`<br>Steady: `3500/m`  **Scopes:** `Catalogs Read`  # noqa: E501
+        Get a catalog category bulk create job with the given job ID. An `include` parameter can be provided to get the following related resource data: `categories`.<br><br>*Rate limits*:<br>Burst: `350/s`<br>Steady: `3500/m`  **Scopes:** `catalogs:read`  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.get_create_categories_job(job_id, async_req=True)
         >>> result = thread.get()
 
         Args:
@@ -5657,15 +5657,15 @@
 
     def get_create_categories_jobs(
         self,
         **kwargs
     ):
         """Get Create Categories Jobs  # noqa: E501
 
-        Get all catalog category bulk create jobs. Returns a maximum of 100 jobs per request.<br><br>*Rate limits*:<br>Burst: `350/s`<br>Steady: `3500/m`  **Scopes:** `Catalogs Read`  # noqa: E501
+        Get all catalog category bulk create jobs. Returns a maximum of 100 jobs per request.<br><br>*Rate limits*:<br>Burst: `350/s`<br>Steady: `3500/m`  **Scopes:** `catalogs:read`  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.get_create_categories_jobs(async_req=True)
         >>> result = thread.get()
 
 
@@ -5739,15 +5739,15 @@
     def get_create_items_job(
         self,
         job_id,
         **kwargs
     ):
         """Get Create Items Job  # noqa: E501
 
-        Get a catalog item bulk create job with the given job ID. An `include` parameter can be provided to get the following related resource data: `items`.<br><br>*Rate limits*:<br>Burst: `350/s`<br>Steady: `3500/m`  **Scopes:** `Catalogs Read`  # noqa: E501
+        Get a catalog item bulk create job with the given job ID. An `include` parameter can be provided to get the following related resource data: `items`.<br><br>*Rate limits*:<br>Burst: `350/s`<br>Steady: `3500/m`  **Scopes:** `catalogs:read`  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.get_create_items_job(job_id, async_req=True)
         >>> result = thread.get()
 
         Args:
@@ -5824,15 +5824,15 @@
 
     def get_create_items_jobs(
         self,
         **kwargs
     ):
         """Get Create Items Jobs  # noqa: E501
 
-        Get all catalog item bulk create jobs. Returns a maximum of 100 jobs per request.<br><br>*Rate limits*:<br>Burst: `350/s`<br>Steady: `3500/m`  **Scopes:** `Catalogs Read`  # noqa: E501
+        Get all catalog item bulk create jobs. Returns a maximum of 100 jobs per request.<br><br>*Rate limits*:<br>Burst: `350/s`<br>Steady: `3500/m`  **Scopes:** `catalogs:read`  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.get_create_items_jobs(async_req=True)
         >>> result = thread.get()
 
 
@@ -5906,15 +5906,15 @@
     def get_create_variants_job(
         self,
         job_id,
         **kwargs
     ):
         """Get Create Variants Job  # noqa: E501
 
-        Get a catalog variant bulk create job with the given job ID. An `include` parameter can be provided to get the following related resource data: `variants`.<br><br>*Rate limits*:<br>Burst: `350/s`<br>Steady: `3500/m`  **Scopes:** `Catalogs Read`  # noqa: E501
+        Get a catalog variant bulk create job with the given job ID. An `include` parameter can be provided to get the following related resource data: `variants`.<br><br>*Rate limits*:<br>Burst: `350/s`<br>Steady: `3500/m`  **Scopes:** `catalogs:read`  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.get_create_variants_job(job_id, async_req=True)
         >>> result = thread.get()
 
         Args:
@@ -5991,15 +5991,15 @@
 
     def get_create_variants_jobs(
         self,
         **kwargs
     ):
         """Get Create Variants Jobs  # noqa: E501
 
-        Get all catalog variant bulk create jobs. Returns a maximum of 100 jobs per request.<br><br>*Rate limits*:<br>Burst: `350/s`<br>Steady: `3500/m`  **Scopes:** `Catalogs Read`  # noqa: E501
+        Get all catalog variant bulk create jobs. Returns a maximum of 100 jobs per request.<br><br>*Rate limits*:<br>Burst: `350/s`<br>Steady: `3500/m`  **Scopes:** `catalogs:read`  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.get_create_variants_jobs(async_req=True)
         >>> result = thread.get()
 
 
@@ -6073,15 +6073,15 @@
     def get_delete_categories_job(
         self,
         job_id,
         **kwargs
     ):
         """Get Delete Categories Job  # noqa: E501
 
-        Get a catalog category bulk delete job with the given job ID.<br><br>*Rate limits*:<br>Burst: `350/s`<br>Steady: `3500/m`  **Scopes:** `Catalogs Read`  # noqa: E501
+        Get a catalog category bulk delete job with the given job ID.<br><br>*Rate limits*:<br>Burst: `350/s`<br>Steady: `3500/m`  **Scopes:** `catalogs:read`  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.get_delete_categories_job(job_id, async_req=True)
         >>> result = thread.get()
 
         Args:
@@ -6156,15 +6156,15 @@
 
     def get_delete_categories_jobs(
         self,
         **kwargs
     ):
         """Get Delete Categories Jobs  # noqa: E501
 
-        Get all catalog category bulk delete jobs. Returns a maximum of 100 jobs per request.<br><br>*Rate limits*:<br>Burst: `350/s`<br>Steady: `3500/m`  **Scopes:** `Catalogs Read`  # noqa: E501
+        Get all catalog category bulk delete jobs. Returns a maximum of 100 jobs per request.<br><br>*Rate limits*:<br>Burst: `350/s`<br>Steady: `3500/m`  **Scopes:** `catalogs:read`  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.get_delete_categories_jobs(async_req=True)
         >>> result = thread.get()
 
 
@@ -6238,15 +6238,15 @@
     def get_delete_items_job(
         self,
         job_id,
         **kwargs
     ):
         """Get Delete Items Job  # noqa: E501
 
-        Get a catalog item bulk delete job with the given job ID.<br><br>*Rate limits*:<br>Burst: `350/s`<br>Steady: `3500/m`  **Scopes:** `Catalogs Read`  # noqa: E501
+        Get a catalog item bulk delete job with the given job ID.<br><br>*Rate limits*:<br>Burst: `350/s`<br>Steady: `3500/m`  **Scopes:** `catalogs:read`  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.get_delete_items_job(job_id, async_req=True)
         >>> result = thread.get()
 
         Args:
@@ -6321,15 +6321,15 @@
 
     def get_delete_items_jobs(
         self,
         **kwargs
     ):
         """Get Delete Items Jobs  # noqa: E501
 
-        Get all catalog item bulk delete jobs. Returns a maximum of 100 jobs per request.<br><br>*Rate limits*:<br>Burst: `350/s`<br>Steady: `3500/m`  **Scopes:** `Catalogs Read`  # noqa: E501
+        Get all catalog item bulk delete jobs. Returns a maximum of 100 jobs per request.<br><br>*Rate limits*:<br>Burst: `350/s`<br>Steady: `3500/m`  **Scopes:** `catalogs:read`  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.get_delete_items_jobs(async_req=True)
         >>> result = thread.get()
 
 
@@ -6403,15 +6403,15 @@
     def get_delete_variants_job(
         self,
         job_id,
         **kwargs
     ):
         """Get Delete Variants Job  # noqa: E501
 
-        Get a catalog variant bulk delete job with the given job ID.<br><br>*Rate limits*:<br>Burst: `350/s`<br>Steady: `3500/m`  **Scopes:** `Catalogs Read`  # noqa: E501
+        Get a catalog variant bulk delete job with the given job ID.<br><br>*Rate limits*:<br>Burst: `350/s`<br>Steady: `3500/m`  **Scopes:** `catalogs:read`  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.get_delete_variants_job(job_id, async_req=True)
         >>> result = thread.get()
 
         Args:
@@ -6486,15 +6486,15 @@
 
     def get_delete_variants_jobs(
         self,
         **kwargs
     ):
         """Get Delete Variants Jobs  # noqa: E501
 
-        Get all catalog variant bulk delete jobs. Returns a maximum of 100 jobs per request.<br><br>*Rate limits*:<br>Burst: `350/s`<br>Steady: `3500/m`  **Scopes:** `Catalogs Read`  # noqa: E501
+        Get all catalog variant bulk delete jobs. Returns a maximum of 100 jobs per request.<br><br>*Rate limits*:<br>Burst: `350/s`<br>Steady: `3500/m`  **Scopes:** `catalogs:read`  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.get_delete_variants_jobs(async_req=True)
         >>> result = thread.get()
 
 
@@ -6568,15 +6568,15 @@
     def get_update_categories_job(
         self,
         job_id,
         **kwargs
     ):
         """Get Update Categories Job  # noqa: E501
 
-        Get a catalog category bulk update job with the given job ID. An `include` parameter can be provided to get the following related resource data: `categories`.<br><br>*Rate limits*:<br>Burst: `350/s`<br>Steady: `3500/m`  **Scopes:** `Catalogs Read`  # noqa: E501
+        Get a catalog category bulk update job with the given job ID. An `include` parameter can be provided to get the following related resource data: `categories`.<br><br>*Rate limits*:<br>Burst: `350/s`<br>Steady: `3500/m`  **Scopes:** `catalogs:read`  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.get_update_categories_job(job_id, async_req=True)
         >>> result = thread.get()
 
         Args:
@@ -6653,15 +6653,15 @@
 
     def get_update_categories_jobs(
         self,
         **kwargs
     ):
         """Get Update Categories Jobs  # noqa: E501
 
-        Get all catalog category bulk update jobs. Returns a maximum of 100 jobs per request.<br><br>*Rate limits*:<br>Burst: `350/s`<br>Steady: `3500/m`  **Scopes:** `Catalogs Read`  # noqa: E501
+        Get all catalog category bulk update jobs. Returns a maximum of 100 jobs per request.<br><br>*Rate limits*:<br>Burst: `350/s`<br>Steady: `3500/m`  **Scopes:** `catalogs:read`  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.get_update_categories_jobs(async_req=True)
         >>> result = thread.get()
 
 
@@ -6735,15 +6735,15 @@
     def get_update_items_job(
         self,
         job_id,
         **kwargs
     ):
         """Get Update Items Job  # noqa: E501
 
-        Get a catalog item bulk update job with the given job ID. An `include` parameter can be provided to get the following related resource data: `items`.<br><br>*Rate limits*:<br>Burst: `350/s`<br>Steady: `3500/m`  **Scopes:** `Catalogs Read`  # noqa: E501
+        Get a catalog item bulk update job with the given job ID. An `include` parameter can be provided to get the following related resource data: `items`.<br><br>*Rate limits*:<br>Burst: `350/s`<br>Steady: `3500/m`  **Scopes:** `catalogs:read`  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.get_update_items_job(job_id, async_req=True)
         >>> result = thread.get()
 
         Args:
@@ -6820,15 +6820,15 @@
 
     def get_update_items_jobs(
         self,
         **kwargs
     ):
         """Get Update Items Jobs  # noqa: E501
 
-        Get all catalog item bulk update jobs. Returns a maximum of 100 jobs per request.<br><br>*Rate limits*:<br>Burst: `350/s`<br>Steady: `3500/m`  **Scopes:** `Catalogs Read`  # noqa: E501
+        Get all catalog item bulk update jobs. Returns a maximum of 100 jobs per request.<br><br>*Rate limits*:<br>Burst: `350/s`<br>Steady: `3500/m`  **Scopes:** `catalogs:read`  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.get_update_items_jobs(async_req=True)
         >>> result = thread.get()
 
 
@@ -6902,15 +6902,15 @@
     def get_update_variants_job(
         self,
         job_id,
         **kwargs
     ):
         """Get Update Variants Job  # noqa: E501
 
-        Get a catalog variate bulk update job with the given job ID. An `include` parameter can be provided to get the following related resource data: `variants`.<br><br>*Rate limits*:<br>Burst: `350/s`<br>Steady: `3500/m`  **Scopes:** `Catalogs Read`  # noqa: E501
+        Get a catalog variate bulk update job with the given job ID. An `include` parameter can be provided to get the following related resource data: `variants`.<br><br>*Rate limits*:<br>Burst: `350/s`<br>Steady: `3500/m`  **Scopes:** `catalogs:read`  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.get_update_variants_job(job_id, async_req=True)
         >>> result = thread.get()
 
         Args:
@@ -6987,15 +6987,15 @@
 
     def get_update_variants_jobs(
         self,
         **kwargs
     ):
         """Get Update Variants Jobs  # noqa: E501
 
-        Get all catalog variant bulk update jobs. Returns a maximum of 100 jobs per request.<br><br>*Rate limits*:<br>Burst: `350/s`<br>Steady: `3500/m`  **Scopes:** `Catalogs Read`  # noqa: E501
+        Get all catalog variant bulk update jobs. Returns a maximum of 100 jobs per request.<br><br>*Rate limits*:<br>Burst: `350/s`<br>Steady: `3500/m`  **Scopes:** `catalogs:read`  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.get_update_variants_jobs(async_req=True)
         >>> result = thread.get()
 
 
@@ -7069,15 +7069,15 @@
     def spawn_create_categories_job(
         self,
         catalog_category_create_job_create_query,
         **kwargs
     ):
         """Spawn Create Categories Job  # noqa: E501
 
-        Create a catalog category bulk create job to create a batch of catalog categories. Accepts up to 100 catalog categories per request. The maximum allowed payload size is 4MB.<br><br>*Rate limits*:<br>Burst: `75/s`<br>Steady: `700/m`  **Scopes:** `Catalogs Write`  # noqa: E501
+        Create a catalog category bulk create job to create a batch of catalog categories. Accepts up to 100 catalog categories per request. The maximum allowed payload size is 4MB.<br><br>*Rate limits*:<br>Burst: `75/s`<br>Steady: `700/m`  **Scopes:** `catalogs:write`  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.spawn_create_categories_job(catalog_category_create_job_create_query, async_req=True)
         >>> result = thread.get()
 
         Args:
@@ -7152,15 +7152,15 @@
     def spawn_create_items_job(
         self,
         catalog_item_create_job_create_query,
         **kwargs
     ):
         """Spawn Create Items Job  # noqa: E501
 
-        Create a catalog item bulk create job to create a batch of catalog items. Accepts up to 100 catalog items per request. The maximum allowed payload size is 4MB.<br><br>*Rate limits*:<br>Burst: `75/s`<br>Steady: `700/m`  **Scopes:** `Catalogs Write`  # noqa: E501
+        Create a catalog item bulk create job to create a batch of catalog items. Accepts up to 100 catalog items per request. The maximum allowed payload size is 4MB.<br><br>*Rate limits*:<br>Burst: `75/s`<br>Steady: `700/m`  **Scopes:** `catalogs:write`  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.spawn_create_items_job(catalog_item_create_job_create_query, async_req=True)
         >>> result = thread.get()
 
         Args:
@@ -7235,15 +7235,15 @@
     def spawn_create_variants_job(
         self,
         catalog_variant_create_job_create_query,
         **kwargs
     ):
         """Spawn Create Variants Job  # noqa: E501
 
-        Create a catalog variant bulk create job to create a batch of catalog variants. Accepts up to 100 catalog variants per request. The maximum allowed payload size is 4MB.<br><br>*Rate limits*:<br>Burst: `75/s`<br>Steady: `700/m`  **Scopes:** `Catalogs Write`  # noqa: E501
+        Create a catalog variant bulk create job to create a batch of catalog variants. Accepts up to 100 catalog variants per request. The maximum allowed payload size is 4MB.<br><br>*Rate limits*:<br>Burst: `75/s`<br>Steady: `700/m`  **Scopes:** `catalogs:write`  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.spawn_create_variants_job(catalog_variant_create_job_create_query, async_req=True)
         >>> result = thread.get()
 
         Args:
@@ -7318,15 +7318,15 @@
     def spawn_delete_categories_job(
         self,
         catalog_category_delete_job_create_query,
         **kwargs
     ):
         """Spawn Delete Categories Job  # noqa: E501
 
-        Create a catalog category bulk delete job to delete a batch of catalog categories. Accepts up to 100 catalog categories per request. The maximum allowed payload size is 4MB.<br><br>*Rate limits*:<br>Burst: `75/s`<br>Steady: `700/m`  **Scopes:** `Catalogs Write`  # noqa: E501
+        Create a catalog category bulk delete job to delete a batch of catalog categories. Accepts up to 100 catalog categories per request. The maximum allowed payload size is 4MB.<br><br>*Rate limits*:<br>Burst: `75/s`<br>Steady: `700/m`  **Scopes:** `catalogs:write`  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.spawn_delete_categories_job(catalog_category_delete_job_create_query, async_req=True)
         >>> result = thread.get()
 
         Args:
@@ -7401,15 +7401,15 @@
     def spawn_delete_items_job(
         self,
         catalog_item_delete_job_create_query,
         **kwargs
     ):
         """Spawn Delete Items Job  # noqa: E501
 
-        Create a catalog item bulk delete job to delete a batch of catalog items. Accepts up to 100 catalog items per request. The maximum allowed payload size is 4MB.<br><br>*Rate limits*:<br>Burst: `75/s`<br>Steady: `700/m`  **Scopes:** `Catalogs Write`  # noqa: E501
+        Create a catalog item bulk delete job to delete a batch of catalog items. Accepts up to 100 catalog items per request. The maximum allowed payload size is 4MB.<br><br>*Rate limits*:<br>Burst: `75/s`<br>Steady: `700/m`  **Scopes:** `catalogs:write`  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.spawn_delete_items_job(catalog_item_delete_job_create_query, async_req=True)
         >>> result = thread.get()
 
         Args:
@@ -7484,15 +7484,15 @@
     def spawn_delete_variants_job(
         self,
         catalog_variant_delete_job_create_query,
         **kwargs
     ):
         """Spawn Delete Variants Job  # noqa: E501
 
-        Create a catalog variant bulk delete job to delete a batch of catalog variants. Accepts up to 100 catalog variants per request. The maximum allowed payload size is 4MB.<br><br>*Rate limits*:<br>Burst: `75/s`<br>Steady: `700/m`  **Scopes:** `Catalogs Write`  # noqa: E501
+        Create a catalog variant bulk delete job to delete a batch of catalog variants. Accepts up to 100 catalog variants per request. The maximum allowed payload size is 4MB.<br><br>*Rate limits*:<br>Burst: `75/s`<br>Steady: `700/m`  **Scopes:** `catalogs:write`  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.spawn_delete_variants_job(catalog_variant_delete_job_create_query, async_req=True)
         >>> result = thread.get()
 
         Args:
@@ -7567,15 +7567,15 @@
     def spawn_update_categories_job(
         self,
         catalog_category_update_job_create_query,
         **kwargs
     ):
         """Spawn Update Categories Job  # noqa: E501
 
-        Create a catalog category bulk update job to update a batch of catalog categories. Accepts up to 100 catalog categories per request. The maximum allowed payload size is 4MB.<br><br>*Rate limits*:<br>Burst: `75/s`<br>Steady: `700/m`  **Scopes:** `Catalogs Write`  # noqa: E501
+        Create a catalog category bulk update job to update a batch of catalog categories. Accepts up to 100 catalog categories per request. The maximum allowed payload size is 4MB.<br><br>*Rate limits*:<br>Burst: `75/s`<br>Steady: `700/m`  **Scopes:** `catalogs:write`  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.spawn_update_categories_job(catalog_category_update_job_create_query, async_req=True)
         >>> result = thread.get()
 
         Args:
@@ -7650,15 +7650,15 @@
     def spawn_update_items_job(
         self,
         catalog_item_update_job_create_query,
         **kwargs
     ):
         """Spawn Update Items Job  # noqa: E501
 
-        Create a catalog item bulk update job to update a batch of catalog items. Accepts up to 100 catalog items per request. The maximum allowed payload size is 4MB.<br><br>*Rate limits*:<br>Burst: `75/s`<br>Steady: `700/m`  **Scopes:** `Catalogs Write`  # noqa: E501
+        Create a catalog item bulk update job to update a batch of catalog items. Accepts up to 100 catalog items per request. The maximum allowed payload size is 4MB.<br><br>*Rate limits*:<br>Burst: `75/s`<br>Steady: `700/m`  **Scopes:** `catalogs:write`  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.spawn_update_items_job(catalog_item_update_job_create_query, async_req=True)
         >>> result = thread.get()
 
         Args:
@@ -7733,15 +7733,15 @@
     def spawn_update_variants_job(
         self,
         catalog_variant_update_job_create_query,
         **kwargs
     ):
         """Spawn Update Variants Job  # noqa: E501
 
-        Create a catalog variant bulk update job to update a batch of catalog variants. Accepts up to 100 catalog variants per request. The maximum allowed payload size is 4MB.<br><br>*Rate limits*:<br>Burst: `75/s`<br>Steady: `700/m`  **Scopes:** `Catalogs Write`  # noqa: E501
+        Create a catalog variant bulk update job to update a batch of catalog variants. Accepts up to 100 catalog variants per request. The maximum allowed payload size is 4MB.<br><br>*Rate limits*:<br>Burst: `75/s`<br>Steady: `700/m`  **Scopes:** `catalogs:write`  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.spawn_update_variants_job(catalog_variant_update_job_create_query, async_req=True)
         >>> result = thread.get()
 
         Args:
@@ -7817,15 +7817,15 @@
         self,
         id,
         catalog_category_update_query,
         **kwargs
     ):
         """Update Catalog Category  # noqa: E501
 
-        Update a catalog category with the given category ID.<br><br>*Rate limits*:<br>Burst: `75/s`<br>Steady: `700/m`  **Scopes:** `Catalogs Write`  # noqa: E501
+        Update a catalog category with the given category ID.<br><br>*Rate limits*:<br>Burst: `75/s`<br>Steady: `700/m`  **Scopes:** `catalogs:write`  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.update_catalog_category(id, catalog_category_update_query, async_req=True)
         >>> result = thread.get()
 
         Args:
@@ -7904,15 +7904,15 @@
         self,
         id,
         catalog_category_item_op,
         **kwargs
     ):
         """Update Catalog Category Relationships Items  # noqa: E501
 
-        Update item relationships for the given category ID.<br><br>*Rate limits*:<br>Burst: `75/s`<br>Steady: `700/m`  **Scopes:** `Catalogs Write`  # noqa: E501
+        Update item relationships for the given category ID.<br><br>*Rate limits*:<br>Burst: `75/s`<br>Steady: `700/m`  **Scopes:** `catalogs:write`  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.update_catalog_category_relationships_items(id, catalog_category_item_op, async_req=True)
         >>> result = thread.get()
 
         Args:
@@ -7991,15 +7991,15 @@
         self,
         id,
         catalog_item_update_query,
         **kwargs
     ):
         """Update Catalog Item  # noqa: E501
 
-        Update a catalog item with the given item ID.<br><br>*Rate limits*:<br>Burst: `75/s`<br>Steady: `700/m`  **Scopes:** `Catalogs Write`  # noqa: E501
+        Update a catalog item with the given item ID.<br><br>*Rate limits*:<br>Burst: `75/s`<br>Steady: `700/m`  **Scopes:** `catalogs:write`  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.update_catalog_item(id, catalog_item_update_query, async_req=True)
         >>> result = thread.get()
 
         Args:
@@ -8078,15 +8078,15 @@
         self,
         id,
         catalog_item_category_op,
         **kwargs
     ):
         """Update Catalog Item Relationships Categories  # noqa: E501
 
-        Update catalog category relationships for the given item ID.<br><br>*Rate limits*:<br>Burst: `75/s`<br>Steady: `700/m`  **Scopes:** `Catalogs Write`  # noqa: E501
+        Update catalog category relationships for the given item ID.<br><br>*Rate limits*:<br>Burst: `75/s`<br>Steady: `700/m`  **Scopes:** `catalogs:write`  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.update_catalog_item_relationships_categories(id, catalog_item_category_op, async_req=True)
         >>> result = thread.get()
 
         Args:
@@ -8165,15 +8165,15 @@
         self,
         id,
         catalog_variant_update_query,
         **kwargs
     ):
         """Update Catalog Variant  # noqa: E501
 
-        Update a catalog item variant with the given variant ID.<br><br>*Rate limits*:<br>Burst: `75/s`<br>Steady: `700/m`  **Scopes:** `Catalogs Write`  # noqa: E501
+        Update a catalog item variant with the given variant ID.<br><br>*Rate limits*:<br>Burst: `75/s`<br>Steady: `700/m`  **Scopes:** `catalogs:write`  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.update_catalog_variant(id, catalog_variant_update_query, async_req=True)
         >>> result = thread.get()
 
         Args:
```

### Comparing `klaviyo-api-2.0.1/src/openapi_client/api/client_api.py` & `klaviyo-api-2.0.2/src/openapi_client/api/client_api.py`

 * *Files 3% similar despite different names*

```diff
@@ -210,23 +210,23 @@
         self,
         company_id,
         event_create_query,
         **kwargs
     ):
         """Create Client Event  # noqa: E501
 
-        Create a new event to track a profile's activity. This endpoint is specifically designed to be called from publicly-browseable, client-side environments only. To create events from server-based applications, please use [POST /api/events](https://developers.klaviyo.com/en/reference/create_event)<br><br>*Rate limits*:<br>Burst: `350/s`<br>Steady: `3500/m`  **Scopes:** `Events Write`  # noqa: E501
+        Create a new event to track a profile's activity. This endpoint is specifically designed to be called from publicly-browseable, client-side environments only. To create events from server-based applications, please use [POST /api/events](https://developers.klaviyo.com/en/reference/create_event)<br><br>*Rate limits*:<br>Burst: `350/s`<br>Steady: `3500/m`  **Scopes:** `events:write`  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.create_client_event(company_id, event_create_query, async_req=True)
         >>> result = thread.get()
 
         Args:
-            company_id (str): ID of the Company to create event
+            company_id (str): Your Public API Key / Site ID. See [this article](https://help.klaviyo.com/hc/en-us/articles/115005062267) for more details.
             event_create_query (EventCreateQuery): Event to create.
 
         Keyword Args:
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
@@ -297,23 +297,23 @@
         self,
         company_id,
         onsite_profile_create_query,
         **kwargs
     ):
         """Create or Update Client Profile  # noqa: E501
 
-        Create and update properties about a profile without tracking an associated event. This endpoint is specifically designed to be called from publicly-browseable, client-side environments only. To create profiles from server applications (e.g. custom server-side scripts / applications), please use [POST /api/profiles](https://developers.klaviyo.com/en/reference/create_profile)<br><br>*Rate limits*:<br>Burst: `350/s`<br>Steady: `3500/m`  **Scopes:** `Profiles Write`  # noqa: E501
+        Create and update properties about a profile without tracking an associated event. This endpoint is specifically designed to be called from publicly-browseable, client-side environments only. To create profiles from server applications (e.g. custom server-side scripts / applications), please use [POST /api/profiles](https://developers.klaviyo.com/en/reference/create_profile)<br><br>*Rate limits*:<br>Burst: `350/s`<br>Steady: `3500/m`  **Scopes:** `profiles:write`  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.create_client_profile(company_id, onsite_profile_create_query, async_req=True)
         >>> result = thread.get()
 
         Args:
-            company_id (str): 
+            company_id (str): Your Public API Key / Site ID. See [this article](https://help.klaviyo.com/hc/en-us/articles/115005062267) for more details.
             onsite_profile_create_query (OnsiteProfileCreateQuery):
 
         Keyword Args:
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
@@ -384,23 +384,23 @@
         self,
         company_id,
         onsite_subscription_create_query,
         **kwargs
     ):
         """Create Client Subscription  # noqa: E501
 
-        Create a new subscription for the given list ID and channel:  * Email `email` * SMS `phone_number`  This endpoint is specifically designed to be called from publicly-browseable, client-side environments only. To create subscriptions from server-based applications, please use [POST /api/profile-subscription-bulk-create-jobs](https://developers.klaviyo.com/en/reference/subscribe_profiles)<br><br>*Rate limits*:<br>Burst: `100/s`<br>Steady: `100/m`  **Scopes:** `Subscriptions Write`  # noqa: E501
+        Create a new subscription for the given list ID and channel:  * Email `email` * SMS `phone_number`  This endpoint is specifically designed to be called from publicly-browseable, client-side environments only. To create subscriptions from server-based applications, please use [POST /api/profile-subscription-bulk-create-jobs](https://developers.klaviyo.com/en/reference/subscribe_profiles)<br><br>*Rate limits*:<br>Burst: `100/s`<br>Steady: `700/m`  **Scopes:** `subscriptions:write`  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.create_client_subscription(company_id, onsite_subscription_create_query, async_req=True)
         >>> result = thread.get()
 
         Args:
-            company_id (str): Your company ID.
+            company_id (str): Your Public API Key / Site ID. See [this article](https://help.klaviyo.com/hc/en-us/articles/115005062267) for more details.
             onsite_subscription_create_query (OnsiteSubscriptionCreateQuery): Creates a subscription and consent records for Email and or SMS channels based on the provided email and phone_number attributes respectively. One of either email or phone_number must be provided. To create a subscription and consent record for only one channel but still include the other channel as a profile property the consent channel can be provided as a top level attribute and the other channel can be included in the properties object.
 
         Keyword Args:
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
```

### Comparing `klaviyo-api-2.0.1/src/openapi_client/api/data_privacy_api.py` & `klaviyo-api-2.0.2/src/openapi_client/api/data_privacy_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -93,15 +93,15 @@
     def request_profile_deletion(
         self,
         data_privacy_create_deletion_job_query,
         **kwargs
     ):
         """Request Profile Deletion  # noqa: E501
 
-        Request a deletion for the profiles corresponding to one of the following identifiers: `email`, `phone_number`, or `profile_id`. If multiple identifiers are provided, we will return an error. All profiles that match the provided identifier will be deleted.         The deletion occurs asynchronously; however, once it has completed, the deleted profile will appear on the [Deleted Profiles page](https://www.klaviyo.com/account/deleted).         For more information on the deletion process, please refer to our [Help Center docs on how to handle GDPR and CCPA deletion requests](https://help.klaviyo.com/hc/en-us/articles/360004217631-How-to-Handle-GDPR-Requests#record-gdpr-and-ccpa%20%20-deletion-requests2).<br><br>*Rate limits*:<br>Burst: `3/s`<br>Steady: `60/m`  **Scopes:** `Data Privacy Write`  # noqa: E501
+        Request a deletion for the profiles corresponding to one of the following identifiers: `email`, `phone_number`, or `profile_id`. If multiple identifiers are provided, we will return an error. All profiles that match the provided identifier will be deleted.         The deletion occurs asynchronously; however, once it has completed, the deleted profile will appear on the [Deleted Profiles page](https://www.klaviyo.com/account/deleted).         For more information on the deletion process, please refer to our [Help Center docs on how to handle GDPR and CCPA deletion requests](https://help.klaviyo.com/hc/en-us/articles/360004217631-How-to-Handle-GDPR-Requests#record-gdpr-and-ccpa%20%20-deletion-requests2).<br><br>*Rate limits*:<br>Burst: `3/s`<br>Steady: `60/m`  **Scopes:** `data-privacy:write`  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.request_profile_deletion(data_privacy_create_deletion_job_query, async_req=True)
         >>> result = thread.get()
 
         Args:
```

### Comparing `klaviyo-api-2.0.1/src/openapi_client/api/events_api.py` & `klaviyo-api-2.0.2/src/openapi_client/api/events_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -696,15 +696,15 @@
     def create_event(
         self,
         event_create_query,
         **kwargs
     ):
         """Create Event  # noqa: E501
 
-        Create an event. Events are created asynchronously. Successful response indicates that the event was validated and submitted for processing, but does not guarantee that processing is complete.<br><br>*Rate limits*:<br>Burst: `350/s`<br>Steady: `3500/m`  **Scopes:** `Events Write`  # noqa: E501
+        Create an event. Events are created asynchronously. Successful response indicates that the event was validated and submitted for processing, but does not guarantee that processing is complete.<br><br>*Rate limits*:<br>Burst: `350/s`<br>Steady: `3500/m`  **Scopes:** `events:write`  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.create_event(event_create_query, async_req=True)
         >>> result = thread.get()
 
         Args:
@@ -779,15 +779,15 @@
     def get_event(
         self,
         id,
         **kwargs
     ):
         """Get Event  # noqa: E501
 
-        Get an event with the given event ID. Include parameters can be provided to get the following related resource data: `metrics`, `profiles`<br><br>*Rate limits*:<br>Burst: `10/s`<br>Steady: `150/m`  **Scopes:** `Events Read`  # noqa: E501
+        Get an event with the given event ID. Include parameters can be provided to get the following related resource data: `metrics`, `profiles`<br><br>*Rate limits*:<br>Burst: `10/s`<br>Steady: `150/m`  **Scopes:** `events:read`  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.get_event(id, async_req=True)
         >>> result = thread.get()
 
         Args:
@@ -866,15 +866,15 @@
     def get_event_metrics(
         self,
         id,
         **kwargs
     ):
         """Get Event Metrics  # noqa: E501
 
-        Get the metric for an event with the given event ID.<br><br>*Rate limits*:<br>Burst: `350/s`<br>Steady: `3500/m`  **Scopes:** `Events Read` `Metrics Read`  # noqa: E501
+        Get the metric for an event with the given event ID.<br><br>*Rate limits*:<br>Burst: `350/s`<br>Steady: `3500/m`  **Scopes:** `events:read` `metrics:read`  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.get_event_metrics(id, async_req=True)
         >>> result = thread.get()
 
         Args:
@@ -950,15 +950,15 @@
     def get_event_profiles(
         self,
         id,
         **kwargs
     ):
         """Get Event Profiles  # noqa: E501
 
-        Get the profile associated with an event with the given event ID.<br><br>*Rate limits*:<br>Burst: `350/s`<br>Steady: `3500/m`  **Scopes:** `Events Read` `Profiles Read`  # noqa: E501
+        Get the profile associated with an event with the given event ID.<br><br>*Rate limits*:<br>Burst: `350/s`<br>Steady: `3500/m`  **Scopes:** `events:read` `profiles:read`  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.get_event_profiles(id, async_req=True)
         >>> result = thread.get()
 
         Args:
@@ -1035,15 +1035,15 @@
     def get_event_relationships_metrics(
         self,
         id,
         **kwargs
     ):
         """Get Event Relationships Metrics  # noqa: E501
 
-        Get a list of related Metrics for an Event<br><br>*Rate limits*:<br>Burst: `350/s`<br>Steady: `3500/m`  **Scopes:** `Events Read` `Metrics Read`  # noqa: E501
+        Get a list of related Metrics for an Event<br><br>*Rate limits*:<br>Burst: `350/s`<br>Steady: `3500/m`  **Scopes:** `events:read` `metrics:read`  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.get_event_relationships_metrics(id, async_req=True)
         >>> result = thread.get()
 
         Args:
@@ -1118,15 +1118,15 @@
     def get_event_relationships_profiles(
         self,
         id,
         **kwargs
     ):
         """Get Event Relationships Profiles  # noqa: E501
 
-        Get profile [relationships](https://developers.klaviyo.com/en/reference/api_overview#relationships) for an event with the given event ID.<br><br>*Rate limits*:<br>Burst: `350/s`<br>Steady: `3500/m`  **Scopes:** `Events Read` `Profiles Read`  # noqa: E501
+        Get profile [relationships](https://developers.klaviyo.com/en/reference/api_overview#relationships) for an event with the given event ID.<br><br>*Rate limits*:<br>Burst: `350/s`<br>Steady: `3500/m`  **Scopes:** `events:read` `profiles:read`  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.get_event_relationships_profiles(id, async_req=True)
         >>> result = thread.get()
 
         Args:
@@ -1200,15 +1200,15 @@
 
     def get_events(
         self,
         **kwargs
     ):
         """Get Events  # noqa: E501
 
-        Get all events in an account Requests can be sorted by the following fields: `datetime`, `timestamp` Include parameters can be provided to get the following related resource data: `metrics`, `profiles` Returns a maximum of 200 events per page.<br><br>*Rate limits*:<br>Burst: `350/s`<br>Steady: `3500/m`  **Scopes:** `Events Read`  # noqa: E501
+        Get all events in an account Requests can be sorted by the following fields: `datetime`, `timestamp` Include parameters can be provided to get the following related resource data: `metrics`, `profiles` Returns a maximum of 200 events per page.<br><br>*Rate limits*:<br>Burst: `350/s`<br>Steady: `3500/m`  **Scopes:** `events:read`  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.get_events(async_req=True)
         >>> result = thread.get()
```

### Comparing `klaviyo-api-2.0.1/src/openapi_client/api/flows_api.py` & `klaviyo-api-2.0.2/src/openapi_client/api/flows_api.py`

 * *Files 6% similar despite different names*

```diff
@@ -337,30 +337,37 @@
             },
             params_map={
                 'all': [
                     'action_id',
                     'fields_flow_message',
                     'filter',
                     'page_cursor',
+                    'page_size',
                     'sort',
                 ],
                 'required': [
                     'action_id',
                 ],
                 'nullable': [
                 ],
                 'enum': [
                     'fields_flow_message',
                     'sort',
                 ],
                 'validation': [
+                    'page_size',
                 ]
             },
             root_map={
                 'validations': {
+                    ('page_size',): {
+
+                        'inclusive_maximum': 50,
+                        'inclusive_minimum': 1,
+                    },
                 },
                 'allowed_values': {
                     ('fields_flow_message',): {
 
                         "NAME": "name",
                         "CHANNEL": "channel",
                         "CONTENT": "content",
@@ -384,29 +391,33 @@
                         (str,),
                     'fields_flow_message':
                         ([str],),
                     'filter':
                         (str,),
                     'page_cursor':
                         (str,),
+                    'page_size':
+                        (int,),
                     'sort':
                         (str,),
                 },
                 'attribute_map': {
                     'action_id': 'action_id',
                     'fields_flow_message': 'fields[flow-message]',
                     'filter': 'filter',
                     'page_cursor': 'page[cursor]',
+                    'page_size': 'page[size]',
                     'sort': 'sort',
                 },
                 'location_map': {
                     'action_id': 'path',
                     'fields_flow_message': 'query',
                     'filter': 'query',
                     'page_cursor': 'query',
+                    'page_size': 'query',
                     'sort': 'query',
                 },
                 'collection_format_map': {
                     'fields_flow_message': 'csv',
                 }
             },
             headers_map={
@@ -480,29 +491,36 @@
                 'servers': None,
             },
             params_map={
                 'all': [
                     'id',
                     'filter',
                     'page_cursor',
+                    'page_size',
                     'sort',
                 ],
                 'required': [
                     'id',
                 ],
                 'nullable': [
                 ],
                 'enum': [
                     'sort',
                 ],
                 'validation': [
+                    'page_size',
                 ]
             },
             root_map={
                 'validations': {
+                    ('page_size',): {
+
+                        'inclusive_maximum': 50,
+                        'inclusive_minimum': 1,
+                    },
                 },
                 'allowed_values': {
                     ('sort',): {
 
                         "CREATED": "created",
                         "-CREATED": "-created",
                         "ID": "id",
@@ -516,27 +534,31 @@
                 'openapi_types': {
                     'id':
                         (str,),
                     'filter':
                         (str,),
                     'page_cursor':
                         (str,),
+                    'page_size':
+                        (int,),
                     'sort':
                         (str,),
                 },
                 'attribute_map': {
                     'id': 'id',
                     'filter': 'filter',
                     'page_cursor': 'page[cursor]',
+                    'page_size': 'page[size]',
                     'sort': 'sort',
                 },
                 'location_map': {
                     'id': 'path',
                     'filter': 'query',
                     'page_cursor': 'query',
+                    'page_size': 'query',
                     'sort': 'query',
                 },
                 'collection_format_map': {
                 }
             },
             headers_map={
                 'accept': [
@@ -559,30 +581,37 @@
             },
             params_map={
                 'all': [
                     'flow_id',
                     'fields_flow_action',
                     'filter',
                     'page_cursor',
+                    'page_size',
                     'sort',
                 ],
                 'required': [
                     'flow_id',
                 ],
                 'nullable': [
                 ],
                 'enum': [
                     'fields_flow_action',
                     'sort',
                 ],
                 'validation': [
+                    'page_size',
                 ]
             },
             root_map={
                 'validations': {
+                    ('page_size',): {
+
+                        'inclusive_maximum': 50,
+                        'inclusive_minimum': 1,
+                    },
                 },
                 'allowed_values': {
                     ('fields_flow_action',): {
 
                         "ACTION_TYPE": "action_type",
                         "STATUS": "status",
                         "CREATED": "created",
@@ -617,29 +646,33 @@
                         (str,),
                     'fields_flow_action':
                         ([str],),
                     'filter':
                         (str,),
                     'page_cursor':
                         (str,),
+                    'page_size':
+                        (int,),
                     'sort':
                         (str,),
                 },
                 'attribute_map': {
                     'flow_id': 'flow_id',
                     'fields_flow_action': 'fields[flow-action]',
                     'filter': 'filter',
                     'page_cursor': 'page[cursor]',
+                    'page_size': 'page[size]',
                     'sort': 'sort',
                 },
                 'location_map': {
                     'flow_id': 'path',
                     'fields_flow_action': 'query',
                     'filter': 'query',
                     'page_cursor': 'query',
+                    'page_size': 'query',
                     'sort': 'query',
                 },
                 'collection_format_map': {
                     'fields_flow_action': 'csv',
                 }
             },
             headers_map={
@@ -888,29 +921,36 @@
                 'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'id',
                     'filter',
+                    'page_size',
                     'sort',
                 ],
                 'required': [
                     'id',
                 ],
                 'nullable': [
                 ],
                 'enum': [
                     'sort',
                 ],
                 'validation': [
+                    'page_size',
                 ]
             },
             root_map={
                 'validations': {
+                    ('page_size',): {
+
+                        'inclusive_maximum': 100,
+                        'inclusive_minimum': 1,
+                    },
                 },
                 'allowed_values': {
                     ('sort',): {
 
                         "CREATED": "created",
                         "-CREATED": "-created",
                         "ID": "id",
@@ -922,25 +962,29 @@
                     },
                 },
                 'openapi_types': {
                     'id':
                         (str,),
                     'filter':
                         (str,),
+                    'page_size':
+                        (int,),
                     'sort':
                         (str,),
                 },
                 'attribute_map': {
                     'id': 'id',
                     'filter': 'filter',
+                    'page_size': 'page[size]',
                     'sort': 'sort',
                 },
                 'location_map': {
                     'id': 'path',
                     'filter': 'query',
+                    'page_size': 'query',
                     'sort': 'query',
                 },
                 'collection_format_map': {
                 }
             },
             headers_map={
                 'accept': [
@@ -1077,30 +1121,37 @@
             params_map={
                 'all': [
                     'fields_flow_action',
                     'fields_flow',
                     'filter',
                     'include',
                     'page_cursor',
+                    'page_size',
                     'sort',
                 ],
                 'required': [],
                 'nullable': [
                 ],
                 'enum': [
                     'fields_flow_action',
                     'fields_flow',
                     'include',
                     'sort',
                 ],
                 'validation': [
+                    'page_size',
                 ]
             },
             root_map={
                 'validations': {
+                    ('page_size',): {
+
+                        'inclusive_maximum': 50,
+                        'inclusive_minimum': 1,
+                    },
                 },
                 'allowed_values': {
                     ('fields_flow_action',): {
 
                         "ACTION_TYPE": "action_type",
                         "STATUS": "status",
                         "CREATED": "created",
@@ -1152,31 +1203,35 @@
                         ([str],),
                     'filter':
                         (str,),
                     'include':
                         ([str],),
                     'page_cursor':
                         (str,),
+                    'page_size':
+                        (int,),
                     'sort':
                         (str,),
                 },
                 'attribute_map': {
                     'fields_flow_action': 'fields[flow-action]',
                     'fields_flow': 'fields[flow]',
                     'filter': 'filter',
                     'include': 'include',
                     'page_cursor': 'page[cursor]',
+                    'page_size': 'page[size]',
                     'sort': 'sort',
                 },
                 'location_map': {
                     'fields_flow_action': 'query',
                     'fields_flow': 'query',
                     'filter': 'query',
                     'include': 'query',
                     'page_cursor': 'query',
+                    'page_size': 'query',
                     'sort': 'query',
                 },
                 'collection_format_map': {
                     'fields_flow_action': 'csv',
                     'fields_flow': 'csv',
                     'include': 'csv',
                 }
@@ -1251,15 +1306,15 @@
     def get_flow(
         self,
         id,
         **kwargs
     ):
         """Get Flow  # noqa: E501
 
-        Get a flow with the given flow ID. Include parameters can be provided to get the following related resource data: `flow-actions`<br><br>*Rate limits*:<br>Burst: `3/s`<br>Steady: `60/m`  **Scopes:** `Flows Read`  # noqa: E501
+        Get a flow with the given flow ID. Include parameters can be provided to get the following related resource data: `flow-actions`<br><br>*Rate limits*:<br>Burst: `3/s`<br>Steady: `60/m`  **Scopes:** `flows:read`  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.get_flow(id, async_req=True)
         >>> result = thread.get()
 
         Args:
@@ -1337,15 +1392,15 @@
     def get_flow_action(
         self,
         id,
         **kwargs
     ):
         """Get Flow Action  # noqa: E501
 
-        Get a flow action from a flow with the given flow action ID. Include parameters can be provided to get the following related resource data: `flows`, `flow-messages`<br><br>*Rate limits*:<br>Burst: `3/s`<br>Steady: `60/m`  **Scopes:** `Flows Read`  # noqa: E501
+        Get a flow action from a flow with the given flow action ID. Include parameters can be provided to get the following related resource data: `flows`, `flow-messages`<br><br>*Rate limits*:<br>Burst: `3/s`<br>Steady: `60/m`  **Scopes:** `flows:read`  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.get_flow_action(id, async_req=True)
         >>> result = thread.get()
 
         Args:
@@ -1424,15 +1479,15 @@
     def get_flow_action_flow(
         self,
         action_id,
         **kwargs
     ):
         """Get Flow For Flow Action  # noqa: E501
 
-        Get the flow associated with the given action ID.<br><br>*Rate limits*:<br>Burst: `3/s`<br>Steady: `60/m`  **Scopes:** `Flows Read`  # noqa: E501
+        Get the flow associated with the given action ID.<br><br>*Rate limits*:<br>Burst: `3/s`<br>Steady: `60/m`  **Scopes:** `flows:read`  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.get_flow_action_flow(action_id, async_req=True)
         >>> result = thread.get()
 
         Args:
@@ -1508,28 +1563,29 @@
     def get_flow_action_messages(
         self,
         action_id,
         **kwargs
     ):
         """Get Messages For Flow Action  # noqa: E501
 
-        Get all flow messages associated with the given flow action ID.  Returns a maximum of 50 flow message relationships per request, which can be paginated with cursor-based pagination.<br><br>*Rate limits*:<br>Burst: `3/s`<br>Steady: `60/m`  **Scopes:** `Flows Read`  # noqa: E501
+        Get all flow messages associated with the given flow action ID.  Returns a maximum of 50 flow message relationships per request, which can be paginated with cursor-based pagination.<br><br>*Rate limits*:<br>Burst: `3/s`<br>Steady: `60/m`  **Scopes:** `flows:read`  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.get_flow_action_messages(action_id, async_req=True)
         >>> result = thread.get()
 
         Args:
             action_id (str): 
 
         Keyword Args:
             fields_flow_message ([str]): For more information please visit https://developers.klaviyo.com/en/v2023-02-22/reference/api-overview#sparse-fieldsets. [optional]
             filter (str): For more information please visit https://developers.klaviyo.com/en/v2023-02-22/reference/api-overview#filtering<br>Allowed field(s)/operator(s):<br>`id`: `any`<br>`name`: `contains`, `ends-with`, `equals`, `starts-with`<br>`created`: `equals`, `greater-or-equal`, `greater-than`, `less-or-equal`, `less-than`<br>`updated`: `equals`, `greater-or-equal`, `greater-than`, `less-or-equal`, `less-than`. [optional]
             page_cursor (str): For more information please visit https://developers.klaviyo.com/en/v2023-02-22/reference/api-overview#pagination. [optional]
+            page_size (int): Default: 50. Min: 1. Max: 50.. [optional] if omitted the server will use the default value of 50
             sort (str): For more information please visit https://developers.klaviyo.com/en/v2023-02-22/reference/api-overview#sorting. [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
@@ -1595,15 +1651,15 @@
     def get_flow_action_relationships_flow(
         self,
         id,
         **kwargs
     ):
         """Get Flow Action Relationships Flow  # noqa: E501
 
-        Get the flow associated with the given action ID.<br><br>*Rate limits*:<br>Burst: `3/s`<br>Steady: `60/m`  **Scopes:** `Flows Read`  # noqa: E501
+        Get the flow associated with the given action ID.<br><br>*Rate limits*:<br>Burst: `3/s`<br>Steady: `60/m`  **Scopes:** `flows:read`  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.get_flow_action_relationships_flow(id, async_req=True)
         >>> result = thread.get()
 
         Args:
@@ -1678,27 +1734,28 @@
     def get_flow_action_relationships_messages(
         self,
         id,
         **kwargs
     ):
         """Get Flow Action Relationships Messages  # noqa: E501
 
-        Get all relationships for flow messages associated with the given flow action ID.  Returns a maximum of 50 flow message relationships per request, which can be paginated with cursor-based pagination.<br><br>*Rate limits*:<br>Burst: `3/s`<br>Steady: `60/m`  **Scopes:** `Flows Read`  # noqa: E501
+        Get all relationships for flow messages associated with the given flow action ID.  Returns a maximum of 50 flow message relationships per request, which can be paginated with cursor-based pagination.<br><br>*Rate limits*:<br>Burst: `3/s`<br>Steady: `60/m`  **Scopes:** `flows:read`  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.get_flow_action_relationships_messages(id, async_req=True)
         >>> result = thread.get()
 
         Args:
             id (str): 
 
         Keyword Args:
             filter (str): For more information please visit https://developers.klaviyo.com/en/v2023-02-22/reference/api-overview#filtering<br>Allowed field(s)/operator(s):<br>`name`: `contains`, `ends-with`, `equals`, `starts-with`<br>`created`: `equals`, `greater-or-equal`, `greater-than`, `less-or-equal`, `less-than`<br>`updated`: `equals`, `greater-or-equal`, `greater-than`, `less-or-equal`, `less-than`. [optional]
             page_cursor (str): For more information please visit https://developers.klaviyo.com/en/v2023-02-22/reference/api-overview#pagination. [optional]
+            page_size (int): Default: 50. Min: 1. Max: 50.. [optional] if omitted the server will use the default value of 50
             sort (str): For more information please visit https://developers.klaviyo.com/en/v2023-02-22/reference/api-overview#sorting. [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
@@ -1764,28 +1821,29 @@
     def get_flow_flow_actions(
         self,
         flow_id,
         **kwargs
     ):
         """Get Flow Actions For Flow  # noqa: E501
 
-        Get all flow actions associated with the given flow ID.  Returns a maximum of 50 flows per request, which can be paginated with cursor-based pagination.<br><br>*Rate limits*:<br>Burst: `3/s`<br>Steady: `60/m`  **Scopes:** `Flows Read`  # noqa: E501
+        Get all flow actions associated with the given flow ID.  Returns a maximum of 50 flows per request, which can be paginated with cursor-based pagination.<br><br>*Rate limits*:<br>Burst: `3/s`<br>Steady: `60/m`  **Scopes:** `flows:read`  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.get_flow_flow_actions(flow_id, async_req=True)
         >>> result = thread.get()
 
         Args:
             flow_id (str): 
 
         Keyword Args:
             fields_flow_action ([str]): For more information please visit https://developers.klaviyo.com/en/v2023-02-22/reference/api-overview#sparse-fieldsets. [optional]
             filter (str): For more information please visit https://developers.klaviyo.com/en/v2023-02-22/reference/api-overview#filtering<br>Allowed field(s)/operator(s):<br>`id`: `any`<br>`action_type`: `any`, `equals`<br>`status`: `equals`<br>`created`: `equals`, `greater-or-equal`, `greater-than`, `less-or-equal`, `less-than`<br>`updated`: `equals`, `greater-or-equal`, `greater-than`, `less-or-equal`, `less-than`. [optional]
             page_cursor (str): For more information please visit https://developers.klaviyo.com/en/v2023-02-22/reference/api-overview#pagination. [optional]
+            page_size (int): Default: 50. Min: 1. Max: 50.. [optional] if omitted the server will use the default value of 50
             sort (str): For more information please visit https://developers.klaviyo.com/en/v2023-02-22/reference/api-overview#sorting. [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
@@ -1851,15 +1909,15 @@
     def get_flow_message(
         self,
         id,
         **kwargs
     ):
         """Get Flow Message  # noqa: E501
 
-        Get the flow message of a flow with the given message ID. Include parameters can be provided to get the following related resource data: 'flow-actions'<br><br>*Rate limits*:<br>Burst: `3/s`<br>Steady: `60/m`  **Scopes:** `Flows Read`  # noqa: E501
+        Get the flow message of a flow with the given message ID. Include parameters can be provided to get the following related resource data: 'flow-actions'<br><br>*Rate limits*:<br>Burst: `3/s`<br>Steady: `60/m`  **Scopes:** `flows:read`  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.get_flow_message(id, async_req=True)
         >>> result = thread.get()
 
         Args:
@@ -1937,15 +1995,15 @@
     def get_flow_message_action(
         self,
         message_id,
         **kwargs
     ):
         """Get Flow Action For Message  # noqa: E501
 
-        Get the flow action for a flow message with the given message ID.<br><br>*Rate limits*:<br>Burst: `3/s`<br>Steady: `60/m`  **Scopes:** `Flows Read`  # noqa: E501
+        Get the flow action for a flow message with the given message ID.<br><br>*Rate limits*:<br>Burst: `3/s`<br>Steady: `60/m`  **Scopes:** `flows:read`  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.get_flow_message_action(message_id, async_req=True)
         >>> result = thread.get()
 
         Args:
@@ -2021,15 +2079,15 @@
     def get_flow_message_relationships_action(
         self,
         id,
         **kwargs
     ):
         """Get Flow Message Relationships Action  # noqa: E501
 
-        Get the [relationship](https://developers.klaviyo.com/en/reference/api_overview#relationships) for a flow message's flow action, given the flow ID.<br><br>*Rate limits*:<br>Burst: `3/s`<br>Steady: `60/m`  **Scopes:** `Flows Read`  # noqa: E501
+        Get the [relationship](https://developers.klaviyo.com/en/reference/api_overview#relationships) for a flow message's flow action, given the flow ID.<br><br>*Rate limits*:<br>Burst: `3/s`<br>Steady: `60/m`  **Scopes:** `flows:read`  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.get_flow_message_relationships_action(id, async_req=True)
         >>> result = thread.get()
 
         Args:
@@ -2104,26 +2162,27 @@
     def get_flow_relationships_flow_actions(
         self,
         id,
         **kwargs
     ):
         """Get Flow Relationships Flow Actions  # noqa: E501
 
-        Get all [relationships](https://developers.klaviyo.com/en/reference/api_overview#relationships) for flow actions associated with the given flow ID. Flow action relationships can be sorted by the following fields, in ascending and descending order: `id`,  `status`, `created`, `updated` Use filters to narrow your results. Returns a maximum of 50 flow action relationships per request, which can be paginated with offset pagination. Offset pagination uses the following parameters: `page[size]` and `page[number]`.<br><br>*Rate limits*:<br>Burst: `3/s`<br>Steady: `60/m`  **Scopes:** `Flows Read`  # noqa: E501
+        Get all [relationships](https://developers.klaviyo.com/en/reference/api_overview#relationships) for flow actions associated with the given flow ID. Flow action relationships can be sorted by the following fields, in ascending and descending order: `id`,  `status`, `created`, `updated` Use filters to narrow your results. Returns a maximum of 50 flow action relationships per request, which can be paginated with offset pagination. Offset pagination uses the following parameters: `page[size]` and `page[number]`.<br><br>*Rate limits*:<br>Burst: `3/s`<br>Steady: `60/m`  **Scopes:** `flows:read`  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.get_flow_relationships_flow_actions(id, async_req=True)
         >>> result = thread.get()
 
         Args:
             id (str): 
 
         Keyword Args:
             filter (str): For more information please visit https://developers.klaviyo.com/en/v2023-02-22/reference/api-overview#filtering<br>Allowed field(s)/operator(s):<br>`action_type`: `equals`<br>`status`: `equals`<br>`created`: `equals`, `greater-or-equal`, `greater-than`, `less-or-equal`, `less-than`<br>`updated`: `equals`, `greater-or-equal`, `greater-than`, `less-or-equal`, `less-than`. [optional]
+            page_size (int): Default: 50. Min: 1. Max: 100.. [optional] if omitted the server will use the default value of 50
             sort (str): For more information please visit https://developers.klaviyo.com/en/v2023-02-22/reference/api-overview#sorting. [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
@@ -2189,15 +2248,15 @@
     def get_flow_relationships_tags(
         self,
         id,
         **kwargs
     ):
         """Get Flow Relationships Tags  # noqa: E501
 
-        Return the tag IDs of all tags associated with the given flow.<br><br>*Rate limits*:<br>Burst: `3/s`<br>Steady: `60/m`  **Scopes:** `Flows Read` `Tags Read`  # noqa: E501
+        Return the tag IDs of all tags associated with the given flow.<br><br>*Rate limits*:<br>Burst: `3/s`<br>Steady: `60/m`  **Scopes:** `flows:read` `tags:read`  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.get_flow_relationships_tags(id, async_req=True)
         >>> result = thread.get()
 
         Args:
@@ -2272,15 +2331,15 @@
     def get_flow_tags(
         self,
         flow_id,
         **kwargs
     ):
         """Get Flow Tags  # noqa: E501
 
-        Return all tags associated with the given flow ID.<br><br>*Rate limits*:<br>Burst: `3/s`<br>Steady: `60/m`  **Scopes:** `Flows Read` `Tags Read`  # noqa: E501
+        Return all tags associated with the given flow ID.<br><br>*Rate limits*:<br>Burst: `3/s`<br>Steady: `60/m`  **Scopes:** `flows:read` `tags:read`  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.get_flow_tags(flow_id, async_req=True)
         >>> result = thread.get()
 
         Args:
@@ -2355,28 +2414,29 @@
 
     def get_flows(
         self,
         **kwargs
     ):
         """Get Flows  # noqa: E501
 
-        Get all flows in an account.  Returns a maximum of 50 flows per request, which can be paginated with cursor-based pagination.<br><br>*Rate limits*:<br>Burst: `3/s`<br>Steady: `60/m`  **Scopes:** `Flows Read`  # noqa: E501
+        Get all flows in an account.  Returns a maximum of 50 flows per request, which can be paginated with cursor-based pagination.<br><br>*Rate limits*:<br>Burst: `3/s`<br>Steady: `60/m`  **Scopes:** `flows:read`  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.get_flows(async_req=True)
         >>> result = thread.get()
 
 
         Keyword Args:
             fields_flow_action ([str]): For more information please visit https://developers.klaviyo.com/en/v2023-02-22/reference/api-overview#sparse-fieldsets. [optional]
             fields_flow ([str]): For more information please visit https://developers.klaviyo.com/en/v2023-02-22/reference/api-overview#sparse-fieldsets. [optional]
             filter (str): For more information please visit https://developers.klaviyo.com/en/v2023-02-22/reference/api-overview#filtering<br>Allowed field(s)/operator(s):<br>`id`: `any`<br>`name`: `contains`, `ends-with`, `equals`, `starts-with`<br>`status`: `equals`<br>`archived`: `equals`<br>`created`: `equals`, `greater-or-equal`, `greater-than`, `less-or-equal`, `less-than`<br>`updated`: `equals`, `greater-or-equal`, `greater-than`, `less-or-equal`, `less-than`<br>`trigger_type`: `equals`. [optional]
             include ([str]): For more information please visit https://developers.klaviyo.com/en/v2023-02-22/reference/api-overview#relationships. [optional]
             page_cursor (str): For more information please visit https://developers.klaviyo.com/en/v2023-02-22/reference/api-overview#pagination. [optional]
+            page_size (int): Default: 50. Min: 1. Max: 50.. [optional] if omitted the server will use the default value of 50
             sort (str): For more information please visit https://developers.klaviyo.com/en/v2023-02-22/reference/api-overview#sorting. [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
@@ -2441,15 +2501,15 @@
         self,
         id,
         flow_update_query,
         **kwargs
     ):
         """Update Flow Status  # noqa: E501
 
-        Update the status of a flow with the given flow ID, and all actions in that flow.<br><br>*Rate limits*:<br>Burst: `3/s`<br>Steady: `60/m`  **Scopes:** `Flows Write`  # noqa: E501
+        Update the status of a flow with the given flow ID, and all actions in that flow.<br><br>*Rate limits*:<br>Burst: `3/s`<br>Steady: `60/m`  **Scopes:** `flows:write`  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.update_flow(id, flow_update_query, async_req=True)
         >>> result = thread.get()
 
         Args:
```

### Comparing `klaviyo-api-2.0.1/src/openapi_client/api/lists_api.py` & `klaviyo-api-2.0.2/src/openapi_client/api/lists_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -349,18 +349,24 @@
                 'nullable': [
                 ],
                 'enum': [
                     'additional_fields_profile',
                     'fields_profile',
                 ],
                 'validation': [
+                    'page_size',
                 ]
             },
             root_map={
                 'validations': {
+                    ('page_size',): {
+
+                        'inclusive_maximum': 100,
+                        'inclusive_minimum': 1,
+                    },
                 },
                 'allowed_values': {
                     ('additional_fields_profile',): {
 
                         "PREDICTIVE_ANALYTICS": "predictive_analytics"
                     },
                     ('fields_profile',): {
@@ -762,15 +768,15 @@
     def create_list(
         self,
         list_create_query,
         **kwargs
     ):
         """Create List  # noqa: E501
 
-        Create a new list.<br><br>*Rate limits*:<br>Burst: `10/s`<br>Steady: `150/m`  **Scopes:** `List Write`  # noqa: E501
+        Create a new list.<br><br>*Rate limits*:<br>Burst: `10/s`<br>Steady: `150/m`  **Scopes:** `list:write`  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.create_list(list_create_query, async_req=True)
         >>> result = thread.get()
 
         Args:
@@ -846,15 +852,15 @@
         self,
         id,
         list_members_add_query,
         **kwargs
     ):
         """Add Profile To List  # noqa: E501
 
-        Add a profile to a list with the given list ID. It is recommended that you use the [Subscribe Profiles endpoint](https://developers.klaviyo.com/en/reference/subscribe_profiles) if you're trying to give a profile consent to receive email marketing. This endpoint accepts a maximum of 1000 profiles per call.<br><br>*Rate limits*:<br>Burst: `10/s`<br>Steady: `150/m`  **Scopes:** `List Write` `Profiles Write`  # noqa: E501
+        Add a profile to a list with the given list ID. It is recommended that you use the [Subscribe Profiles endpoint](https://developers.klaviyo.com/en/reference/subscribe_profiles) if you're trying to give a profile consent to receive email marketing. This endpoint accepts a maximum of 1000 profiles per call.<br><br>*Rate limits*:<br>Burst: `10/s`<br>Steady: `150/m`  **Scopes:** `list:write` `profiles:write`  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.create_list_relationships(id, list_members_add_query, async_req=True)
         >>> result = thread.get()
 
         Args:
@@ -932,15 +938,15 @@
     def delete_list(
         self,
         id,
         **kwargs
     ):
         """Delete List  # noqa: E501
 
-        Delete a list with the given list ID.<br><br>*Rate limits*:<br>Burst: `10/s`<br>Steady: `150/m`  **Scopes:** `List Write`  # noqa: E501
+        Delete a list with the given list ID.<br><br>*Rate limits*:<br>Burst: `10/s`<br>Steady: `150/m`  **Scopes:** `list:write`  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.delete_list(id, async_req=True)
         >>> result = thread.get()
 
         Args:
@@ -1016,15 +1022,15 @@
         self,
         id,
         list_members_delete_query,
         **kwargs
     ):
         """Remove Profile From List  # noqa: E501
 
-        Remove a profile from a list with the given list ID. The provided profile will no longer receive marketing from this particular list once removed. Removing a profile from a list will not impact the profile's consent status or subscription status in general. To update a profile's subscription status, please use the [Unsubscribe Profiles endpoint](https://developers.klaviyo.com/en/reference/unsubscribe_profiles). This endpoint accepts a maximum of 1000 profiles per call.<br><br>*Rate limits*:<br>Burst: `10/s`<br>Steady: `150/m`  **Scopes:** `List Write` `Profiles Write`  # noqa: E501
+        Remove a profile from a list with the given list ID. The provided profile will no longer receive marketing from this particular list once removed. Removing a profile from a list will not impact the profile's consent status or subscription status in general. To update a profile's subscription status, please use the [Unsubscribe Profiles endpoint](https://developers.klaviyo.com/en/reference/unsubscribe_profiles). This endpoint accepts a maximum of 1000 profiles per call.<br><br>*Rate limits*:<br>Burst: `10/s`<br>Steady: `150/m`  **Scopes:** `list:write` `profiles:write`  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.delete_list_relationships(id, list_members_delete_query, async_req=True)
         >>> result = thread.get()
 
         Args:
@@ -1102,15 +1108,15 @@
     def get_list(
         self,
         id,
         **kwargs
     ):
         """Get List  # noqa: E501
 
-        Get a list with the given list ID.<br><br>*Rate limits*:<br>Burst: `10/s`<br>Steady: `150/m`  **Scopes:** `List Write`  # noqa: E501
+        Get a list with the given list ID.<br><br>*Rate limits*:<br>Burst: `10/s`<br>Steady: `150/m`  **Scopes:** `list:write`  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.get_list(id, async_req=True)
         >>> result = thread.get()
 
         Args:
@@ -1186,30 +1192,30 @@
     def get_list_profiles(
         self,
         list_id,
         **kwargs
     ):
         """Get List Profiles  # noqa: E501
 
-        Get all profiles within a list with the given list ID. Filter to request a subset of all profiles. Profiles can be filtered by `email`, `phone_number`, and `push_token` fields. You can adjust the number of results per page via the `page[size]` query parameter, e.g. `?page[size]=25`. **Default**: 20. **Max**: 100.<br><br>*Rate limits*:<br>Burst: `10/s`<br>Steady: `150/m`  **Scopes:** `List Read` `Profiles Read`  # noqa: E501
+        Get all profiles within a list with the given list ID. Filter to request a subset of all profiles. Profiles can be filtered by `email`, `phone_number`, and `push_token` fields.<br><br>*Rate limits*:<br>Burst: `10/s`<br>Steady: `150/m`  **Scopes:** `list:read` `profiles:read`  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.get_list_profiles(list_id, async_req=True)
         >>> result = thread.get()
 
         Args:
             list_id (str): Primary key that uniquely identifies this list. Generated by Klaviyo.
 
         Keyword Args:
             additional_fields_profile ([str]): Request additional fields not included by default in the response. Supported values: 'predictive_analytics'. [optional]
             fields_profile ([str]): For more information please visit https://developers.klaviyo.com/en/v2023-02-22/reference/api-overview#sparse-fieldsets. [optional]
             filter (str): For more information please visit https://developers.klaviyo.com/en/v2023-02-22/reference/api-overview#filtering<br>Allowed field(s)/operator(s):<br>`email`: `any`<br>`phone_number`: `any`<br>`push_token`: `any`<br>`_kx`: `equals`. [optional]
             page_cursor (str): For more information please visit https://developers.klaviyo.com/en/v2023-02-22/reference/api-overview#pagination. [optional]
-            page_size (int): The number of results to return per page. Default = 20. Max = 100. [optional]
+            page_size (int): Default: 20. Min: 1. Max: 100.. [optional] if omitted the server will use the default value of 20
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
@@ -1274,15 +1280,15 @@
     def get_list_relationships_profiles(
         self,
         id,
         **kwargs
     ):
         """Get List Relationships Profiles  # noqa: E501
 
-        Get profile membership [relationships](https://developers.klaviyo.com/en/reference/api_overview#relationships) for a list with the given list ID. You can adjust the number of results per page via the `page[size]` query parameter, e.g. `?page[size]=25`. **Default**: 20. **Max**: 100.<br><br>*Rate limits*:<br>Burst: `10/s`<br>Steady: `150/m`  **Scopes:** `List Read` `Profiles Read`  # noqa: E501
+        Get profile membership [relationships](https://developers.klaviyo.com/en/reference/api_overview#relationships) for a list with the given list ID.<br><br>*Rate limits*:<br>Burst: `10/s`<br>Steady: `150/m`  **Scopes:** `list:read` `profiles:read`  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.get_list_relationships_profiles(id, async_req=True)
         >>> result = thread.get()
 
         Args:
@@ -1358,15 +1364,15 @@
     def get_list_relationships_tags(
         self,
         id,
         **kwargs
     ):
         """Get List Relationships Tags  # noqa: E501
 
-        Returns the tag IDs of all tags associated with the given list.<br><br>*Rate limits*:<br>Burst: `3/s`<br>Steady: `60/m`  **Scopes:** `List Read` `Tags Read`  # noqa: E501
+        Returns the tag IDs of all tags associated with the given list.<br><br>*Rate limits*:<br>Burst: `3/s`<br>Steady: `60/m`  **Scopes:** `list:read` `tags:read`  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.get_list_relationships_tags(id, async_req=True)
         >>> result = thread.get()
 
         Args:
@@ -1441,15 +1447,15 @@
     def get_list_tags(
         self,
         list_id,
         **kwargs
     ):
         """Get List Tags  # noqa: E501
 
-        Return all tags associated with the given list ID.<br><br>*Rate limits*:<br>Burst: `3/s`<br>Steady: `60/m`  **Scopes:** `List Read` `Tags Read`  # noqa: E501
+        Return all tags associated with the given list ID.<br><br>*Rate limits*:<br>Burst: `3/s`<br>Steady: `60/m`  **Scopes:** `list:read` `tags:read`  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.get_list_tags(list_id, async_req=True)
         >>> result = thread.get()
 
         Args:
@@ -1524,15 +1530,15 @@
 
     def get_lists(
         self,
         **kwargs
     ):
         """Get Lists  # noqa: E501
 
-        Get all lists in an account. Filter to request a subset of all lists. Lists can be filtered by `id`, `name`, `created`, and `updated` fields. Returns a maximum of 10 results per page.<br><br>*Rate limits*:<br>Burst: `10/s`<br>Steady: `150/m`  **Scopes:** `List Read`  # noqa: E501
+        Get all lists in an account. Filter to request a subset of all lists. Lists can be filtered by `id`, `name`, `created`, and `updated` fields. Returns a maximum of 10 results per page.<br><br>*Rate limits*:<br>Burst: `10/s`<br>Steady: `150/m`  **Scopes:** `list:read`  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.get_lists(async_req=True)
         >>> result = thread.get()
 
 
@@ -1607,15 +1613,15 @@
         self,
         id,
         list_partial_update_query,
         **kwargs
     ):
         """Update List  # noqa: E501
 
-        Update the name of a list with the given list ID.<br><br>*Rate limits*:<br>Burst: `10/s`<br>Steady: `150/m`  **Scopes:** `List Write`  # noqa: E501
+        Update the name of a list with the given list ID.<br><br>*Rate limits*:<br>Burst: `10/s`<br>Steady: `150/m`  **Scopes:** `list:write`  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.update_list(id, list_partial_update_query, async_req=True)
         >>> result = thread.get()
 
         Args:
```

### Comparing `klaviyo-api-2.0.1/src/openapi_client/api/metrics_api.py` & `klaviyo-api-2.0.2/src/openapi_client/api/metrics_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -226,15 +226,15 @@
     def get_metric(
         self,
         id,
         **kwargs
     ):
         """Get Metric  # noqa: E501
 
-        Get a metric with the given metric ID.<br><br>*Rate limits*:<br>Burst: `10/s`<br>Steady: `150/m`  **Scopes:** `Metrics Read`  # noqa: E501
+        Get a metric with the given metric ID.<br><br>*Rate limits*:<br>Burst: `10/s`<br>Steady: `150/m`  **Scopes:** `metrics:read`  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.get_metric(id, async_req=True)
         >>> result = thread.get()
 
         Args:
@@ -309,15 +309,15 @@
 
     def get_metrics(
         self,
         **kwargs
     ):
         """Get Metrics  # noqa: E501
 
-        Get all metrics in an account. Requests can be filtered by the following fields: integration `name`, integration `category` Returns a maximum of 200 results per page.<br><br>*Rate limits*:<br>Burst: `10/s`<br>Steady: `150/m`  **Scopes:** `Metrics Read`  # noqa: E501
+        Get all metrics in an account. Requests can be filtered by the following fields: integration `name`, integration `category` Returns a maximum of 200 results per page.<br><br>*Rate limits*:<br>Burst: `10/s`<br>Steady: `150/m`  **Scopes:** `metrics:read`  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.get_metrics(async_req=True)
         >>> result = thread.get()
 
 
@@ -391,15 +391,15 @@
     def query_metric_aggregates(
         self,
         metric_aggregate_query,
         **kwargs
     ):
         """Query Metric Aggregates  # noqa: E501
 
-        Query and aggregate event data associated with a metric, including native Klaviyo metrics, integration-specific metrics, and custom events. Queries must be passed in the JSON body of your `POST` request.  Results can be filtered and grouped by time, event, or profile dimensions.  **Request body parameters** (nested under `attributes`):  * `return_fields`: request specific fields using [sparse fieldsets](https://developers.klaviyo.com/en/reference/api_overview#sparse-fieldsets) * `sort`: sort results by a specified field, such as `\"-timestamp\"` * `page_cursor`: results can be paginated with [cursor-based pagination](https://developers.klaviyo.com/en/reference/api_overview#pagination) * `page_size`: limit the number of returned results per page * `by`: optional attributes used to group by the aggregation function     * When using `by` attributes, an empty `dimensions` response is expected when the counts for the events do not have the associated dimension requested by the set `by` attribute. For example, a query including `\"by\": [\"$flow\"]` will return an empty dimensions response for counts of metrics not associated with a `$flow` * `measurement`: the measurement key supports the following values:     * `\"sum_value\"`: perform a summation of the `_Event Value_`, optionally partitioned over any dimension provided in the `by` field     * `\"count\"`: counts the number of events associated to a metric, optionally partitioned over any dimension provided in the `by` field     * `\"unique\"` counts the number of unique customers associated to a metric, optionally partitioned over any dimension provided in the `by` field * `interval`: aggregation interval, such as `\"hour\"`,`\"day\"`,`\"week\"`, and `\"month\"` * `metric_id`: the metric ID used in the aggregation * `filter`: list of filters for specific fields, must include time range using ISO 8601 format (`\"YYYY-MM-DDTHH:MM:SS.mmmmmm\"`)     * The time range can be filtered by providing a `greater-or-equal` filter on the datetime field, such as `\"greater-or-equal(datetime,2021-07-01T00:00:00)\"` and a `less-than` filter on the same datetime field, such as `\"less-than(datetime,2022-07-01T00:00:00)\"`     * The time range may span a maximum of one year. Time range dates may be set to a maximum of 5 years prior to the current date     * Filter the list of supported aggregate dimensions using the common filter syntax, such as `\"equals(URL,\\\"https://www.klaviyo.com/\\\")\"` * `timezone`: the timezone used when processing the query. Case sensitive. This field is validated against a list of common timezones from the [IANA Time Zone Database](https://www.iana.org/time-zones)     * While the payload accepts a timezone, the response datetimes returned will be in UTC.  For a comprehensive list of native Klaviyo metrics and their associated attributes for grouping and filtering, please refer to the [metrics attributes guide](https://developers.klaviyo.com/en/docs/supported_metrics_and_attributes).<br><br>*Rate limits*:<br>Burst: `3/s`<br>Steady: `60/m`  **Scopes:** `Metrics Read`  # noqa: E501
+        Query and aggregate event data associated with a metric, including native Klaviyo metrics, integration-specific metrics, and custom events. Queries must be passed in the JSON body of your `POST` request.  Results can be filtered and grouped by time, event, or profile dimensions.  To learn more about how to use this endpoint, check out our new [Using the Query Metric Aggregates Endpoint guide](https://developers.klaviyo.com/en/docs/using-the-query-metric-aggregates-endpoint).  **Request body parameters** (nested under `attributes`):  * `return_fields`: request specific fields using [sparse fieldsets](https://developers.klaviyo.com/en/reference/api_overview#sparse-fieldsets) * `sort`: sort results by a specified field, such as `\"-timestamp\"` * `page_cursor`: results can be paginated with [cursor-based pagination](https://developers.klaviyo.com/en/reference/api_overview#pagination) * `page_size`: limit the number of returned results per page * `by`: optional attributes used to group by the aggregation function     * When using `by` attributes, an empty `dimensions` response is expected when the counts for the events do not have the associated dimension requested by the set `by` attribute. For example, a query including `\"by\": [\"$flow\"]` will return an empty dimensions response for counts of metrics not associated with a `$flow` * `measurement`: the measurement key supports the following values:     * `\"sum_value\"`: perform a summation of the `_Event Value_`, optionally partitioned over any dimension provided in the `by` field     * `\"count\"`: counts the number of events associated to a metric, optionally partitioned over any dimension provided in the `by` field     * `\"unique\"` counts the number of unique customers associated to a metric, optionally partitioned over any dimension provided in the `by` field * `interval`: aggregation interval, such as `\"hour\"`,`\"day\"`,`\"week\"`, and `\"month\"` * `metric_id`: the metric ID used in the aggregation * `filter`: list of filters for specific fields, must include time range using ISO 8601 format (`\"YYYY-MM-DDTHH:MM:SS.mmmmmm\"`)     * The time range can be filtered by providing a `greater-or-equal` filter on the datetime field, such as `\"greater-or-equal(datetime,2021-07-01T00:00:00)\"` and a `less-than` filter on the same datetime field, such as `\"less-than(datetime,2022-07-01T00:00:00)\"`     * The time range may span a maximum of one year. Time range dates may be set to a maximum of 5 years prior to the current date     * Filter the list of supported aggregate dimensions using the common filter syntax, such as `\"equals(URL,\\\"https://www.klaviyo.com/\\\")\"` * `timezone`: the timezone used when processing the query. Case sensitive. This field is validated against a list of common timezones from the [IANA Time Zone Database](https://www.iana.org/time-zones)     * While the payload accepts a timezone, the response datetimes returned will be in UTC.  For a comprehensive list of native Klaviyo metrics and their associated attributes for grouping and filtering, please refer to the [metrics attributes guide](https://developers.klaviyo.com/en/docs/supported_metrics_and_attributes).<br><br>*Rate limits*:<br>Burst: `3/s`<br>Steady: `60/m`  **Scopes:** `metrics:read`  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.query_metric_aggregates(metric_aggregate_query, async_req=True)
         >>> result = thread.get()
 
         Args:
```

### Comparing `klaviyo-api-2.0.1/src/openapi_client/api/profiles_api.py` & `klaviyo-api-2.0.2/src/openapi_client/api/profiles_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,51 +52,40 @@
                 'operation_id': 'create_profile',
                 'http_method': 'POST',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'profile_create_query',
-                    'additional_fields_profile',
                 ],
                 'required': [
                     'profile_create_query',
                 ],
                 'nullable': [
                 ],
                 'enum': [
-                    'additional_fields_profile',
                 ],
                 'validation': [
                 ]
             },
             root_map={
                 'validations': {
                 },
                 'allowed_values': {
-                    ('additional_fields_profile',): {
-
-                        "PREDICTIVE_ANALYTICS": "predictive_analytics"
-                    },
                 },
                 'openapi_types': {
                     'profile_create_query':
                         (ProfileCreateQuery,),
-                    'additional_fields_profile':
-                        ([str],),
                 },
                 'attribute_map': {
-                    'additional_fields_profile': 'additional-fields[profile]',
                 },
                 'location_map': {
                     'profile_create_query': 'body',
-                    'additional_fields_profile': 'query',
                 },
                 'collection_format_map': {
-                    'additional_fields_profile': 'csv',
                 }
             },
             headers_map={
                 'accept': [
                     'application/json'
                 ],
                 'content_type': [
@@ -512,30 +501,36 @@
             },
             params_map={
                 'all': [
                     'additional_fields_profile',
                     'fields_profile',
                     'filter',
                     'page_cursor',
-                    'sort',
                     'page_size',
+                    'sort',
                 ],
                 'required': [],
                 'nullable': [
                 ],
                 'enum': [
                     'additional_fields_profile',
                     'fields_profile',
                     'sort',
                 ],
                 'validation': [
+                    'page_size',
                 ]
             },
             root_map={
                 'validations': {
+                    ('page_size',): {
+
+                        'inclusive_maximum': 100,
+                        'inclusive_minimum': 1,
+                    },
                 },
                 'allowed_values': {
                     ('additional_fields_profile',): {
 
                         "PREDICTIVE_ANALYTICS": "predictive_analytics"
                     },
                     ('fields_profile',): {
@@ -612,34 +607,34 @@
                         ([str],),
                     'fields_profile':
                         ([str],),
                     'filter':
                         (str,),
                     'page_cursor':
                         (str,),
-                    'sort':
-                        (str,),
                     'page_size':
                         (int,),
+                    'sort':
+                        (str,),
                 },
                 'attribute_map': {
                     'additional_fields_profile': 'additional-fields[profile]',
                     'fields_profile': 'fields[profile]',
                     'filter': 'filter',
                     'page_cursor': 'page[cursor]',
-                    'sort': 'sort',
                     'page_size': 'page[size]',
+                    'sort': 'sort',
                 },
                 'location_map': {
                     'additional_fields_profile': 'query',
                     'fields_profile': 'query',
                     'filter': 'query',
                     'page_cursor': 'query',
-                    'sort': 'query',
                     'page_size': 'query',
+                    'sort': 'query',
                 },
                 'collection_format_map': {
                     'additional_fields_profile': 'csv',
                     'fields_profile': 'csv',
                 }
             },
             headers_map={
@@ -869,56 +864,45 @@
                 'http_method': 'PATCH',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'id',
                     'profile_partial_update_query',
-                    'additional_fields_profile',
                 ],
                 'required': [
                     'id',
                     'profile_partial_update_query',
                 ],
                 'nullable': [
                 ],
                 'enum': [
-                    'additional_fields_profile',
                 ],
                 'validation': [
                 ]
             },
             root_map={
                 'validations': {
                 },
                 'allowed_values': {
-                    ('additional_fields_profile',): {
-
-                        "PREDICTIVE_ANALYTICS": "predictive_analytics"
-                    },
                 },
                 'openapi_types': {
                     'id':
                         (str,),
                     'profile_partial_update_query':
                         (ProfilePartialUpdateQuery,),
-                    'additional_fields_profile':
-                        ([str],),
                 },
                 'attribute_map': {
                     'id': 'id',
-                    'additional_fields_profile': 'additional-fields[profile]',
                 },
                 'location_map': {
                     'id': 'path',
                     'profile_partial_update_query': 'body',
-                    'additional_fields_profile': 'query',
                 },
                 'collection_format_map': {
-                    'additional_fields_profile': 'csv',
                 }
             },
             headers_map={
                 'accept': [
                     'application/json'
                 ],
                 'content_type': [
@@ -931,26 +915,25 @@
     def create_profile(
         self,
         profile_create_query,
         **kwargs
     ):
         """Create Profile  # noqa: E501
 
-        Create a new profile. If you use a phone number as the profile identifier and SMS is not set up in the Klaviyo account, you'll need to include at least one other identifier attribute (`email` or `external_id`) in addition to the `phone_number` attribute for the API call to work.<br><br>*Rate limits*:<br>Burst: `75/s`<br>Steady: `700/m`  **Scopes:** `Profiles Write`  # noqa: E501
+        Create a new profile. If you use a phone number as the profile identifier and SMS is not set up in the Klaviyo account, you'll need to include at least one other identifier attribute (`email` or `external_id`) in addition to the `phone_number` attribute for the API call to work.<br><br>*Rate limits*:<br>Burst: `75/s`<br>Steady: `700/m`  **Scopes:** `profiles:write`  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.create_profile(profile_create_query, async_req=True)
         >>> result = thread.get()
 
         Args:
             profile_create_query (ProfileCreateQuery):
 
         Keyword Args:
-            additional_fields_profile ([str]): Request additional fields not included by default in the response. Supported values: 'predictive_analytics'. [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
@@ -1015,15 +998,15 @@
     def get_profile(
         self,
         id,
         **kwargs
     ):
         """Get Profile  # noqa: E501
 
-        Get the profile with the given profile ID. Include parameters can be provided to get the following related resource data: `lists` memberships, `segments` memberships\"<br><br>*Rate limits*:<br>Burst: `75/s`<br>Steady: `700/m`  **Scopes:** `Profiles Read`  # noqa: E501
+        Get the profile with the given profile ID. Include parameters can be provided to get the following related resource data: `lists` memberships, `segments` memberships\"<br><br>*Rate limits*:<br>Burst: `75/s`<br>Steady: `700/m`  **Scopes:** `profiles:read`  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.get_profile(id, async_req=True)
         >>> result = thread.get()
 
         Args:
@@ -1103,15 +1086,15 @@
     def get_profile_lists(
         self,
         profile_id,
         **kwargs
     ):
         """Get Profile Lists  # noqa: E501
 
-        Get list memberships for a profile with the given profile ID.<br><br>*Rate limits*:<br>Burst: `3/s`<br>Steady: `60/m`  **Scopes:** `List Read` `Profiles Read`  # noqa: E501
+        Get list memberships for a profile with the given profile ID.<br><br>*Rate limits*:<br>Burst: `3/s`<br>Steady: `60/m`  **Scopes:** `list:read` `profiles:read`  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.get_profile_lists(profile_id, async_req=True)
         >>> result = thread.get()
 
         Args:
@@ -1187,15 +1170,15 @@
     def get_profile_relationships_lists(
         self,
         id,
         **kwargs
     ):
         """Get Profile Relationships Lists  # noqa: E501
 
-        Get list memberships for a profile with the given profile ID.<br><br>*Rate limits*:<br>Burst: `3/s`<br>Steady: `60/m`  **Scopes:** `List Read` `Profiles Read`  # noqa: E501
+        Get list memberships for a profile with the given profile ID.<br><br>*Rate limits*:<br>Burst: `3/s`<br>Steady: `60/m`  **Scopes:** `list:read` `profiles:read`  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.get_profile_relationships_lists(id, async_req=True)
         >>> result = thread.get()
 
         Args:
@@ -1270,15 +1253,15 @@
     def get_profile_relationships_segments(
         self,
         id,
         **kwargs
     ):
         """Get Profile Relationships Segments  # noqa: E501
 
-        Get segment membership relationships for a profile with the given profile ID.<br><br>*Rate limits*:<br>Burst: `3/s`<br>Steady: `60/m`  **Scopes:** `Profiles Read` `Segments Read`  # noqa: E501
+        Get segment membership relationships for a profile with the given profile ID.<br><br>*Rate limits*:<br>Burst: `3/s`<br>Steady: `60/m`  **Scopes:** `profiles:read` `segments:read`  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.get_profile_relationships_segments(id, async_req=True)
         >>> result = thread.get()
 
         Args:
@@ -1353,15 +1336,15 @@
     def get_profile_segments(
         self,
         profile_id,
         **kwargs
     ):
         """Get Profile Segments  # noqa: E501
 
-        Get segment memberships for a profile with the given profile ID.<br><br>*Rate limits*:<br>Burst: `3/s`<br>Steady: `60/m`  **Scopes:** `Profiles Read` `Segments Read`  # noqa: E501
+        Get segment memberships for a profile with the given profile ID.<br><br>*Rate limits*:<br>Burst: `3/s`<br>Steady: `60/m`  **Scopes:** `profiles:read` `segments:read`  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.get_profile_segments(profile_id, async_req=True)
         >>> result = thread.get()
 
         Args:
@@ -1436,29 +1419,29 @@
 
     def get_profiles(
         self,
         **kwargs
     ):
         """Get Profiles  # noqa: E501
 
-        Get all profiles in an account. Profiles can be sorted by the following fields in ascending and descending order: `id`, `created`, `updated`, `email` You can adjust the number of results per page via the `page[size]` query parameter, e.g. `?page[size]=25`. **Default**: 20. **Max**: 100.<br><br>*Rate limits*:<br>Burst: `10/s`<br>Steady: `150/m`  **Scopes:** `Profiles Read`  # noqa: E501
+        Get all profiles in an account. Profiles can be sorted by the following fields in ascending and descending order: `id`, `created`, `updated`, `email`<br><br>*Rate limits*:<br>Burst: `10/s`<br>Steady: `150/m`  **Scopes:** `profiles:read`  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.get_profiles(async_req=True)
         >>> result = thread.get()
 
 
         Keyword Args:
             additional_fields_profile ([str]): Request additional fields not included by default in the response. Supported values: 'predictive_analytics'. [optional]
             fields_profile ([str]): For more information please visit https://developers.klaviyo.com/en/v2023-02-22/reference/api-overview#sparse-fieldsets. [optional]
             filter (str): For more information please visit https://developers.klaviyo.com/en/v2023-02-22/reference/api-overview#filtering<br>Allowed field(s)/operator(s):<br>`id`: `any`, `equals`<br>`email`: `any`, `equals`<br>`phone_number`: `any`, `equals`<br>`external_id`: `any`, `equals`<br>`_kx`: `equals`<br>`created`: `greater-than`, `less-than`<br>`updated`: `greater-than`, `less-than`. [optional]
             page_cursor (str): For more information please visit https://developers.klaviyo.com/en/v2023-02-22/reference/api-overview#pagination. [optional]
+            page_size (int): Default: 20. Min: 1. Max: 100.. [optional] if omitted the server will use the default value of 20
             sort (str): For more information please visit https://developers.klaviyo.com/en/v2023-02-22/reference/api-overview#sorting. [optional]
-            page_size (int): The number of results to return per page. Default = 20. Max = 100. [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
@@ -1521,15 +1504,15 @@
     def subscribe_profiles(
         self,
         subscription_create_job_create_query,
         **kwargs
     ):
         """Subscribe Profiles  # noqa: E501
 
-        Subscribe one or more profiles to email marketing, SMS marketing, or both. If the list has double opt-in enabled, profiles will receive a message requiring their confirmation before subscribing. Otherwise, profiles will be immediately subscribed without receiving a confirmation message. To add someone to a list without changing their subscription status, use [Add Profile to List](https://developers.klaviyo.com/en/reference/create_list_relationships). This API will remove any `UNSUBSCRIBE`, `SPAM_REPORT` or `USER_SUPPRESSED` suppressions from the provided profiles. Learn more about suppressed profiles in [this document](https://help.klaviyo.com/hc/en-us/articles/115005246108-Understanding-suppressed-email-profiles#what-is-a-suppressed-profile-1). Maximum number of profile can be submitted for subscription: 100<br><br>*Rate limits*:<br>Burst: `75/s`<br>Steady: `700/m`  **Scopes:** `List Write` `Profiles Write` `Subscriptions Write`  # noqa: E501
+        Subscribe one or more profiles to email marketing, SMS marketing, or both. If the list has double opt-in enabled, profiles will receive a message requiring their confirmation before subscribing. Otherwise, profiles will be immediately subscribed without receiving a confirmation message. To add someone to a list without changing their subscription status, use [Add Profile to List](https://developers.klaviyo.com/en/reference/create_list_relationships). This API will remove any `UNSUBSCRIBE`, `SPAM_REPORT` or `USER_SUPPRESSED` suppressions from the provided profiles. Learn more about suppressed profiles in [this document](https://help.klaviyo.com/hc/en-us/articles/115005246108-Understanding-suppressed-email-profiles#what-is-a-suppressed-profile-1). Maximum number of profile can be submitted for subscription: 100<br><br>*Rate limits*:<br>Burst: `75/s`<br>Steady: `700/m`  **Scopes:** `list:write` `profiles:write` `subscriptions:write`  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.subscribe_profiles(subscription_create_job_create_query, async_req=True)
         >>> result = thread.get()
 
         Args:
@@ -1604,15 +1587,15 @@
     def suppress_profiles(
         self,
         suppression_create_job_create_query,
         **kwargs
     ):
         """Suppress Profiles  # noqa: E501
 
-        Manually suppress one or more profiles. Such profiles will have `USER_SUPPRESSED` as their suppression reason. Manually suppressed profiles _will not_ receive email marketing. Learn more about suppressed profiles [in this document](https://help.klaviyo.com/hc/en-us/articles/115005246108-Understanding-suppressed-email-profiles#what-is-a-suppressed-profile-1). Not supported for SMS marketing. Maximum number of profile can be submitted for suppression: 100<br><br>*Rate limits*:<br>Burst: `75/s`<br>Steady: `700/m`  **Scopes:** `Profiles Write` `Subscriptions Write`  # noqa: E501
+        Manually suppress one or more profiles. Such profiles will have `USER_SUPPRESSED` as their suppression reason. Manually suppressed profiles _will not_ receive email marketing. Learn more about suppressed profiles [in this document](https://help.klaviyo.com/hc/en-us/articles/115005246108-Understanding-suppressed-email-profiles#what-is-a-suppressed-profile-1). Not supported for SMS marketing. Maximum number of profile can be submitted for suppression: 100<br><br>*Rate limits*:<br>Burst: `75/s`<br>Steady: `700/m`  **Scopes:** `profiles:write` `subscriptions:write`  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.suppress_profiles(suppression_create_job_create_query, async_req=True)
         >>> result = thread.get()
 
         Args:
@@ -1687,15 +1670,15 @@
     def unsubscribe_profiles(
         self,
         unsubscription_create_job_create_query,
         **kwargs
     ):
         """Unsubscribe Profiles  # noqa: E501
 
-        Unsubscribe one or more profiles to email marketing, SMS marketing, or both. To remove someone from a list without changing their subscription status, use [Remove Profile from List](https://developers.klaviyo.com/en/reference/delete_list_relationships). Maximum number of profile can be submitted for unsubscription: 100<br><br>*Rate limits*:<br>Burst: `75/s`<br>Steady: `700/m`  **Scopes:** `List Write` `Profiles Write` `Subscriptions Write`  # noqa: E501
+        Unsubscribe one or more profiles to email marketing, SMS marketing, or both. To remove someone from a list without changing their subscription status, use [Remove Profile from List](https://developers.klaviyo.com/en/reference/delete_list_relationships). Maximum number of profile can be submitted for unsubscription: 100<br><br>*Rate limits*:<br>Burst: `75/s`<br>Steady: `700/m`  **Scopes:** `list:write` `profiles:write` `subscriptions:write`  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.unsubscribe_profiles(unsubscription_create_job_create_query, async_req=True)
         >>> result = thread.get()
 
         Args:
@@ -1770,15 +1753,15 @@
     def unsuppress_profiles(
         self,
         unsuppression_create_job_create_query,
         **kwargs
     ):
         """Unsuppress Profiles  # noqa: E501
 
-        Unsuppress one or more profiles, this will remove any Manual Suppressions (USER_SUPPRESSED) on these profiles. A profile may receive email marketing after a manual suppression is removed so long as they have not revoked consent, i.e. unsubscribed. Not supported for SMS marketing. Only manual suppressions (USER_SUPPRESSED) will be removed. `UNSUBSCRIBE` and `SPAM_REPORT` suppressions are removed whenever a [profile resubscribes](https://developers.klaviyo.com/en/reference/subscribe_profiles). `INVALID_EMAIL` and `HARD_BOUNCE` suppressions cannot be removed by the API. Maximum number of profile can be submitted for unsuppression: 100<br><br>*Rate limits*:<br>Burst: `75/s`<br>Steady: `700/m`  **Scopes:** `Subscriptions Write`  # noqa: E501
+        Unsuppress one or more profiles, this will remove any Manual Suppressions (USER_SUPPRESSED) on these profiles. A profile may receive email marketing after a manual suppression is removed so long as they have not revoked consent, i.e. unsubscribed. Not supported for SMS marketing. Only manual suppressions (USER_SUPPRESSED) will be removed. `UNSUBSCRIBE` and `SPAM_REPORT` suppressions are removed whenever a [profile resubscribes](https://developers.klaviyo.com/en/reference/subscribe_profiles). `INVALID_EMAIL` and `HARD_BOUNCE` suppressions cannot be removed by the API. Maximum number of profile can be submitted for unsuppression: 100<br><br>*Rate limits*:<br>Burst: `75/s`<br>Steady: `700/m`  **Scopes:** `subscriptions:write`  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.unsuppress_profiles(unsuppression_create_job_create_query, async_req=True)
         >>> result = thread.get()
 
         Args:
@@ -1854,27 +1837,26 @@
         self,
         id,
         profile_partial_update_query,
         **kwargs
     ):
         """Update Profile  # noqa: E501
 
-        Update the profile with the given profile ID. If you use a phone number as the profile identifier and SMS is not set up in the Klaviyo account, you'll need to include at least one other identifier attribute (`email` or `external_id`) in addition to the `phone_number` attribute for the API call to work.<br><br>*Rate limits*:<br>Burst: `75/s`<br>Steady: `700/m`  **Scopes:** `Profiles Write`  # noqa: E501
+        Update the profile with the given profile ID. If you use a phone number as the profile identifier and SMS is not set up in the Klaviyo account, you'll need to include at least one other identifier attribute (`email` or `external_id`) in addition to the `phone_number` attribute for the API call to work.<br><br>*Rate limits*:<br>Burst: `75/s`<br>Steady: `700/m`  **Scopes:** `profiles:write`  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.update_profile(id, profile_partial_update_query, async_req=True)
         >>> result = thread.get()
 
         Args:
             id (str): Primary key that uniquely identifies this profile. Generated by Klaviyo.
             profile_partial_update_query (ProfilePartialUpdateQuery):
 
         Keyword Args:
-            additional_fields_profile ([str]): Request additional fields not included by default in the response. Supported values: 'predictive_analytics'. [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
```

### Comparing `klaviyo-api-2.0.1/src/openapi_client/api/segments_api.py` & `klaviyo-api-2.0.2/src/openapi_client/api/segments_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -127,18 +127,24 @@
                 'nullable': [
                 ],
                 'enum': [
                     'additional_fields_profile',
                     'fields_profile',
                 ],
                 'validation': [
+                    'page_size',
                 ]
             },
             root_map={
                 'validations': {
+                    ('page_size',): {
+
+                        'inclusive_maximum': 100,
+                        'inclusive_minimum': 1,
+                    },
                 },
                 'allowed_values': {
                     ('additional_fields_profile',): {
 
                         "PREDICTIVE_ANALYTICS": "predictive_analytics"
                     },
                     ('fields_profile',): {
@@ -540,15 +546,15 @@
     def get_segment(
         self,
         id,
         **kwargs
     ):
         """Get Segment  # noqa: E501
 
-        Get a segment with the given segment ID.<br><br>*Rate limits*:<br>Burst: `10/s`<br>Steady: `150/m`  **Scopes:** `Segments Read`  # noqa: E501
+        Get a segment with the given segment ID.<br><br>*Rate limits*:<br>Burst: `10/s`<br>Steady: `150/m`  **Scopes:** `segments:read`  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.get_segment(id, async_req=True)
         >>> result = thread.get()
 
         Args:
@@ -624,30 +630,30 @@
     def get_segment_profiles(
         self,
         segment_id,
         **kwargs
     ):
         """Get Segment Profiles  # noqa: E501
 
-        Get all profiles within the given segment ID. Filter to request a subset of all profiles. Profiles can be filtered by `email`, `phone_number`, and `push_token` fields. You can adjust the number of results per page via the `page[size]` query parameter, e.g. `?page[size]=25`. **Default**: 20. **Max**: 100.<br><br>*Rate limits*:<br>Burst: `10/s`<br>Steady: `150/m`  **Scopes:** `Profiles Read` `Segments Read`  # noqa: E501
+        Get all profiles within the given segment ID. Filter to request a subset of all profiles. Profiles can be filtered by `email`, `phone_number`, and `push_token` fields.<br><br>*Rate limits*:<br>Burst: `10/s`<br>Steady: `150/m`  **Scopes:** `profiles:read` `segments:read`  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.get_segment_profiles(segment_id, async_req=True)
         >>> result = thread.get()
 
         Args:
             segment_id (str): 
 
         Keyword Args:
             additional_fields_profile ([str]): Request additional fields not included by default in the response. Supported values: 'predictive_analytics'. [optional]
             fields_profile ([str]): For more information please visit https://developers.klaviyo.com/en/v2023-02-22/reference/api-overview#sparse-fieldsets. [optional]
             filter (str): For more information please visit https://developers.klaviyo.com/en/v2023-02-22/reference/api-overview#filtering<br>Allowed field(s)/operator(s):<br>`email`: `any`<br>`phone_number`: `any`<br>`push_token`: `any`<br>`_kx`: `equals`. [optional]
             page_cursor (str): For more information please visit https://developers.klaviyo.com/en/v2023-02-22/reference/api-overview#pagination. [optional]
-            page_size (int): The number of results to return per page. Default = 20. Max = 100. [optional]
+            page_size (int): Default: 20. Min: 1. Max: 100.. [optional] if omitted the server will use the default value of 20
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
@@ -712,15 +718,15 @@
     def get_segment_relationships_profiles(
         self,
         id,
         **kwargs
     ):
         """Get Segment Relationships Profiles  # noqa: E501
 
-        Get all profile membership [relationships](https://developers.klaviyo.com/en/reference/api_overview#relationships) for the given segment ID. You can adjust the number of results per page via the `page[size]` query parameter, e.g. `?page[size]=25`. **Default**: 20. **Max**: 100.<br><br>*Rate limits*:<br>Burst: `10/s`<br>Steady: `150/m`  **Scopes:** `Profiles Read` `Segments Read`  # noqa: E501
+        Get all profile membership [relationships](https://developers.klaviyo.com/en/reference/api_overview#relationships) for the given segment ID.<br><br>*Rate limits*:<br>Burst: `10/s`<br>Steady: `150/m`  **Scopes:** `profiles:read` `segments:read`  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.get_segment_relationships_profiles(id, async_req=True)
         >>> result = thread.get()
 
         Args:
@@ -796,15 +802,15 @@
     def get_segment_relationships_tags(
         self,
         id,
         **kwargs
     ):
         """Get Segment Relationships Tags  # noqa: E501
 
-        If `related_resource` is `tags`, returns the tag IDs of all tags associated with the given segment ID.<br><br>*Rate limits*:<br>Burst: `3/s`<br>Steady: `60/m`  **Scopes:** `Segments Read` `Tags Read`  # noqa: E501
+        If `related_resource` is `tags`, returns the tag IDs of all tags associated with the given segment ID.<br><br>*Rate limits*:<br>Burst: `3/s`<br>Steady: `60/m`  **Scopes:** `segments:read` `tags:read`  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.get_segment_relationships_tags(id, async_req=True)
         >>> result = thread.get()
 
         Args:
@@ -879,15 +885,15 @@
     def get_segment_tags(
         self,
         segment_id,
         **kwargs
     ):
         """Get Segment Tags  # noqa: E501
 
-        Return all tags associated with the given segment ID.<br><br>*Rate limits*:<br>Burst: `3/s`<br>Steady: `60/m`  **Scopes:** `Segments Read` `Tags Read`  # noqa: E501
+        Return all tags associated with the given segment ID.<br><br>*Rate limits*:<br>Burst: `3/s`<br>Steady: `60/m`  **Scopes:** `segments:read` `tags:read`  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.get_segment_tags(segment_id, async_req=True)
         >>> result = thread.get()
 
         Args:
@@ -962,15 +968,15 @@
 
     def get_segments(
         self,
         **kwargs
     ):
         """Get Segments  # noqa: E501
 
-        Get all segments in an account. Filter to request a subset of all segments. Segments can be filtered by `name`, `created`, and `updated` fields. Returns a maximum of 10 results per page.<br><br>*Rate limits*:<br>Burst: `10/s`<br>Steady: `150/m`  **Scopes:** `Segments Read`  # noqa: E501
+        Get all segments in an account. Filter to request a subset of all segments. Segments can be filtered by `name`, `created`, and `updated` fields. Returns a maximum of 10 results per page.<br><br>*Rate limits*:<br>Burst: `10/s`<br>Steady: `150/m`  **Scopes:** `segments:read`  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.get_segments(async_req=True)
         >>> result = thread.get()
 
 
@@ -1045,15 +1051,15 @@
         self,
         id,
         segment_partial_update_query,
         **kwargs
     ):
         """Update Segment  # noqa: E501
 
-        Update the name of a segment with the given segment ID.<br><br>*Rate limits*:<br>Burst: `10/s`<br>Steady: `150/m`  **Scopes:** `Segments Write`  # noqa: E501
+        Update the name of a segment with the given segment ID.<br><br>*Rate limits*:<br>Burst: `10/s`<br>Steady: `150/m`  **Scopes:** `segments:write`  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.update_segment(id, segment_partial_update_query, async_req=True)
         >>> result = thread.get()
 
         Args:
```

### Comparing `klaviyo-api-2.0.1/src/openapi_client/api/tags_api.py` & `klaviyo-api-2.0.2/src/openapi_client/api/tags_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1550,15 +1550,15 @@
     def create_tag(
         self,
         tag_create_query,
         **kwargs
     ):
         """Create Tag  # noqa: E501
 
-        Create a tag. An account cannot have more than **500** unique tags. A tag belongs to a single tag group. If the `tag_group_id` is not specified, the tag is added to the account's default tag group.<br><br>*Rate limits*:<br>Burst: `3/s`<br>Steady: `60/m`  **Scopes:** `Tags Read` `Tags Write`  # noqa: E501
+        Create a tag. An account cannot have more than **500** unique tags. A tag belongs to a single tag group. If the `tag_group_id` is not specified, the tag is added to the account's default tag group.<br><br>*Rate limits*:<br>Burst: `3/s`<br>Steady: `60/m`  **Scopes:** `tags:read` `tags:write`  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.create_tag(tag_create_query, async_req=True)
         >>> result = thread.get()
 
         Args:
@@ -1633,15 +1633,15 @@
     def create_tag_group(
         self,
         tag_group_create_query,
         **kwargs
     ):
         """Create Tag Group  # noqa: E501
 
-        Create a tag group. An account cannot have more than **50** unique tag groups. If `exclusive` is not specified `true` or `false`, the tag group defaults to non-exclusive. If a tag group is non-exclusive, any given related resource (campaign, flow, etc.) can be linked to multiple tags from that tag group. If a tag group is exclusive, any given related resource can only be linked to one tag from that tag group.<br><br>*Rate limits*:<br>Burst: `3/s`<br>Steady: `60/m`  **Scopes:** `Tags Read` `Tags Write`  # noqa: E501
+        Create a tag group. An account cannot have more than **50** unique tag groups. If `exclusive` is not specified `true` or `false`, the tag group defaults to non-exclusive. If a tag group is non-exclusive, any given related resource (campaign, flow, etc.) can be linked to multiple tags from that tag group. If a tag group is exclusive, any given related resource can only be linked to one tag from that tag group.<br><br>*Rate limits*:<br>Burst: `3/s`<br>Steady: `60/m`  **Scopes:** `tags:read` `tags:write`  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.create_tag_group(tag_group_create_query, async_req=True)
         >>> result = thread.get()
 
         Args:
@@ -1717,15 +1717,15 @@
         self,
         id,
         tag_campaign_op,
         **kwargs
     ):
         """Create Tag Relationships Campaigns  # noqa: E501
 
-        Associate a tag with one or more campaigns. Any campaign cannot be associated with more than **100** tags.  Use the request body to pass in the ID(s) of the campaign(s) that will be associated with the tag.<br><br>*Rate limits*:<br>Burst: `3/s`<br>Steady: `60/m`  **Scopes:** `Campaigns Write` `Tags Write`  # noqa: E501
+        Associate a tag with one or more campaigns. Any campaign cannot be associated with more than **100** tags.  Use the request body to pass in the ID(s) of the campaign(s) that will be associated with the tag.<br><br>*Rate limits*:<br>Burst: `3/s`<br>Steady: `60/m`  **Scopes:** `campaigns:write` `tags:write`  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.create_tag_relationships_campaigns(id, tag_campaign_op, async_req=True)
         >>> result = thread.get()
 
         Args:
@@ -1804,15 +1804,15 @@
         self,
         id,
         tag_flow_op,
         **kwargs
     ):
         """Create Tag Relationships Flows  # noqa: E501
 
-        Associate a tag with one or more flows. Any flow cannot be associated with more than **100** tags.  Use the request body to pass in the ID(s) of the flow(s) that will be associated with the tag.<br><br>*Rate limits*:<br>Burst: `3/s`<br>Steady: `60/m`  **Scopes:** `Flows Write` `Tags Write`  # noqa: E501
+        Associate a tag with one or more flows. Any flow cannot be associated with more than **100** tags.  Use the request body to pass in the ID(s) of the flow(s) that will be associated with the tag.<br><br>*Rate limits*:<br>Burst: `3/s`<br>Steady: `60/m`  **Scopes:** `flows:write` `tags:write`  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.create_tag_relationships_flows(id, tag_flow_op, async_req=True)
         >>> result = thread.get()
 
         Args:
@@ -1891,15 +1891,15 @@
         self,
         id,
         tag_list_op,
         **kwargs
     ):
         """Create Tag Relationships Lists  # noqa: E501
 
-        Associate a tag with one or more lists. Any list cannot be associated with more than **100** tags.  Use the request body to pass in the ID(s) of the lists(s) that will be associated with the tag.<br><br>*Rate limits*:<br>Burst: `3/s`<br>Steady: `60/m`  **Scopes:** `List Write` `Tags Write`  # noqa: E501
+        Associate a tag with one or more lists. Any list cannot be associated with more than **100** tags.  Use the request body to pass in the ID(s) of the lists(s) that will be associated with the tag.<br><br>*Rate limits*:<br>Burst: `3/s`<br>Steady: `60/m`  **Scopes:** `list:write` `tags:write`  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.create_tag_relationships_lists(id, tag_list_op, async_req=True)
         >>> result = thread.get()
 
         Args:
@@ -1978,15 +1978,15 @@
         self,
         id,
         tag_segment_op,
         **kwargs
     ):
         """Create Tag Relationships Segments  # noqa: E501
 
-        Associate a tag with one or more segments. Any segment cannot be associated with more than **100** tags.  Use the request body to pass in the ID(s) of the segments(s) that will be associated with the tag.<br><br>*Rate limits*:<br>Burst: `3/s`<br>Steady: `60/m`  **Scopes:** `Segments Write` `Tags Write`  # noqa: E501
+        Associate a tag with one or more segments. Any segment cannot be associated with more than **100** tags.  Use the request body to pass in the ID(s) of the segments(s) that will be associated with the tag.<br><br>*Rate limits*:<br>Burst: `3/s`<br>Steady: `60/m`  **Scopes:** `segments:write` `tags:write`  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.create_tag_relationships_segments(id, tag_segment_op, async_req=True)
         >>> result = thread.get()
 
         Args:
@@ -2064,15 +2064,15 @@
     def delete_tag(
         self,
         id,
         **kwargs
     ):
         """Delete Tag  # noqa: E501
 
-        Delete the tag with the given tag ID. Any associations between the tag and other resources will also be removed.<br><br>*Rate limits*:<br>Burst: `3/s`<br>Steady: `60/m`  **Scopes:** `Tags Read` `Tags Write`  # noqa: E501
+        Delete the tag with the given tag ID. Any associations between the tag and other resources will also be removed.<br><br>*Rate limits*:<br>Burst: `3/s`<br>Steady: `60/m`  **Scopes:** `tags:read` `tags:write`  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.delete_tag(id, async_req=True)
         >>> result = thread.get()
 
         Args:
@@ -2147,15 +2147,15 @@
     def delete_tag_group(
         self,
         id,
         **kwargs
     ):
         """Delete Tag Group  # noqa: E501
 
-        Delete the tag group with the given tag group ID. Any tags inside that tag group, and any associations between those tags and other resources, will also be removed. The default tag group cannot be deleted.<br><br>*Rate limits*:<br>Burst: `3/s`<br>Steady: `60/m`  **Scopes:** `Tags Read` `Tags Write`  # noqa: E501
+        Delete the tag group with the given tag group ID. Any tags inside that tag group, and any associations between those tags and other resources, will also be removed. The default tag group cannot be deleted.<br><br>*Rate limits*:<br>Burst: `3/s`<br>Steady: `60/m`  **Scopes:** `tags:read` `tags:write`  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.delete_tag_group(id, async_req=True)
         >>> result = thread.get()
 
         Args:
@@ -2231,15 +2231,15 @@
         self,
         id,
         tag_campaign_op,
         **kwargs
     ):
         """Delete Tag Relationships Campaigns  # noqa: E501
 
-        Remove a tag's association with one or more campaigns.  Use the request body to pass in the ID(s) of the campaign(s) whose association with the tag will be removed.<br><br>*Rate limits*:<br>Burst: `3/s`<br>Steady: `60/m`  **Scopes:** `Campaigns Write` `Tags Write`  # noqa: E501
+        Remove a tag's association with one or more campaigns.  Use the request body to pass in the ID(s) of the campaign(s) whose association with the tag will be removed.<br><br>*Rate limits*:<br>Burst: `3/s`<br>Steady: `60/m`  **Scopes:** `campaigns:write` `tags:write`  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.delete_tag_relationships_campaigns(id, tag_campaign_op, async_req=True)
         >>> result = thread.get()
 
         Args:
@@ -2318,15 +2318,15 @@
         self,
         id,
         tag_flow_op,
         **kwargs
     ):
         """Delete Tag Relationships Flows  # noqa: E501
 
-        Remove a tag's association with one or more flows.  Use the request body to pass in the ID(s) of the flows(s) whose association with the tag will be removed.<br><br>*Rate limits*:<br>Burst: `3/s`<br>Steady: `60/m`  **Scopes:** `Flows Write` `Tags Write`  # noqa: E501
+        Remove a tag's association with one or more flows.  Use the request body to pass in the ID(s) of the flows(s) whose association with the tag will be removed.<br><br>*Rate limits*:<br>Burst: `3/s`<br>Steady: `60/m`  **Scopes:** `flows:write` `tags:write`  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.delete_tag_relationships_flows(id, tag_flow_op, async_req=True)
         >>> result = thread.get()
 
         Args:
@@ -2405,15 +2405,15 @@
         self,
         id,
         tag_list_op,
         **kwargs
     ):
         """Delete Tag Relationships Lists  # noqa: E501
 
-        Remove a tag's association with one or more lists.  Use the request body to pass in the ID(s) of the list(s) whose association with the tag will be removed.<br><br>*Rate limits*:<br>Burst: `3/s`<br>Steady: `60/m`  **Scopes:** `List Write` `Tags Write`  # noqa: E501
+        Remove a tag's association with one or more lists.  Use the request body to pass in the ID(s) of the list(s) whose association with the tag will be removed.<br><br>*Rate limits*:<br>Burst: `3/s`<br>Steady: `60/m`  **Scopes:** `list:write` `tags:write`  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.delete_tag_relationships_lists(id, tag_list_op, async_req=True)
         >>> result = thread.get()
 
         Args:
@@ -2492,15 +2492,15 @@
         self,
         id,
         tag_segment_op,
         **kwargs
     ):
         """Delete Tag Relationships Segments  # noqa: E501
 
-        Remove a tag's association with one or more segments.  Use the request body to pass in the ID(s) of the segments(s) whose association with the tag will be removed.<br><br>*Rate limits*:<br>Burst: `3/s`<br>Steady: `60/m`  **Scopes:** `Segments Write` `Tags Write`  # noqa: E501
+        Remove a tag's association with one or more segments.  Use the request body to pass in the ID(s) of the segments(s) whose association with the tag will be removed.<br><br>*Rate limits*:<br>Burst: `3/s`<br>Steady: `60/m`  **Scopes:** `segments:write` `tags:write`  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.delete_tag_relationships_segments(id, tag_segment_op, async_req=True)
         >>> result = thread.get()
 
         Args:
@@ -2578,15 +2578,15 @@
     def get_tag(
         self,
         id,
         **kwargs
     ):
         """Get Tag  # noqa: E501
 
-        Retrieve the tag with the given tag ID.<br><br>*Rate limits*:<br>Burst: `3/s`<br>Steady: `60/m`  **Scopes:** `Tags Read`  # noqa: E501
+        Retrieve the tag with the given tag ID.<br><br>*Rate limits*:<br>Burst: `3/s`<br>Steady: `60/m`  **Scopes:** `tags:read`  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.get_tag(id, async_req=True)
         >>> result = thread.get()
 
         Args:
@@ -2662,15 +2662,15 @@
     def get_tag_group(
         self,
         id,
         **kwargs
     ):
         """Get Tag Group  # noqa: E501
 
-        Retrieve the tag group with the given tag group ID.<br><br>*Rate limits*:<br>Burst: `3/s`<br>Steady: `60/m`  **Scopes:** `Tags Read`  # noqa: E501
+        Retrieve the tag group with the given tag group ID.<br><br>*Rate limits*:<br>Burst: `3/s`<br>Steady: `60/m`  **Scopes:** `tags:read`  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.get_tag_group(id, async_req=True)
         >>> result = thread.get()
 
         Args:
@@ -2746,15 +2746,15 @@
     def get_tag_group_relationships_tags(
         self,
         id,
         **kwargs
     ):
         """Get Tag Group Relationships Tags  # noqa: E501
 
-        Returns the tag IDs of all tags inside the given tag group.<br><br>*Rate limits*:<br>Burst: `3/s`<br>Steady: `60/m`  **Scopes:** `Tags Read`  # noqa: E501
+        Returns the tag IDs of all tags inside the given tag group.<br><br>*Rate limits*:<br>Burst: `3/s`<br>Steady: `60/m`  **Scopes:** `tags:read`  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.get_tag_group_relationships_tags(id, async_req=True)
         >>> result = thread.get()
 
         Args:
@@ -2829,15 +2829,15 @@
     def get_tag_group_tags(
         self,
         id,
         **kwargs
     ):
         """Get Tag Group Tags  # noqa: E501
 
-        Return the tags for a given tag group ID.<br><br>*Rate limits*:<br>Burst: `3/s`<br>Steady: `60/m`  **Scopes:** `Tags Read`  # noqa: E501
+        Return the tags for a given tag group ID.<br><br>*Rate limits*:<br>Burst: `3/s`<br>Steady: `60/m`  **Scopes:** `tags:read`  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.get_tag_group_tags(id, async_req=True)
         >>> result = thread.get()
 
         Args:
@@ -2912,15 +2912,15 @@
 
     def get_tag_groups(
         self,
         **kwargs
     ):
         """Get Tag Groups  # noqa: E501
 
-        List all tag groups in an account. Every account has one default tag group. Tag groups can be filtered by `name`, `exclusive`, and `default`, and sorted by `name` or `id` in ascending or descending order. Returns a maximum of 25 tag groups per request, which can be paginated with [cursor-based pagination](https://developers.klaviyo.com/en/v2022-10-17/reference/api_overview#pagination).<br><br>*Rate limits*:<br>Burst: `3/s`<br>Steady: `60/m`  **Scopes:** `Tags Read`  # noqa: E501
+        List all tag groups in an account. Every account has one default tag group. Tag groups can be filtered by `name`, `exclusive`, and `default`, and sorted by `name` or `id` in ascending or descending order. Returns a maximum of 25 tag groups per request, which can be paginated with [cursor-based pagination](https://developers.klaviyo.com/en/v2022-10-17/reference/api_overview#pagination).<br><br>*Rate limits*:<br>Burst: `3/s`<br>Steady: `60/m`  **Scopes:** `tags:read`  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.get_tag_groups(async_req=True)
         >>> result = thread.get()
 
 
@@ -2995,15 +2995,15 @@
     def get_tag_relationships_campaigns(
         self,
         id,
         **kwargs
     ):
         """Get Tag Relationships Campaigns  # noqa: E501
 
-        Returns the IDs of all campaigns associated with the given tag.<br><br>*Rate limits*:<br>Burst: `3/s`<br>Steady: `60/m`  **Scopes:** `Campaigns Read` `Tags Read`  # noqa: E501
+        Returns the IDs of all campaigns associated with the given tag.<br><br>*Rate limits*:<br>Burst: `3/s`<br>Steady: `60/m`  **Scopes:** `campaigns:read` `tags:read`  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.get_tag_relationships_campaigns(id, async_req=True)
         >>> result = thread.get()
 
         Args:
@@ -3078,15 +3078,15 @@
     def get_tag_relationships_flows(
         self,
         id,
         **kwargs
     ):
         """Get Tag Relationships Flows  # noqa: E501
 
-        Returns the IDs of all flows associated with the given tag.<br><br>*Rate limits*:<br>Burst: `3/s`<br>Steady: `60/m`  **Scopes:** `Flows Read` `Tags Read`  # noqa: E501
+        Returns the IDs of all flows associated with the given tag.<br><br>*Rate limits*:<br>Burst: `3/s`<br>Steady: `60/m`  **Scopes:** `flows:read` `tags:read`  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.get_tag_relationships_flows(id, async_req=True)
         >>> result = thread.get()
 
         Args:
@@ -3161,15 +3161,15 @@
     def get_tag_relationships_lists(
         self,
         id,
         **kwargs
     ):
         """Get Tag Relationships Lists  # noqa: E501
 
-        Returns the IDs of all lists associated with the given tag.<br><br>*Rate limits*:<br>Burst: `3/s`<br>Steady: `60/m`  **Scopes:** `List Read` `Tags Read`  # noqa: E501
+        Returns the IDs of all lists associated with the given tag.<br><br>*Rate limits*:<br>Burst: `3/s`<br>Steady: `60/m`  **Scopes:** `list:read` `tags:read`  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.get_tag_relationships_lists(id, async_req=True)
         >>> result = thread.get()
 
         Args:
@@ -3244,15 +3244,15 @@
     def get_tag_relationships_segments(
         self,
         id,
         **kwargs
     ):
         """Get Tag Relationships Segments  # noqa: E501
 
-        Returns the IDs of all segments associated with the given tag.<br><br>*Rate limits*:<br>Burst: `3/s`<br>Steady: `60/m`  **Scopes:** `Segments Read` `Tags Read`  # noqa: E501
+        Returns the IDs of all segments associated with the given tag.<br><br>*Rate limits*:<br>Burst: `3/s`<br>Steady: `60/m`  **Scopes:** `segments:read` `tags:read`  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.get_tag_relationships_segments(id, async_req=True)
         >>> result = thread.get()
 
         Args:
@@ -3327,15 +3327,15 @@
     def get_tag_relationships_tag_group(
         self,
         id,
         **kwargs
     ):
         """Get Tag Relationships Tag Group  # noqa: E501
 
-        Returns the ids of all tag groups related to the given tag.<br><br>*Rate limits*:<br>Burst: `3/s`<br>Steady: `60/m`  **Scopes:** `Tags Read`  # noqa: E501
+        Returns the ids of all tag groups related to the given tag.<br><br>*Rate limits*:<br>Burst: `3/s`<br>Steady: `60/m`  **Scopes:** `tags:read`  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.get_tag_relationships_tag_group(id, async_req=True)
         >>> result = thread.get()
 
         Args:
@@ -3410,15 +3410,15 @@
     def get_tag_tag_group(
         self,
         id,
         **kwargs
     ):
         """Get Tag Tag Group  # noqa: E501
 
-        Returns the tag group resource for a given tag ID.<br><br>*Rate limits*:<br>Burst: `3/s`<br>Steady: `60/m`  **Scopes:** `Tags Read`  # noqa: E501
+        Returns the tag group resource for a given tag ID.<br><br>*Rate limits*:<br>Burst: `3/s`<br>Steady: `60/m`  **Scopes:** `tags:read`  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.get_tag_tag_group(id, async_req=True)
         >>> result = thread.get()
 
         Args:
@@ -3493,15 +3493,15 @@
 
     def get_tags(
         self,
         **kwargs
     ):
         """Get Tags  # noqa: E501
 
-        List all tags in an account. Tags can be filtered by `name`, and sorted by `name` or `id` in ascending or descending order. Returns a maximum of 50 tags per request, which can be paginated with [cursor-based pagination](https://developers.klaviyo.com/en/v2022-10-17/reference/api_overview#pagination).<br><br>*Rate limits*:<br>Burst: `3/s`<br>Steady: `60/m`  **Scopes:** `Tags Read`  # noqa: E501
+        List all tags in an account. Tags can be filtered by `name`, and sorted by `name` or `id` in ascending or descending order. Returns a maximum of 50 tags per request, which can be paginated with [cursor-based pagination](https://developers.klaviyo.com/en/v2022-10-17/reference/api_overview#pagination).<br><br>*Rate limits*:<br>Burst: `3/s`<br>Steady: `60/m`  **Scopes:** `tags:read`  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.get_tags(async_req=True)
         >>> result = thread.get()
 
 
@@ -3577,15 +3577,15 @@
         self,
         id,
         tag_update_query,
         **kwargs
     ):
         """Update Tag  # noqa: E501
 
-        Update the tag with the given tag ID. Only a tag's `name` can be changed. A tag cannot be moved from one tag group to another.<br><br>*Rate limits*:<br>Burst: `3/s`<br>Steady: `60/m`  **Scopes:** `Tags Read` `Tags Write`  # noqa: E501
+        Update the tag with the given tag ID. Only a tag's `name` can be changed. A tag cannot be moved from one tag group to another.<br><br>*Rate limits*:<br>Burst: `3/s`<br>Steady: `60/m`  **Scopes:** `tags:read` `tags:write`  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.update_tag(id, tag_update_query, async_req=True)
         >>> result = thread.get()
 
         Args:
@@ -3664,15 +3664,15 @@
         self,
         id,
         tag_group_update_query,
         **kwargs
     ):
         """Update Tag Group  # noqa: E501
 
-        Update the tag group with the given tag group ID. Only a tag group's `name` can be changed. A tag group's `exclusive` or `default` value cannot be changed.<br><br>*Rate limits*:<br>Burst: `3/s`<br>Steady: `60/m`  **Scopes:** `Tags Read` `Tags Write`  # noqa: E501
+        Update the tag group with the given tag group ID. Only a tag group's `name` can be changed. A tag group's `exclusive` or `default` value cannot be changed.<br><br>*Rate limits*:<br>Burst: `3/s`<br>Steady: `60/m`  **Scopes:** `tags:read` `tags:write`  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.update_tag_group(id, tag_group_update_query, async_req=True)
         >>> result = thread.get()
 
         Args:
```

### Comparing `klaviyo-api-2.0.1/src/openapi_client/api/templates_api.py` & `klaviyo-api-2.0.2/src/openapi_client/api/templates_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -465,15 +465,15 @@
     def create_template(
         self,
         template_create_query,
         **kwargs
     ):
         """Create Template  # noqa: E501
 
-        Create a new custom HTML template. If there are 1,000 or more templates in an account, creation will fail as there is a limit of 1,000 templates that can be created via the API. Request specific fields using [sparse fieldsets](https://developers.klaviyo.com/en/reference/api_overview#sparse-fieldsets).<br><br>*Rate limits*:<br>Burst: `10/s`<br>Steady: `150/m`  **Scopes:** `Templates Write`  # noqa: E501
+        Create a new custom HTML template. If there are 1,000 or more templates in an account, creation will fail as there is a limit of 1,000 templates that can be created via the API. Request specific fields using [sparse fieldsets](https://developers.klaviyo.com/en/reference/api_overview#sparse-fieldsets).<br><br>*Rate limits*:<br>Burst: `10/s`<br>Steady: `150/m`  **Scopes:** `template:write`  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.create_template(template_create_query, async_req=True)
         >>> result = thread.get()
 
         Args:
@@ -548,15 +548,15 @@
     def create_template_clone(
         self,
         template_clone_query,
         **kwargs
     ):
         """Create Template Clone  # noqa: E501
 
-        Create a clone of a template with the given template ID.<br><br>*Rate limits*:<br>Burst: `10/s`<br>Steady: `150/m`  **Scopes:** `Templates Write`  # noqa: E501
+        Create a clone of a template with the given template ID.<br><br>*Rate limits*:<br>Burst: `10/s`<br>Steady: `150/m`  **Scopes:** `template:write`  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.create_template_clone(template_clone_query, async_req=True)
         >>> result = thread.get()
 
         Args:
@@ -631,15 +631,15 @@
     def create_template_render(
         self,
         template_render_query,
         **kwargs
     ):
         """Create Template Render  # noqa: E501
 
-        Render a template with the given template ID and context attribute. Returns the HTML and plain text versions of the email template.  **Request body parameters** (nested under `attributes`):  * `return_fields`: Request specific fields using [sparse fieldsets](https://developers.klaviyo.com/en/reference/api_overview#sparse-fieldsets). * `context`: This is the context your email template will be rendered with. You must pass in a `context` object as a JSON object.  Email templates are rendered with contexts in a similar manner to Django templates. Nested template variables can be referenced via dot notation. Template variables without corresponding `context` values are treated as `FALSE` and output nothing.  Ex. `{ \"name\" : \"George Washington\", \"state\" : \"VA\" }`<br><br>*Rate limits*:<br>Burst: `3/s`<br>Steady: `60/m`  **Scopes:** `Templates Read`  # noqa: E501
+        Render a template with the given template ID and context attribute. Returns the HTML and plain text versions of the email template.  **Request body parameters** (nested under `attributes`):  * `return_fields`: Request specific fields using [sparse fieldsets](https://developers.klaviyo.com/en/reference/api_overview#sparse-fieldsets). * `context`: This is the context your email template will be rendered with. You must pass in a `context` object as a JSON object.  Email templates are rendered with contexts in a similar manner to Django templates. Nested template variables can be referenced via dot notation. Template variables without corresponding `context` values are treated as `FALSE` and output nothing.  Ex. `{ \"name\" : \"George Washington\", \"state\" : \"VA\" }`<br><br>*Rate limits*:<br>Burst: `3/s`<br>Steady: `60/m`  **Scopes:** `templates:read`  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.create_template_render(template_render_query, async_req=True)
         >>> result = thread.get()
 
         Args:
@@ -714,15 +714,15 @@
     def delete_template(
         self,
         id,
         **kwargs
     ):
         """Delete Template  # noqa: E501
 
-        Delete a template with the given template ID.<br><br>*Rate limits*:<br>Burst: `10/s`<br>Steady: `150/m`  **Scopes:** `Templates Write`  # noqa: E501
+        Delete a template with the given template ID.<br><br>*Rate limits*:<br>Burst: `10/s`<br>Steady: `150/m`  **Scopes:** `template:write`  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.delete_template(id, async_req=True)
         >>> result = thread.get()
 
         Args:
@@ -797,15 +797,15 @@
     def get_template(
         self,
         id,
         **kwargs
     ):
         """Get Template  # noqa: E501
 
-        Get a template with the given template ID.<br><br>*Rate limits*:<br>Burst: `10/s`<br>Steady: `150/m`  **Scopes:** `Templates Read`  # noqa: E501
+        Get a template with the given template ID.<br><br>*Rate limits*:<br>Burst: `10/s`<br>Steady: `150/m`  **Scopes:** `templates:read`  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.get_template(id, async_req=True)
         >>> result = thread.get()
 
         Args:
@@ -880,15 +880,15 @@
 
     def get_templates(
         self,
         **kwargs
     ):
         """Get Templates  # noqa: E501
 
-        Get all templates in an account. Filter to request a subset of all templates. Templates can be sorted by the following fields, in ascending and descending order: `id`, `name`, `created`, `updated` Returns a maximum of 20 results per page.<br><br>*Rate limits*:<br>Burst: `10/s`<br>Steady: `150/m`  **Scopes:** `Templates Read`  # noqa: E501
+        Get all templates in an account. Filter to request a subset of all templates. Templates can be sorted by the following fields, in ascending and descending order: `id`, `name`, `created`, `updated` Returns a maximum of 10 results per page.<br><br>*Rate limits*:<br>Burst: `10/s`<br>Steady: `150/m`  **Scopes:** `templates:read`  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.get_templates(async_req=True)
         >>> result = thread.get()
 
 
@@ -964,15 +964,15 @@
         self,
         id,
         template_update_query,
         **kwargs
     ):
         """Update Template  # noqa: E501
 
-        Update a template with the given template ID. Does not currently update drag & drop templates.<br><br>*Rate limits*:<br>Burst: `10/s`<br>Steady: `150/m`  **Scopes:** `Templates Write`  # noqa: E501
+        Update a template with the given template ID. Does not currently update drag & drop templates.<br><br>*Rate limits*:<br>Burst: `10/s`<br>Steady: `150/m`  **Scopes:** `template:write`  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.update_template(id, template_update_query, async_req=True)
         >>> result = thread.get()
 
         Args:
```

### Comparing `klaviyo-api-2.0.1/src/openapi_client/api_client.py` & `klaviyo-api-2.0.2/src/openapi_client/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -73,15 +73,15 @@
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'klaviyo-api-python/2.0.1'
+        self.user_agent = 'klaviyo-api-python/2.0.2'
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.close()
```

### Comparing `klaviyo-api-2.0.1/src/openapi_client/apis/__init__.py` & `klaviyo-api-2.0.2/src/openapi_client/apis/__init__.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.1/src/openapi_client/configuration.py` & `klaviyo-api-2.0.2/src/openapi_client/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -406,15 +406,15 @@
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
                "Version of the API: 2023-02-22\n"\
-               "SDK Package Version: 2.0.1".\
+               "SDK Package Version: 2.0.2".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `klaviyo-api-2.0.1/src/openapi_client/exceptions.py` & `klaviyo-api-2.0.2/src/openapi_client/exceptions.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.1/src/openapi_client/model/audiences_sub_object.py` & `klaviyo-api-2.0.2/src/openapi_client/model/audiences_sub_object.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.1/src/openapi_client/model/campaign_clone_query.py` & `klaviyo-api-2.0.2/src/openapi_client/model/campaign_clone_query.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.1/src/openapi_client/model/campaign_clone_query_resource_object.py` & `klaviyo-api-2.0.2/src/openapi_client/model/campaign_clone_query_resource_object.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.1/src/openapi_client/model/campaign_clone_query_resource_object_attributes.py` & `klaviyo-api-2.0.2/src/openapi_client/model/campaign_clone_query_resource_object_attributes.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.1/src/openapi_client/model/campaign_create_query.py` & `klaviyo-api-2.0.2/src/openapi_client/model/campaign_create_query.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.1/src/openapi_client/model/campaign_create_query_resource_object.py` & `klaviyo-api-2.0.2/src/openapi_client/model/campaign_create_query_resource_object.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.1/src/openapi_client/model/campaign_create_query_resource_object_attributes.py` & `klaviyo-api-2.0.2/src/openapi_client/model/campaign_create_query_resource_object_attributes.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.1/src/openapi_client/model/campaign_enum.py` & `klaviyo-api-2.0.2/src/openapi_client/model/campaign_enum.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.1/src/openapi_client/model/campaign_message_assign_template_query.py` & `klaviyo-api-2.0.2/src/openapi_client/model/campaign_message_assign_template_query.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.1/src/openapi_client/model/campaign_message_assign_template_query_resource_object.py` & `klaviyo-api-2.0.2/src/openapi_client/model/campaign_message_assign_template_query_resource_object.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.1/src/openapi_client/model/campaign_message_assign_template_query_resource_object_attributes.py` & `klaviyo-api-2.0.2/src/openapi_client/model/campaign_message_assign_template_query_resource_object_attributes.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.1/src/openapi_client/model/campaign_message_enum.py` & `klaviyo-api-2.0.2/src/openapi_client/model/campaign_message_enum.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.1/src/openapi_client/model/campaign_message_partial_update_query.py` & `klaviyo-api-2.0.2/src/openapi_client/model/campaign_message_partial_update_query.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.1/src/openapi_client/model/campaign_message_partial_update_query_resource_object.py` & `klaviyo-api-2.0.2/src/openapi_client/model/campaign_message_partial_update_query_resource_object.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.1/src/openapi_client/model/campaign_message_partial_update_query_resource_object_attributes.py` & `klaviyo-api-2.0.2/src/openapi_client/model/campaign_message_partial_update_query_resource_object_attributes.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.1/src/openapi_client/model/campaign_partial_update_query.py` & `klaviyo-api-2.0.2/src/openapi_client/model/campaign_partial_update_query.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.1/src/openapi_client/model/campaign_partial_update_query_resource_object.py` & `klaviyo-api-2.0.2/src/openapi_client/model/campaign_partial_update_query_resource_object.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.1/src/openapi_client/model/campaign_partial_update_query_resource_object_attributes.py` & `klaviyo-api-2.0.2/src/openapi_client/model/campaign_partial_update_query_resource_object_attributes.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.1/src/openapi_client/model/campaign_recipient_estimation_enum.py` & `klaviyo-api-2.0.2/src/openapi_client/model/campaign_recipient_estimation_job_enum.py`

 * *Files 5% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from openapi_client.exceptions import ApiAttributeError
 
 
 
-class CampaignRecipientEstimationEnum(ModelSimple):
+class CampaignRecipientEstimationJobEnum(ModelSimple):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -49,15 +49,15 @@
           inclusive_minimum, and regex.
       additional_properties_type (tuple): A tuple of classes accepted
           as additional properties values.
     """
 
     allowed_values = {
         ('value',): {
-            'CAMPAIGN-RECIPIENT-ESTIMATION': "campaign-recipient-estimation",
+            'CAMPAIGN-RECIPIENT-ESTIMATION-JOB': "campaign-recipient-estimation-job",
         },
     }
 
     validations = {
     }
 
     additional_properties_type = None
@@ -96,23 +96,23 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):
-        """CampaignRecipientEstimationEnum - a model defined in OpenAPI
+        """CampaignRecipientEstimationJobEnum - a model defined in OpenAPI
 
         Note that value can be passed either in args or in kwargs, but not in both.
 
         Args:
-            args[0] (str): if omitted defaults to "campaign-recipient-estimation", must be one of ["campaign-recipient-estimation", ]  # noqa: E501
+            args[0] (str): if omitted defaults to "campaign-recipient-estimation-job", must be one of ["campaign-recipient-estimation-job", ]  # noqa: E501
 
         Keyword Args:
-            value (str): if omitted defaults to "campaign-recipient-estimation", must be one of ["campaign-recipient-estimation", ]  # noqa: E501
+            value (str): if omitted defaults to "campaign-recipient-estimation-job", must be one of ["campaign-recipient-estimation-job", ]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
@@ -145,15 +145,15 @@
 
         if 'value' in kwargs:
             value = kwargs.pop('value')
         elif args:
             args = list(args)
             value = args.pop(0)
         else:
-            value = "campaign-recipient-estimation"
+            value = "campaign-recipient-estimation-job"
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
 
         if args:
@@ -186,23 +186,23 @@
                 path_to_item=_path_to_item,
                 valid_classes=(self.__class__,),
             )
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):
-        """CampaignRecipientEstimationEnum - a model defined in OpenAPI
+        """CampaignRecipientEstimationJobEnum - a model defined in OpenAPI
 
         Note that value can be passed either in args or in kwargs, but not in both.
 
         Args:
-            args[0] (str): if omitted defaults to "campaign-recipient-estimation", must be one of ["campaign-recipient-estimation", ]  # noqa: E501
+            args[0] (str): if omitted defaults to "campaign-recipient-estimation-job", must be one of ["campaign-recipient-estimation-job", ]  # noqa: E501
 
         Keyword Args:
-            value (str): if omitted defaults to "campaign-recipient-estimation", must be one of ["campaign-recipient-estimation", ]  # noqa: E501
+            value (str): if omitted defaults to "campaign-recipient-estimation-job", must be one of ["campaign-recipient-estimation-job", ]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
@@ -237,15 +237,15 @@
 
         if 'value' in kwargs:
             value = kwargs.pop('value')
         elif args:
             args = list(args)
             value = args.pop(0)
         else:
-            value = "campaign-recipient-estimation"
+            value = "campaign-recipient-estimation-job"
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
 
         if args:
```

### Comparing `klaviyo-api-2.0.1/src/openapi_client/model/campaign_recipient_estimation_job_create_query.py` & `klaviyo-api-2.0.2/src/openapi_client/model/campaign_recipient_estimation_job_create_query.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.1/src/openapi_client/model/campaign_recipient_estimation_job_create_query_resource_object.py` & `klaviyo-api-2.0.2/src/openapi_client/model/campaign_recipient_estimation_job_create_query_resource_object.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.1/src/openapi_client/model/campaign_recipient_estimation_job_create_query_resource_object_attributes.py` & `klaviyo-api-2.0.2/src/openapi_client/model/campaign_recipient_estimation_job_create_query_resource_object_attributes.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.1/src/openapi_client/model/campaign_recipient_estimation_job_enum.py` & `klaviyo-api-2.0.2/src/openapi_client/model/catalog_variant_bulk_delete_job_enum.py`

 * *Files 10% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from openapi_client.exceptions import ApiAttributeError
 
 
 
-class CampaignRecipientEstimationJobEnum(ModelSimple):
+class CatalogVariantBulkDeleteJobEnum(ModelSimple):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -49,15 +49,15 @@
           inclusive_minimum, and regex.
       additional_properties_type (tuple): A tuple of classes accepted
           as additional properties values.
     """
 
     allowed_values = {
         ('value',): {
-            'CAMPAIGN-RECIPIENT-ESTIMATION-JOB': "campaign-recipient-estimation-job",
+            'CATALOG-VARIANT-BULK-DELETE-JOB': "catalog-variant-bulk-delete-job",
         },
     }
 
     validations = {
     }
 
     additional_properties_type = None
@@ -96,23 +96,23 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):
-        """CampaignRecipientEstimationJobEnum - a model defined in OpenAPI
+        """CatalogVariantBulkDeleteJobEnum - a model defined in OpenAPI
 
         Note that value can be passed either in args or in kwargs, but not in both.
 
         Args:
-            args[0] (str): if omitted defaults to "campaign-recipient-estimation-job", must be one of ["campaign-recipient-estimation-job", ]  # noqa: E501
+            args[0] (str): if omitted defaults to "catalog-variant-bulk-delete-job", must be one of ["catalog-variant-bulk-delete-job", ]  # noqa: E501
 
         Keyword Args:
-            value (str): if omitted defaults to "campaign-recipient-estimation-job", must be one of ["campaign-recipient-estimation-job", ]  # noqa: E501
+            value (str): if omitted defaults to "catalog-variant-bulk-delete-job", must be one of ["catalog-variant-bulk-delete-job", ]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
@@ -145,15 +145,15 @@
 
         if 'value' in kwargs:
             value = kwargs.pop('value')
         elif args:
             args = list(args)
             value = args.pop(0)
         else:
-            value = "campaign-recipient-estimation-job"
+            value = "catalog-variant-bulk-delete-job"
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
 
         if args:
@@ -186,23 +186,23 @@
                 path_to_item=_path_to_item,
                 valid_classes=(self.__class__,),
             )
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):
-        """CampaignRecipientEstimationJobEnum - a model defined in OpenAPI
+        """CatalogVariantBulkDeleteJobEnum - a model defined in OpenAPI
 
         Note that value can be passed either in args or in kwargs, but not in both.
 
         Args:
-            args[0] (str): if omitted defaults to "campaign-recipient-estimation-job", must be one of ["campaign-recipient-estimation-job", ]  # noqa: E501
+            args[0] (str): if omitted defaults to "catalog-variant-bulk-delete-job", must be one of ["catalog-variant-bulk-delete-job", ]  # noqa: E501
 
         Keyword Args:
-            value (str): if omitted defaults to "campaign-recipient-estimation-job", must be one of ["campaign-recipient-estimation-job", ]  # noqa: E501
+            value (str): if omitted defaults to "catalog-variant-bulk-delete-job", must be one of ["catalog-variant-bulk-delete-job", ]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
@@ -237,15 +237,15 @@
 
         if 'value' in kwargs:
             value = kwargs.pop('value')
         elif args:
             args = list(args)
             value = args.pop(0)
         else:
-            value = "campaign-recipient-estimation-job"
+            value = "catalog-variant-bulk-delete-job"
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
 
         if args:
```

### Comparing `klaviyo-api-2.0.1/src/openapi_client/model/campaign_send_job_create_query.py` & `klaviyo-api-2.0.2/src/openapi_client/model/campaign_send_job_create_query.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.1/src/openapi_client/model/campaign_send_job_create_query_resource_object.py` & `klaviyo-api-2.0.2/src/openapi_client/model/campaign_send_job_create_query_resource_object.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.1/src/openapi_client/model/campaign_send_job_create_query_resource_object_attributes.py` & `klaviyo-api-2.0.2/src/openapi_client/model/campaign_send_job_create_query_resource_object_attributes.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.1/src/openapi_client/model/campaign_send_job_enum.py` & `klaviyo-api-2.0.2/src/openapi_client/model/campaign_send_job_enum.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.1/src/openapi_client/model/campaign_send_job_partial_update_query.py` & `klaviyo-api-2.0.2/src/openapi_client/model/campaign_send_job_partial_update_query.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.1/src/openapi_client/model/campaign_send_job_partial_update_query_resource_object.py` & `klaviyo-api-2.0.2/src/openapi_client/model/campaign_send_job_partial_update_query_resource_object.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.1/src/openapi_client/model/campaign_send_job_partial_update_query_resource_object_attributes.py` & `klaviyo-api-2.0.2/src/openapi_client/model/campaign_send_job_partial_update_query_resource_object_attributes.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.1/src/openapi_client/model/catalog_category_bulk_create_job_enum.py` & `klaviyo-api-2.0.2/src/openapi_client/model/catalog_category_bulk_create_job_enum.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.1/src/openapi_client/model/catalog_category_bulk_delete_job_enum.py` & `klaviyo-api-2.0.2/src/openapi_client/model/catalog_category_bulk_delete_job_enum.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.1/src/openapi_client/model/catalog_category_bulk_update_job_enum.py` & `klaviyo-api-2.0.2/src/openapi_client/model/catalog_category_bulk_update_job_enum.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.1/src/openapi_client/model/catalog_category_create_job_create_query.py` & `klaviyo-api-2.0.2/src/openapi_client/model/catalog_category_create_job_create_query.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.1/src/openapi_client/model/catalog_category_create_job_create_query_resource_object.py` & `klaviyo-api-2.0.2/src/openapi_client/model/catalog_category_create_job_create_query_resource_object.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.1/src/openapi_client/model/catalog_category_create_job_create_query_resource_object_attributes.py` & `klaviyo-api-2.0.2/src/openapi_client/model/catalog_category_create_job_create_query_resource_object_attributes.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.1/src/openapi_client/model/catalog_category_create_query.py` & `klaviyo-api-2.0.2/src/openapi_client/model/catalog_category_create_query.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.1/src/openapi_client/model/catalog_category_create_query_resource_object.py` & `klaviyo-api-2.0.2/src/openapi_client/model/catalog_category_create_query_resource_object.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.1/src/openapi_client/model/catalog_category_create_query_resource_object_attributes.py` & `klaviyo-api-2.0.2/src/openapi_client/model/catalog_category_create_query_resource_object_attributes.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.1/src/openapi_client/model/catalog_category_delete_job_create_query.py` & `klaviyo-api-2.0.2/src/openapi_client/model/catalog_category_delete_job_create_query.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.1/src/openapi_client/model/catalog_category_delete_job_create_query_resource_object.py` & `klaviyo-api-2.0.2/src/openapi_client/model/catalog_category_delete_job_create_query_resource_object.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.1/src/openapi_client/model/catalog_category_delete_job_create_query_resource_object_attributes.py` & `klaviyo-api-2.0.2/src/openapi_client/model/catalog_category_delete_job_create_query_resource_object_attributes.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.1/src/openapi_client/model/catalog_category_delete_query_resource_object.py` & `klaviyo-api-2.0.2/src/openapi_client/model/catalog_category_delete_query_resource_object.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.1/src/openapi_client/model/catalog_category_enum.py` & `klaviyo-api-2.0.2/src/openapi_client/model/catalog_category_enum.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.1/src/openapi_client/model/catalog_category_item_op.py` & `klaviyo-api-2.0.2/src/openapi_client/model/catalog_category_item_op.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.1/src/openapi_client/model/catalog_category_update_job_create_query.py` & `klaviyo-api-2.0.2/src/openapi_client/model/catalog_category_update_job_create_query.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.1/src/openapi_client/model/catalog_category_update_job_create_query_resource_object.py` & `klaviyo-api-2.0.2/src/openapi_client/model/catalog_category_update_job_create_query_resource_object.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.1/src/openapi_client/model/catalog_category_update_job_create_query_resource_object_attributes.py` & `klaviyo-api-2.0.2/src/openapi_client/model/catalog_category_update_job_create_query_resource_object_attributes.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.1/src/openapi_client/model/catalog_category_update_query.py` & `klaviyo-api-2.0.2/src/openapi_client/model/catalog_category_update_query.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.1/src/openapi_client/model/catalog_category_update_query_resource_object.py` & `klaviyo-api-2.0.2/src/openapi_client/model/catalog_category_update_query_resource_object.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.1/src/openapi_client/model/catalog_category_update_query_resource_object_attributes.py` & `klaviyo-api-2.0.2/src/openapi_client/model/catalog_category_update_query_resource_object_attributes.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.1/src/openapi_client/model/catalog_category_update_query_resource_object_relationships.py` & `klaviyo-api-2.0.2/src/openapi_client/model/catalog_category_update_query_resource_object_relationships.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.1/src/openapi_client/model/catalog_category_update_query_resource_object_relationships_items.py` & `klaviyo-api-2.0.2/src/openapi_client/model/catalog_category_update_query_resource_object_relationships_items.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.1/src/openapi_client/model/catalog_category_update_query_resource_object_relationships_items_data_inner.py` & `klaviyo-api-2.0.2/src/openapi_client/model/catalog_category_update_query_resource_object_relationships_items_data_inner.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.1/src/openapi_client/model/catalog_item_bulk_create_job_enum.py` & `klaviyo-api-2.0.2/src/openapi_client/model/catalog_item_bulk_create_job_enum.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.1/src/openapi_client/model/catalog_item_bulk_delete_job_enum.py` & `klaviyo-api-2.0.2/src/openapi_client/model/catalog_item_bulk_delete_job_enum.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.1/src/openapi_client/model/catalog_item_bulk_update_job_enum.py` & `klaviyo-api-2.0.2/src/openapi_client/model/catalog_item_bulk_update_job_enum.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.1/src/openapi_client/model/catalog_item_category_op.py` & `klaviyo-api-2.0.2/src/openapi_client/model/catalog_item_category_op.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.1/src/openapi_client/model/catalog_item_create_job_create_query.py` & `klaviyo-api-2.0.2/src/openapi_client/model/catalog_item_create_job_create_query.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.1/src/openapi_client/model/catalog_item_create_job_create_query_resource_object.py` & `klaviyo-api-2.0.2/src/openapi_client/model/catalog_item_create_job_create_query_resource_object.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.1/src/openapi_client/model/catalog_item_create_job_create_query_resource_object_attributes.py` & `klaviyo-api-2.0.2/src/openapi_client/model/catalog_item_create_job_create_query_resource_object_attributes.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.1/src/openapi_client/model/catalog_item_create_query.py` & `klaviyo-api-2.0.2/src/openapi_client/model/catalog_item_create_query.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.1/src/openapi_client/model/catalog_item_create_query_resource_object.py` & `klaviyo-api-2.0.2/src/openapi_client/model/catalog_item_create_query_resource_object.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.1/src/openapi_client/model/catalog_item_create_query_resource_object_attributes.py` & `klaviyo-api-2.0.2/src/openapi_client/model/catalog_item_create_query_resource_object_attributes.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.1/src/openapi_client/model/catalog_item_create_query_resource_object_relationships.py` & `klaviyo-api-2.0.2/src/openapi_client/model/catalog_item_create_query_resource_object_relationships.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.1/src/openapi_client/model/catalog_item_create_query_resource_object_relationships_categories.py` & `klaviyo-api-2.0.2/src/openapi_client/model/catalog_item_create_query_resource_object_relationships_categories.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.1/src/openapi_client/model/catalog_item_create_query_resource_object_relationships_categories_data_inner.py` & `klaviyo-api-2.0.2/src/openapi_client/model/catalog_item_create_query_resource_object_relationships_categories_data_inner.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.1/src/openapi_client/model/catalog_item_delete_job_create_query.py` & `klaviyo-api-2.0.2/src/openapi_client/model/catalog_item_delete_job_create_query.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.1/src/openapi_client/model/catalog_item_delete_job_create_query_resource_object.py` & `klaviyo-api-2.0.2/src/openapi_client/model/catalog_item_delete_job_create_query_resource_object.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.1/src/openapi_client/model/catalog_item_delete_job_create_query_resource_object_attributes.py` & `klaviyo-api-2.0.2/src/openapi_client/model/catalog_item_delete_job_create_query_resource_object_attributes.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.1/src/openapi_client/model/catalog_item_delete_query_resource_object.py` & `klaviyo-api-2.0.2/src/openapi_client/model/catalog_item_delete_query_resource_object.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.1/src/openapi_client/model/catalog_item_enum.py` & `klaviyo-api-2.0.2/src/openapi_client/model/catalog_item_enum.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.1/src/openapi_client/model/catalog_item_update_job_create_query.py` & `klaviyo-api-2.0.2/src/openapi_client/model/catalog_item_update_job_create_query.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.1/src/openapi_client/model/catalog_item_update_job_create_query_resource_object.py` & `klaviyo-api-2.0.2/src/openapi_client/model/catalog_item_update_job_create_query_resource_object.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.1/src/openapi_client/model/catalog_item_update_job_create_query_resource_object_attributes.py` & `klaviyo-api-2.0.2/src/openapi_client/model/catalog_item_update_job_create_query_resource_object_attributes.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.1/src/openapi_client/model/catalog_item_update_query.py` & `klaviyo-api-2.0.2/src/openapi_client/model/catalog_item_update_query.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.1/src/openapi_client/model/catalog_item_update_query_resource_object.py` & `klaviyo-api-2.0.2/src/openapi_client/model/catalog_item_update_query_resource_object.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.1/src/openapi_client/model/catalog_item_update_query_resource_object_attributes.py` & `klaviyo-api-2.0.2/src/openapi_client/model/catalog_item_update_query_resource_object_attributes.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.1/src/openapi_client/model/catalog_job_error_payload.py` & `klaviyo-api-2.0.2/src/openapi_client/model/tag_campaign_op_data_inner.py`

 * *Files 5% similar despite different names*

```diff
@@ -26,20 +26,16 @@
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
 from openapi_client.exceptions import ApiAttributeError
 
 
-def lazy_import():
-    from openapi_client.model.error_source import ErrorSource
-    globals()['ErrorSource'] = ErrorSource
 
-
-class CatalogJobErrorPayload(ModelNormal):
+class TagCampaignOpDataInner(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -56,80 +52,72 @@
           min_items, exclusive_maximum, inclusive_maximum, exclusive_minimum,
           inclusive_minimum, and regex.
       additional_properties_type (tuple): A tuple of classes accepted
           as additional properties values.
     """
 
     allowed_values = {
+        ('type',): {
+            'CAMPAIGN': "campaign",
+        },
     }
 
     validations = {
     }
 
     @cached_property
     def additional_properties_type():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
         """
-        lazy_import()
         return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
 
     _nullable = False
 
     @cached_property
     def openapi_types():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
-        lazy_import()
         return {
-            'source': (ErrorSource,),  # noqa: E501
-            'detail': (str,),  # noqa: E501
-            'code': (str,),  # noqa: E501
+            'type': (str,),  # noqa: E501
             'id': (str,),  # noqa: E501
-            'title': (str,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'source': 'source',  # noqa: E501
-        'detail': 'detail',  # noqa: E501
-        'code': 'code',  # noqa: E501
+        'type': 'type',  # noqa: E501
         'id': 'id',  # noqa: E501
-        'title': 'title',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, source, detail, code, id, title, *args, **kwargs):  # noqa: E501
-        """CatalogJobErrorPayload - a model defined in OpenAPI
+    def _from_openapi_data(cls, id, *args, **kwargs):  # noqa: E501
+        """TagCampaignOpDataInner - a model defined in OpenAPI
 
         Args:
-            source (ErrorSource):
-            detail (str): Specific details about the error.
-            code (str): A code for classifying the error type.
-            id (str): Unique identifier for the error.
-            title (str): A high-level message about the error.
+            id (str):
 
         Keyword Args:
+            type (str): defaults to "campaign", must be one of ["campaign", ]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
@@ -154,14 +142,15 @@
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
         """
 
+        type = kwargs.get('type', "campaign")
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
 
         self = super(OpenApiModel, cls).__new__(cls)
@@ -183,19 +172,16 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.source = source
-        self.detail = detail
-        self.code = code
+        self.type = type
         self.id = id
-        self.title = title
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -208,25 +194,22 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, source, detail, code, id, title, *args, **kwargs):  # noqa: E501
-        """CatalogJobErrorPayload - a model defined in OpenAPI
+    def __init__(self, id, *args, **kwargs):  # noqa: E501
+        """TagCampaignOpDataInner - a model defined in OpenAPI
 
         Args:
-            source (ErrorSource):
-            detail (str): Specific details about the error.
-            code (str): A code for classifying the error type.
-            id (str): Unique identifier for the error.
-            title (str): A high-level message about the error.
+            id (str):
 
         Keyword Args:
+            type (str): defaults to "campaign", must be one of ["campaign", ]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
@@ -251,14 +234,15 @@
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
         """
 
+        type = kwargs.get('type', "campaign")
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
 
         if args:
@@ -278,19 +262,16 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.source = source
-        self.detail = detail
-        self.code = code
+        self.type = type
         self.id = id
-        self.title = title
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `klaviyo-api-2.0.1/src/openapi_client/model/catalog_variant_bulk_create_job_enum.py` & `klaviyo-api-2.0.2/src/openapi_client/model/catalog_variant_bulk_create_job_enum.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.1/src/openapi_client/model/catalog_variant_bulk_delete_job_enum.py` & `klaviyo-api-2.0.2/src/openapi_client/model/catalog_variant_bulk_update_job_enum.py`

 * *Files 6% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from openapi_client.exceptions import ApiAttributeError
 
 
 
-class CatalogVariantBulkDeleteJobEnum(ModelSimple):
+class CatalogVariantBulkUpdateJobEnum(ModelSimple):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -49,15 +49,15 @@
           inclusive_minimum, and regex.
       additional_properties_type (tuple): A tuple of classes accepted
           as additional properties values.
     """
 
     allowed_values = {
         ('value',): {
-            'CATALOG-VARIANT-BULK-DELETE-JOB': "catalog-variant-bulk-delete-job",
+            'CATALOG-VARIANT-BULK-UPDATE-JOB': "catalog-variant-bulk-update-job",
         },
     }
 
     validations = {
     }
 
     additional_properties_type = None
@@ -96,23 +96,23 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):
-        """CatalogVariantBulkDeleteJobEnum - a model defined in OpenAPI
+        """CatalogVariantBulkUpdateJobEnum - a model defined in OpenAPI
 
         Note that value can be passed either in args or in kwargs, but not in both.
 
         Args:
-            args[0] (str): if omitted defaults to "catalog-variant-bulk-delete-job", must be one of ["catalog-variant-bulk-delete-job", ]  # noqa: E501
+            args[0] (str): if omitted defaults to "catalog-variant-bulk-update-job", must be one of ["catalog-variant-bulk-update-job", ]  # noqa: E501
 
         Keyword Args:
-            value (str): if omitted defaults to "catalog-variant-bulk-delete-job", must be one of ["catalog-variant-bulk-delete-job", ]  # noqa: E501
+            value (str): if omitted defaults to "catalog-variant-bulk-update-job", must be one of ["catalog-variant-bulk-update-job", ]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
@@ -145,15 +145,15 @@
 
         if 'value' in kwargs:
             value = kwargs.pop('value')
         elif args:
             args = list(args)
             value = args.pop(0)
         else:
-            value = "catalog-variant-bulk-delete-job"
+            value = "catalog-variant-bulk-update-job"
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
 
         if args:
@@ -186,23 +186,23 @@
                 path_to_item=_path_to_item,
                 valid_classes=(self.__class__,),
             )
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):
-        """CatalogVariantBulkDeleteJobEnum - a model defined in OpenAPI
+        """CatalogVariantBulkUpdateJobEnum - a model defined in OpenAPI
 
         Note that value can be passed either in args or in kwargs, but not in both.
 
         Args:
-            args[0] (str): if omitted defaults to "catalog-variant-bulk-delete-job", must be one of ["catalog-variant-bulk-delete-job", ]  # noqa: E501
+            args[0] (str): if omitted defaults to "catalog-variant-bulk-update-job", must be one of ["catalog-variant-bulk-update-job", ]  # noqa: E501
 
         Keyword Args:
-            value (str): if omitted defaults to "catalog-variant-bulk-delete-job", must be one of ["catalog-variant-bulk-delete-job", ]  # noqa: E501
+            value (str): if omitted defaults to "catalog-variant-bulk-update-job", must be one of ["catalog-variant-bulk-update-job", ]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
@@ -237,15 +237,15 @@
 
         if 'value' in kwargs:
             value = kwargs.pop('value')
         elif args:
             args = list(args)
             value = args.pop(0)
         else:
-            value = "catalog-variant-bulk-delete-job"
+            value = "catalog-variant-bulk-update-job"
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
 
         if args:
```

### Comparing `klaviyo-api-2.0.1/src/openapi_client/model/catalog_variant_bulk_update_job_enum.py` & `klaviyo-api-2.0.2/src/openapi_client/model/catalog_variant_enum.py`

 * *Files 8% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from openapi_client.exceptions import ApiAttributeError
 
 
 
-class CatalogVariantBulkUpdateJobEnum(ModelSimple):
+class CatalogVariantEnum(ModelSimple):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -49,15 +49,15 @@
           inclusive_minimum, and regex.
       additional_properties_type (tuple): A tuple of classes accepted
           as additional properties values.
     """
 
     allowed_values = {
         ('value',): {
-            'CATALOG-VARIANT-BULK-UPDATE-JOB': "catalog-variant-bulk-update-job",
+            'CATALOG-VARIANT': "catalog-variant",
         },
     }
 
     validations = {
     }
 
     additional_properties_type = None
@@ -96,23 +96,23 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):
-        """CatalogVariantBulkUpdateJobEnum - a model defined in OpenAPI
+        """CatalogVariantEnum - a model defined in OpenAPI
 
         Note that value can be passed either in args or in kwargs, but not in both.
 
         Args:
-            args[0] (str): if omitted defaults to "catalog-variant-bulk-update-job", must be one of ["catalog-variant-bulk-update-job", ]  # noqa: E501
+            args[0] (str): if omitted defaults to "catalog-variant", must be one of ["catalog-variant", ]  # noqa: E501
 
         Keyword Args:
-            value (str): if omitted defaults to "catalog-variant-bulk-update-job", must be one of ["catalog-variant-bulk-update-job", ]  # noqa: E501
+            value (str): if omitted defaults to "catalog-variant", must be one of ["catalog-variant", ]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
@@ -145,15 +145,15 @@
 
         if 'value' in kwargs:
             value = kwargs.pop('value')
         elif args:
             args = list(args)
             value = args.pop(0)
         else:
-            value = "catalog-variant-bulk-update-job"
+            value = "catalog-variant"
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
 
         if args:
@@ -186,23 +186,23 @@
                 path_to_item=_path_to_item,
                 valid_classes=(self.__class__,),
             )
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):
-        """CatalogVariantBulkUpdateJobEnum - a model defined in OpenAPI
+        """CatalogVariantEnum - a model defined in OpenAPI
 
         Note that value can be passed either in args or in kwargs, but not in both.
 
         Args:
-            args[0] (str): if omitted defaults to "catalog-variant-bulk-update-job", must be one of ["catalog-variant-bulk-update-job", ]  # noqa: E501
+            args[0] (str): if omitted defaults to "catalog-variant", must be one of ["catalog-variant", ]  # noqa: E501
 
         Keyword Args:
-            value (str): if omitted defaults to "catalog-variant-bulk-update-job", must be one of ["catalog-variant-bulk-update-job", ]  # noqa: E501
+            value (str): if omitted defaults to "catalog-variant", must be one of ["catalog-variant", ]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
@@ -237,15 +237,15 @@
 
         if 'value' in kwargs:
             value = kwargs.pop('value')
         elif args:
             args = list(args)
             value = args.pop(0)
         else:
-            value = "catalog-variant-bulk-update-job"
+            value = "catalog-variant"
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
 
         if args:
```

### Comparing `klaviyo-api-2.0.1/src/openapi_client/model/catalog_variant_create_job_create_query.py` & `klaviyo-api-2.0.2/src/openapi_client/model/catalog_variant_create_job_create_query.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.1/src/openapi_client/model/catalog_variant_create_job_create_query_resource_object.py` & `klaviyo-api-2.0.2/src/openapi_client/model/catalog_variant_create_job_create_query_resource_object.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.1/src/openapi_client/model/catalog_variant_create_job_create_query_resource_object_attributes.py` & `klaviyo-api-2.0.2/src/openapi_client/model/catalog_variant_create_job_create_query_resource_object_attributes.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.1/src/openapi_client/model/catalog_variant_create_query.py` & `klaviyo-api-2.0.2/src/openapi_client/model/catalog_variant_create_query.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.1/src/openapi_client/model/catalog_variant_create_query_resource_object.py` & `klaviyo-api-2.0.2/src/openapi_client/model/catalog_variant_create_query_resource_object.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.1/src/openapi_client/model/catalog_variant_create_query_resource_object_attributes.py` & `klaviyo-api-2.0.2/src/openapi_client/model/catalog_variant_create_query_resource_object_attributes.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.1/src/openapi_client/model/catalog_variant_delete_job_create_query.py` & `klaviyo-api-2.0.2/src/openapi_client/model/catalog_variant_delete_job_create_query.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.1/src/openapi_client/model/catalog_variant_delete_job_create_query_resource_object.py` & `klaviyo-api-2.0.2/src/openapi_client/model/catalog_variant_delete_job_create_query_resource_object.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.1/src/openapi_client/model/catalog_variant_delete_job_create_query_resource_object_attributes.py` & `klaviyo-api-2.0.2/src/openapi_client/model/catalog_variant_delete_job_create_query_resource_object_attributes.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.1/src/openapi_client/model/catalog_variant_delete_query_resource_object.py` & `klaviyo-api-2.0.2/src/openapi_client/model/catalog_variant_delete_query_resource_object.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.1/src/openapi_client/model/catalog_variant_enum.py` & `klaviyo-api-2.0.2/src/openapi_client/model/flow_enum.py`

 * *Files 3% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from openapi_client.exceptions import ApiAttributeError
 
 
 
-class CatalogVariantEnum(ModelSimple):
+class FlowEnum(ModelSimple):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -49,15 +49,15 @@
           inclusive_minimum, and regex.
       additional_properties_type (tuple): A tuple of classes accepted
           as additional properties values.
     """
 
     allowed_values = {
         ('value',): {
-            'CATALOG-VARIANT': "catalog-variant",
+            'FLOW': "flow",
         },
     }
 
     validations = {
     }
 
     additional_properties_type = None
@@ -96,23 +96,23 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):
-        """CatalogVariantEnum - a model defined in OpenAPI
+        """FlowEnum - a model defined in OpenAPI
 
         Note that value can be passed either in args or in kwargs, but not in both.
 
         Args:
-            args[0] (str): if omitted defaults to "catalog-variant", must be one of ["catalog-variant", ]  # noqa: E501
+            args[0] (str): if omitted defaults to "flow", must be one of ["flow", ]  # noqa: E501
 
         Keyword Args:
-            value (str): if omitted defaults to "catalog-variant", must be one of ["catalog-variant", ]  # noqa: E501
+            value (str): if omitted defaults to "flow", must be one of ["flow", ]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
@@ -145,15 +145,15 @@
 
         if 'value' in kwargs:
             value = kwargs.pop('value')
         elif args:
             args = list(args)
             value = args.pop(0)
         else:
-            value = "catalog-variant"
+            value = "flow"
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
 
         if args:
@@ -186,23 +186,23 @@
                 path_to_item=_path_to_item,
                 valid_classes=(self.__class__,),
             )
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):
-        """CatalogVariantEnum - a model defined in OpenAPI
+        """FlowEnum - a model defined in OpenAPI
 
         Note that value can be passed either in args or in kwargs, but not in both.
 
         Args:
-            args[0] (str): if omitted defaults to "catalog-variant", must be one of ["catalog-variant", ]  # noqa: E501
+            args[0] (str): if omitted defaults to "flow", must be one of ["flow", ]  # noqa: E501
 
         Keyword Args:
-            value (str): if omitted defaults to "catalog-variant", must be one of ["catalog-variant", ]  # noqa: E501
+            value (str): if omitted defaults to "flow", must be one of ["flow", ]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
@@ -237,15 +237,15 @@
 
         if 'value' in kwargs:
             value = kwargs.pop('value')
         elif args:
             args = list(args)
             value = args.pop(0)
         else:
-            value = "catalog-variant"
+            value = "flow"
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
 
         if args:
```

### Comparing `klaviyo-api-2.0.1/src/openapi_client/model/catalog_variant_update_job_create_query.py` & `klaviyo-api-2.0.2/src/openapi_client/model/catalog_variant_update_job_create_query.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.1/src/openapi_client/model/catalog_variant_update_job_create_query_resource_object.py` & `klaviyo-api-2.0.2/src/openapi_client/model/catalog_variant_update_job_create_query_resource_object.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.1/src/openapi_client/model/catalog_variant_update_job_create_query_resource_object_attributes.py` & `klaviyo-api-2.0.2/src/openapi_client/model/catalog_variant_update_job_create_query_resource_object_attributes.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.1/src/openapi_client/model/catalog_variant_update_query.py` & `klaviyo-api-2.0.2/src/openapi_client/model/catalog_variant_update_query.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.1/src/openapi_client/model/catalog_variant_update_query_resource_object.py` & `klaviyo-api-2.0.2/src/openapi_client/model/catalog_variant_update_query_resource_object.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.1/src/openapi_client/model/catalog_variant_update_query_resource_object_attributes.py` & `klaviyo-api-2.0.2/src/openapi_client/model/catalog_variant_update_query_resource_object_attributes.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.1/src/openapi_client/model/collection_links.py` & `klaviyo-api-2.0.2/src/openapi_client/model/tag_flow_op_data_inner.py`

 * *Files 6% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from openapi_client.exceptions import ApiAttributeError
 
 
 
-class CollectionLinks(ModelNormal):
+class TagFlowOpDataInner(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -52,14 +52,17 @@
           min_items, exclusive_maximum, inclusive_maximum, exclusive_minimum,
           inclusive_minimum, and regex.
       additional_properties_type (tuple): A tuple of classes accepted
           as additional properties values.
     """
 
     allowed_values = {
+        ('type',): {
+            'FLOW': "flow",
+        },
     }
 
     validations = {
     }
 
     @cached_property
     def additional_properties_type():
@@ -78,48 +81,43 @@
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         return {
-            '_self': (str,),  # noqa: E501
-            'next': (str,),  # noqa: E501
-            'prev': (str,),  # noqa: E501
-            'last': (str,),  # noqa: E501
-            'first': (str,),  # noqa: E501
+            'type': (str,),  # noqa: E501
+            'id': (str,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        '_self': 'self',  # noqa: E501
-        'next': 'next',  # noqa: E501
-        'prev': 'prev',  # noqa: E501
-        'last': 'last',  # noqa: E501
-        'first': 'first',  # noqa: E501
+        'type': 'type',  # noqa: E501
+        'id': 'id',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, _self, *args, **kwargs):  # noqa: E501
-        """CollectionLinks - a model defined in OpenAPI
+    def _from_openapi_data(cls, id, *args, **kwargs):  # noqa: E501
+        """TagFlowOpDataInner - a model defined in OpenAPI
 
         Args:
-            _self (str):
+            id (str):
 
         Keyword Args:
+            type (str): defaults to "flow", must be one of ["flow", ]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
@@ -142,20 +140,17 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            next (str): [optional]  # noqa: E501
-            prev (str): [optional]  # noqa: E501
-            last (str): [optional]  # noqa: E501
-            first (str): [optional]  # noqa: E501
         """
 
+        type = kwargs.get('type', "flow")
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
 
         self = super(OpenApiModel, cls).__new__(cls)
@@ -177,15 +172,16 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self._self = _self
+        self.type = type
+        self.id = id
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -198,21 +194,22 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, _self, *args, **kwargs):  # noqa: E501
-        """CollectionLinks - a model defined in OpenAPI
+    def __init__(self, id, *args, **kwargs):  # noqa: E501
+        """TagFlowOpDataInner - a model defined in OpenAPI
 
         Args:
-            _self (str):
+            id (str):
 
         Keyword Args:
+            type (str): defaults to "flow", must be one of ["flow", ]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
@@ -235,20 +232,17 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            next (str): [optional]  # noqa: E501
-            prev (str): [optional]  # noqa: E501
-            last (str): [optional]  # noqa: E501
-            first (str): [optional]  # noqa: E501
         """
 
+        type = kwargs.get('type', "flow")
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
 
         if args:
@@ -268,15 +262,16 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self._self = _self
+        self.type = type
+        self.id = id
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `klaviyo-api-2.0.1/src/openapi_client/model/content_sub_object.py` & `klaviyo-api-2.0.2/src/openapi_client/model/content_sub_object.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.1/src/openapi_client/model/data_privacy_create_deletion_job_query.py` & `klaviyo-api-2.0.2/src/openapi_client/model/data_privacy_create_deletion_job_query.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.1/src/openapi_client/model/data_privacy_create_deletion_job_query_resource_object.py` & `klaviyo-api-2.0.2/src/openapi_client/model/data_privacy_create_deletion_job_query_resource_object.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.1/src/openapi_client/model/data_privacy_create_deletion_job_query_resource_object_attributes.py` & `klaviyo-api-2.0.2/src/openapi_client/model/data_privacy_create_deletion_job_query_resource_object_attributes.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.1/src/openapi_client/model/data_privacy_deletion_job_enum.py` & `klaviyo-api-2.0.2/src/openapi_client/model/data_privacy_deletion_job_enum.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.1/src/openapi_client/model/email_channel.py` & `klaviyo-api-2.0.2/src/openapi_client/model/get_create_variants_jobs5_xx_response_errors_inner_source.py`

 * *Files 5% similar despite different names*

```diff
@@ -26,20 +26,16 @@
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
 from openapi_client.exceptions import ApiAttributeError
 
 
-def lazy_import():
-    from openapi_client.model.email_marketing import EmailMarketing
-    globals()['EmailMarketing'] = EmailMarketing
 
-
-class EmailChannel(ModelNormal):
+class GetCreateVariantsJobs5XXResponseErrorsInnerSource(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -67,52 +63,52 @@
 
     @cached_property
     def additional_properties_type():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
         """
-        lazy_import()
         return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
 
     _nullable = False
 
     @cached_property
     def openapi_types():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
-        lazy_import()
         return {
-            'marketing': (EmailMarketing,),  # noqa: E501
+            'parameter': (str,),  # noqa: E501
+            'pointer': (str,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'marketing': 'marketing',  # noqa: E501
+        'parameter': 'parameter',  # noqa: E501
+        'pointer': 'pointer',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """EmailChannel - a model defined in OpenAPI
+        """GetCreateVariantsJobs5XXResponseErrorsInnerSource - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -137,15 +133,16 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            marketing (EmailMarketing): [optional]  # noqa: E501
+            parameter (str): [optional]  # noqa: E501
+            pointer (str): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -190,15 +187,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """EmailChannel - a model defined in OpenAPI
+        """GetCreateVariantsJobs5XXResponseErrorsInnerSource - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -223,15 +220,16 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            marketing (EmailMarketing): [optional]  # noqa: E501
+            parameter (str): [optional]  # noqa: E501
+            pointer (str): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `klaviyo-api-2.0.1/src/openapi_client/model/email_marketing.py` & `klaviyo-api-2.0.2/src/openapi_client/model/onsite_subscription_create_query_resource_object_attributes.py`

 * *Files 13% similar despite different names*

```diff
@@ -26,22 +26,16 @@
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
 from openapi_client.exceptions import ApiAttributeError
 
 
-def lazy_import():
-    from openapi_client.model.email_marketing_list_suppression import EmailMarketingListSuppression
-    from openapi_client.model.email_marketing_suppression import EmailMarketingSuppression
-    globals()['EmailMarketingListSuppression'] = EmailMarketingListSuppression
-    globals()['EmailMarketingSuppression'] = EmailMarketingSuppression
 
-
-class EmailMarketing(ModelNormal):
+class OnsiteSubscriptionCreateQueryResourceObjectAttributes(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -69,70 +63,61 @@
 
     @cached_property
     def additional_properties_type():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
         """
-        lazy_import()
         return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
 
     _nullable = False
 
     @cached_property
     def openapi_types():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
-        lazy_import()
         return {
-            'consent': (str,),  # noqa: E501
-            'method': (str,),  # noqa: E501
-            'custom_method_detail': (str,),  # noqa: E501
-            'method_detail': (str,),  # noqa: E501
-            'suppressions': (EmailMarketingSuppression,),  # noqa: E501
-            'list_suppressions': (EmailMarketingListSuppression,),  # noqa: E501
-            'double_optin': (bool,),  # noqa: E501
-            'timestamp': (datetime,),  # noqa: E501
+            'list_id': (str, none_type,),  # noqa: E501
+            'phone_number': (str, none_type,),  # noqa: E501
+            'properties': ({str: (bool, date, datetime, dict, float, int, list, str, none_type)},),  # noqa: E501
+            'email': (str, none_type,),  # noqa: E501
+            'custom_source': (str, none_type,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'consent': 'consent',  # noqa: E501
-        'method': 'method',  # noqa: E501
-        'custom_method_detail': 'custom_method_detail',  # noqa: E501
-        'method_detail': 'method_detail',  # noqa: E501
-        'suppressions': 'suppressions',  # noqa: E501
-        'list_suppressions': 'list_suppressions',  # noqa: E501
-        'double_optin': 'double_optin',  # noqa: E501
-        'timestamp': 'timestamp',  # noqa: E501
+        'list_id': 'list_id',  # noqa: E501
+        'phone_number': 'phone_number',  # noqa: E501
+        'properties': 'properties',  # noqa: E501
+        'email': 'email',  # noqa: E501
+        'custom_source': 'custom_source',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, consent, method, *args, **kwargs):  # noqa: E501
-        """EmailMarketing - a model defined in OpenAPI
+    def _from_openapi_data(cls, list_id, *args, **kwargs):  # noqa: E501
+        """OnsiteSubscriptionCreateQueryResourceObjectAttributes - a model defined in OpenAPI
 
         Args:
-            consent (str): The consent status for email marketing.
-            method (str): The method by which the profile was subscribed to email marketing.
+            list_id (str, none_type): The list ID to add the newly subscribed profile to.
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -157,20 +142,18 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            custom_method_detail (str): Additional detail provided by the caller when the profile was subscribed. This may be empty if no details were provided.. [optional]  # noqa: E501
-            method_detail (str): Additional details about the method by which the profile was subscribed to SMS marketing. This may be empty if no details were provided.. [optional]  # noqa: E501
-            suppressions (EmailMarketingSuppression): [optional]  # noqa: E501
-            list_suppressions (EmailMarketingListSuppression): [optional]  # noqa: E501
-            double_optin (bool): Whether the profile was subscribed to email marketing using a double opt-in.. [optional]  # noqa: E501
-            timestamp (datetime): The timestamp when consent record or updated for email marketing, in ISO 8601 format (YYYY-MM-DDTHH:MM:SS.mmmmmm).. [optional]  # noqa: E501
+            phone_number (str, none_type): Phone number to create subscription and SMS consent record for, in E.164 format.. [optional]  # noqa: E501
+            properties ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}): Profile properties to set on the newly subscribed profile.. [optional]  # noqa: E501
+            email (str, none_type): Email address to create subscription and email consent record for.. [optional]  # noqa: E501
+            custom_source (str, none_type): A custom method detail or source to store on the consent records for this subscription.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -194,16 +177,15 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.consent = consent
-        self.method = method
+        self.list_id = list_id
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -216,20 +198,19 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, consent, method, *args, **kwargs):  # noqa: E501
-        """EmailMarketing - a model defined in OpenAPI
+    def __init__(self, list_id, *args, **kwargs):  # noqa: E501
+        """OnsiteSubscriptionCreateQueryResourceObjectAttributes - a model defined in OpenAPI
 
         Args:
-            consent (str): The consent status for email marketing.
-            method (str): The method by which the profile was subscribed to email marketing.
+            list_id (str, none_type): The list ID to add the newly subscribed profile to.
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -254,20 +235,18 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            custom_method_detail (str): Additional detail provided by the caller when the profile was subscribed. This may be empty if no details were provided.. [optional]  # noqa: E501
-            method_detail (str): Additional details about the method by which the profile was subscribed to SMS marketing. This may be empty if no details were provided.. [optional]  # noqa: E501
-            suppressions (EmailMarketingSuppression): [optional]  # noqa: E501
-            list_suppressions (EmailMarketingListSuppression): [optional]  # noqa: E501
-            double_optin (bool): Whether the profile was subscribed to email marketing using a double opt-in.. [optional]  # noqa: E501
-            timestamp (datetime): The timestamp when consent record or updated for email marketing, in ISO 8601 format (YYYY-MM-DDTHH:MM:SS.mmmmmm).. [optional]  # noqa: E501
+            phone_number (str, none_type): Phone number to create subscription and SMS consent record for, in E.164 format.. [optional]  # noqa: E501
+            properties ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}): Profile properties to set on the newly subscribed profile.. [optional]  # noqa: E501
+            email (str, none_type): Email address to create subscription and email consent record for.. [optional]  # noqa: E501
+            custom_source (str, none_type): A custom method detail or source to store on the consent records for this subscription.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -289,16 +268,15 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.consent = consent
-        self.method = method
+        self.list_id = list_id
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `klaviyo-api-2.0.1/src/openapi_client/model/email_marketing_list_suppression.py` & `klaviyo-api-2.0.2/src/openapi_client/model/profile_location_latitude.py`

 * *Files 6% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from openapi_client.exceptions import ApiAttributeError
 
 
 
-class EmailMarketingListSuppression(ModelNormal):
+class ProfileLocationLatitude(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -78,44 +78,33 @@
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         return {
-            'timestamp': (datetime,),  # noqa: E501
-            'reason': (str,),  # noqa: E501
-            'list_id': (str,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'timestamp': 'timestamp',  # noqa: E501
-        'reason': 'reason',  # noqa: E501
-        'list_id': 'list_id',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, timestamp, reason, list_id, *args, **kwargs):  # noqa: E501
-        """EmailMarketingListSuppression - a model defined in OpenAPI
-
-        Args:
-            timestamp (datetime): The timestamp when the profile was suppressed from the list, in ISO 8601 format (YYYY-MM-DDTHH:MM:SS.mmmmmm).
-            reason (str): The reason the profile was suppressed from the list.
-            list_id (str): The ID of list to which the suppression applies.
+    def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
+        """ProfileLocationLatitude - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -171,17 +160,14 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.timestamp = timestamp
-        self.reason = reason
-        self.list_id = list_id
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -194,21 +180,16 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, timestamp, reason, list_id, *args, **kwargs):  # noqa: E501
-        """EmailMarketingListSuppression - a model defined in OpenAPI
-
-        Args:
-            timestamp (datetime): The timestamp when the profile was suppressed from the list, in ISO 8601 format (YYYY-MM-DDTHH:MM:SS.mmmmmm).
-            reason (str): The reason the profile was suppressed from the list.
-            list_id (str): The ID of list to which the suppression applies.
+    def __init__(self, *args, **kwargs):  # noqa: E501
+        """ProfileLocationLatitude - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -262,17 +243,14 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.timestamp = timestamp
-        self.reason = reason
-        self.list_id = list_id
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `klaviyo-api-2.0.1/src/openapi_client/model/email_marketing_suppression.py` & `klaviyo-api-2.0.2/src/openapi_client/model/suppression.py`

 * *Files 5% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from openapi_client.exceptions import ApiAttributeError
 
 
 
-class EmailMarketingSuppression(ModelNormal):
+class Suppression(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -78,41 +78,38 @@
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         return {
-            'timestamp': (datetime,),  # noqa: E501
-            'reason': (str,),  # noqa: E501
+            'email': (str,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'timestamp': 'timestamp',  # noqa: E501
-        'reason': 'reason',  # noqa: E501
+        'email': 'email',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, timestamp, reason, *args, **kwargs):  # noqa: E501
-        """EmailMarketingSuppression - a model defined in OpenAPI
+    def _from_openapi_data(cls, email, *args, **kwargs):  # noqa: E501
+        """Suppression - a model defined in OpenAPI
 
         Args:
-            timestamp (datetime): The timestamp when the profile was suppressed from the list, in ISO 8601 format (YYYY-MM-DDTHH:MM:SS.mmmmmm).
-            reason (str): The reason the profile was suppressed from the list.
+            email (str): The email of the profile to suppress / unsuppress.
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -168,16 +165,15 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.timestamp = timestamp
-        self.reason = reason
+        self.email = email
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -190,20 +186,19 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, timestamp, reason, *args, **kwargs):  # noqa: E501
-        """EmailMarketingSuppression - a model defined in OpenAPI
+    def __init__(self, email, *args, **kwargs):  # noqa: E501
+        """Suppression - a model defined in OpenAPI
 
         Args:
-            timestamp (datetime): The timestamp when the profile was suppressed from the list, in ISO 8601 format (YYYY-MM-DDTHH:MM:SS.mmmmmm).
-            reason (str): The reason the profile was suppressed from the list.
+            email (str): The email of the profile to suppress / unsuppress.
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -257,16 +252,15 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.timestamp = timestamp
-        self.reason = reason
+        self.email = email
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `klaviyo-api-2.0.1/src/openapi_client/model/email_message_content.py` & `klaviyo-api-2.0.2/src/openapi_client/model/tag_create_query_resource_object_attributes.py`

 * *Files 7% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from openapi_client.exceptions import ApiAttributeError
 
 
 
-class EmailMessageContent(ModelNormal):
+class TagCreateQueryResourceObjectAttributes(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -78,47 +78,40 @@
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         return {
-            'preview_text': (str,),  # noqa: E501
-            'from_email': (str,),  # noqa: E501
-            'from_name': (str,),  # noqa: E501
-            'subject': (str,),  # noqa: E501
+            'name': (str, none_type,),  # noqa: E501
+            'tag_group_id': (str, none_type,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'preview_text': 'preview_text',  # noqa: E501
-        'from_email': 'from_email',  # noqa: E501
-        'from_name': 'from_name',  # noqa: E501
-        'subject': 'subject',  # noqa: E501
+        'name': 'name',  # noqa: E501
+        'tag_group_id': 'tag_group_id',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, preview_text, from_email, from_name, subject, *args, **kwargs):  # noqa: E501
-        """EmailMessageContent - a model defined in OpenAPI
+    def _from_openapi_data(cls, name, *args, **kwargs):  # noqa: E501
+        """TagCreateQueryResourceObjectAttributes - a model defined in OpenAPI
 
         Args:
-            preview_text (str):
-            from_email (str):
-            from_name (str):
-            subject (str):
+            name (str, none_type): The Tag name
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -143,14 +136,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
+            tag_group_id (str, none_type): The ID of the Tag Group to associate the Tag with. If this field is not specified, the Tag will be associated with the company's Default Tag Group.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -174,18 +168,15 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.preview_text = preview_text
-        self.from_email = from_email
-        self.from_name = from_name
-        self.subject = subject
+        self.name = name
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -198,22 +189,19 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, preview_text, from_email, from_name, subject, *args, **kwargs):  # noqa: E501
-        """EmailMessageContent - a model defined in OpenAPI
+    def __init__(self, name, *args, **kwargs):  # noqa: E501
+        """TagCreateQueryResourceObjectAttributes - a model defined in OpenAPI
 
         Args:
-            preview_text (str):
-            from_email (str):
-            from_name (str):
-            subject (str):
+            name (str, none_type): The Tag name
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -238,14 +226,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
+            tag_group_id (str, none_type): The ID of the Tag Group to associate the Tag with. If this field is not specified, the Tag will be associated with the company's Default Tag Group.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -267,18 +256,15 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.preview_text = preview_text
-        self.from_email = from_email
-        self.from_name = from_name
-        self.subject = subject
+        self.name = name
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `klaviyo-api-2.0.1/src/openapi_client/model/email_tracking_options.py` & `klaviyo-api-2.0.2/src/openapi_client/model/tag_group_update_query_resource_object_attributes.py`

 * *Files 8% similar despite different names*

```diff
@@ -26,20 +26,16 @@
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
 from openapi_client.exceptions import ApiAttributeError
 
 
-def lazy_import():
-    from openapi_client.model.utm_param_info import UtmParamInfo
-    globals()['UtmParamInfo'] = UtmParamInfo
 
-
-class EmailTrackingOptions(ModelNormal):
+class TagGroupUpdateQueryResourceObjectAttributes(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -67,64 +63,55 @@
 
     @cached_property
     def additional_properties_type():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
         """
-        lazy_import()
         return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
 
     _nullable = False
 
     @cached_property
     def openapi_types():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
-        lazy_import()
         return {
-            'is_tracking_clicks': (bool,),  # noqa: E501
-            'utm_params': ([UtmParamInfo],),  # noqa: E501
-            'is_tracking_opens': (bool,),  # noqa: E501
-            'add_utm': (bool,),  # noqa: E501
+            'name': (str, none_type,),  # noqa: E501
+            'return_fields': ([str],),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'is_tracking_clicks': 'is_tracking_clicks',  # noqa: E501
-        'utm_params': 'utm_params',  # noqa: E501
-        'is_tracking_opens': 'is_tracking_opens',  # noqa: E501
-        'add_utm': 'add_utm',  # noqa: E501
+        'name': 'name',  # noqa: E501
+        'return_fields': 'return_fields',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, is_tracking_clicks, utm_params, is_tracking_opens, add_utm, *args, **kwargs):  # noqa: E501
-        """EmailTrackingOptions - a model defined in OpenAPI
+    def _from_openapi_data(cls, name, *args, **kwargs):  # noqa: E501
+        """TagGroupUpdateQueryResourceObjectAttributes - a model defined in OpenAPI
 
         Args:
-            is_tracking_clicks (bool):
-            utm_params ([UtmParamInfo]):
-            is_tracking_opens (bool):
-            add_utm (bool):
+            name (str, none_type): The Tag Group name
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -149,14 +136,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
+            return_fields ([str]): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -180,18 +168,15 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.is_tracking_clicks = is_tracking_clicks
-        self.utm_params = utm_params
-        self.is_tracking_opens = is_tracking_opens
-        self.add_utm = add_utm
+        self.name = name
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -204,22 +189,19 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, is_tracking_clicks, utm_params, is_tracking_opens, add_utm, *args, **kwargs):  # noqa: E501
-        """EmailTrackingOptions - a model defined in OpenAPI
+    def __init__(self, name, *args, **kwargs):  # noqa: E501
+        """TagGroupUpdateQueryResourceObjectAttributes - a model defined in OpenAPI
 
         Args:
-            is_tracking_clicks (bool):
-            utm_params ([UtmParamInfo]):
-            is_tracking_opens (bool):
-            add_utm (bool):
+            name (str, none_type): The Tag Group name
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -244,14 +226,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
+            return_fields ([str]): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -273,18 +256,15 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.is_tracking_clicks = is_tracking_clicks
-        self.utm_params = utm_params
-        self.is_tracking_opens = is_tracking_opens
-        self.add_utm = add_utm
+        self.name = name
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `klaviyo-api-2.0.1/src/openapi_client/model/error_source.py` & `klaviyo-api-2.0.2/src/openapi_client/model/tag_flow_op.py`

 * *Files 3% similar despite different names*

```diff
@@ -26,16 +26,20 @@
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
 from openapi_client.exceptions import ApiAttributeError
 
 
+def lazy_import():
+    from openapi_client.model.tag_flow_op_data_inner import TagFlowOpDataInner
+    globals()['TagFlowOpDataInner'] = TagFlowOpDataInner
 
-class ErrorSource(ModelNormal):
+
+class TagFlowOp(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -63,55 +67,57 @@
 
     @cached_property
     def additional_properties_type():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
         """
+        lazy_import()
         return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
 
     _nullable = False
 
     @cached_property
     def openapi_types():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
+        lazy_import()
         return {
-            'pointer': (str,),  # noqa: E501
+            'data': ([TagFlowOpDataInner],),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'pointer': 'pointer',  # noqa: E501
+        'data': 'data',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """ErrorSource - a model defined in OpenAPI
+    def _from_openapi_data(cls, data, *args, **kwargs):  # noqa: E501
+        """TagFlowOp - a model defined in OpenAPI
 
         Args:
+            data ([TagFlowOpDataInner]):
 
         Keyword Args:
-            pointer (str): A pointer to the source of the error in the request payload.. defaults to "/data"  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
@@ -136,15 +142,14 @@
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
         """
 
-        pointer = kwargs.get('pointer', "/data")
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
 
         self = super(OpenApiModel, cls).__new__(cls)
@@ -166,15 +171,15 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.pointer = pointer
+        self.data = data
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -187,21 +192,21 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, *args, **kwargs):  # noqa: E501
-        """ErrorSource - a model defined in OpenAPI
+    def __init__(self, data, *args, **kwargs):  # noqa: E501
+        """TagFlowOp - a model defined in OpenAPI
 
         Args:
+            data ([TagFlowOpDataInner]):
 
         Keyword Args:
-            pointer (str): A pointer to the source of the error in the request payload.. defaults to "/data"  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
@@ -226,15 +231,14 @@
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
         """
 
-        pointer = kwargs.get('pointer', "/data")
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
 
         if args:
@@ -254,15 +258,15 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.pointer = pointer
+        self.data = data
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `klaviyo-api-2.0.1/src/openapi_client/model/event_create_query.py` & `klaviyo-api-2.0.2/src/openapi_client/model/event_create_query.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.1/src/openapi_client/model/event_create_query_resource_object.py` & `klaviyo-api-2.0.2/src/openapi_client/model/event_create_query_resource_object.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.1/src/openapi_client/model/event_create_query_resource_object_attributes.py` & `klaviyo-api-2.0.2/src/openapi_client/model/event_create_query_resource_object_attributes.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.1/src/openapi_client/model/event_enum.py` & `klaviyo-api-2.0.2/src/openapi_client/model/event_enum.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.1/src/openapi_client/model/flow_action_enum.py` & `klaviyo-api-2.0.2/src/openapi_client/model/list_enum.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from openapi_client.exceptions import ApiAttributeError
 
 
 
-class FlowActionEnum(ModelSimple):
+class ListEnum(ModelSimple):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -49,15 +49,15 @@
           inclusive_minimum, and regex.
       additional_properties_type (tuple): A tuple of classes accepted
           as additional properties values.
     """
 
     allowed_values = {
         ('value',): {
-            'FLOW-ACTION': "flow-action",
+            'LIST': "list",
         },
     }
 
     validations = {
     }
 
     additional_properties_type = None
@@ -96,23 +96,23 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):
-        """FlowActionEnum - a model defined in OpenAPI
+        """ListEnum - a model defined in OpenAPI
 
         Note that value can be passed either in args or in kwargs, but not in both.
 
         Args:
-            args[0] (str): if omitted defaults to "flow-action", must be one of ["flow-action", ]  # noqa: E501
+            args[0] (str): if omitted defaults to "list", must be one of ["list", ]  # noqa: E501
 
         Keyword Args:
-            value (str): if omitted defaults to "flow-action", must be one of ["flow-action", ]  # noqa: E501
+            value (str): if omitted defaults to "list", must be one of ["list", ]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
@@ -145,15 +145,15 @@
 
         if 'value' in kwargs:
             value = kwargs.pop('value')
         elif args:
             args = list(args)
             value = args.pop(0)
         else:
-            value = "flow-action"
+            value = "list"
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
 
         if args:
@@ -186,23 +186,23 @@
                 path_to_item=_path_to_item,
                 valid_classes=(self.__class__,),
             )
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):
-        """FlowActionEnum - a model defined in OpenAPI
+        """ListEnum - a model defined in OpenAPI
 
         Note that value can be passed either in args or in kwargs, but not in both.
 
         Args:
-            args[0] (str): if omitted defaults to "flow-action", must be one of ["flow-action", ]  # noqa: E501
+            args[0] (str): if omitted defaults to "list", must be one of ["list", ]  # noqa: E501
 
         Keyword Args:
-            value (str): if omitted defaults to "flow-action", must be one of ["flow-action", ]  # noqa: E501
+            value (str): if omitted defaults to "list", must be one of ["list", ]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
@@ -237,15 +237,15 @@
 
         if 'value' in kwargs:
             value = kwargs.pop('value')
         elif args:
             args = list(args)
             value = args.pop(0)
         else:
-            value = "flow-action"
+            value = "list"
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
 
         if args:
```

### Comparing `klaviyo-api-2.0.1/src/openapi_client/model/flow_enum.py` & `klaviyo-api-2.0.2/src/openapi_client/model/tag_group_enum.py`

 * *Files 3% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from openapi_client.exceptions import ApiAttributeError
 
 
 
-class FlowEnum(ModelSimple):
+class TagGroupEnum(ModelSimple):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -49,15 +49,15 @@
           inclusive_minimum, and regex.
       additional_properties_type (tuple): A tuple of classes accepted
           as additional properties values.
     """
 
     allowed_values = {
         ('value',): {
-            'FLOW': "flow",
+            'TAG-GROUP': "tag-group",
         },
     }
 
     validations = {
     }
 
     additional_properties_type = None
@@ -96,23 +96,23 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):
-        """FlowEnum - a model defined in OpenAPI
+        """TagGroupEnum - a model defined in OpenAPI
 
         Note that value can be passed either in args or in kwargs, but not in both.
 
         Args:
-            args[0] (str): if omitted defaults to "flow", must be one of ["flow", ]  # noqa: E501
+            args[0] (str): if omitted defaults to "tag-group", must be one of ["tag-group", ]  # noqa: E501
 
         Keyword Args:
-            value (str): if omitted defaults to "flow", must be one of ["flow", ]  # noqa: E501
+            value (str): if omitted defaults to "tag-group", must be one of ["tag-group", ]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
@@ -145,15 +145,15 @@
 
         if 'value' in kwargs:
             value = kwargs.pop('value')
         elif args:
             args = list(args)
             value = args.pop(0)
         else:
-            value = "flow"
+            value = "tag-group"
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
 
         if args:
@@ -186,23 +186,23 @@
                 path_to_item=_path_to_item,
                 valid_classes=(self.__class__,),
             )
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):
-        """FlowEnum - a model defined in OpenAPI
+        """TagGroupEnum - a model defined in OpenAPI
 
         Note that value can be passed either in args or in kwargs, but not in both.
 
         Args:
-            args[0] (str): if omitted defaults to "flow", must be one of ["flow", ]  # noqa: E501
+            args[0] (str): if omitted defaults to "tag-group", must be one of ["tag-group", ]  # noqa: E501
 
         Keyword Args:
-            value (str): if omitted defaults to "flow", must be one of ["flow", ]  # noqa: E501
+            value (str): if omitted defaults to "tag-group", must be one of ["tag-group", ]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
@@ -237,15 +237,15 @@
 
         if 'value' in kwargs:
             value = kwargs.pop('value')
         elif args:
             args = list(args)
             value = args.pop(0)
         else:
-            value = "flow"
+            value = "tag-group"
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
 
         if args:
```

### Comparing `klaviyo-api-2.0.1/src/openapi_client/model/flow_message_enum.py` & `klaviyo-api-2.0.2/src/openapi_client/model/profile_enum.py`

 * *Files 3% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from openapi_client.exceptions import ApiAttributeError
 
 
 
-class FlowMessageEnum(ModelSimple):
+class ProfileEnum(ModelSimple):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -49,15 +49,15 @@
           inclusive_minimum, and regex.
       additional_properties_type (tuple): A tuple of classes accepted
           as additional properties values.
     """
 
     allowed_values = {
         ('value',): {
-            'FLOW-MESSAGE': "flow-message",
+            'PROFILE': "profile",
         },
     }
 
     validations = {
     }
 
     additional_properties_type = None
@@ -96,23 +96,23 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):
-        """FlowMessageEnum - a model defined in OpenAPI
+        """ProfileEnum - a model defined in OpenAPI
 
         Note that value can be passed either in args or in kwargs, but not in both.
 
         Args:
-            args[0] (str): if omitted defaults to "flow-message", must be one of ["flow-message", ]  # noqa: E501
+            args[0] (str): if omitted defaults to "profile", must be one of ["profile", ]  # noqa: E501
 
         Keyword Args:
-            value (str): if omitted defaults to "flow-message", must be one of ["flow-message", ]  # noqa: E501
+            value (str): if omitted defaults to "profile", must be one of ["profile", ]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
@@ -145,15 +145,15 @@
 
         if 'value' in kwargs:
             value = kwargs.pop('value')
         elif args:
             args = list(args)
             value = args.pop(0)
         else:
-            value = "flow-message"
+            value = "profile"
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
 
         if args:
@@ -186,23 +186,23 @@
                 path_to_item=_path_to_item,
                 valid_classes=(self.__class__,),
             )
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):
-        """FlowMessageEnum - a model defined in OpenAPI
+        """ProfileEnum - a model defined in OpenAPI
 
         Note that value can be passed either in args or in kwargs, but not in both.
 
         Args:
-            args[0] (str): if omitted defaults to "flow-message", must be one of ["flow-message", ]  # noqa: E501
+            args[0] (str): if omitted defaults to "profile", must be one of ["profile", ]  # noqa: E501
 
         Keyword Args:
-            value (str): if omitted defaults to "flow-message", must be one of ["flow-message", ]  # noqa: E501
+            value (str): if omitted defaults to "profile", must be one of ["profile", ]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
@@ -237,15 +237,15 @@
 
         if 'value' in kwargs:
             value = kwargs.pop('value')
         elif args:
             args = list(args)
             value = args.pop(0)
         else:
-            value = "flow-message"
+            value = "profile"
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
 
         if args:
```

### Comparing `klaviyo-api-2.0.1/src/openapi_client/model/flow_update_query.py` & `klaviyo-api-2.0.2/src/openapi_client/model/flow_update_query.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.1/src/openapi_client/model/flow_update_query_resource_object.py` & `klaviyo-api-2.0.2/src/openapi_client/model/flow_update_query_resource_object.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.1/src/openapi_client/model/flow_update_query_resource_object_attributes.py` & `klaviyo-api-2.0.2/src/openapi_client/model/flow_update_query_resource_object_attributes.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.1/src/openapi_client/model/get_create_variants_jobs5_xx_response.py` & `klaviyo-api-2.0.2/src/openapi_client/model/get_create_variants_jobs5_xx_response.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.1/src/openapi_client/model/get_create_variants_jobs5_xx_response_errors_inner.py` & `klaviyo-api-2.0.2/src/openapi_client/model/get_create_variants_jobs5_xx_response_errors_inner.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.1/src/openapi_client/model/get_create_variants_jobs5_xx_response_errors_inner_source.py` & `klaviyo-api-2.0.2/src/openapi_client/model/tag_group_create_query_resource_object_attributes.py`

 * *Files 3% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from openapi_client.exceptions import ApiAttributeError
 
 
 
-class GetCreateVariantsJobs5XXResponseErrorsInnerSource(ModelNormal):
+class TagGroupCreateQueryResourceObjectAttributes(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -78,37 +78,40 @@
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         return {
-            'parameter': (str,),  # noqa: E501
-            'pointer': (str,),  # noqa: E501
+            'name': (str, none_type,),  # noqa: E501
+            'exclusive': (bool,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'parameter': 'parameter',  # noqa: E501
-        'pointer': 'pointer',  # noqa: E501
+        'name': 'name',  # noqa: E501
+        'exclusive': 'exclusive',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """GetCreateVariantsJobs5XXResponseErrorsInnerSource - a model defined in OpenAPI
+    def _from_openapi_data(cls, name, *args, **kwargs):  # noqa: E501
+        """TagGroupCreateQueryResourceObjectAttributes - a model defined in OpenAPI
+
+        Args:
+            name (str, none_type): The Tag Group name
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -133,16 +136,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            parameter (str): [optional]  # noqa: E501
-            pointer (str): [optional]  # noqa: E501
+            exclusive (bool): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -166,14 +168,15 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
+        self.name = name
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -186,16 +189,19 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, *args, **kwargs):  # noqa: E501
-        """GetCreateVariantsJobs5XXResponseErrorsInnerSource - a model defined in OpenAPI
+    def __init__(self, name, *args, **kwargs):  # noqa: E501
+        """TagGroupCreateQueryResourceObjectAttributes - a model defined in OpenAPI
+
+        Args:
+            name (str, none_type): The Tag Group name
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -220,16 +226,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            parameter (str): [optional]  # noqa: E501
-            pointer (str): [optional]  # noqa: E501
+            exclusive (bool): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -251,14 +256,15 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
+        self.name = name
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `klaviyo-api-2.0.1/src/openapi_client/model/list_create_query.py` & `klaviyo-api-2.0.2/src/openapi_client/model/list_create_query.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.1/src/openapi_client/model/list_create_query_resource_object.py` & `klaviyo-api-2.0.2/src/openapi_client/model/list_create_query_resource_object.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.1/src/openapi_client/model/list_create_query_resource_object_attributes.py` & `klaviyo-api-2.0.2/src/openapi_client/model/list_create_query_resource_object_attributes.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.1/src/openapi_client/model/list_enum.py` & `klaviyo-api-2.0.2/src/openapi_client/model/segment_enum.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from openapi_client.exceptions import ApiAttributeError
 
 
 
-class ListEnum(ModelSimple):
+class SegmentEnum(ModelSimple):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -49,15 +49,15 @@
           inclusive_minimum, and regex.
       additional_properties_type (tuple): A tuple of classes accepted
           as additional properties values.
     """
 
     allowed_values = {
         ('value',): {
-            'LIST': "list",
+            'SEGMENT': "segment",
         },
     }
 
     validations = {
     }
 
     additional_properties_type = None
@@ -96,23 +96,23 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):
-        """ListEnum - a model defined in OpenAPI
+        """SegmentEnum - a model defined in OpenAPI
 
         Note that value can be passed either in args or in kwargs, but not in both.
 
         Args:
-            args[0] (str): if omitted defaults to "list", must be one of ["list", ]  # noqa: E501
+            args[0] (str): if omitted defaults to "segment", must be one of ["segment", ]  # noqa: E501
 
         Keyword Args:
-            value (str): if omitted defaults to "list", must be one of ["list", ]  # noqa: E501
+            value (str): if omitted defaults to "segment", must be one of ["segment", ]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
@@ -145,15 +145,15 @@
 
         if 'value' in kwargs:
             value = kwargs.pop('value')
         elif args:
             args = list(args)
             value = args.pop(0)
         else:
-            value = "list"
+            value = "segment"
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
 
         if args:
@@ -186,23 +186,23 @@
                 path_to_item=_path_to_item,
                 valid_classes=(self.__class__,),
             )
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):
-        """ListEnum - a model defined in OpenAPI
+        """SegmentEnum - a model defined in OpenAPI
 
         Note that value can be passed either in args or in kwargs, but not in both.
 
         Args:
-            args[0] (str): if omitted defaults to "list", must be one of ["list", ]  # noqa: E501
+            args[0] (str): if omitted defaults to "segment", must be one of ["segment", ]  # noqa: E501
 
         Keyword Args:
-            value (str): if omitted defaults to "list", must be one of ["list", ]  # noqa: E501
+            value (str): if omitted defaults to "segment", must be one of ["segment", ]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
@@ -237,15 +237,15 @@
 
         if 'value' in kwargs:
             value = kwargs.pop('value')
         elif args:
             args = list(args)
             value = args.pop(0)
         else:
-            value = "list"
+            value = "segment"
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
 
         if args:
```

### Comparing `klaviyo-api-2.0.1/src/openapi_client/model/list_members_add_query.py` & `klaviyo-api-2.0.2/src/openapi_client/model/list_members_add_query.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.1/src/openapi_client/model/list_members_add_query_data_inner.py` & `klaviyo-api-2.0.2/src/openapi_client/model/list_members_add_query_data_inner.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.1/src/openapi_client/model/list_members_delete_query.py` & `klaviyo-api-2.0.2/src/openapi_client/model/list_members_delete_query.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.1/src/openapi_client/model/list_partial_update_query.py` & `klaviyo-api-2.0.2/src/openapi_client/model/list_partial_update_query.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.1/src/openapi_client/model/list_partial_update_query_resource_object.py` & `klaviyo-api-2.0.2/src/openapi_client/model/list_partial_update_query_resource_object.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.1/src/openapi_client/model/metric_aggregate_enum.py` & `klaviyo-api-2.0.2/src/openapi_client/model/metric_aggregate_enum.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.1/src/openapi_client/model/metric_aggregate_query.py` & `klaviyo-api-2.0.2/src/openapi_client/model/metric_aggregate_query.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.1/src/openapi_client/model/metric_aggregate_query_resource_object.py` & `klaviyo-api-2.0.2/src/openapi_client/model/metric_aggregate_query_resource_object.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.1/src/openapi_client/model/metric_aggregate_query_resource_object_attributes.py` & `klaviyo-api-2.0.2/src/openapi_client/model/metric_aggregate_query_resource_object_attributes.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.1/src/openapi_client/model/metric_aggregate_row_dto.py` & `klaviyo-api-2.0.2/src/openapi_client/model/subscription_create_job_create_query.py`

 * *Files 8% similar despite different names*

```diff
@@ -26,16 +26,20 @@
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
 from openapi_client.exceptions import ApiAttributeError
 
 
+def lazy_import():
+    from openapi_client.model.subscription_create_job_create_query_resource_object import SubscriptionCreateJobCreateQueryResourceObject
+    globals()['SubscriptionCreateJobCreateQueryResourceObject'] = SubscriptionCreateJobCreateQueryResourceObject
 
-class MetricAggregateRowDTO(ModelNormal):
+
+class SubscriptionCreateJobCreateQuery(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -63,56 +67,55 @@
 
     @cached_property
     def additional_properties_type():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
         """
+        lazy_import()
         return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
 
     _nullable = False
 
     @cached_property
     def openapi_types():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
+        lazy_import()
         return {
-            'measurements': ({str: (bool, date, datetime, dict, float, int, list, str, none_type)},),  # noqa: E501
-            'dimensions': ([str],),  # noqa: E501
+            'data': (SubscriptionCreateJobCreateQueryResourceObject,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'measurements': 'measurements',  # noqa: E501
-        'dimensions': 'dimensions',  # noqa: E501
+        'data': 'data',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, measurements, dimensions, *args, **kwargs):  # noqa: E501
-        """MetricAggregateRowDTO - a model defined in OpenAPI
+    def _from_openapi_data(cls, data, *args, **kwargs):  # noqa: E501
+        """SubscriptionCreateJobCreateQuery - a model defined in OpenAPI
 
         Args:
-            measurements ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}): Dictionary of measurement_key, values
-            dimensions ([str]): List of dimensions associated with this set of measurements
+            data (SubscriptionCreateJobCreateQueryResourceObject):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -168,16 +171,15 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.measurements = measurements
-        self.dimensions = dimensions
+        self.data = data
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -190,20 +192,19 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, measurements, dimensions, *args, **kwargs):  # noqa: E501
-        """MetricAggregateRowDTO - a model defined in OpenAPI
+    def __init__(self, data, *args, **kwargs):  # noqa: E501
+        """SubscriptionCreateJobCreateQuery - a model defined in OpenAPI
 
         Args:
-            measurements ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}): Dictionary of measurement_key, values
-            dimensions ([str]): List of dimensions associated with this set of measurements
+            data (SubscriptionCreateJobCreateQueryResourceObject):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -257,16 +258,15 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.measurements = measurements
-        self.dimensions = dimensions
+        self.data = data
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `klaviyo-api-2.0.1/src/openapi_client/model/metric_create_query.py` & `klaviyo-api-2.0.2/src/openapi_client/model/metric_create_query.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.1/src/openapi_client/model/metric_enum.py` & `klaviyo-api-2.0.2/src/openapi_client/model/tag_enum.py`

 * *Files 3% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from openapi_client.exceptions import ApiAttributeError
 
 
 
-class MetricEnum(ModelSimple):
+class TagEnum(ModelSimple):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -49,15 +49,15 @@
           inclusive_minimum, and regex.
       additional_properties_type (tuple): A tuple of classes accepted
           as additional properties values.
     """
 
     allowed_values = {
         ('value',): {
-            'METRIC': "metric",
+            'TAG': "tag",
         },
     }
 
     validations = {
     }
 
     additional_properties_type = None
@@ -96,23 +96,23 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):
-        """MetricEnum - a model defined in OpenAPI
+        """TagEnum - a model defined in OpenAPI
 
         Note that value can be passed either in args or in kwargs, but not in both.
 
         Args:
-            args[0] (str): if omitted defaults to "metric", must be one of ["metric", ]  # noqa: E501
+            args[0] (str): if omitted defaults to "tag", must be one of ["tag", ]  # noqa: E501
 
         Keyword Args:
-            value (str): if omitted defaults to "metric", must be one of ["metric", ]  # noqa: E501
+            value (str): if omitted defaults to "tag", must be one of ["tag", ]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
@@ -145,15 +145,15 @@
 
         if 'value' in kwargs:
             value = kwargs.pop('value')
         elif args:
             args = list(args)
             value = args.pop(0)
         else:
-            value = "metric"
+            value = "tag"
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
 
         if args:
@@ -186,23 +186,23 @@
                 path_to_item=_path_to_item,
                 valid_classes=(self.__class__,),
             )
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):
-        """MetricEnum - a model defined in OpenAPI
+        """TagEnum - a model defined in OpenAPI
 
         Note that value can be passed either in args or in kwargs, but not in both.
 
         Args:
-            args[0] (str): if omitted defaults to "metric", must be one of ["metric", ]  # noqa: E501
+            args[0] (str): if omitted defaults to "tag", must be one of ["tag", ]  # noqa: E501
 
         Keyword Args:
-            value (str): if omitted defaults to "metric", must be one of ["metric", ]  # noqa: E501
+            value (str): if omitted defaults to "tag", must be one of ["tag", ]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
@@ -237,15 +237,15 @@
 
         if 'value' in kwargs:
             value = kwargs.pop('value')
         elif args:
             args = list(args)
             value = args.pop(0)
         else:
-            value = "metric"
+            value = "tag"
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
 
         if args:
```

### Comparing `klaviyo-api-2.0.1/src/openapi_client/model/object_links.py` & `klaviyo-api-2.0.2/src/openapi_client/model/tag_update_query_resource_object_attributes.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from openapi_client.exceptions import ApiAttributeError
 
 
 
-class ObjectLinks(ModelNormal):
+class TagUpdateQueryResourceObjectAttributes(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -78,38 +78,38 @@
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         return {
-            '_self': (str,),  # noqa: E501
+            'name': (str, none_type,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        '_self': 'self',  # noqa: E501
+        'name': 'name',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, _self, *args, **kwargs):  # noqa: E501
-        """ObjectLinks - a model defined in OpenAPI
+    def _from_openapi_data(cls, name, *args, **kwargs):  # noqa: E501
+        """TagUpdateQueryResourceObjectAttributes - a model defined in OpenAPI
 
         Args:
-            _self (str):
+            name (str, none_type): The Tag name
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -165,15 +165,15 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self._self = _self
+        self.name = name
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -186,19 +186,19 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, _self, *args, **kwargs):  # noqa: E501
-        """ObjectLinks - a model defined in OpenAPI
+    def __init__(self, name, *args, **kwargs):  # noqa: E501
+        """TagUpdateQueryResourceObjectAttributes - a model defined in OpenAPI
 
         Args:
-            _self (str):
+            name (str, none_type): The Tag name
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -252,15 +252,15 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self._self = _self
+        self.name = name
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `klaviyo-api-2.0.1/src/openapi_client/model/onsite_profile_create_query.py` & `klaviyo-api-2.0.2/src/openapi_client/model/onsite_profile_create_query.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.1/src/openapi_client/model/onsite_profile_create_query_resource_object.py` & `klaviyo-api-2.0.2/src/openapi_client/model/onsite_profile_create_query_resource_object.py`

 * *Files 5% similar despite different names*

```diff
@@ -28,18 +28,16 @@
     OpenApiModel
 )
 from openapi_client.exceptions import ApiAttributeError
 
 
 def lazy_import():
     from openapi_client.model.onsite_profile_create_query_resource_object_attributes import OnsiteProfileCreateQueryResourceObjectAttributes
-    from openapi_client.model.onsite_profile_meta import OnsiteProfileMeta
     from openapi_client.model.profile_enum import ProfileEnum
     globals()['OnsiteProfileCreateQueryResourceObjectAttributes'] = OnsiteProfileCreateQueryResourceObjectAttributes
-    globals()['OnsiteProfileMeta'] = OnsiteProfileMeta
     globals()['ProfileEnum'] = ProfileEnum
 
 
 class OnsiteProfileCreateQueryResourceObject(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
@@ -90,26 +88,24 @@
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
             'attributes': (OnsiteProfileCreateQueryResourceObjectAttributes,),  # noqa: E501
             'type': (ProfileEnum,),  # noqa: E501
-            'meta': (OnsiteProfileMeta,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
         'attributes': 'attributes',  # noqa: E501
         'type': 'type',  # noqa: E501
-        'meta': 'meta',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
@@ -149,15 +145,14 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            meta (OnsiteProfileMeta): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -241,15 +236,14 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            meta (OnsiteProfileMeta): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `klaviyo-api-2.0.1/src/openapi_client/model/onsite_profile_create_query_resource_object_attributes.py` & `klaviyo-api-2.0.2/src/openapi_client/model/onsite_profile_create_query_resource_object_attributes.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.1/src/openapi_client/model/onsite_profile_meta.py` & `klaviyo-api-2.0.2/src/openapi_client/model/tag_update_query.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,19 +27,19 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from openapi_client.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from openapi_client.model.onsite_profile_meta_identifiers import OnsiteProfileMetaIdentifiers
-    globals()['OnsiteProfileMetaIdentifiers'] = OnsiteProfileMetaIdentifiers
+    from openapi_client.model.tag_update_query_resource_object import TagUpdateQueryResourceObject
+    globals()['TagUpdateQueryResourceObject'] = TagUpdateQueryResourceObject
 
 
-class OnsiteProfileMeta(ModelNormal):
+class TagUpdateQuery(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -84,38 +84,38 @@
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
-            'identifiers': (OnsiteProfileMetaIdentifiers,),  # noqa: E501
+            'data': (TagUpdateQueryResourceObject,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'identifiers': 'identifiers',  # noqa: E501
+        'data': 'data',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, identifiers, *args, **kwargs):  # noqa: E501
-        """OnsiteProfileMeta - a model defined in OpenAPI
+    def _from_openapi_data(cls, data, *args, **kwargs):  # noqa: E501
+        """TagUpdateQuery - a model defined in OpenAPI
 
         Args:
-            identifiers (OnsiteProfileMetaIdentifiers):
+            data (TagUpdateQueryResourceObject):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -171,15 +171,15 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.identifiers = identifiers
+        self.data = data
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -192,19 +192,19 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, identifiers, *args, **kwargs):  # noqa: E501
-        """OnsiteProfileMeta - a model defined in OpenAPI
+    def __init__(self, data, *args, **kwargs):  # noqa: E501
+        """TagUpdateQuery - a model defined in OpenAPI
 
         Args:
-            identifiers (OnsiteProfileMetaIdentifiers):
+            data (TagUpdateQueryResourceObject):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -258,15 +258,15 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.identifiers = identifiers
+        self.data = data
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `klaviyo-api-2.0.1/src/openapi_client/model/onsite_profile_meta_identifiers.py` & `klaviyo-api-2.0.2/src/openapi_client/model/template_clone_query_resource_object_attributes.py`

 * *Files 9% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from openapi_client.exceptions import ApiAttributeError
 
 
 
-class OnsiteProfileMetaIdentifiers(ModelNormal):
+class TemplateCloneQueryResourceObjectAttributes(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -78,45 +78,42 @@
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         return {
-            'phone_number': (str,),  # noqa: E501
-            'anonymous_id': (str,),  # noqa: E501
-            'email': (str,),  # noqa: E501
-            'kx': (str,),  # noqa: E501
-            'external_id': (str,),  # noqa: E501
-            'id': (str,),  # noqa: E501
+            'id': (str, none_type,),  # noqa: E501
+            'return_fields': ([str],),  # noqa: E501
+            'name': (str, none_type,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'phone_number': 'phone_number',  # noqa: E501
-        'anonymous_id': 'anonymous_id',  # noqa: E501
-        'email': 'email',  # noqa: E501
-        'kx': '_kx',  # noqa: E501
-        'external_id': 'external_id',  # noqa: E501
         'id': 'id',  # noqa: E501
+        'return_fields': 'return_fields',  # noqa: E501
+        'name': 'name',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """OnsiteProfileMetaIdentifiers - a model defined in OpenAPI
+    def _from_openapi_data(cls, id, *args, **kwargs):  # noqa: E501
+        """TemplateCloneQueryResourceObjectAttributes - a model defined in OpenAPI
+
+        Args:
+            id (str, none_type): The ID of template to be cloned
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -141,20 +138,16 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            phone_number (str): Individual's phone number in E.164 format. [optional]  # noqa: E501
-            anonymous_id (str): [optional]  # noqa: E501
-            email (str): Individual's email address. [optional]  # noqa: E501
-            kx (str):  Also known as the `exchange_id`, this is an encrypted identifier used for identifying a profile by Klaviyo's web tracking.  You can use this field as a filter when retrieving profiles via the Get Profiles endpoint. . [optional]  # noqa: E501
-            external_id (str): A unique identifier used by customers to associate Klaviyo profiles with profiles in an external system, such as a point-of-sale system. Format varies based on the external system.. [optional]  # noqa: E501
-            id (str): Primary key that uniquely identifies this profile. Generated by Klaviyo.. [optional]  # noqa: E501
+            return_fields ([str]): Any subset of TemplateResponse fields. [optional]  # noqa: E501
+            name (str, none_type): The name of the template. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -178,14 +171,15 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
+        self.id = id
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -198,16 +192,19 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, *args, **kwargs):  # noqa: E501
-        """OnsiteProfileMetaIdentifiers - a model defined in OpenAPI
+    def __init__(self, id, *args, **kwargs):  # noqa: E501
+        """TemplateCloneQueryResourceObjectAttributes - a model defined in OpenAPI
+
+        Args:
+            id (str, none_type): The ID of template to be cloned
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -232,20 +229,16 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            phone_number (str): Individual's phone number in E.164 format. [optional]  # noqa: E501
-            anonymous_id (str): [optional]  # noqa: E501
-            email (str): Individual's email address. [optional]  # noqa: E501
-            kx (str):  Also known as the `exchange_id`, this is an encrypted identifier used for identifying a profile by Klaviyo's web tracking.  You can use this field as a filter when retrieving profiles via the Get Profiles endpoint. . [optional]  # noqa: E501
-            external_id (str): A unique identifier used by customers to associate Klaviyo profiles with profiles in an external system, such as a point-of-sale system. Format varies based on the external system.. [optional]  # noqa: E501
-            id (str): Primary key that uniquely identifies this profile. Generated by Klaviyo.. [optional]  # noqa: E501
+            return_fields ([str]): Any subset of TemplateResponse fields. [optional]  # noqa: E501
+            name (str, none_type): The name of the template. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -267,14 +260,15 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
+        self.id = id
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `klaviyo-api-2.0.1/src/openapi_client/model/onsite_subscription_create_query.py` & `klaviyo-api-2.0.2/src/openapi_client/model/onsite_subscription_create_query.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.1/src/openapi_client/model/onsite_subscription_create_query_resource_object.py` & `klaviyo-api-2.0.2/src/openapi_client/model/onsite_subscription_create_query_resource_object.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.1/src/openapi_client/model/onsite_subscription_create_query_resource_object_attributes.py` & `klaviyo-api-2.0.2/src/openapi_client/model/template_update_query_resource_object_attributes.py`

 * *Files 7% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from openapi_client.exceptions import ApiAttributeError
 
 
 
-class OnsiteSubscriptionCreateQueryResourceObjectAttributes(ModelNormal):
+class TemplateUpdateQueryResourceObjectAttributes(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -78,46 +78,41 @@
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         return {
-            'list_id': (str, none_type,),  # noqa: E501
-            'phone_number': (str, none_type,),  # noqa: E501
-            'properties': ({str: (bool, date, datetime, dict, float, int, list, str, none_type)},),  # noqa: E501
-            'email': (str, none_type,),  # noqa: E501
-            'custom_source': (str, none_type,),  # noqa: E501
+            'text': (str, none_type,),  # noqa: E501
+            'html': (str, none_type,),  # noqa: E501
+            'name': (str, none_type,),  # noqa: E501
+            'return_fields': ([str],),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'list_id': 'list_id',  # noqa: E501
-        'phone_number': 'phone_number',  # noqa: E501
-        'properties': 'properties',  # noqa: E501
-        'email': 'email',  # noqa: E501
-        'custom_source': 'custom_source',  # noqa: E501
+        'text': 'text',  # noqa: E501
+        'html': 'html',  # noqa: E501
+        'name': 'name',  # noqa: E501
+        'return_fields': 'return_fields',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, list_id, *args, **kwargs):  # noqa: E501
-        """OnsiteSubscriptionCreateQueryResourceObjectAttributes - a model defined in OpenAPI
-
-        Args:
-            list_id (str, none_type): The list ID to add the newly subscribed profile to.
+    def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
+        """TemplateUpdateQueryResourceObjectAttributes - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -142,18 +137,18 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            phone_number (str, none_type): Phone number to create subscription and SMS consent record for, in E.164 format.. [optional]  # noqa: E501
-            properties ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}): Profile properties to set on the newly subscribed profile.. [optional]  # noqa: E501
-            email (str, none_type): Email address to create subscription and email consent record for.. [optional]  # noqa: E501
-            custom_source (str, none_type): A custom method detail or source to store on the consent records for this subscription.. [optional]  # noqa: E501
+            text (str, none_type): The plaintext of the template. [optional]  # noqa: E501
+            html (str, none_type): The HTML of the template. [optional]  # noqa: E501
+            name (str, none_type): The name of the template. [optional]  # noqa: E501
+            return_fields ([str]): Provide fields to limit the returned data. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -177,15 +172,14 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.list_id = list_id
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -198,19 +192,16 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, list_id, *args, **kwargs):  # noqa: E501
-        """OnsiteSubscriptionCreateQueryResourceObjectAttributes - a model defined in OpenAPI
-
-        Args:
-            list_id (str, none_type): The list ID to add the newly subscribed profile to.
+    def __init__(self, *args, **kwargs):  # noqa: E501
+        """TemplateUpdateQueryResourceObjectAttributes - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -235,18 +226,18 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            phone_number (str, none_type): Phone number to create subscription and SMS consent record for, in E.164 format.. [optional]  # noqa: E501
-            properties ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}): Profile properties to set on the newly subscribed profile.. [optional]  # noqa: E501
-            email (str, none_type): Email address to create subscription and email consent record for.. [optional]  # noqa: E501
-            custom_source (str, none_type): A custom method detail or source to store on the consent records for this subscription.. [optional]  # noqa: E501
+            text (str, none_type): The plaintext of the template. [optional]  # noqa: E501
+            html (str, none_type): The HTML of the template. [optional]  # noqa: E501
+            name (str, none_type): The name of the template. [optional]  # noqa: E501
+            return_fields ([str]): Provide fields to limit the returned data. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -268,15 +259,14 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.list_id = list_id
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `klaviyo-api-2.0.1/src/openapi_client/model/predictive_analytics.py` & `klaviyo-api-2.0.2/src/openapi_client/model/tracking_options_sub_object.py`

 * *Files 15% similar despite different names*

```diff
@@ -26,16 +26,20 @@
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
 from openapi_client.exceptions import ApiAttributeError
 
 
+def lazy_import():
+    from openapi_client.model.utm_params_sub_object import UTMParamsSubObject
+    globals()['UTMParamsSubObject'] = UTMParamsSubObject
 
-class PredictiveAnalytics(ModelNormal):
+
+class TrackingOptionsSubObject(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -63,66 +67,58 @@
 
     @cached_property
     def additional_properties_type():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
         """
+        lazy_import()
         return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
 
     _nullable = False
 
     @cached_property
     def openapi_types():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
+        lazy_import()
         return {
-            'predicted_clv': (float,),  # noqa: E501
-            'total_clv': (float,),  # noqa: E501
-            'expected_date_of_next_order': (datetime,),  # noqa: E501
-            'churn_probability': (float,),  # noqa: E501
-            'historic_number_of_orders': (int,),  # noqa: E501
-            'predicted_number_of_orders': (float,),  # noqa: E501
-            'average_days_between_orders': (float,),  # noqa: E501
-            'average_order_value': (float,),  # noqa: E501
-            'historic_clv': (float,),  # noqa: E501
+            'is_tracking_clicks': (bool,),  # noqa: E501
+            'is_add_utm': (bool,),  # noqa: E501
+            'utm_params': ([UTMParamsSubObject],),  # noqa: E501
+            'is_tracking_opens': (bool,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'predicted_clv': 'predicted_clv',  # noqa: E501
-        'total_clv': 'total_clv',  # noqa: E501
-        'expected_date_of_next_order': 'expected_date_of_next_order',  # noqa: E501
-        'churn_probability': 'churn_probability',  # noqa: E501
-        'historic_number_of_orders': 'historic_number_of_orders',  # noqa: E501
-        'predicted_number_of_orders': 'predicted_number_of_orders',  # noqa: E501
-        'average_days_between_orders': 'average_days_between_orders',  # noqa: E501
-        'average_order_value': 'average_order_value',  # noqa: E501
-        'historic_clv': 'historic_clv',  # noqa: E501
+        'is_tracking_clicks': 'is_tracking_clicks',  # noqa: E501
+        'is_add_utm': 'is_add_utm',  # noqa: E501
+        'utm_params': 'utm_params',  # noqa: E501
+        'is_tracking_opens': 'is_tracking_opens',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """PredictiveAnalytics - a model defined in OpenAPI
+        """TrackingOptionsSubObject - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -147,23 +143,18 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            predicted_clv (float): Predicted value of all placed orders in the next 365 days. [optional]  # noqa: E501
-            total_clv (float): Sum of historic and predicted CLV. [optional]  # noqa: E501
-            expected_date_of_next_order (datetime): Expected date of next order, as calculated at the time of their most recent order. [optional]  # noqa: E501
-            churn_probability (float): Probability the customer has churned. [optional]  # noqa: E501
-            historic_number_of_orders (int): Number of already placed orders. [optional]  # noqa: E501
-            predicted_number_of_orders (float): Predicted number of placed orders in the next 365 days. [optional]  # noqa: E501
-            average_days_between_orders (float): Average number of days between orders (None if only one order has been placed). [optional]  # noqa: E501
-            average_order_value (float): Average value of placed orders. [optional]  # noqa: E501
-            historic_clv (float): Total value of all historically placed orders. [optional]  # noqa: E501
+            is_tracking_clicks (bool): Whether the campaign is tracking click events. If not specified, uses company defaults.. [optional]  # noqa: E501
+            is_add_utm (bool): Whether the campaign needs UTM parameters. If set to False, UTM params will not be used.. [optional]  # noqa: E501
+            utm_params ([UTMParamsSubObject]): A list of UTM parameters. If an empty list is given and is_add_utm is True, uses company defaults.. [optional]  # noqa: E501
+            is_tracking_opens (bool): Whether the campaign is tracking open events. If not specified, uses company defaults.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -208,15 +199,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """PredictiveAnalytics - a model defined in OpenAPI
+        """TrackingOptionsSubObject - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -241,23 +232,18 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            predicted_clv (float): Predicted value of all placed orders in the next 365 days. [optional]  # noqa: E501
-            total_clv (float): Sum of historic and predicted CLV. [optional]  # noqa: E501
-            expected_date_of_next_order (datetime): Expected date of next order, as calculated at the time of their most recent order. [optional]  # noqa: E501
-            churn_probability (float): Probability the customer has churned. [optional]  # noqa: E501
-            historic_number_of_orders (int): Number of already placed orders. [optional]  # noqa: E501
-            predicted_number_of_orders (float): Predicted number of placed orders in the next 365 days. [optional]  # noqa: E501
-            average_days_between_orders (float): Average number of days between orders (None if only one order has been placed). [optional]  # noqa: E501
-            average_order_value (float): Average value of placed orders. [optional]  # noqa: E501
-            historic_clv (float): Total value of all historically placed orders. [optional]  # noqa: E501
+            is_tracking_clicks (bool): Whether the campaign is tracking click events. If not specified, uses company defaults.. [optional]  # noqa: E501
+            is_add_utm (bool): Whether the campaign needs UTM parameters. If set to False, UTM params will not be used.. [optional]  # noqa: E501
+            utm_params ([UTMParamsSubObject]): A list of UTM parameters. If an empty list is given and is_add_utm is True, uses company defaults.. [optional]  # noqa: E501
+            is_tracking_opens (bool): Whether the campaign is tracking open events. If not specified, uses company defaults.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `klaviyo-api-2.0.1/src/openapi_client/model/profile_aggregate_enum.py` & `klaviyo-api-2.0.2/src/openapi_client/model/profile_suppression_bulk_create_job_enum.py`

 * *Files 6% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from openapi_client.exceptions import ApiAttributeError
 
 
 
-class ProfileAggregateEnum(ModelSimple):
+class ProfileSuppressionBulkCreateJobEnum(ModelSimple):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -49,15 +49,15 @@
           inclusive_minimum, and regex.
       additional_properties_type (tuple): A tuple of classes accepted
           as additional properties values.
     """
 
     allowed_values = {
         ('value',): {
-            'PROFILE-AGGREGATE': "profile-aggregate",
+            'PROFILE-SUPPRESSION-BULK-CREATE-JOB': "profile-suppression-bulk-create-job",
         },
     }
 
     validations = {
     }
 
     additional_properties_type = None
@@ -96,23 +96,23 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):
-        """ProfileAggregateEnum - a model defined in OpenAPI
+        """ProfileSuppressionBulkCreateJobEnum - a model defined in OpenAPI
 
         Note that value can be passed either in args or in kwargs, but not in both.
 
         Args:
-            args[0] (str): if omitted defaults to "profile-aggregate", must be one of ["profile-aggregate", ]  # noqa: E501
+            args[0] (str): if omitted defaults to "profile-suppression-bulk-create-job", must be one of ["profile-suppression-bulk-create-job", ]  # noqa: E501
 
         Keyword Args:
-            value (str): if omitted defaults to "profile-aggregate", must be one of ["profile-aggregate", ]  # noqa: E501
+            value (str): if omitted defaults to "profile-suppression-bulk-create-job", must be one of ["profile-suppression-bulk-create-job", ]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
@@ -145,15 +145,15 @@
 
         if 'value' in kwargs:
             value = kwargs.pop('value')
         elif args:
             args = list(args)
             value = args.pop(0)
         else:
-            value = "profile-aggregate"
+            value = "profile-suppression-bulk-create-job"
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
 
         if args:
@@ -186,23 +186,23 @@
                 path_to_item=_path_to_item,
                 valid_classes=(self.__class__,),
             )
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):
-        """ProfileAggregateEnum - a model defined in OpenAPI
+        """ProfileSuppressionBulkCreateJobEnum - a model defined in OpenAPI
 
         Note that value can be passed either in args or in kwargs, but not in both.
 
         Args:
-            args[0] (str): if omitted defaults to "profile-aggregate", must be one of ["profile-aggregate", ]  # noqa: E501
+            args[0] (str): if omitted defaults to "profile-suppression-bulk-create-job", must be one of ["profile-suppression-bulk-create-job", ]  # noqa: E501
 
         Keyword Args:
-            value (str): if omitted defaults to "profile-aggregate", must be one of ["profile-aggregate", ]  # noqa: E501
+            value (str): if omitted defaults to "profile-suppression-bulk-create-job", must be one of ["profile-suppression-bulk-create-job", ]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
@@ -237,15 +237,15 @@
 
         if 'value' in kwargs:
             value = kwargs.pop('value')
         elif args:
             args = list(args)
             value = args.pop(0)
         else:
-            value = "profile-aggregate"
+            value = "profile-suppression-bulk-create-job"
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
 
         if args:
```

### Comparing `klaviyo-api-2.0.1/src/openapi_client/model/profile_create_query.py` & `klaviyo-api-2.0.2/src/openapi_client/model/profile_create_query.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.1/src/openapi_client/model/profile_create_query_resource_object.py` & `klaviyo-api-2.0.2/src/openapi_client/model/profile_create_query_resource_object.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.1/src/openapi_client/model/profile_create_query_resource_object_attributes.py` & `klaviyo-api-2.0.2/src/openapi_client/model/profile_create_query_resource_object_attributes.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.1/src/openapi_client/model/profile_enum.py` & `klaviyo-api-2.0.2/src/openapi_client/model/template_enum.py`

 * *Files 5% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from openapi_client.exceptions import ApiAttributeError
 
 
 
-class ProfileEnum(ModelSimple):
+class TemplateEnum(ModelSimple):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -49,15 +49,15 @@
           inclusive_minimum, and regex.
       additional_properties_type (tuple): A tuple of classes accepted
           as additional properties values.
     """
 
     allowed_values = {
         ('value',): {
-            'PROFILE': "profile",
+            'TEMPLATE': "template",
         },
     }
 
     validations = {
     }
 
     additional_properties_type = None
@@ -96,23 +96,23 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):
-        """ProfileEnum - a model defined in OpenAPI
+        """TemplateEnum - a model defined in OpenAPI
 
         Note that value can be passed either in args or in kwargs, but not in both.
 
         Args:
-            args[0] (str): if omitted defaults to "profile", must be one of ["profile", ]  # noqa: E501
+            args[0] (str): if omitted defaults to "template", must be one of ["template", ]  # noqa: E501
 
         Keyword Args:
-            value (str): if omitted defaults to "profile", must be one of ["profile", ]  # noqa: E501
+            value (str): if omitted defaults to "template", must be one of ["template", ]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
@@ -145,15 +145,15 @@
 
         if 'value' in kwargs:
             value = kwargs.pop('value')
         elif args:
             args = list(args)
             value = args.pop(0)
         else:
-            value = "profile"
+            value = "template"
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
 
         if args:
@@ -186,23 +186,23 @@
                 path_to_item=_path_to_item,
                 valid_classes=(self.__class__,),
             )
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):
-        """ProfileEnum - a model defined in OpenAPI
+        """TemplateEnum - a model defined in OpenAPI
 
         Note that value can be passed either in args or in kwargs, but not in both.
 
         Args:
-            args[0] (str): if omitted defaults to "profile", must be one of ["profile", ]  # noqa: E501
+            args[0] (str): if omitted defaults to "template", must be one of ["template", ]  # noqa: E501
 
         Keyword Args:
-            value (str): if omitted defaults to "profile", must be one of ["profile", ]  # noqa: E501
+            value (str): if omitted defaults to "template", must be one of ["template", ]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
@@ -237,15 +237,15 @@
 
         if 'value' in kwargs:
             value = kwargs.pop('value')
         elif args:
             args = list(args)
             value = args.pop(0)
         else:
-            value = "profile"
+            value = "template"
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
 
         if args:
```

### Comparing `klaviyo-api-2.0.1/src/openapi_client/model/profile_location.py` & `klaviyo-api-2.0.2/src/openapi_client/model/profile_location.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.1/src/openapi_client/model/profile_location_latitude.py` & `klaviyo-api-2.0.2/src/openapi_client/model/profile_location_longitude.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from openapi_client.exceptions import ApiAttributeError
 
 
 
-class ProfileLocationLatitude(ModelNormal):
+class ProfileLocationLongitude(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -96,15 +96,15 @@
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """ProfileLocationLatitude - a model defined in OpenAPI
+        """ProfileLocationLongitude - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -181,15 +181,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """ProfileLocationLatitude - a model defined in OpenAPI
+        """ProfileLocationLongitude - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
```

### Comparing `klaviyo-api-2.0.1/src/openapi_client/model/profile_location_longitude.py` & `klaviyo-api-2.0.2/src/openapi_client/model/sto_schedule_options.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from openapi_client.exceptions import ApiAttributeError
 
 
 
-class ProfileLocationLongitude(ModelNormal):
+class STOScheduleOptions(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -78,33 +78,38 @@
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         return {
+            'date': (date,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
+        'date': 'date',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """ProfileLocationLongitude - a model defined in OpenAPI
+    def _from_openapi_data(cls, date, *args, **kwargs):  # noqa: E501
+        """STOScheduleOptions - a model defined in OpenAPI
+
+        Args:
+            date (date): The day to send on
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -160,14 +165,15 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
+        self.date = date
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -180,16 +186,19 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, *args, **kwargs):  # noqa: E501
-        """ProfileLocationLongitude - a model defined in OpenAPI
+    def __init__(self, date, *args, **kwargs):  # noqa: E501
+        """STOScheduleOptions - a model defined in OpenAPI
+
+        Args:
+            date (date): The day to send on
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -243,14 +252,15 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
+        self.date = date
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `klaviyo-api-2.0.1/src/openapi_client/model/profile_partial_update_query.py` & `klaviyo-api-2.0.2/src/openapi_client/model/profile_partial_update_query.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.1/src/openapi_client/model/profile_partial_update_query_resource_object.py` & `klaviyo-api-2.0.2/src/openapi_client/model/profile_partial_update_query_resource_object.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.1/src/openapi_client/model/profile_subscription_bulk_create_job_enum.py` & `klaviyo-api-2.0.2/src/openapi_client/model/profile_subscription_bulk_create_job_enum.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.1/src/openapi_client/model/profile_suppression_bulk_create_job_enum.py` & `klaviyo-api-2.0.2/src/openapi_client/model/profile_unsuppression_bulk_create_job_enum.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from openapi_client.exceptions import ApiAttributeError
 
 
 
-class ProfileSuppressionBulkCreateJobEnum(ModelSimple):
+class ProfileUnsuppressionBulkCreateJobEnum(ModelSimple):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -49,15 +49,15 @@
           inclusive_minimum, and regex.
       additional_properties_type (tuple): A tuple of classes accepted
           as additional properties values.
     """
 
     allowed_values = {
         ('value',): {
-            'PROFILE-SUPPRESSION-BULK-CREATE-JOB': "profile-suppression-bulk-create-job",
+            'PROFILE-UNSUPPRESSION-BULK-CREATE-JOB': "profile-unsuppression-bulk-create-job",
         },
     }
 
     validations = {
     }
 
     additional_properties_type = None
@@ -96,23 +96,23 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):
-        """ProfileSuppressionBulkCreateJobEnum - a model defined in OpenAPI
+        """ProfileUnsuppressionBulkCreateJobEnum - a model defined in OpenAPI
 
         Note that value can be passed either in args or in kwargs, but not in both.
 
         Args:
-            args[0] (str): if omitted defaults to "profile-suppression-bulk-create-job", must be one of ["profile-suppression-bulk-create-job", ]  # noqa: E501
+            args[0] (str): if omitted defaults to "profile-unsuppression-bulk-create-job", must be one of ["profile-unsuppression-bulk-create-job", ]  # noqa: E501
 
         Keyword Args:
-            value (str): if omitted defaults to "profile-suppression-bulk-create-job", must be one of ["profile-suppression-bulk-create-job", ]  # noqa: E501
+            value (str): if omitted defaults to "profile-unsuppression-bulk-create-job", must be one of ["profile-unsuppression-bulk-create-job", ]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
@@ -145,15 +145,15 @@
 
         if 'value' in kwargs:
             value = kwargs.pop('value')
         elif args:
             args = list(args)
             value = args.pop(0)
         else:
-            value = "profile-suppression-bulk-create-job"
+            value = "profile-unsuppression-bulk-create-job"
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
 
         if args:
@@ -186,23 +186,23 @@
                 path_to_item=_path_to_item,
                 valid_classes=(self.__class__,),
             )
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):
-        """ProfileSuppressionBulkCreateJobEnum - a model defined in OpenAPI
+        """ProfileUnsuppressionBulkCreateJobEnum - a model defined in OpenAPI
 
         Note that value can be passed either in args or in kwargs, but not in both.
 
         Args:
-            args[0] (str): if omitted defaults to "profile-suppression-bulk-create-job", must be one of ["profile-suppression-bulk-create-job", ]  # noqa: E501
+            args[0] (str): if omitted defaults to "profile-unsuppression-bulk-create-job", must be one of ["profile-unsuppression-bulk-create-job", ]  # noqa: E501
 
         Keyword Args:
-            value (str): if omitted defaults to "profile-suppression-bulk-create-job", must be one of ["profile-suppression-bulk-create-job", ]  # noqa: E501
+            value (str): if omitted defaults to "profile-unsuppression-bulk-create-job", must be one of ["profile-unsuppression-bulk-create-job", ]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
@@ -237,15 +237,15 @@
 
         if 'value' in kwargs:
             value = kwargs.pop('value')
         elif args:
             args = list(args)
             value = args.pop(0)
         else:
-            value = "profile-suppression-bulk-create-job"
+            value = "profile-unsuppression-bulk-create-job"
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
 
         if args:
```

### Comparing `klaviyo-api-2.0.1/src/openapi_client/model/profile_unsubscription_bulk_create_job_enum.py` & `klaviyo-api-2.0.2/src/openapi_client/model/profile_unsubscription_bulk_create_job_enum.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.1/src/openapi_client/model/profile_unsuppression_bulk_create_job_enum.py` & `klaviyo-api-2.0.2/src/openapi_client/model/segment_partial_update_query_resource_object_attributes.py`

 * *Files 12% similar despite different names*

```diff
@@ -27,92 +27,91 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from openapi_client.exceptions import ApiAttributeError
 
 
 
-class ProfileUnsuppressionBulkCreateJobEnum(ModelSimple):
+class SegmentPartialUpdateQueryResourceObjectAttributes(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
           and the for var_name this is (var_name,). The value is a dict
           with a capitalized key describing the allowed value and an allowed
           value. These dicts store the allowed enum values.
+      attribute_map (dict): The key is attribute name
+          and the value is json key in definition.
+      discriminator_value_class_map (dict): A dict to go from the discriminator
+          variable value to the discriminator class name.
       validations (dict): The key is the tuple path to the attribute
           and the for var_name this is (var_name,). The value is a dict
           that stores validations for max_length, min_length, max_items,
           min_items, exclusive_maximum, inclusive_maximum, exclusive_minimum,
           inclusive_minimum, and regex.
       additional_properties_type (tuple): A tuple of classes accepted
           as additional properties values.
     """
 
     allowed_values = {
-        ('value',): {
-            'PROFILE-UNSUPPRESSION-BULK-CREATE-JOB': "profile-unsuppression-bulk-create-job",
-        },
     }
 
     validations = {
     }
 
-    additional_properties_type = None
+    @cached_property
+    def additional_properties_type():
+        """
+        This must be a method because a model may have properties that are
+        of type self, this must run after the class is loaded
+        """
+        return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
 
     _nullable = False
 
     @cached_property
     def openapi_types():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         return {
-            'value': (str,),
+            'name': (str, none_type,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
-    attribute_map = {}
-
-    read_only_vars = set()
+    attribute_map = {
+        'name': 'name',  # noqa: E501
+    }
 
-    _composed_schemas = None
+    read_only_vars = {
+    }
 
-    required_properties = set([
-        '_data_store',
-        '_check_type',
-        '_spec_property_naming',
-        '_path_to_item',
-        '_configuration',
-        '_visited_composed_classes',
-    ])
+    _composed_schemas = {}
 
+    @classmethod
     @convert_js_args_to_python_args
-    def __init__(self, *args, **kwargs):
-        """ProfileUnsuppressionBulkCreateJobEnum - a model defined in OpenAPI
-
-        Note that value can be passed either in args or in kwargs, but not in both.
+    def _from_openapi_data(cls, name, *args, **kwargs):  # noqa: E501
+        """SegmentPartialUpdateQueryResourceObjectAttributes - a model defined in OpenAPI
 
         Args:
-            args[0] (str): if omitted defaults to "profile-unsuppression-bulk-create-job", must be one of ["profile-unsuppression-bulk-create-job", ]  # noqa: E501
+            name (str, none_type):
 
         Keyword Args:
-            value (str): if omitted defaults to "profile-unsuppression-bulk-create-job", must be one of ["profile-unsuppression-bulk-create-job", ]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
@@ -136,30 +135,23 @@
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
         """
-        # required up here when default value is not given
-        _path_to_item = kwargs.pop('_path_to_item', ())
-
-        if 'value' in kwargs:
-            value = kwargs.pop('value')
-        elif args:
-            args = list(args)
-            value = args.pop(0)
-        else:
-            value = "profile-unsuppression-bulk-create-job"
 
         _check_type = kwargs.pop('_check_type', True)
-        _spec_property_naming = kwargs.pop('_spec_property_naming', False)
+        _spec_property_naming = kwargs.pop('_spec_property_naming', True)
+        _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
 
+        self = super(OpenApiModel, cls).__new__(cls)
+
         if args:
             for arg in args:
                 if isinstance(arg, dict):
                     kwargs.update(arg)
                 else:
                     raise ApiTypeError(
                         "Invalid positional arguments=%s passed to %s. Remove those invalid positional arguments." % (
@@ -172,37 +164,43 @@
 
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
-        self.value = value
-        if kwargs:
-            raise ApiTypeError(
-                "Invalid named arguments=%s passed to %s. Remove those invalid named arguments." % (
-                    kwargs,
-                    self.__class__.__name__,
-                ),
-                path_to_item=_path_to_item,
-                valid_classes=(self.__class__,),
-            )
 
-    @classmethod
-    @convert_js_args_to_python_args
-    def _from_openapi_data(cls, *args, **kwargs):
-        """ProfileUnsuppressionBulkCreateJobEnum - a model defined in OpenAPI
+        self.name = name
+        for var_name, var_value in kwargs.items():
+            if var_name not in self.attribute_map and \
+                        self._configuration is not None and \
+                        self._configuration.discard_unknown_keys and \
+                        self.additional_properties_type is None:
+                # discard variable.
+                continue
+            setattr(self, var_name, var_value)
+        return self
 
-        Note that value can be passed either in args or in kwargs, but not in both.
+    required_properties = set([
+        '_data_store',
+        '_check_type',
+        '_spec_property_naming',
+        '_path_to_item',
+        '_configuration',
+        '_visited_composed_classes',
+    ])
+
+    @convert_js_args_to_python_args
+    def __init__(self, name, *args, **kwargs):  # noqa: E501
+        """SegmentPartialUpdateQueryResourceObjectAttributes - a model defined in OpenAPI
 
         Args:
-            args[0] (str): if omitted defaults to "profile-unsuppression-bulk-create-job", must be one of ["profile-unsuppression-bulk-create-job", ]  # noqa: E501
+            name (str, none_type):
 
         Keyword Args:
-            value (str): if omitted defaults to "profile-unsuppression-bulk-create-job", must be one of ["profile-unsuppression-bulk-create-job", ]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
@@ -226,29 +224,18 @@
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
         """
-        # required up here when default value is not given
-        _path_to_item = kwargs.pop('_path_to_item', ())
-
-        self = super(OpenApiModel, cls).__new__(cls)
-
-        if 'value' in kwargs:
-            value = kwargs.pop('value')
-        elif args:
-            args = list(args)
-            value = args.pop(0)
-        else:
-            value = "profile-unsuppression-bulk-create-job"
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
+        _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
 
         if args:
             for arg in args:
                 if isinstance(arg, dict):
                     kwargs.update(arg)
@@ -264,19 +251,20 @@
 
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
-        self.value = value
-        if kwargs:
-            raise ApiTypeError(
-                "Invalid named arguments=%s passed to %s. Remove those invalid named arguments." % (
-                    kwargs,
-                    self.__class__.__name__,
-                ),
-                path_to_item=_path_to_item,
-                valid_classes=(self.__class__,),
-            )
 
-        return self
+        self.name = name
+        for var_name, var_value in kwargs.items():
+            if var_name not in self.attribute_map and \
+                        self._configuration is not None and \
+                        self._configuration.discard_unknown_keys and \
+                        self.additional_properties_type is None:
+                # discard variable.
+                continue
+            setattr(self, var_name, var_value)
+            if var_name in self.read_only_vars:
+                raise ApiAttributeError(f"`{var_name}` is a read-only attribute. Use `from_openapi_data` to instantiate "
+                                     f"class with read only attributes.")
```

### Comparing `klaviyo-api-2.0.1/src/openapi_client/model/segment_enum.py` & `klaviyo-api-2.0.2/src/openapi_client/model/subscription_enum.py`

 * *Files 10% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from openapi_client.exceptions import ApiAttributeError
 
 
 
-class SegmentEnum(ModelSimple):
+class SubscriptionEnum(ModelSimple):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -49,15 +49,15 @@
           inclusive_minimum, and regex.
       additional_properties_type (tuple): A tuple of classes accepted
           as additional properties values.
     """
 
     allowed_values = {
         ('value',): {
-            'SEGMENT': "segment",
+            'SUBSCRIPTION': "subscription",
         },
     }
 
     validations = {
     }
 
     additional_properties_type = None
@@ -96,23 +96,23 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):
-        """SegmentEnum - a model defined in OpenAPI
+        """SubscriptionEnum - a model defined in OpenAPI
 
         Note that value can be passed either in args or in kwargs, but not in both.
 
         Args:
-            args[0] (str): if omitted defaults to "segment", must be one of ["segment", ]  # noqa: E501
+            args[0] (str): if omitted defaults to "subscription", must be one of ["subscription", ]  # noqa: E501
 
         Keyword Args:
-            value (str): if omitted defaults to "segment", must be one of ["segment", ]  # noqa: E501
+            value (str): if omitted defaults to "subscription", must be one of ["subscription", ]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
@@ -145,15 +145,15 @@
 
         if 'value' in kwargs:
             value = kwargs.pop('value')
         elif args:
             args = list(args)
             value = args.pop(0)
         else:
-            value = "segment"
+            value = "subscription"
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
 
         if args:
@@ -186,23 +186,23 @@
                 path_to_item=_path_to_item,
                 valid_classes=(self.__class__,),
             )
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):
-        """SegmentEnum - a model defined in OpenAPI
+        """SubscriptionEnum - a model defined in OpenAPI
 
         Note that value can be passed either in args or in kwargs, but not in both.
 
         Args:
-            args[0] (str): if omitted defaults to "segment", must be one of ["segment", ]  # noqa: E501
+            args[0] (str): if omitted defaults to "subscription", must be one of ["subscription", ]  # noqa: E501
 
         Keyword Args:
-            value (str): if omitted defaults to "segment", must be one of ["segment", ]  # noqa: E501
+            value (str): if omitted defaults to "subscription", must be one of ["subscription", ]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
@@ -237,15 +237,15 @@
 
         if 'value' in kwargs:
             value = kwargs.pop('value')
         elif args:
             args = list(args)
             value = args.pop(0)
         else:
-            value = "segment"
+            value = "subscription"
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
 
         if args:
```

### Comparing `klaviyo-api-2.0.1/src/openapi_client/model/segment_partial_update_query.py` & `klaviyo-api-2.0.2/src/openapi_client/model/segment_partial_update_query.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.1/src/openapi_client/model/segment_partial_update_query_resource_object.py` & `klaviyo-api-2.0.2/src/openapi_client/model/segment_partial_update_query_resource_object.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.1/src/openapi_client/model/segment_partial_update_query_resource_object_attributes.py` & `klaviyo-api-2.0.2/src/openapi_client/model/tag_segment_op_data_inner.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from openapi_client.exceptions import ApiAttributeError
 
 
 
-class SegmentPartialUpdateQueryResourceObjectAttributes(ModelNormal):
+class TagSegmentOpDataInner(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -52,14 +52,17 @@
           min_items, exclusive_maximum, inclusive_maximum, exclusive_minimum,
           inclusive_minimum, and regex.
       additional_properties_type (tuple): A tuple of classes accepted
           as additional properties values.
     """
 
     allowed_values = {
+        ('type',): {
+            'SEGMENT': "segment",
+        },
     }
 
     validations = {
     }
 
     @cached_property
     def additional_properties_type():
@@ -78,40 +81,43 @@
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         return {
-            'name': (str, none_type,),  # noqa: E501
+            'type': (str,),  # noqa: E501
+            'id': (str,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'name': 'name',  # noqa: E501
+        'type': 'type',  # noqa: E501
+        'id': 'id',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, name, *args, **kwargs):  # noqa: E501
-        """SegmentPartialUpdateQueryResourceObjectAttributes - a model defined in OpenAPI
+    def _from_openapi_data(cls, id, *args, **kwargs):  # noqa: E501
+        """TagSegmentOpDataInner - a model defined in OpenAPI
 
         Args:
-            name (str, none_type):
+            id (str):
 
         Keyword Args:
+            type (str): defaults to "segment", must be one of ["segment", ]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
@@ -136,14 +142,15 @@
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
         """
 
+        type = kwargs.get('type', "segment")
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
 
         self = super(OpenApiModel, cls).__new__(cls)
@@ -165,15 +172,16 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.name = name
+        self.type = type
+        self.id = id
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -186,21 +194,22 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, name, *args, **kwargs):  # noqa: E501
-        """SegmentPartialUpdateQueryResourceObjectAttributes - a model defined in OpenAPI
+    def __init__(self, id, *args, **kwargs):  # noqa: E501
+        """TagSegmentOpDataInner - a model defined in OpenAPI
 
         Args:
-            name (str, none_type):
+            id (str):
 
         Keyword Args:
+            type (str): defaults to "segment", must be one of ["segment", ]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
@@ -225,14 +234,15 @@
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
         """
 
+        type = kwargs.get('type', "segment")
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
 
         if args:
@@ -252,15 +262,16 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.name = name
+        self.type = type
+        self.id = id
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `klaviyo-api-2.0.1/src/openapi_client/model/send_options.py` & `klaviyo-api-2.0.2/src/openapi_client/model/send_options_sub_object.py`

 * *Files 5% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from openapi_client.exceptions import ApiAttributeError
 
 
 
-class SendOptions(ModelNormal):
+class SendOptionsSubObject(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -78,41 +78,35 @@
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         return {
-            'is_transactional': (bool,),  # noqa: E501
             'use_smart_sending': (bool,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'is_transactional': 'is_transactional',  # noqa: E501
         'use_smart_sending': 'use_smart_sending',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, is_transactional, use_smart_sending, *args, **kwargs):  # noqa: E501
-        """SendOptions - a model defined in OpenAPI
-
-        Args:
-            is_transactional (bool):
-            use_smart_sending (bool):
+    def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
+        """SendOptionsSubObject - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -137,14 +131,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
+            use_smart_sending (bool): Use smart sending. Defaults to True. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -168,16 +163,14 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.is_transactional = is_transactional
-        self.use_smart_sending = use_smart_sending
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -190,20 +183,16 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, is_transactional, use_smart_sending, *args, **kwargs):  # noqa: E501
-        """SendOptions - a model defined in OpenAPI
-
-        Args:
-            is_transactional (bool):
-            use_smart_sending (bool):
+    def __init__(self, *args, **kwargs):  # noqa: E501
+        """SendOptionsSubObject - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -228,14 +217,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
+            use_smart_sending (bool): Use smart sending. Defaults to True. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -257,16 +247,14 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.is_transactional = is_transactional
-        self.use_smart_sending = use_smart_sending
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `klaviyo-api-2.0.1/src/openapi_client/model/send_options_sub_object.py` & `klaviyo-api-2.0.2/src/openapi_client/model/tag_campaign_op.py`

 * *Files 5% similar despite different names*

```diff
@@ -26,16 +26,20 @@
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
 from openapi_client.exceptions import ApiAttributeError
 
 
+def lazy_import():
+    from openapi_client.model.tag_campaign_op_data_inner import TagCampaignOpDataInner
+    globals()['TagCampaignOpDataInner'] = TagCampaignOpDataInner
 
-class SendOptionsSubObject(ModelNormal):
+
+class TagCampaignOp(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -63,50 +67,55 @@
 
     @cached_property
     def additional_properties_type():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
         """
+        lazy_import()
         return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
 
     _nullable = False
 
     @cached_property
     def openapi_types():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
+        lazy_import()
         return {
-            'use_smart_sending': (bool,),  # noqa: E501
+            'data': ([TagCampaignOpDataInner],),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'use_smart_sending': 'use_smart_sending',  # noqa: E501
+        'data': 'data',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """SendOptionsSubObject - a model defined in OpenAPI
+    def _from_openapi_data(cls, data, *args, **kwargs):  # noqa: E501
+        """TagCampaignOp - a model defined in OpenAPI
+
+        Args:
+            data ([TagCampaignOpDataInner]):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -131,15 +140,14 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            use_smart_sending (bool): Use smart sending. Defaults to True. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -163,14 +171,15 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
+        self.data = data
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -183,16 +192,19 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, *args, **kwargs):  # noqa: E501
-        """SendOptionsSubObject - a model defined in OpenAPI
+    def __init__(self, data, *args, **kwargs):  # noqa: E501
+        """TagCampaignOp - a model defined in OpenAPI
+
+        Args:
+            data ([TagCampaignOpDataInner]):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -217,15 +229,14 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            use_smart_sending (bool): Use smart sending. Defaults to True. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -247,14 +258,15 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
+        self.data = data
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `klaviyo-api-2.0.1/src/openapi_client/model/send_strategy_sub_object.py` & `klaviyo-api-2.0.2/src/openapi_client/model/send_strategy_sub_object.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.1/src/openapi_client/model/send_time_sub_object.py` & `klaviyo-api-2.0.2/src/openapi_client/model/template_render_query.py`

 * *Files 7% similar despite different names*

```diff
@@ -26,16 +26,20 @@
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
 from openapi_client.exceptions import ApiAttributeError
 
 
+def lazy_import():
+    from openapi_client.model.template_render_query_resource_object import TemplateRenderQueryResourceObject
+    globals()['TemplateRenderQueryResourceObject'] = TemplateRenderQueryResourceObject
 
-class SendTimeSubObject(ModelNormal):
+
+class TemplateRenderQuery(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -63,56 +67,55 @@
 
     @cached_property
     def additional_properties_type():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
         """
+        lazy_import()
         return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
 
     _nullable = False
 
     @cached_property
     def openapi_types():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
+        lazy_import()
         return {
-            'is_local': (bool,),  # noqa: E501
-            'datetime': (datetime,),  # noqa: E501
+            'data': (TemplateRenderQueryResourceObject,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'is_local': 'is_local',  # noqa: E501
-        'datetime': 'datetime',  # noqa: E501
+        'data': 'data',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, is_local, datetime, *args, **kwargs):  # noqa: E501
-        """SendTimeSubObject - a model defined in OpenAPI
+    def _from_openapi_data(cls, data, *args, **kwargs):  # noqa: E501
+        """TemplateRenderQuery - a model defined in OpenAPI
 
         Args:
-            is_local (bool): Whether that datetime is to be a local datetime for the recipient
-            datetime (datetime): The datetime that the message is to be sent
+            data (TemplateRenderQueryResourceObject):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -168,16 +171,15 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.is_local = is_local
-        self.datetime = datetime
+        self.data = data
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -190,20 +192,19 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, is_local, datetime, *args, **kwargs):  # noqa: E501
-        """SendTimeSubObject - a model defined in OpenAPI
+    def __init__(self, data, *args, **kwargs):  # noqa: E501
+        """TemplateRenderQuery - a model defined in OpenAPI
 
         Args:
-            is_local (bool): Whether that datetime is to be a local datetime for the recipient
-            datetime (datetime): The datetime that the message is to be sent
+            data (TemplateRenderQueryResourceObject):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -257,16 +258,15 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.is_local = is_local
-        self.datetime = datetime
+        self.data = data
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `klaviyo-api-2.0.1/src/openapi_client/model/sms_channel.py` & `klaviyo-api-2.0.2/src/openapi_client/model/tag_segment_op.py`

 * *Files 5% similar despite different names*

```diff
@@ -27,19 +27,19 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from openapi_client.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from openapi_client.model.sms_marketing import SMSMarketing
-    globals()['SMSMarketing'] = SMSMarketing
+    from openapi_client.model.tag_segment_op_data_inner import TagSegmentOpDataInner
+    globals()['TagSegmentOpDataInner'] = TagSegmentOpDataInner
 
 
-class SMSChannel(ModelNormal):
+class TagSegmentOp(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -84,35 +84,38 @@
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
-            'marketing': (SMSMarketing,),  # noqa: E501
+            'data': ([TagSegmentOpDataInner],),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'marketing': 'marketing',  # noqa: E501
+        'data': 'data',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """SMSChannel - a model defined in OpenAPI
+    def _from_openapi_data(cls, data, *args, **kwargs):  # noqa: E501
+        """TagSegmentOp - a model defined in OpenAPI
+
+        Args:
+            data ([TagSegmentOpDataInner]):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -137,15 +140,14 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            marketing (SMSMarketing): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -169,14 +171,15 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
+        self.data = data
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -189,16 +192,19 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, *args, **kwargs):  # noqa: E501
-        """SMSChannel - a model defined in OpenAPI
+    def __init__(self, data, *args, **kwargs):  # noqa: E501
+        """TagSegmentOp - a model defined in OpenAPI
+
+        Args:
+            data ([TagSegmentOpDataInner]):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -223,15 +229,14 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            marketing (SMSMarketing): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -253,14 +258,15 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
+        self.data = data
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `klaviyo-api-2.0.1/src/openapi_client/model/sms_marketing.py` & `klaviyo-api-2.0.2/src/openapi_client/model/unsubscription_create_job_create_query.py`

 * *Files 10% similar despite different names*

```diff
@@ -26,16 +26,20 @@
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
 from openapi_client.exceptions import ApiAttributeError
 
 
+def lazy_import():
+    from openapi_client.model.unsubscription_create_job_create_query_resource_object import UnsubscriptionCreateJobCreateQueryResourceObject
+    globals()['UnsubscriptionCreateJobCreateQueryResourceObject'] = UnsubscriptionCreateJobCreateQueryResourceObject
 
-class SMSMarketing(ModelNormal):
+
+class UnsubscriptionCreateJobCreateQuery(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -63,62 +67,55 @@
 
     @cached_property
     def additional_properties_type():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
         """
+        lazy_import()
         return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
 
     _nullable = False
 
     @cached_property
     def openapi_types():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
+        lazy_import()
         return {
-            'consent': (str,),  # noqa: E501
-            'method_detail': (str,),  # noqa: E501
-            'method': (str,),  # noqa: E501
-            'timestamp': (datetime,),  # noqa: E501
+            'data': (UnsubscriptionCreateJobCreateQueryResourceObject,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'consent': 'consent',  # noqa: E501
-        'method_detail': 'method_detail',  # noqa: E501
-        'method': 'method',  # noqa: E501
-        'timestamp': 'timestamp',  # noqa: E501
+        'data': 'data',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, consent, method_detail, method, timestamp, *args, **kwargs):  # noqa: E501
-        """SMSMarketing - a model defined in OpenAPI
+    def _from_openapi_data(cls, data, *args, **kwargs):  # noqa: E501
+        """UnsubscriptionCreateJobCreateQuery - a model defined in OpenAPI
 
         Args:
-            consent (str): The consent status for SMS marketing.
-            method_detail (str): Additional details about the method which the profile was subscribed to SMS marketing. This may be empty if no details were provided.
-            method (str): The method by which the profile was subscribed to SMS marketing.
-            timestamp (datetime): The timestamp when consent record or updated for SMS marketing, in ISO 8601 format (YYYY-MM-DDTHH:MM:SS.mmmmmm).
+            data (UnsubscriptionCreateJobCreateQueryResourceObject):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -174,18 +171,15 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.consent = consent
-        self.method_detail = method_detail
-        self.method = method
-        self.timestamp = timestamp
+        self.data = data
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -198,22 +192,19 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, consent, method_detail, method, timestamp, *args, **kwargs):  # noqa: E501
-        """SMSMarketing - a model defined in OpenAPI
+    def __init__(self, data, *args, **kwargs):  # noqa: E501
+        """UnsubscriptionCreateJobCreateQuery - a model defined in OpenAPI
 
         Args:
-            consent (str): The consent status for SMS marketing.
-            method_detail (str): Additional details about the method which the profile was subscribed to SMS marketing. This may be empty if no details were provided.
-            method (str): The method by which the profile was subscribed to SMS marketing.
-            timestamp (datetime): The timestamp when consent record or updated for SMS marketing, in ISO 8601 format (YYYY-MM-DDTHH:MM:SS.mmmmmm).
+            data (UnsubscriptionCreateJobCreateQueryResourceObject):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -267,18 +258,15 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.consent = consent
-        self.method_detail = method_detail
-        self.method = method
-        self.timestamp = timestamp
+        self.data = data
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `klaviyo-api-2.0.1/src/openapi_client/model/sms_message_content.py` & `klaviyo-api-2.0.2/src/openapi_client/model/tag_list_op.py`

 * *Files 6% similar despite different names*

```diff
@@ -26,16 +26,20 @@
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
 from openapi_client.exceptions import ApiAttributeError
 
 
+def lazy_import():
+    from openapi_client.model.tag_list_op_data_inner import TagListOpDataInner
+    globals()['TagListOpDataInner'] = TagListOpDataInner
 
-class SMSMessageContent(ModelNormal):
+
+class TagListOp(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -63,56 +67,55 @@
 
     @cached_property
     def additional_properties_type():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
         """
+        lazy_import()
         return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
 
     _nullable = False
 
     @cached_property
     def openapi_types():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
+        lazy_import()
         return {
-            'body': (str,),  # noqa: E501
-            'media': (str,),  # noqa: E501
+            'data': ([TagListOpDataInner],),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'body': 'body',  # noqa: E501
-        'media': 'media',  # noqa: E501
+        'data': 'data',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, body, media, *args, **kwargs):  # noqa: E501
-        """SMSMessageContent - a model defined in OpenAPI
+    def _from_openapi_data(cls, data, *args, **kwargs):  # noqa: E501
+        """TagListOp - a model defined in OpenAPI
 
         Args:
-            body (str):
-            media (str):
+            data ([TagListOpDataInner]):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -168,16 +171,15 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.body = body
-        self.media = media
+        self.data = data
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -190,20 +192,19 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, body, media, *args, **kwargs):  # noqa: E501
-        """SMSMessageContent - a model defined in OpenAPI
+    def __init__(self, data, *args, **kwargs):  # noqa: E501
+        """TagListOp - a model defined in OpenAPI
 
         Args:
-            body (str):
-            media (str):
+            data ([TagListOpDataInner]):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -257,16 +258,15 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.body = body
-        self.media = media
+        self.data = data
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `klaviyo-api-2.0.1/src/openapi_client/model/sms_render_options.py` & `klaviyo-api-2.0.2/src/openapi_client/model/template_clone_query.py`

 * *Files 12% similar despite different names*

```diff
@@ -26,16 +26,20 @@
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
 from openapi_client.exceptions import ApiAttributeError
 
 
+def lazy_import():
+    from openapi_client.model.template_clone_query_resource_object import TemplateCloneQueryResourceObject
+    globals()['TemplateCloneQueryResourceObject'] = TemplateCloneQueryResourceObject
 
-class SMSRenderOptions(ModelNormal):
+
+class TemplateCloneQuery(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -63,62 +67,55 @@
 
     @cached_property
     def additional_properties_type():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
         """
+        lazy_import()
         return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
 
     _nullable = False
 
     @cached_property
     def openapi_types():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
+        lazy_import()
         return {
-            'add_opt_out_language': (bool,),  # noqa: E501
-            'shorten_links': (bool,),  # noqa: E501
-            'add_info_link': (bool,),  # noqa: E501
-            'add_org_prefix': (bool,),  # noqa: E501
+            'data': (TemplateCloneQueryResourceObject,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'add_opt_out_language': 'add_opt_out_language',  # noqa: E501
-        'shorten_links': 'shorten_links',  # noqa: E501
-        'add_info_link': 'add_info_link',  # noqa: E501
-        'add_org_prefix': 'add_org_prefix',  # noqa: E501
+        'data': 'data',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, add_opt_out_language, shorten_links, add_info_link, add_org_prefix, *args, **kwargs):  # noqa: E501
-        """SMSRenderOptions - a model defined in OpenAPI
+    def _from_openapi_data(cls, data, *args, **kwargs):  # noqa: E501
+        """TemplateCloneQuery - a model defined in OpenAPI
 
         Args:
-            add_opt_out_language (bool):
-            shorten_links (bool):
-            add_info_link (bool):
-            add_org_prefix (bool):
+            data (TemplateCloneQueryResourceObject):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -174,18 +171,15 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.add_opt_out_language = add_opt_out_language
-        self.shorten_links = shorten_links
-        self.add_info_link = add_info_link
-        self.add_org_prefix = add_org_prefix
+        self.data = data
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -198,22 +192,19 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, add_opt_out_language, shorten_links, add_info_link, add_org_prefix, *args, **kwargs):  # noqa: E501
-        """SMSRenderOptions - a model defined in OpenAPI
+    def __init__(self, data, *args, **kwargs):  # noqa: E501
+        """TemplateCloneQuery - a model defined in OpenAPI
 
         Args:
-            add_opt_out_language (bool):
-            shorten_links (bool):
-            add_info_link (bool):
-            add_org_prefix (bool):
+            data (TemplateCloneQueryResourceObject):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -267,18 +258,15 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.add_opt_out_language = add_opt_out_language
-        self.shorten_links = shorten_links
-        self.add_info_link = add_info_link
-        self.add_org_prefix = add_org_prefix
+        self.data = data
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `klaviyo-api-2.0.1/src/openapi_client/model/sms_tracking_options.py` & `klaviyo-api-2.0.2/src/openapi_client/model/utm_params_sub_object.py`

 * *Files 9% similar despite different names*

```diff
@@ -26,20 +26,16 @@
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
 from openapi_client.exceptions import ApiAttributeError
 
 
-def lazy_import():
-    from openapi_client.model.utm_param_info import UtmParamInfo
-    globals()['UtmParamInfo'] = UtmParamInfo
 
-
-class SMSTrackingOptions(ModelNormal):
+class UTMParamsSubObject(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -67,58 +63,56 @@
 
     @cached_property
     def additional_properties_type():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
         """
-        lazy_import()
         return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
 
     _nullable = False
 
     @cached_property
     def openapi_types():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
-        lazy_import()
         return {
-            'utm_params': ([UtmParamInfo],),  # noqa: E501
-            'add_utm': (bool,),  # noqa: E501
+            'name': (str,),  # noqa: E501
+            'value': (str,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'utm_params': 'utm_params',  # noqa: E501
-        'add_utm': 'add_utm',  # noqa: E501
+        'name': 'name',  # noqa: E501
+        'value': 'value',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, utm_params, add_utm, *args, **kwargs):  # noqa: E501
-        """SMSTrackingOptions - a model defined in OpenAPI
+    def _from_openapi_data(cls, name, value, *args, **kwargs):  # noqa: E501
+        """UTMParamsSubObject - a model defined in OpenAPI
 
         Args:
-            utm_params ([UtmParamInfo]):
-            add_utm (bool):
+            name (str): Name of the UTM param
+            value (str): Value of the UTM param. Can be templated data.
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -174,16 +168,16 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.utm_params = utm_params
-        self.add_utm = add_utm
+        self.name = name
+        self.value = value
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -196,20 +190,20 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, utm_params, add_utm, *args, **kwargs):  # noqa: E501
-        """SMSTrackingOptions - a model defined in OpenAPI
+    def __init__(self, name, value, *args, **kwargs):  # noqa: E501
+        """UTMParamsSubObject - a model defined in OpenAPI
 
         Args:
-            utm_params ([UtmParamInfo]):
-            add_utm (bool):
+            name (str): Name of the UTM param
+            value (str): Value of the UTM param. Can be templated data.
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -263,16 +257,16 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.utm_params = utm_params
-        self.add_utm = add_utm
+        self.name = name
+        self.value = value
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `klaviyo-api-2.0.1/src/openapi_client/model/static_schedule_options.py` & `klaviyo-api-2.0.2/src/openapi_client/model/static_schedule_options.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.1/src/openapi_client/model/sto_schedule_options.py` & `klaviyo-api-2.0.2/src/openapi_client/model/tag_list_op_data_inner.py`

 * *Files 8% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from openapi_client.exceptions import ApiAttributeError
 
 
 
-class STOScheduleOptions(ModelNormal):
+class TagListOpDataInner(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -52,14 +52,17 @@
           min_items, exclusive_maximum, inclusive_maximum, exclusive_minimum,
           inclusive_minimum, and regex.
       additional_properties_type (tuple): A tuple of classes accepted
           as additional properties values.
     """
 
     allowed_values = {
+        ('type',): {
+            'LIST': "list",
+        },
     }
 
     validations = {
     }
 
     @cached_property
     def additional_properties_type():
@@ -78,40 +81,43 @@
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         return {
-            'date': (date,),  # noqa: E501
+            'type': (str,),  # noqa: E501
+            'id': (str,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'date': 'date',  # noqa: E501
+        'type': 'type',  # noqa: E501
+        'id': 'id',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, date, *args, **kwargs):  # noqa: E501
-        """STOScheduleOptions - a model defined in OpenAPI
+    def _from_openapi_data(cls, id, *args, **kwargs):  # noqa: E501
+        """TagListOpDataInner - a model defined in OpenAPI
 
         Args:
-            date (date): The day to send on
+            id (str):
 
         Keyword Args:
+            type (str): defaults to "list", must be one of ["list", ]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
@@ -136,14 +142,15 @@
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
         """
 
+        type = kwargs.get('type', "list")
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
 
         self = super(OpenApiModel, cls).__new__(cls)
@@ -165,15 +172,16 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.date = date
+        self.type = type
+        self.id = id
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -186,21 +194,22 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, date, *args, **kwargs):  # noqa: E501
-        """STOScheduleOptions - a model defined in OpenAPI
+    def __init__(self, id, *args, **kwargs):  # noqa: E501
+        """TagListOpDataInner - a model defined in OpenAPI
 
         Args:
-            date (date): The day to send on
+            id (str):
 
         Keyword Args:
+            type (str): defaults to "list", must be one of ["list", ]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
@@ -225,14 +234,15 @@
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
         """
 
+        type = kwargs.get('type', "list")
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
 
         if args:
@@ -252,15 +262,16 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.date = date
+        self.type = type
+        self.id = id
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `klaviyo-api-2.0.1/src/openapi_client/model/subscription.py` & `klaviyo-api-2.0.2/src/openapi_client/model/subscription.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.1/src/openapi_client/model/subscription_channels.py` & `klaviyo-api-2.0.2/src/openapi_client/model/subscription_channels.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.1/src/openapi_client/model/subscription_create_job_create_query.py` & `klaviyo-api-2.0.2/src/openapi_client/model/suppression_create_job_create_query_resource_object_attributes.py`

 * *Files 5% similar despite different names*

```diff
@@ -27,19 +27,19 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from openapi_client.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from openapi_client.model.subscription_create_job_create_query_resource_object import SubscriptionCreateJobCreateQueryResourceObject
-    globals()['SubscriptionCreateJobCreateQueryResourceObject'] = SubscriptionCreateJobCreateQueryResourceObject
+    from openapi_client.model.suppression import Suppression
+    globals()['Suppression'] = Suppression
 
 
-class SubscriptionCreateJobCreateQuery(ModelNormal):
+class SuppressionCreateJobCreateQueryResourceObjectAttributes(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -84,38 +84,38 @@
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
-            'data': (SubscriptionCreateJobCreateQueryResourceObject,),  # noqa: E501
+            'suppressions': ([Suppression],),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'data': 'data',  # noqa: E501
+        'suppressions': 'suppressions',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, data, *args, **kwargs):  # noqa: E501
-        """SubscriptionCreateJobCreateQuery - a model defined in OpenAPI
+    def _from_openapi_data(cls, suppressions, *args, **kwargs):  # noqa: E501
+        """SuppressionCreateJobCreateQueryResourceObjectAttributes - a model defined in OpenAPI
 
         Args:
-            data (SubscriptionCreateJobCreateQueryResourceObject):
+            suppressions ([Suppression]): One or more suppressions to be created.
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -171,15 +171,15 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.data = data
+        self.suppressions = suppressions
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -192,19 +192,19 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, data, *args, **kwargs):  # noqa: E501
-        """SubscriptionCreateJobCreateQuery - a model defined in OpenAPI
+    def __init__(self, suppressions, *args, **kwargs):  # noqa: E501
+        """SuppressionCreateJobCreateQueryResourceObjectAttributes - a model defined in OpenAPI
 
         Args:
-            data (SubscriptionCreateJobCreateQueryResourceObject):
+            suppressions ([Suppression]): One or more suppressions to be created.
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -258,15 +258,15 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.data = data
+        self.suppressions = suppressions
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `klaviyo-api-2.0.1/src/openapi_client/model/subscription_create_job_create_query_resource_object.py` & `klaviyo-api-2.0.2/src/openapi_client/model/subscription_create_job_create_query_resource_object.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.1/src/openapi_client/model/subscription_create_job_create_query_resource_object_attributes.py` & `klaviyo-api-2.0.2/src/openapi_client/model/subscription_create_job_create_query_resource_object_attributes.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.1/src/openapi_client/model/subscription_enum.py` & `klaviyo-api-2.0.2/src/openapi_client/model/unsubscription_create_job_create_query_resource_object_attributes.py`

 * *Files 20% similar despite different names*

```diff
@@ -27,92 +27,92 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from openapi_client.exceptions import ApiAttributeError
 
 
 
-class SubscriptionEnum(ModelSimple):
+class UnsubscriptionCreateJobCreateQueryResourceObjectAttributes(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
           and the for var_name this is (var_name,). The value is a dict
           with a capitalized key describing the allowed value and an allowed
           value. These dicts store the allowed enum values.
+      attribute_map (dict): The key is attribute name
+          and the value is json key in definition.
+      discriminator_value_class_map (dict): A dict to go from the discriminator
+          variable value to the discriminator class name.
       validations (dict): The key is the tuple path to the attribute
           and the for var_name this is (var_name,). The value is a dict
           that stores validations for max_length, min_length, max_items,
           min_items, exclusive_maximum, inclusive_maximum, exclusive_minimum,
           inclusive_minimum, and regex.
       additional_properties_type (tuple): A tuple of classes accepted
           as additional properties values.
     """
 
     allowed_values = {
-        ('value',): {
-            'SUBSCRIPTION': "subscription",
-        },
     }
 
     validations = {
     }
 
-    additional_properties_type = None
+    @cached_property
+    def additional_properties_type():
+        """
+        This must be a method because a model may have properties that are
+        of type self, this must run after the class is loaded
+        """
+        return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
 
     _nullable = False
 
     @cached_property
     def openapi_types():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         return {
-            'value': (str,),
+            'phone_numbers': ([str],),  # noqa: E501
+            'emails': ([str],),  # noqa: E501
+            'list_id': (str, none_type,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
-    attribute_map = {}
-
-    read_only_vars = set()
+    attribute_map = {
+        'phone_numbers': 'phone_numbers',  # noqa: E501
+        'emails': 'emails',  # noqa: E501
+        'list_id': 'list_id',  # noqa: E501
+    }
 
-    _composed_schemas = None
+    read_only_vars = {
+    }
 
-    required_properties = set([
-        '_data_store',
-        '_check_type',
-        '_spec_property_naming',
-        '_path_to_item',
-        '_configuration',
-        '_visited_composed_classes',
-    ])
+    _composed_schemas = {}
 
+    @classmethod
     @convert_js_args_to_python_args
-    def __init__(self, *args, **kwargs):
-        """SubscriptionEnum - a model defined in OpenAPI
-
-        Note that value can be passed either in args or in kwargs, but not in both.
-
-        Args:
-            args[0] (str): if omitted defaults to "subscription", must be one of ["subscription", ]  # noqa: E501
+    def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
+        """UnsubscriptionCreateJobCreateQueryResourceObjectAttributes - a model defined in OpenAPI
 
         Keyword Args:
-            value (str): if omitted defaults to "subscription", must be one of ["subscription", ]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
@@ -135,31 +135,27 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
+            phone_numbers ([str]): The phone numbers to unsubscribe if any.. [optional]  # noqa: E501
+            emails ([str]): The emails to unsubscribe if any.. [optional]  # noqa: E501
+            list_id (str, none_type): Optional, the list to remove the profiles from. [optional]  # noqa: E501
         """
-        # required up here when default value is not given
-        _path_to_item = kwargs.pop('_path_to_item', ())
-
-        if 'value' in kwargs:
-            value = kwargs.pop('value')
-        elif args:
-            args = list(args)
-            value = args.pop(0)
-        else:
-            value = "subscription"
 
         _check_type = kwargs.pop('_check_type', True)
-        _spec_property_naming = kwargs.pop('_spec_property_naming', False)
+        _spec_property_naming = kwargs.pop('_spec_property_naming', True)
+        _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
 
+        self = super(OpenApiModel, cls).__new__(cls)
+
         if args:
             for arg in args:
                 if isinstance(arg, dict):
                     kwargs.update(arg)
                 else:
                     raise ApiTypeError(
                         "Invalid positional arguments=%s passed to %s. Remove those invalid positional arguments." % (
@@ -172,37 +168,39 @@
 
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
-        self.value = value
-        if kwargs:
-            raise ApiTypeError(
-                "Invalid named arguments=%s passed to %s. Remove those invalid named arguments." % (
-                    kwargs,
-                    self.__class__.__name__,
-                ),
-                path_to_item=_path_to_item,
-                valid_classes=(self.__class__,),
-            )
 
-    @classmethod
-    @convert_js_args_to_python_args
-    def _from_openapi_data(cls, *args, **kwargs):
-        """SubscriptionEnum - a model defined in OpenAPI
+        for var_name, var_value in kwargs.items():
+            if var_name not in self.attribute_map and \
+                        self._configuration is not None and \
+                        self._configuration.discard_unknown_keys and \
+                        self.additional_properties_type is None:
+                # discard variable.
+                continue
+            setattr(self, var_name, var_value)
+        return self
 
-        Note that value can be passed either in args or in kwargs, but not in both.
+    required_properties = set([
+        '_data_store',
+        '_check_type',
+        '_spec_property_naming',
+        '_path_to_item',
+        '_configuration',
+        '_visited_composed_classes',
+    ])
 
-        Args:
-            args[0] (str): if omitted defaults to "subscription", must be one of ["subscription", ]  # noqa: E501
+    @convert_js_args_to_python_args
+    def __init__(self, *args, **kwargs):  # noqa: E501
+        """UnsubscriptionCreateJobCreateQueryResourceObjectAttributes - a model defined in OpenAPI
 
         Keyword Args:
-            value (str): if omitted defaults to "subscription", must be one of ["subscription", ]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
@@ -225,30 +223,22 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
+            phone_numbers ([str]): The phone numbers to unsubscribe if any.. [optional]  # noqa: E501
+            emails ([str]): The emails to unsubscribe if any.. [optional]  # noqa: E501
+            list_id (str, none_type): Optional, the list to remove the profiles from. [optional]  # noqa: E501
         """
-        # required up here when default value is not given
-        _path_to_item = kwargs.pop('_path_to_item', ())
-
-        self = super(OpenApiModel, cls).__new__(cls)
-
-        if 'value' in kwargs:
-            value = kwargs.pop('value')
-        elif args:
-            args = list(args)
-            value = args.pop(0)
-        else:
-            value = "subscription"
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
+        _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
 
         if args:
             for arg in args:
                 if isinstance(arg, dict):
                     kwargs.update(arg)
@@ -264,19 +254,19 @@
 
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
-        self.value = value
-        if kwargs:
-            raise ApiTypeError(
-                "Invalid named arguments=%s passed to %s. Remove those invalid named arguments." % (
-                    kwargs,
-                    self.__class__.__name__,
-                ),
-                path_to_item=_path_to_item,
-                valid_classes=(self.__class__,),
-            )
 
-        return self
+        for var_name, var_value in kwargs.items():
+            if var_name not in self.attribute_map and \
+                        self._configuration is not None and \
+                        self._configuration.discard_unknown_keys and \
+                        self.additional_properties_type is None:
+                # discard variable.
+                continue
+            setattr(self, var_name, var_value)
+            if var_name in self.read_only_vars:
+                raise ApiAttributeError(f"`{var_name}` is a read-only attribute. Use `from_openapi_data` to instantiate "
+                                     f"class with read only attributes.")
```

### Comparing `klaviyo-api-2.0.1/src/openapi_client/model/subscriptions.py` & `klaviyo-api-2.0.2/src/openapi_client/model/tag_create_query.py`

 * *Files 7% similar despite different names*

```diff
@@ -27,21 +27,19 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from openapi_client.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from openapi_client.model.email_channel import EmailChannel
-    from openapi_client.model.sms_channel import SMSChannel
-    globals()['EmailChannel'] = EmailChannel
-    globals()['SMSChannel'] = SMSChannel
+    from openapi_client.model.tag_create_query_resource_object import TagCreateQueryResourceObject
+    globals()['TagCreateQueryResourceObject'] = TagCreateQueryResourceObject
 
 
-class Subscriptions(ModelNormal):
+class TagCreateQuery(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -86,37 +84,38 @@
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
-            'sms': (SMSChannel,),  # noqa: E501
-            'email': (EmailChannel,),  # noqa: E501
+            'data': (TagCreateQueryResourceObject,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'sms': 'sms',  # noqa: E501
-        'email': 'email',  # noqa: E501
+        'data': 'data',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """Subscriptions - a model defined in OpenAPI
+    def _from_openapi_data(cls, data, *args, **kwargs):  # noqa: E501
+        """TagCreateQuery - a model defined in OpenAPI
+
+        Args:
+            data (TagCreateQueryResourceObject):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -141,16 +140,14 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            sms (SMSChannel): [optional]  # noqa: E501
-            email (EmailChannel): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -174,14 +171,15 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
+        self.data = data
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -194,16 +192,19 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, *args, **kwargs):  # noqa: E501
-        """Subscriptions - a model defined in OpenAPI
+    def __init__(self, data, *args, **kwargs):  # noqa: E501
+        """TagCreateQuery - a model defined in OpenAPI
+
+        Args:
+            data (TagCreateQueryResourceObject):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -228,16 +229,14 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            sms (SMSChannel): [optional]  # noqa: E501
-            email (EmailChannel): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -259,14 +258,15 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
+        self.data = data
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `klaviyo-api-2.0.1/src/openapi_client/model/suppression.py` & `klaviyo-api-2.0.2/src/openapi_client/model/unsuppression_create_job_create_query_resource_object_attributes.py`

 * *Files 6% similar despite different names*

```diff
@@ -26,16 +26,20 @@
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
 from openapi_client.exceptions import ApiAttributeError
 
 
+def lazy_import():
+    from openapi_client.model.suppression import Suppression
+    globals()['Suppression'] = Suppression
 
-class Suppression(ModelNormal):
+
+class UnsuppressionCreateJobCreateQueryResourceObjectAttributes(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -63,53 +67,55 @@
 
     @cached_property
     def additional_properties_type():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
         """
+        lazy_import()
         return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
 
     _nullable = False
 
     @cached_property
     def openapi_types():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
+        lazy_import()
         return {
-            'email': (str,),  # noqa: E501
+            'suppressions': ([Suppression],),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'email': 'email',  # noqa: E501
+        'suppressions': 'suppressions',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, email, *args, **kwargs):  # noqa: E501
-        """Suppression - a model defined in OpenAPI
+    def _from_openapi_data(cls, suppressions, *args, **kwargs):  # noqa: E501
+        """UnsuppressionCreateJobCreateQueryResourceObjectAttributes - a model defined in OpenAPI
 
         Args:
-            email (str): The email of the profile to suppress / unsuppress.
+            suppressions ([Suppression]): One or more suppressions to be removed.
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -165,15 +171,15 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.email = email
+        self.suppressions = suppressions
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -186,19 +192,19 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, email, *args, **kwargs):  # noqa: E501
-        """Suppression - a model defined in OpenAPI
+    def __init__(self, suppressions, *args, **kwargs):  # noqa: E501
+        """UnsuppressionCreateJobCreateQueryResourceObjectAttributes - a model defined in OpenAPI
 
         Args:
-            email (str): The email of the profile to suppress / unsuppress.
+            suppressions ([Suppression]): One or more suppressions to be removed.
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -252,15 +258,15 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.email = email
+        self.suppressions = suppressions
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `klaviyo-api-2.0.1/src/openapi_client/model/suppression_create_job_create_query.py` & `klaviyo-api-2.0.2/src/openapi_client/model/suppression_create_job_create_query.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.1/src/openapi_client/model/suppression_create_job_create_query_resource_object.py` & `klaviyo-api-2.0.2/src/openapi_client/model/suppression_create_job_create_query_resource_object.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.1/src/openapi_client/model/suppression_create_job_create_query_resource_object_attributes.py` & `klaviyo-api-2.0.2/src/openapi_client/model/tag_group_create_query.py`

 * *Files 6% similar despite different names*

```diff
@@ -27,19 +27,19 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from openapi_client.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from openapi_client.model.suppression import Suppression
-    globals()['Suppression'] = Suppression
+    from openapi_client.model.tag_group_create_query_resource_object import TagGroupCreateQueryResourceObject
+    globals()['TagGroupCreateQueryResourceObject'] = TagGroupCreateQueryResourceObject
 
 
-class SuppressionCreateJobCreateQueryResourceObjectAttributes(ModelNormal):
+class TagGroupCreateQuery(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -84,38 +84,38 @@
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
-            'suppressions': ([Suppression],),  # noqa: E501
+            'data': (TagGroupCreateQueryResourceObject,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'suppressions': 'suppressions',  # noqa: E501
+        'data': 'data',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, suppressions, *args, **kwargs):  # noqa: E501
-        """SuppressionCreateJobCreateQueryResourceObjectAttributes - a model defined in OpenAPI
+    def _from_openapi_data(cls, data, *args, **kwargs):  # noqa: E501
+        """TagGroupCreateQuery - a model defined in OpenAPI
 
         Args:
-            suppressions ([Suppression]): One or more suppressions to be created.
+            data (TagGroupCreateQueryResourceObject):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -171,15 +171,15 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.suppressions = suppressions
+        self.data = data
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -192,19 +192,19 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, suppressions, *args, **kwargs):  # noqa: E501
-        """SuppressionCreateJobCreateQueryResourceObjectAttributes - a model defined in OpenAPI
+    def __init__(self, data, *args, **kwargs):  # noqa: E501
+        """TagGroupCreateQuery - a model defined in OpenAPI
 
         Args:
-            suppressions ([Suppression]): One or more suppressions to be created.
+            data (TagGroupCreateQueryResourceObject):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -258,15 +258,15 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.suppressions = suppressions
+        self.data = data
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `klaviyo-api-2.0.1/src/openapi_client/model/tag_campaign_op.py` & `klaviyo-api-2.0.2/src/openapi_client/model/tag_group_update_query.py`

 * *Files 5% similar despite different names*

```diff
@@ -27,19 +27,19 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from openapi_client.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from openapi_client.model.tag_campaign_op_data_inner import TagCampaignOpDataInner
-    globals()['TagCampaignOpDataInner'] = TagCampaignOpDataInner
+    from openapi_client.model.tag_group_update_query_resource_object import TagGroupUpdateQueryResourceObject
+    globals()['TagGroupUpdateQueryResourceObject'] = TagGroupUpdateQueryResourceObject
 
 
-class TagCampaignOp(ModelNormal):
+class TagGroupUpdateQuery(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -84,15 +84,15 @@
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
-            'data': ([TagCampaignOpDataInner],),  # noqa: E501
+            'data': (TagGroupUpdateQueryResourceObject,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
@@ -104,18 +104,18 @@
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, data, *args, **kwargs):  # noqa: E501
-        """TagCampaignOp - a model defined in OpenAPI
+        """TagGroupUpdateQuery - a model defined in OpenAPI
 
         Args:
-            data ([TagCampaignOpDataInner]):
+            data (TagGroupUpdateQueryResourceObject):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -193,18 +193,18 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, data, *args, **kwargs):  # noqa: E501
-        """TagCampaignOp - a model defined in OpenAPI
+        """TagGroupUpdateQuery - a model defined in OpenAPI
 
         Args:
-            data ([TagCampaignOpDataInner]):
+            data (TagGroupUpdateQueryResourceObject):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
```

### Comparing `klaviyo-api-2.0.1/src/openapi_client/model/tag_campaign_op_data_inner.py` & `klaviyo-api-2.0.2/src/openapi_client/model/template_render_query_resource_object.py`

 * *Files 9% similar despite different names*

```diff
@@ -26,16 +26,22 @@
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
 from openapi_client.exceptions import ApiAttributeError
 
 
+def lazy_import():
+    from openapi_client.model.template_enum import TemplateEnum
+    from openapi_client.model.template_render_query_resource_object_attributes import TemplateRenderQueryResourceObjectAttributes
+    globals()['TemplateEnum'] = TemplateEnum
+    globals()['TemplateRenderQueryResourceObjectAttributes'] = TemplateRenderQueryResourceObjectAttributes
 
-class TagCampaignOpDataInner(ModelNormal):
+
+class TemplateRenderQueryResourceObject(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -52,72 +58,71 @@
           min_items, exclusive_maximum, inclusive_maximum, exclusive_minimum,
           inclusive_minimum, and regex.
       additional_properties_type (tuple): A tuple of classes accepted
           as additional properties values.
     """
 
     allowed_values = {
-        ('type',): {
-            'CAMPAIGN': "campaign",
-        },
     }
 
     validations = {
     }
 
     @cached_property
     def additional_properties_type():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
         """
+        lazy_import()
         return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
 
     _nullable = False
 
     @cached_property
     def openapi_types():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
+        lazy_import()
         return {
-            'type': (str,),  # noqa: E501
-            'id': (str,),  # noqa: E501
+            'attributes': (TemplateRenderQueryResourceObjectAttributes,),  # noqa: E501
+            'type': (TemplateEnum,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
+        'attributes': 'attributes',  # noqa: E501
         'type': 'type',  # noqa: E501
-        'id': 'id',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, id, *args, **kwargs):  # noqa: E501
-        """TagCampaignOpDataInner - a model defined in OpenAPI
+    def _from_openapi_data(cls, attributes, type, *args, **kwargs):  # noqa: E501
+        """TemplateRenderQueryResourceObject - a model defined in OpenAPI
 
         Args:
-            id (str):
+            attributes (TemplateRenderQueryResourceObjectAttributes):
+            type (TemplateEnum):
 
         Keyword Args:
-            type (str): defaults to "campaign", must be one of ["campaign", ]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
@@ -142,15 +147,14 @@
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
         """
 
-        type = kwargs.get('type', "campaign")
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
 
         self = super(OpenApiModel, cls).__new__(cls)
@@ -172,16 +176,16 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
+        self.attributes = attributes
         self.type = type
-        self.id = id
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -194,22 +198,22 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, id, *args, **kwargs):  # noqa: E501
-        """TagCampaignOpDataInner - a model defined in OpenAPI
+    def __init__(self, attributes, type, *args, **kwargs):  # noqa: E501
+        """TemplateRenderQueryResourceObject - a model defined in OpenAPI
 
         Args:
-            id (str):
+            attributes (TemplateRenderQueryResourceObjectAttributes):
+            type (TemplateEnum):
 
         Keyword Args:
-            type (str): defaults to "campaign", must be one of ["campaign", ]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
@@ -234,15 +238,14 @@
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
         """
 
-        type = kwargs.get('type', "campaign")
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
 
         if args:
@@ -262,16 +265,16 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
+        self.attributes = attributes
         self.type = type
-        self.id = id
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `klaviyo-api-2.0.1/src/openapi_client/model/tag_create_query.py` & `klaviyo-api-2.0.2/src/openapi_client/model/template_create_query.py`

 * *Files 6% similar despite different names*

```diff
@@ -27,19 +27,19 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from openapi_client.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from openapi_client.model.tag_create_query_resource_object import TagCreateQueryResourceObject
-    globals()['TagCreateQueryResourceObject'] = TagCreateQueryResourceObject
+    from openapi_client.model.template_create_query_resource_object import TemplateCreateQueryResourceObject
+    globals()['TemplateCreateQueryResourceObject'] = TemplateCreateQueryResourceObject
 
 
-class TagCreateQuery(ModelNormal):
+class TemplateCreateQuery(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -84,15 +84,15 @@
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
-            'data': (TagCreateQueryResourceObject,),  # noqa: E501
+            'data': (TemplateCreateQueryResourceObject,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
@@ -104,18 +104,18 @@
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, data, *args, **kwargs):  # noqa: E501
-        """TagCreateQuery - a model defined in OpenAPI
+        """TemplateCreateQuery - a model defined in OpenAPI
 
         Args:
-            data (TagCreateQueryResourceObject):
+            data (TemplateCreateQueryResourceObject):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -193,18 +193,18 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, data, *args, **kwargs):  # noqa: E501
-        """TagCreateQuery - a model defined in OpenAPI
+        """TemplateCreateQuery - a model defined in OpenAPI
 
         Args:
-            data (TagCreateQueryResourceObject):
+            data (TemplateCreateQueryResourceObject):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
```

### Comparing `klaviyo-api-2.0.1/src/openapi_client/model/tag_create_query_resource_object.py` & `klaviyo-api-2.0.2/src/openapi_client/model/tag_create_query_resource_object.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.1/src/openapi_client/model/tag_create_query_resource_object_attributes.py` & `klaviyo-api-2.0.2/src/openapi_client/model/unsuppression_create_job_create_query.py`

 * *Files 9% similar despite different names*

```diff
@@ -26,16 +26,20 @@
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
 from openapi_client.exceptions import ApiAttributeError
 
 
+def lazy_import():
+    from openapi_client.model.unsuppression_create_job_create_query_resource_object import UnsuppressionCreateJobCreateQueryResourceObject
+    globals()['UnsuppressionCreateJobCreateQueryResourceObject'] = UnsuppressionCreateJobCreateQueryResourceObject
 
-class TagCreateQueryResourceObjectAttributes(ModelNormal):
+
+class UnsuppressionCreateJobCreateQuery(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -63,55 +67,55 @@
 
     @cached_property
     def additional_properties_type():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
         """
+        lazy_import()
         return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
 
     _nullable = False
 
     @cached_property
     def openapi_types():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
+        lazy_import()
         return {
-            'name': (str, none_type,),  # noqa: E501
-            'tag_group_id': (str, none_type,),  # noqa: E501
+            'data': (UnsuppressionCreateJobCreateQueryResourceObject,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'name': 'name',  # noqa: E501
-        'tag_group_id': 'tag_group_id',  # noqa: E501
+        'data': 'data',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, name, *args, **kwargs):  # noqa: E501
-        """TagCreateQueryResourceObjectAttributes - a model defined in OpenAPI
+    def _from_openapi_data(cls, data, *args, **kwargs):  # noqa: E501
+        """UnsuppressionCreateJobCreateQuery - a model defined in OpenAPI
 
         Args:
-            name (str, none_type): The Tag name
+            data (UnsuppressionCreateJobCreateQueryResourceObject):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -136,15 +140,14 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            tag_group_id (str, none_type): The ID of the Tag Group to associate the Tag with. If this field is not specified, the Tag will be associated with the company's Default Tag Group.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -168,15 +171,15 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.name = name
+        self.data = data
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -189,19 +192,19 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, name, *args, **kwargs):  # noqa: E501
-        """TagCreateQueryResourceObjectAttributes - a model defined in OpenAPI
+    def __init__(self, data, *args, **kwargs):  # noqa: E501
+        """UnsuppressionCreateJobCreateQuery - a model defined in OpenAPI
 
         Args:
-            name (str, none_type): The Tag name
+            data (UnsuppressionCreateJobCreateQueryResourceObject):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -226,15 +229,14 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            tag_group_id (str, none_type): The ID of the Tag Group to associate the Tag with. If this field is not specified, the Tag will be associated with the company's Default Tag Group.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -256,15 +258,15 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.name = name
+        self.data = data
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `klaviyo-api-2.0.1/src/openapi_client/model/tag_enum.py` & `klaviyo-api-2.0.2/src/openapi_client/model/throttled_schedule_options.py`

 * *Files 18% similar despite different names*

```diff
@@ -27,92 +27,94 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from openapi_client.exceptions import ApiAttributeError
 
 
 
-class TagEnum(ModelSimple):
+class ThrottledScheduleOptions(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
           and the for var_name this is (var_name,). The value is a dict
           with a capitalized key describing the allowed value and an allowed
           value. These dicts store the allowed enum values.
+      attribute_map (dict): The key is attribute name
+          and the value is json key in definition.
+      discriminator_value_class_map (dict): A dict to go from the discriminator
+          variable value to the discriminator class name.
       validations (dict): The key is the tuple path to the attribute
           and the for var_name this is (var_name,). The value is a dict
           that stores validations for max_length, min_length, max_items,
           min_items, exclusive_maximum, inclusive_maximum, exclusive_minimum,
           inclusive_minimum, and regex.
       additional_properties_type (tuple): A tuple of classes accepted
           as additional properties values.
     """
 
     allowed_values = {
-        ('value',): {
-            'TAG': "tag",
-        },
     }
 
     validations = {
     }
 
-    additional_properties_type = None
+    @cached_property
+    def additional_properties_type():
+        """
+        This must be a method because a model may have properties that are
+        of type self, this must run after the class is loaded
+        """
+        return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
 
     _nullable = False
 
     @cached_property
     def openapi_types():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         return {
-            'value': (str,),
+            'throttle_percentage': (int,),  # noqa: E501
+            'datetime': (datetime,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
-    attribute_map = {}
-
-    read_only_vars = set()
+    attribute_map = {
+        'throttle_percentage': 'throttle_percentage',  # noqa: E501
+        'datetime': 'datetime',  # noqa: E501
+    }
 
-    _composed_schemas = None
+    read_only_vars = {
+    }
 
-    required_properties = set([
-        '_data_store',
-        '_check_type',
-        '_spec_property_naming',
-        '_path_to_item',
-        '_configuration',
-        '_visited_composed_classes',
-    ])
+    _composed_schemas = {}
 
+    @classmethod
     @convert_js_args_to_python_args
-    def __init__(self, *args, **kwargs):
-        """TagEnum - a model defined in OpenAPI
-
-        Note that value can be passed either in args or in kwargs, but not in both.
+    def _from_openapi_data(cls, throttle_percentage, datetime, *args, **kwargs):  # noqa: E501
+        """ThrottledScheduleOptions - a model defined in OpenAPI
 
         Args:
-            args[0] (str): if omitted defaults to "tag", must be one of ["tag", ]  # noqa: E501
+            throttle_percentage (int): The percentage of recipients per hour to send to. Allowed values: [10, 11, 13, 14, 17, 20, 25, 33, 50]
+            datetime (datetime): The time to send at
 
         Keyword Args:
-            value (str): if omitted defaults to "tag", must be one of ["tag", ]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
@@ -136,30 +138,23 @@
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
         """
-        # required up here when default value is not given
-        _path_to_item = kwargs.pop('_path_to_item', ())
-
-        if 'value' in kwargs:
-            value = kwargs.pop('value')
-        elif args:
-            args = list(args)
-            value = args.pop(0)
-        else:
-            value = "tag"
 
         _check_type = kwargs.pop('_check_type', True)
-        _spec_property_naming = kwargs.pop('_spec_property_naming', False)
+        _spec_property_naming = kwargs.pop('_spec_property_naming', True)
+        _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
 
+        self = super(OpenApiModel, cls).__new__(cls)
+
         if args:
             for arg in args:
                 if isinstance(arg, dict):
                     kwargs.update(arg)
                 else:
                     raise ApiTypeError(
                         "Invalid positional arguments=%s passed to %s. Remove those invalid positional arguments." % (
@@ -172,37 +167,45 @@
 
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
-        self.value = value
-        if kwargs:
-            raise ApiTypeError(
-                "Invalid named arguments=%s passed to %s. Remove those invalid named arguments." % (
-                    kwargs,
-                    self.__class__.__name__,
-                ),
-                path_to_item=_path_to_item,
-                valid_classes=(self.__class__,),
-            )
 
-    @classmethod
-    @convert_js_args_to_python_args
-    def _from_openapi_data(cls, *args, **kwargs):
-        """TagEnum - a model defined in OpenAPI
+        self.throttle_percentage = throttle_percentage
+        self.datetime = datetime
+        for var_name, var_value in kwargs.items():
+            if var_name not in self.attribute_map and \
+                        self._configuration is not None and \
+                        self._configuration.discard_unknown_keys and \
+                        self.additional_properties_type is None:
+                # discard variable.
+                continue
+            setattr(self, var_name, var_value)
+        return self
 
-        Note that value can be passed either in args or in kwargs, but not in both.
+    required_properties = set([
+        '_data_store',
+        '_check_type',
+        '_spec_property_naming',
+        '_path_to_item',
+        '_configuration',
+        '_visited_composed_classes',
+    ])
+
+    @convert_js_args_to_python_args
+    def __init__(self, throttle_percentage, datetime, *args, **kwargs):  # noqa: E501
+        """ThrottledScheduleOptions - a model defined in OpenAPI
 
         Args:
-            args[0] (str): if omitted defaults to "tag", must be one of ["tag", ]  # noqa: E501
+            throttle_percentage (int): The percentage of recipients per hour to send to. Allowed values: [10, 11, 13, 14, 17, 20, 25, 33, 50]
+            datetime (datetime): The time to send at
 
         Keyword Args:
-            value (str): if omitted defaults to "tag", must be one of ["tag", ]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
@@ -226,29 +229,18 @@
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
         """
-        # required up here when default value is not given
-        _path_to_item = kwargs.pop('_path_to_item', ())
-
-        self = super(OpenApiModel, cls).__new__(cls)
-
-        if 'value' in kwargs:
-            value = kwargs.pop('value')
-        elif args:
-            args = list(args)
-            value = args.pop(0)
-        else:
-            value = "tag"
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
+        _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
 
         if args:
             for arg in args:
                 if isinstance(arg, dict):
                     kwargs.update(arg)
@@ -264,19 +256,21 @@
 
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
-        self.value = value
-        if kwargs:
-            raise ApiTypeError(
-                "Invalid named arguments=%s passed to %s. Remove those invalid named arguments." % (
-                    kwargs,
-                    self.__class__.__name__,
-                ),
-                path_to_item=_path_to_item,
-                valid_classes=(self.__class__,),
-            )
 
-        return self
+        self.throttle_percentage = throttle_percentage
+        self.datetime = datetime
+        for var_name, var_value in kwargs.items():
+            if var_name not in self.attribute_map and \
+                        self._configuration is not None and \
+                        self._configuration.discard_unknown_keys and \
+                        self.additional_properties_type is None:
+                # discard variable.
+                continue
+            setattr(self, var_name, var_value)
+            if var_name in self.read_only_vars:
+                raise ApiAttributeError(f"`{var_name}` is a read-only attribute. Use `from_openapi_data` to instantiate "
+                                     f"class with read only attributes.")
```

### Comparing `klaviyo-api-2.0.1/src/openapi_client/model/tag_flow_op.py` & `klaviyo-api-2.0.2/src/openapi_client/model/template_update_query.py`

 * *Files 16% similar despite different names*

```diff
@@ -27,19 +27,19 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from openapi_client.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from openapi_client.model.tag_flow_op_data_inner import TagFlowOpDataInner
-    globals()['TagFlowOpDataInner'] = TagFlowOpDataInner
+    from openapi_client.model.template_update_query_resource_object import TemplateUpdateQueryResourceObject
+    globals()['TemplateUpdateQueryResourceObject'] = TemplateUpdateQueryResourceObject
 
 
-class TagFlowOp(ModelNormal):
+class TemplateUpdateQuery(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -84,15 +84,15 @@
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
-            'data': ([TagFlowOpDataInner],),  # noqa: E501
+            'data': (TemplateUpdateQueryResourceObject,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
@@ -104,18 +104,18 @@
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, data, *args, **kwargs):  # noqa: E501
-        """TagFlowOp - a model defined in OpenAPI
+        """TemplateUpdateQuery - a model defined in OpenAPI
 
         Args:
-            data ([TagFlowOpDataInner]):
+            data (TemplateUpdateQueryResourceObject):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -193,18 +193,18 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, data, *args, **kwargs):  # noqa: E501
-        """TagFlowOp - a model defined in OpenAPI
+        """TemplateUpdateQuery - a model defined in OpenAPI
 
         Args:
-            data ([TagFlowOpDataInner]):
+            data (TemplateUpdateQueryResourceObject):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
```

### Comparing `klaviyo-api-2.0.1/src/openapi_client/model/tag_flow_op_data_inner.py` & `klaviyo-api-2.0.2/src/openapi_client/model/template_render_query_resource_object_attributes.py`

 * *Files 13% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from openapi_client.exceptions import ApiAttributeError
 
 
 
-class TagFlowOpDataInner(ModelNormal):
+class TemplateRenderQueryResourceObjectAttributes(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -52,17 +52,14 @@
           min_items, exclusive_maximum, inclusive_maximum, exclusive_minimum,
           inclusive_minimum, and regex.
       additional_properties_type (tuple): A tuple of classes accepted
           as additional properties values.
     """
 
     allowed_values = {
-        ('type',): {
-            'FLOW': "flow",
-        },
     }
 
     validations = {
     }
 
     @cached_property
     def additional_properties_type():
@@ -81,43 +78,45 @@
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         return {
-            'type': (str,),  # noqa: E501
-            'id': (str,),  # noqa: E501
+            'id': (str, none_type,),  # noqa: E501
+            'context': ({str: (bool, date, datetime, dict, float, int, list, str, none_type)},),  # noqa: E501
+            'return_fields': ([str],),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'type': 'type',  # noqa: E501
         'id': 'id',  # noqa: E501
+        'context': 'context',  # noqa: E501
+        'return_fields': 'return_fields',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, id, *args, **kwargs):  # noqa: E501
-        """TagFlowOpDataInner - a model defined in OpenAPI
+    def _from_openapi_data(cls, id, context, *args, **kwargs):  # noqa: E501
+        """TemplateRenderQueryResourceObjectAttributes - a model defined in OpenAPI
 
         Args:
-            id (str):
+            id (str, none_type): The ID of template
+            context ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}): The context for the template render. This must be a JSON object which has values for any tags used in the template. See [this doc](https://help.klaviyo.com/hc/en-us/articles/115005084927-Template-tags-and-variable-syntax-reference-classic-editor-) for more details.
 
         Keyword Args:
-            type (str): defaults to "flow", must be one of ["flow", ]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
@@ -140,17 +139,17 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
+            return_fields ([str]): Provide fields to limit the returned data. [optional]  # noqa: E501
         """
 
-        type = kwargs.get('type', "flow")
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
 
         self = super(OpenApiModel, cls).__new__(cls)
@@ -172,16 +171,16 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.type = type
         self.id = id
+        self.context = context
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -194,22 +193,22 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, id, *args, **kwargs):  # noqa: E501
-        """TagFlowOpDataInner - a model defined in OpenAPI
+    def __init__(self, id, context, *args, **kwargs):  # noqa: E501
+        """TemplateRenderQueryResourceObjectAttributes - a model defined in OpenAPI
 
         Args:
-            id (str):
+            id (str, none_type): The ID of template
+            context ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}): The context for the template render. This must be a JSON object which has values for any tags used in the template. See [this doc](https://help.klaviyo.com/hc/en-us/articles/115005084927-Template-tags-and-variable-syntax-reference-classic-editor-) for more details.
 
         Keyword Args:
-            type (str): defaults to "flow", must be one of ["flow", ]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
@@ -232,17 +231,17 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
+            return_fields ([str]): Provide fields to limit the returned data. [optional]  # noqa: E501
         """
 
-        type = kwargs.get('type', "flow")
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
 
         if args:
@@ -262,16 +261,16 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.type = type
         self.id = id
+        self.context = context
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `klaviyo-api-2.0.1/src/openapi_client/model/tag_group_create_query.py` & `klaviyo-api-2.0.2/src/openapi_client/model/tag_group_create_query_resource_object.py`

 * *Files 8% similar despite different names*

```diff
@@ -27,19 +27,21 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from openapi_client.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from openapi_client.model.tag_group_create_query_resource_object import TagGroupCreateQueryResourceObject
-    globals()['TagGroupCreateQueryResourceObject'] = TagGroupCreateQueryResourceObject
+    from openapi_client.model.tag_group_create_query_resource_object_attributes import TagGroupCreateQueryResourceObjectAttributes
+    from openapi_client.model.tag_group_enum import TagGroupEnum
+    globals()['TagGroupCreateQueryResourceObjectAttributes'] = TagGroupCreateQueryResourceObjectAttributes
+    globals()['TagGroupEnum'] = TagGroupEnum
 
 
-class TagGroupCreateQuery(ModelNormal):
+class TagGroupCreateQueryResourceObject(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -84,38 +86,41 @@
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
-            'data': (TagGroupCreateQueryResourceObject,),  # noqa: E501
+            'attributes': (TagGroupCreateQueryResourceObjectAttributes,),  # noqa: E501
+            'type': (TagGroupEnum,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'data': 'data',  # noqa: E501
+        'attributes': 'attributes',  # noqa: E501
+        'type': 'type',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, data, *args, **kwargs):  # noqa: E501
-        """TagGroupCreateQuery - a model defined in OpenAPI
+    def _from_openapi_data(cls, attributes, type, *args, **kwargs):  # noqa: E501
+        """TagGroupCreateQueryResourceObject - a model defined in OpenAPI
 
         Args:
-            data (TagGroupCreateQueryResourceObject):
+            attributes (TagGroupCreateQueryResourceObjectAttributes):
+            type (TagGroupEnum):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -171,15 +176,16 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.data = data
+        self.attributes = attributes
+        self.type = type
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -192,19 +198,20 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, data, *args, **kwargs):  # noqa: E501
-        """TagGroupCreateQuery - a model defined in OpenAPI
+    def __init__(self, attributes, type, *args, **kwargs):  # noqa: E501
+        """TagGroupCreateQueryResourceObject - a model defined in OpenAPI
 
         Args:
-            data (TagGroupCreateQueryResourceObject):
+            attributes (TagGroupCreateQueryResourceObjectAttributes):
+            type (TagGroupEnum):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -258,15 +265,16 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.data = data
+        self.attributes = attributes
+        self.type = type
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `klaviyo-api-2.0.1/src/openapi_client/model/tag_group_create_query_resource_object.py` & `klaviyo-api-2.0.2/src/openapi_client/model/tag_group_update_query_resource_object.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,21 +27,21 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from openapi_client.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from openapi_client.model.tag_group_create_query_resource_object_attributes import TagGroupCreateQueryResourceObjectAttributes
     from openapi_client.model.tag_group_enum import TagGroupEnum
-    globals()['TagGroupCreateQueryResourceObjectAttributes'] = TagGroupCreateQueryResourceObjectAttributes
+    from openapi_client.model.tag_group_update_query_resource_object_attributes import TagGroupUpdateQueryResourceObjectAttributes
     globals()['TagGroupEnum'] = TagGroupEnum
+    globals()['TagGroupUpdateQueryResourceObjectAttributes'] = TagGroupUpdateQueryResourceObjectAttributes
 
 
-class TagGroupCreateQueryResourceObject(ModelNormal):
+class TagGroupUpdateQueryResourceObject(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -86,41 +86,44 @@
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
-            'attributes': (TagGroupCreateQueryResourceObjectAttributes,),  # noqa: E501
+            'attributes': (TagGroupUpdateQueryResourceObjectAttributes,),  # noqa: E501
             'type': (TagGroupEnum,),  # noqa: E501
+            'id': (str,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
         'attributes': 'attributes',  # noqa: E501
         'type': 'type',  # noqa: E501
+        'id': 'id',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, attributes, type, *args, **kwargs):  # noqa: E501
-        """TagGroupCreateQueryResourceObject - a model defined in OpenAPI
+    def _from_openapi_data(cls, attributes, type, id, *args, **kwargs):  # noqa: E501
+        """TagGroupUpdateQueryResourceObject - a model defined in OpenAPI
 
         Args:
-            attributes (TagGroupCreateQueryResourceObjectAttributes):
+            attributes (TagGroupUpdateQueryResourceObjectAttributes):
             type (TagGroupEnum):
+            id (str): The Tag Group ID
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -178,14 +181,15 @@
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
         self.attributes = attributes
         self.type = type
+        self.id = id
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -198,20 +202,21 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, attributes, type, *args, **kwargs):  # noqa: E501
-        """TagGroupCreateQueryResourceObject - a model defined in OpenAPI
+    def __init__(self, attributes, type, id, *args, **kwargs):  # noqa: E501
+        """TagGroupUpdateQueryResourceObject - a model defined in OpenAPI
 
         Args:
-            attributes (TagGroupCreateQueryResourceObjectAttributes):
+            attributes (TagGroupUpdateQueryResourceObjectAttributes):
             type (TagGroupEnum):
+            id (str): The Tag Group ID
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -267,14 +272,15 @@
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
         self.attributes = attributes
         self.type = type
+        self.id = id
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `klaviyo-api-2.0.1/src/openapi_client/model/tag_group_create_query_resource_object_attributes.py` & `klaviyo-api-2.0.2/src/openapi_client/model/template_clone_query_resource_object.py`

 * *Files 13% similar despite different names*

```diff
@@ -26,16 +26,22 @@
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
 from openapi_client.exceptions import ApiAttributeError
 
 
+def lazy_import():
+    from openapi_client.model.template_clone_query_resource_object_attributes import TemplateCloneQueryResourceObjectAttributes
+    from openapi_client.model.template_enum import TemplateEnum
+    globals()['TemplateCloneQueryResourceObjectAttributes'] = TemplateCloneQueryResourceObjectAttributes
+    globals()['TemplateEnum'] = TemplateEnum
 
-class TagGroupCreateQueryResourceObjectAttributes(ModelNormal):
+
+class TemplateCloneQueryResourceObject(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -63,55 +69,58 @@
 
     @cached_property
     def additional_properties_type():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
         """
+        lazy_import()
         return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
 
     _nullable = False
 
     @cached_property
     def openapi_types():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
+        lazy_import()
         return {
-            'name': (str, none_type,),  # noqa: E501
-            'exclusive': (bool,),  # noqa: E501
+            'attributes': (TemplateCloneQueryResourceObjectAttributes,),  # noqa: E501
+            'type': (TemplateEnum,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'name': 'name',  # noqa: E501
-        'exclusive': 'exclusive',  # noqa: E501
+        'attributes': 'attributes',  # noqa: E501
+        'type': 'type',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, name, *args, **kwargs):  # noqa: E501
-        """TagGroupCreateQueryResourceObjectAttributes - a model defined in OpenAPI
+    def _from_openapi_data(cls, attributes, type, *args, **kwargs):  # noqa: E501
+        """TemplateCloneQueryResourceObject - a model defined in OpenAPI
 
         Args:
-            name (str, none_type): The Tag Group name
+            attributes (TemplateCloneQueryResourceObjectAttributes):
+            type (TemplateEnum):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -136,15 +145,14 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            exclusive (bool): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -168,15 +176,16 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.name = name
+        self.attributes = attributes
+        self.type = type
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -189,19 +198,20 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, name, *args, **kwargs):  # noqa: E501
-        """TagGroupCreateQueryResourceObjectAttributes - a model defined in OpenAPI
+    def __init__(self, attributes, type, *args, **kwargs):  # noqa: E501
+        """TemplateCloneQueryResourceObject - a model defined in OpenAPI
 
         Args:
-            name (str, none_type): The Tag Group name
+            attributes (TemplateCloneQueryResourceObjectAttributes):
+            type (TemplateEnum):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -226,15 +236,14 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            exclusive (bool): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -256,15 +265,16 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.name = name
+        self.attributes = attributes
+        self.type = type
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `klaviyo-api-2.0.1/src/openapi_client/model/tag_group_enum.py` & `klaviyo-api-2.0.2/src/openapi_client/model/unsubscription_create_job_create_query_resource_object.py`

 * *Files 24% similar despite different names*

```diff
@@ -26,93 +26,103 @@
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
 from openapi_client.exceptions import ApiAttributeError
 
 
+def lazy_import():
+    from openapi_client.model.profile_unsubscription_bulk_create_job_enum import ProfileUnsubscriptionBulkCreateJobEnum
+    from openapi_client.model.unsubscription_create_job_create_query_resource_object_attributes import UnsubscriptionCreateJobCreateQueryResourceObjectAttributes
+    globals()['ProfileUnsubscriptionBulkCreateJobEnum'] = ProfileUnsubscriptionBulkCreateJobEnum
+    globals()['UnsubscriptionCreateJobCreateQueryResourceObjectAttributes'] = UnsubscriptionCreateJobCreateQueryResourceObjectAttributes
 
-class TagGroupEnum(ModelSimple):
+
+class UnsubscriptionCreateJobCreateQueryResourceObject(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
           and the for var_name this is (var_name,). The value is a dict
           with a capitalized key describing the allowed value and an allowed
           value. These dicts store the allowed enum values.
+      attribute_map (dict): The key is attribute name
+          and the value is json key in definition.
+      discriminator_value_class_map (dict): A dict to go from the discriminator
+          variable value to the discriminator class name.
       validations (dict): The key is the tuple path to the attribute
           and the for var_name this is (var_name,). The value is a dict
           that stores validations for max_length, min_length, max_items,
           min_items, exclusive_maximum, inclusive_maximum, exclusive_minimum,
           inclusive_minimum, and regex.
       additional_properties_type (tuple): A tuple of classes accepted
           as additional properties values.
     """
 
     allowed_values = {
-        ('value',): {
-            'TAG-GROUP': "tag-group",
-        },
     }
 
     validations = {
     }
 
-    additional_properties_type = None
+    @cached_property
+    def additional_properties_type():
+        """
+        This must be a method because a model may have properties that are
+        of type self, this must run after the class is loaded
+        """
+        lazy_import()
+        return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
 
     _nullable = False
 
     @cached_property
     def openapi_types():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
+        lazy_import()
         return {
-            'value': (str,),
+            'attributes': (UnsubscriptionCreateJobCreateQueryResourceObjectAttributes,),  # noqa: E501
+            'type': (ProfileUnsubscriptionBulkCreateJobEnum,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
-    attribute_map = {}
-
-    read_only_vars = set()
+    attribute_map = {
+        'attributes': 'attributes',  # noqa: E501
+        'type': 'type',  # noqa: E501
+    }
 
-    _composed_schemas = None
+    read_only_vars = {
+    }
 
-    required_properties = set([
-        '_data_store',
-        '_check_type',
-        '_spec_property_naming',
-        '_path_to_item',
-        '_configuration',
-        '_visited_composed_classes',
-    ])
+    _composed_schemas = {}
 
+    @classmethod
     @convert_js_args_to_python_args
-    def __init__(self, *args, **kwargs):
-        """TagGroupEnum - a model defined in OpenAPI
-
-        Note that value can be passed either in args or in kwargs, but not in both.
+    def _from_openapi_data(cls, attributes, type, *args, **kwargs):  # noqa: E501
+        """UnsubscriptionCreateJobCreateQueryResourceObject - a model defined in OpenAPI
 
         Args:
-            args[0] (str): if omitted defaults to "tag-group", must be one of ["tag-group", ]  # noqa: E501
+            attributes (UnsubscriptionCreateJobCreateQueryResourceObjectAttributes):
+            type (ProfileUnsubscriptionBulkCreateJobEnum):
 
         Keyword Args:
-            value (str): if omitted defaults to "tag-group", must be one of ["tag-group", ]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
@@ -136,30 +146,23 @@
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
         """
-        # required up here when default value is not given
-        _path_to_item = kwargs.pop('_path_to_item', ())
-
-        if 'value' in kwargs:
-            value = kwargs.pop('value')
-        elif args:
-            args = list(args)
-            value = args.pop(0)
-        else:
-            value = "tag-group"
 
         _check_type = kwargs.pop('_check_type', True)
-        _spec_property_naming = kwargs.pop('_spec_property_naming', False)
+        _spec_property_naming = kwargs.pop('_spec_property_naming', True)
+        _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
 
+        self = super(OpenApiModel, cls).__new__(cls)
+
         if args:
             for arg in args:
                 if isinstance(arg, dict):
                     kwargs.update(arg)
                 else:
                     raise ApiTypeError(
                         "Invalid positional arguments=%s passed to %s. Remove those invalid positional arguments." % (
@@ -172,37 +175,45 @@
 
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
-        self.value = value
-        if kwargs:
-            raise ApiTypeError(
-                "Invalid named arguments=%s passed to %s. Remove those invalid named arguments." % (
-                    kwargs,
-                    self.__class__.__name__,
-                ),
-                path_to_item=_path_to_item,
-                valid_classes=(self.__class__,),
-            )
 
-    @classmethod
-    @convert_js_args_to_python_args
-    def _from_openapi_data(cls, *args, **kwargs):
-        """TagGroupEnum - a model defined in OpenAPI
+        self.attributes = attributes
+        self.type = type
+        for var_name, var_value in kwargs.items():
+            if var_name not in self.attribute_map and \
+                        self._configuration is not None and \
+                        self._configuration.discard_unknown_keys and \
+                        self.additional_properties_type is None:
+                # discard variable.
+                continue
+            setattr(self, var_name, var_value)
+        return self
+
+    required_properties = set([
+        '_data_store',
+        '_check_type',
+        '_spec_property_naming',
+        '_path_to_item',
+        '_configuration',
+        '_visited_composed_classes',
+    ])
 
-        Note that value can be passed either in args or in kwargs, but not in both.
+    @convert_js_args_to_python_args
+    def __init__(self, attributes, type, *args, **kwargs):  # noqa: E501
+        """UnsubscriptionCreateJobCreateQueryResourceObject - a model defined in OpenAPI
 
         Args:
-            args[0] (str): if omitted defaults to "tag-group", must be one of ["tag-group", ]  # noqa: E501
+            attributes (UnsubscriptionCreateJobCreateQueryResourceObjectAttributes):
+            type (ProfileUnsubscriptionBulkCreateJobEnum):
 
         Keyword Args:
-            value (str): if omitted defaults to "tag-group", must be one of ["tag-group", ]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
@@ -226,29 +237,18 @@
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
         """
-        # required up here when default value is not given
-        _path_to_item = kwargs.pop('_path_to_item', ())
-
-        self = super(OpenApiModel, cls).__new__(cls)
-
-        if 'value' in kwargs:
-            value = kwargs.pop('value')
-        elif args:
-            args = list(args)
-            value = args.pop(0)
-        else:
-            value = "tag-group"
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
+        _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
 
         if args:
             for arg in args:
                 if isinstance(arg, dict):
                     kwargs.update(arg)
@@ -264,19 +264,21 @@
 
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
-        self.value = value
-        if kwargs:
-            raise ApiTypeError(
-                "Invalid named arguments=%s passed to %s. Remove those invalid named arguments." % (
-                    kwargs,
-                    self.__class__.__name__,
-                ),
-                path_to_item=_path_to_item,
-                valid_classes=(self.__class__,),
-            )
 
-        return self
+        self.attributes = attributes
+        self.type = type
+        for var_name, var_value in kwargs.items():
+            if var_name not in self.attribute_map and \
+                        self._configuration is not None and \
+                        self._configuration.discard_unknown_keys and \
+                        self.additional_properties_type is None:
+                # discard variable.
+                continue
+            setattr(self, var_name, var_value)
+            if var_name in self.read_only_vars:
+                raise ApiAttributeError(f"`{var_name}` is a read-only attribute. Use `from_openapi_data` to instantiate "
+                                     f"class with read only attributes.")
```

### Comparing `klaviyo-api-2.0.1/src/openapi_client/model/tag_group_update_query.py` & `klaviyo-api-2.0.2/src/openapi_client/model/template_create_query_resource_object.py`

 * *Files 8% similar despite different names*

```diff
@@ -27,19 +27,21 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from openapi_client.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from openapi_client.model.tag_group_update_query_resource_object import TagGroupUpdateQueryResourceObject
-    globals()['TagGroupUpdateQueryResourceObject'] = TagGroupUpdateQueryResourceObject
+    from openapi_client.model.template_create_query_resource_object_attributes import TemplateCreateQueryResourceObjectAttributes
+    from openapi_client.model.template_enum import TemplateEnum
+    globals()['TemplateCreateQueryResourceObjectAttributes'] = TemplateCreateQueryResourceObjectAttributes
+    globals()['TemplateEnum'] = TemplateEnum
 
 
-class TagGroupUpdateQuery(ModelNormal):
+class TemplateCreateQueryResourceObject(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -84,38 +86,41 @@
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
-            'data': (TagGroupUpdateQueryResourceObject,),  # noqa: E501
+            'attributes': (TemplateCreateQueryResourceObjectAttributes,),  # noqa: E501
+            'type': (TemplateEnum,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'data': 'data',  # noqa: E501
+        'attributes': 'attributes',  # noqa: E501
+        'type': 'type',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, data, *args, **kwargs):  # noqa: E501
-        """TagGroupUpdateQuery - a model defined in OpenAPI
+    def _from_openapi_data(cls, attributes, type, *args, **kwargs):  # noqa: E501
+        """TemplateCreateQueryResourceObject - a model defined in OpenAPI
 
         Args:
-            data (TagGroupUpdateQueryResourceObject):
+            attributes (TemplateCreateQueryResourceObjectAttributes):
+            type (TemplateEnum):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -171,15 +176,16 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.data = data
+        self.attributes = attributes
+        self.type = type
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -192,19 +198,20 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, data, *args, **kwargs):  # noqa: E501
-        """TagGroupUpdateQuery - a model defined in OpenAPI
+    def __init__(self, attributes, type, *args, **kwargs):  # noqa: E501
+        """TemplateCreateQueryResourceObject - a model defined in OpenAPI
 
         Args:
-            data (TagGroupUpdateQueryResourceObject):
+            attributes (TemplateCreateQueryResourceObjectAttributes):
+            type (TemplateEnum):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -258,15 +265,16 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.data = data
+        self.attributes = attributes
+        self.type = type
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `klaviyo-api-2.0.1/src/openapi_client/model/tag_group_update_query_resource_object.py` & `klaviyo-api-2.0.2/src/openapi_client/model/tag_update_query_resource_object.py`

 * *Files 5% similar despite different names*

```diff
@@ -27,21 +27,21 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from openapi_client.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from openapi_client.model.tag_group_enum import TagGroupEnum
-    from openapi_client.model.tag_group_update_query_resource_object_attributes import TagGroupUpdateQueryResourceObjectAttributes
-    globals()['TagGroupEnum'] = TagGroupEnum
-    globals()['TagGroupUpdateQueryResourceObjectAttributes'] = TagGroupUpdateQueryResourceObjectAttributes
+    from openapi_client.model.tag_enum import TagEnum
+    from openapi_client.model.tag_update_query_resource_object_attributes import TagUpdateQueryResourceObjectAttributes
+    globals()['TagEnum'] = TagEnum
+    globals()['TagUpdateQueryResourceObjectAttributes'] = TagUpdateQueryResourceObjectAttributes
 
 
-class TagGroupUpdateQueryResourceObject(ModelNormal):
+class TagUpdateQueryResourceObject(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -86,16 +86,16 @@
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
-            'attributes': (TagGroupUpdateQueryResourceObjectAttributes,),  # noqa: E501
-            'type': (TagGroupEnum,),  # noqa: E501
+            'attributes': (TagUpdateQueryResourceObjectAttributes,),  # noqa: E501
+            'type': (TagEnum,),  # noqa: E501
             'id': (str,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
@@ -110,20 +110,20 @@
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, attributes, type, id, *args, **kwargs):  # noqa: E501
-        """TagGroupUpdateQueryResourceObject - a model defined in OpenAPI
+        """TagUpdateQueryResourceObject - a model defined in OpenAPI
 
         Args:
-            attributes (TagGroupUpdateQueryResourceObjectAttributes):
-            type (TagGroupEnum):
-            id (str): The Tag Group ID
+            attributes (TagUpdateQueryResourceObjectAttributes):
+            type (TagEnum):
+            id (str): The Tag ID
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -203,20 +203,20 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, attributes, type, id, *args, **kwargs):  # noqa: E501
-        """TagGroupUpdateQueryResourceObject - a model defined in OpenAPI
+        """TagUpdateQueryResourceObject - a model defined in OpenAPI
 
         Args:
-            attributes (TagGroupUpdateQueryResourceObjectAttributes):
-            type (TagGroupEnum):
-            id (str): The Tag Group ID
+            attributes (TagUpdateQueryResourceObjectAttributes):
+            type (TagEnum):
+            id (str): The Tag ID
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
```

### Comparing `klaviyo-api-2.0.1/src/openapi_client/model/tag_group_update_query_resource_object_attributes.py` & `klaviyo-api-2.0.2/src/openapi_client/model/template_update_query_resource_object.py`

 * *Files 11% similar despite different names*

```diff
@@ -26,16 +26,22 @@
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
 from openapi_client.exceptions import ApiAttributeError
 
 
+def lazy_import():
+    from openapi_client.model.template_enum import TemplateEnum
+    from openapi_client.model.template_update_query_resource_object_attributes import TemplateUpdateQueryResourceObjectAttributes
+    globals()['TemplateEnum'] = TemplateEnum
+    globals()['TemplateUpdateQueryResourceObjectAttributes'] = TemplateUpdateQueryResourceObjectAttributes
 
-class TagGroupUpdateQueryResourceObjectAttributes(ModelNormal):
+
+class TemplateUpdateQueryResourceObject(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -63,55 +69,61 @@
 
     @cached_property
     def additional_properties_type():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
         """
+        lazy_import()
         return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
 
     _nullable = False
 
     @cached_property
     def openapi_types():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
+        lazy_import()
         return {
-            'name': (str, none_type,),  # noqa: E501
-            'return_fields': ([str],),  # noqa: E501
+            'attributes': (TemplateUpdateQueryResourceObjectAttributes,),  # noqa: E501
+            'type': (TemplateEnum,),  # noqa: E501
+            'id': (str,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'name': 'name',  # noqa: E501
-        'return_fields': 'return_fields',  # noqa: E501
+        'attributes': 'attributes',  # noqa: E501
+        'type': 'type',  # noqa: E501
+        'id': 'id',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, name, *args, **kwargs):  # noqa: E501
-        """TagGroupUpdateQueryResourceObjectAttributes - a model defined in OpenAPI
+    def _from_openapi_data(cls, attributes, type, id, *args, **kwargs):  # noqa: E501
+        """TemplateUpdateQueryResourceObject - a model defined in OpenAPI
 
         Args:
-            name (str, none_type): The Tag Group name
+            attributes (TemplateUpdateQueryResourceObjectAttributes):
+            type (TemplateEnum):
+            id (str): The ID of template
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -136,15 +148,14 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            return_fields ([str]): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -168,15 +179,17 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.name = name
+        self.attributes = attributes
+        self.type = type
+        self.id = id
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -189,19 +202,21 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, name, *args, **kwargs):  # noqa: E501
-        """TagGroupUpdateQueryResourceObjectAttributes - a model defined in OpenAPI
+    def __init__(self, attributes, type, id, *args, **kwargs):  # noqa: E501
+        """TemplateUpdateQueryResourceObject - a model defined in OpenAPI
 
         Args:
-            name (str, none_type): The Tag Group name
+            attributes (TemplateUpdateQueryResourceObjectAttributes):
+            type (TemplateEnum):
+            id (str): The ID of template
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -226,15 +241,14 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            return_fields ([str]): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -256,15 +270,17 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.name = name
+        self.attributes = attributes
+        self.type = type
+        self.id = id
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `klaviyo-api-2.0.1/src/openapi_client/model/tag_list_op.py` & `klaviyo-api-2.0.2/src/openapi_client/model/template_create_query_resource_object_attributes.py`

 * *Files 16% similar despite different names*

```diff
@@ -26,20 +26,16 @@
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
 from openapi_client.exceptions import ApiAttributeError
 
 
-def lazy_import():
-    from openapi_client.model.tag_list_op_data_inner import TagListOpDataInner
-    globals()['TagListOpDataInner'] = TagListOpDataInner
 
-
-class TagListOp(ModelNormal):
+class TemplateCreateQueryResourceObjectAttributes(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -67,55 +63,62 @@
 
     @cached_property
     def additional_properties_type():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
         """
-        lazy_import()
         return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
 
     _nullable = False
 
     @cached_property
     def openapi_types():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
-        lazy_import()
         return {
-            'data': ([TagListOpDataInner],),  # noqa: E501
+            'name': (str, none_type,),  # noqa: E501
+            'editor_type': (str, none_type,),  # noqa: E501
+            'text': (str, none_type,),  # noqa: E501
+            'html': (str, none_type,),  # noqa: E501
+            'return_fields': ([str],),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'data': 'data',  # noqa: E501
+        'name': 'name',  # noqa: E501
+        'editor_type': 'editor_type',  # noqa: E501
+        'text': 'text',  # noqa: E501
+        'html': 'html',  # noqa: E501
+        'return_fields': 'return_fields',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, data, *args, **kwargs):  # noqa: E501
-        """TagListOp - a model defined in OpenAPI
+    def _from_openapi_data(cls, name, editor_type, *args, **kwargs):  # noqa: E501
+        """TemplateCreateQueryResourceObjectAttributes - a model defined in OpenAPI
 
         Args:
-            data ([TagListOpDataInner]):
+            name (str, none_type): The name of the template
+            editor_type (str, none_type): Restricted to CODE
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -140,14 +143,17 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
+            text (str, none_type): The plaintext version of the template. [optional]  # noqa: E501
+            html (str, none_type): The HTML contents of the template. [optional]  # noqa: E501
+            return_fields ([str]): Provide fields to limit the returned data. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -171,15 +177,16 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.data = data
+        self.name = name
+        self.editor_type = editor_type
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -192,19 +199,20 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, data, *args, **kwargs):  # noqa: E501
-        """TagListOp - a model defined in OpenAPI
+    def __init__(self, name, editor_type, *args, **kwargs):  # noqa: E501
+        """TemplateCreateQueryResourceObjectAttributes - a model defined in OpenAPI
 
         Args:
-            data ([TagListOpDataInner]):
+            name (str, none_type): The name of the template
+            editor_type (str, none_type): Restricted to CODE
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -229,14 +237,17 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
+            text (str, none_type): The plaintext version of the template. [optional]  # noqa: E501
+            html (str, none_type): The HTML contents of the template. [optional]  # noqa: E501
+            return_fields ([str]): Provide fields to limit the returned data. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -258,15 +269,16 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.data = data
+        self.name = name
+        self.editor_type = editor_type
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `klaviyo-api-2.0.1/src/openapi_client/model/tag_list_op_data_inner.py` & `klaviyo-api-2.0.2/src/openapi_client/model/unsuppression_create_job_create_query_resource_object.py`

 * *Files 16% similar despite different names*

```diff
@@ -26,16 +26,22 @@
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
 from openapi_client.exceptions import ApiAttributeError
 
 
+def lazy_import():
+    from openapi_client.model.profile_unsuppression_bulk_create_job_enum import ProfileUnsuppressionBulkCreateJobEnum
+    from openapi_client.model.unsuppression_create_job_create_query_resource_object_attributes import UnsuppressionCreateJobCreateQueryResourceObjectAttributes
+    globals()['ProfileUnsuppressionBulkCreateJobEnum'] = ProfileUnsuppressionBulkCreateJobEnum
+    globals()['UnsuppressionCreateJobCreateQueryResourceObjectAttributes'] = UnsuppressionCreateJobCreateQueryResourceObjectAttributes
 
-class TagListOpDataInner(ModelNormal):
+
+class UnsuppressionCreateJobCreateQueryResourceObject(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -52,72 +58,71 @@
           min_items, exclusive_maximum, inclusive_maximum, exclusive_minimum,
           inclusive_minimum, and regex.
       additional_properties_type (tuple): A tuple of classes accepted
           as additional properties values.
     """
 
     allowed_values = {
-        ('type',): {
-            'LIST': "list",
-        },
     }
 
     validations = {
     }
 
     @cached_property
     def additional_properties_type():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
         """
+        lazy_import()
         return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
 
     _nullable = False
 
     @cached_property
     def openapi_types():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
+        lazy_import()
         return {
-            'type': (str,),  # noqa: E501
-            'id': (str,),  # noqa: E501
+            'attributes': (UnsuppressionCreateJobCreateQueryResourceObjectAttributes,),  # noqa: E501
+            'type': (ProfileUnsuppressionBulkCreateJobEnum,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
+        'attributes': 'attributes',  # noqa: E501
         'type': 'type',  # noqa: E501
-        'id': 'id',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, id, *args, **kwargs):  # noqa: E501
-        """TagListOpDataInner - a model defined in OpenAPI
+    def _from_openapi_data(cls, attributes, type, *args, **kwargs):  # noqa: E501
+        """UnsuppressionCreateJobCreateQueryResourceObject - a model defined in OpenAPI
 
         Args:
-            id (str):
+            attributes (UnsuppressionCreateJobCreateQueryResourceObjectAttributes):
+            type (ProfileUnsuppressionBulkCreateJobEnum):
 
         Keyword Args:
-            type (str): defaults to "list", must be one of ["list", ]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
@@ -142,15 +147,14 @@
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
         """
 
-        type = kwargs.get('type', "list")
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
 
         self = super(OpenApiModel, cls).__new__(cls)
@@ -172,16 +176,16 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
+        self.attributes = attributes
         self.type = type
-        self.id = id
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -194,22 +198,22 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, id, *args, **kwargs):  # noqa: E501
-        """TagListOpDataInner - a model defined in OpenAPI
+    def __init__(self, attributes, type, *args, **kwargs):  # noqa: E501
+        """UnsuppressionCreateJobCreateQueryResourceObject - a model defined in OpenAPI
 
         Args:
-            id (str):
+            attributes (UnsuppressionCreateJobCreateQueryResourceObjectAttributes):
+            type (ProfileUnsuppressionBulkCreateJobEnum):
 
         Keyword Args:
-            type (str): defaults to "list", must be one of ["list", ]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
@@ -234,15 +238,14 @@
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
         """
 
-        type = kwargs.get('type', "list")
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
 
         if args:
@@ -262,16 +265,16 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
+        self.attributes = attributes
         self.type = type
-        self.id = id
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `klaviyo-api-2.0.1/src/openapi_client/model_utils.py` & `klaviyo-api-2.0.2/src/openapi_client/model_utils.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.1/src/openapi_client/models/__init__.py` & `klaviyo-api-2.0.2/src/openapi_client/models/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -23,15 +23,14 @@
 from openapi_client.model.campaign_message_enum import CampaignMessageEnum
 from openapi_client.model.campaign_message_partial_update_query import CampaignMessagePartialUpdateQuery
 from openapi_client.model.campaign_message_partial_update_query_resource_object import CampaignMessagePartialUpdateQueryResourceObject
 from openapi_client.model.campaign_message_partial_update_query_resource_object_attributes import CampaignMessagePartialUpdateQueryResourceObjectAttributes
 from openapi_client.model.campaign_partial_update_query import CampaignPartialUpdateQuery
 from openapi_client.model.campaign_partial_update_query_resource_object import CampaignPartialUpdateQueryResourceObject
 from openapi_client.model.campaign_partial_update_query_resource_object_attributes import CampaignPartialUpdateQueryResourceObjectAttributes
-from openapi_client.model.campaign_recipient_estimation_enum import CampaignRecipientEstimationEnum
 from openapi_client.model.campaign_recipient_estimation_job_create_query import CampaignRecipientEstimationJobCreateQuery
 from openapi_client.model.campaign_recipient_estimation_job_create_query_resource_object import CampaignRecipientEstimationJobCreateQueryResourceObject
 from openapi_client.model.campaign_recipient_estimation_job_create_query_resource_object_attributes import CampaignRecipientEstimationJobCreateQueryResourceObjectAttributes
 from openapi_client.model.campaign_recipient_estimation_job_enum import CampaignRecipientEstimationJobEnum
 from openapi_client.model.campaign_send_job_create_query import CampaignSendJobCreateQuery
 from openapi_client.model.campaign_send_job_create_query_resource_object import CampaignSendJobCreateQueryResourceObject
 from openapi_client.model.campaign_send_job_create_query_resource_object_attributes import CampaignSendJobCreateQueryResourceObjectAttributes
@@ -83,15 +82,14 @@
 from openapi_client.model.catalog_item_enum import CatalogItemEnum
 from openapi_client.model.catalog_item_update_job_create_query import CatalogItemUpdateJobCreateQuery
 from openapi_client.model.catalog_item_update_job_create_query_resource_object import CatalogItemUpdateJobCreateQueryResourceObject
 from openapi_client.model.catalog_item_update_job_create_query_resource_object_attributes import CatalogItemUpdateJobCreateQueryResourceObjectAttributes
 from openapi_client.model.catalog_item_update_query import CatalogItemUpdateQuery
 from openapi_client.model.catalog_item_update_query_resource_object import CatalogItemUpdateQueryResourceObject
 from openapi_client.model.catalog_item_update_query_resource_object_attributes import CatalogItemUpdateQueryResourceObjectAttributes
-from openapi_client.model.catalog_job_error_payload import CatalogJobErrorPayload
 from openapi_client.model.catalog_variant_bulk_create_job_enum import CatalogVariantBulkCreateJobEnum
 from openapi_client.model.catalog_variant_bulk_delete_job_enum import CatalogVariantBulkDeleteJobEnum
 from openapi_client.model.catalog_variant_bulk_update_job_enum import CatalogVariantBulkUpdateJobEnum
 from openapi_client.model.catalog_variant_create_job_create_query import CatalogVariantCreateJobCreateQuery
 from openapi_client.model.catalog_variant_create_job_create_query_resource_object import CatalogVariantCreateJobCreateQueryResourceObject
 from openapi_client.model.catalog_variant_create_job_create_query_resource_object_attributes import CatalogVariantCreateJobCreateQueryResourceObjectAttributes
 from openapi_client.model.catalog_variant_create_query import CatalogVariantCreateQuery
@@ -104,34 +102,24 @@
 from openapi_client.model.catalog_variant_enum import CatalogVariantEnum
 from openapi_client.model.catalog_variant_update_job_create_query import CatalogVariantUpdateJobCreateQuery
 from openapi_client.model.catalog_variant_update_job_create_query_resource_object import CatalogVariantUpdateJobCreateQueryResourceObject
 from openapi_client.model.catalog_variant_update_job_create_query_resource_object_attributes import CatalogVariantUpdateJobCreateQueryResourceObjectAttributes
 from openapi_client.model.catalog_variant_update_query import CatalogVariantUpdateQuery
 from openapi_client.model.catalog_variant_update_query_resource_object import CatalogVariantUpdateQueryResourceObject
 from openapi_client.model.catalog_variant_update_query_resource_object_attributes import CatalogVariantUpdateQueryResourceObjectAttributes
-from openapi_client.model.collection_links import CollectionLinks
 from openapi_client.model.content_sub_object import ContentSubObject
 from openapi_client.model.data_privacy_create_deletion_job_query import DataPrivacyCreateDeletionJobQuery
 from openapi_client.model.data_privacy_create_deletion_job_query_resource_object import DataPrivacyCreateDeletionJobQueryResourceObject
 from openapi_client.model.data_privacy_create_deletion_job_query_resource_object_attributes import DataPrivacyCreateDeletionJobQueryResourceObjectAttributes
 from openapi_client.model.data_privacy_deletion_job_enum import DataPrivacyDeletionJobEnum
-from openapi_client.model.email_channel import EmailChannel
-from openapi_client.model.email_marketing import EmailMarketing
-from openapi_client.model.email_marketing_list_suppression import EmailMarketingListSuppression
-from openapi_client.model.email_marketing_suppression import EmailMarketingSuppression
-from openapi_client.model.email_message_content import EmailMessageContent
-from openapi_client.model.email_tracking_options import EmailTrackingOptions
-from openapi_client.model.error_source import ErrorSource
 from openapi_client.model.event_create_query import EventCreateQuery
 from openapi_client.model.event_create_query_resource_object import EventCreateQueryResourceObject
 from openapi_client.model.event_create_query_resource_object_attributes import EventCreateQueryResourceObjectAttributes
 from openapi_client.model.event_enum import EventEnum
-from openapi_client.model.flow_action_enum import FlowActionEnum
 from openapi_client.model.flow_enum import FlowEnum
-from openapi_client.model.flow_message_enum import FlowMessageEnum
 from openapi_client.model.flow_update_query import FlowUpdateQuery
 from openapi_client.model.flow_update_query_resource_object import FlowUpdateQueryResourceObject
 from openapi_client.model.flow_update_query_resource_object_attributes import FlowUpdateQueryResourceObjectAttributes
 from openapi_client.model.get_create_variants_jobs5_xx_response import GetCreateVariantsJobs5XXResponse
 from openapi_client.model.get_create_variants_jobs5_xx_response_errors_inner import GetCreateVariantsJobs5XXResponseErrorsInner
 from openapi_client.model.get_create_variants_jobs5_xx_response_errors_inner_source import GetCreateVariantsJobs5XXResponseErrorsInnerSource
 from openapi_client.model.list_create_query import ListCreateQuery
@@ -143,63 +131,48 @@
 from openapi_client.model.list_members_delete_query import ListMembersDeleteQuery
 from openapi_client.model.list_partial_update_query import ListPartialUpdateQuery
 from openapi_client.model.list_partial_update_query_resource_object import ListPartialUpdateQueryResourceObject
 from openapi_client.model.metric_aggregate_enum import MetricAggregateEnum
 from openapi_client.model.metric_aggregate_query import MetricAggregateQuery
 from openapi_client.model.metric_aggregate_query_resource_object import MetricAggregateQueryResourceObject
 from openapi_client.model.metric_aggregate_query_resource_object_attributes import MetricAggregateQueryResourceObjectAttributes
-from openapi_client.model.metric_aggregate_row_dto import MetricAggregateRowDTO
 from openapi_client.model.metric_create_query import MetricCreateQuery
-from openapi_client.model.metric_enum import MetricEnum
-from openapi_client.model.object_links import ObjectLinks
 from openapi_client.model.onsite_profile_create_query import OnsiteProfileCreateQuery
 from openapi_client.model.onsite_profile_create_query_resource_object import OnsiteProfileCreateQueryResourceObject
 from openapi_client.model.onsite_profile_create_query_resource_object_attributes import OnsiteProfileCreateQueryResourceObjectAttributes
-from openapi_client.model.onsite_profile_meta import OnsiteProfileMeta
-from openapi_client.model.onsite_profile_meta_identifiers import OnsiteProfileMetaIdentifiers
 from openapi_client.model.onsite_subscription_create_query import OnsiteSubscriptionCreateQuery
 from openapi_client.model.onsite_subscription_create_query_resource_object import OnsiteSubscriptionCreateQueryResourceObject
 from openapi_client.model.onsite_subscription_create_query_resource_object_attributes import OnsiteSubscriptionCreateQueryResourceObjectAttributes
-from openapi_client.model.predictive_analytics import PredictiveAnalytics
-from openapi_client.model.profile_aggregate_enum import ProfileAggregateEnum
 from openapi_client.model.profile_create_query import ProfileCreateQuery
 from openapi_client.model.profile_create_query_resource_object import ProfileCreateQueryResourceObject
 from openapi_client.model.profile_create_query_resource_object_attributes import ProfileCreateQueryResourceObjectAttributes
 from openapi_client.model.profile_enum import ProfileEnum
 from openapi_client.model.profile_location import ProfileLocation
 from openapi_client.model.profile_location_latitude import ProfileLocationLatitude
 from openapi_client.model.profile_location_longitude import ProfileLocationLongitude
 from openapi_client.model.profile_partial_update_query import ProfilePartialUpdateQuery
 from openapi_client.model.profile_partial_update_query_resource_object import ProfilePartialUpdateQueryResourceObject
 from openapi_client.model.profile_subscription_bulk_create_job_enum import ProfileSubscriptionBulkCreateJobEnum
 from openapi_client.model.profile_suppression_bulk_create_job_enum import ProfileSuppressionBulkCreateJobEnum
 from openapi_client.model.profile_unsubscription_bulk_create_job_enum import ProfileUnsubscriptionBulkCreateJobEnum
 from openapi_client.model.profile_unsuppression_bulk_create_job_enum import ProfileUnsuppressionBulkCreateJobEnum
-from openapi_client.model.sms_channel import SMSChannel
-from openapi_client.model.sms_marketing import SMSMarketing
-from openapi_client.model.sms_message_content import SMSMessageContent
-from openapi_client.model.sms_render_options import SMSRenderOptions
-from openapi_client.model.sms_tracking_options import SMSTrackingOptions
 from openapi_client.model.sto_schedule_options import STOScheduleOptions
 from openapi_client.model.segment_enum import SegmentEnum
 from openapi_client.model.segment_partial_update_query import SegmentPartialUpdateQuery
 from openapi_client.model.segment_partial_update_query_resource_object import SegmentPartialUpdateQueryResourceObject
 from openapi_client.model.segment_partial_update_query_resource_object_attributes import SegmentPartialUpdateQueryResourceObjectAttributes
-from openapi_client.model.send_options import SendOptions
 from openapi_client.model.send_options_sub_object import SendOptionsSubObject
 from openapi_client.model.send_strategy_sub_object import SendStrategySubObject
-from openapi_client.model.send_time_sub_object import SendTimeSubObject
 from openapi_client.model.static_schedule_options import StaticScheduleOptions
 from openapi_client.model.subscription import Subscription
 from openapi_client.model.subscription_channels import SubscriptionChannels
 from openapi_client.model.subscription_create_job_create_query import SubscriptionCreateJobCreateQuery
 from openapi_client.model.subscription_create_job_create_query_resource_object import SubscriptionCreateJobCreateQueryResourceObject
 from openapi_client.model.subscription_create_job_create_query_resource_object_attributes import SubscriptionCreateJobCreateQueryResourceObjectAttributes
 from openapi_client.model.subscription_enum import SubscriptionEnum
-from openapi_client.model.subscriptions import Subscriptions
 from openapi_client.model.suppression import Suppression
 from openapi_client.model.suppression_create_job_create_query import SuppressionCreateJobCreateQuery
 from openapi_client.model.suppression_create_job_create_query_resource_object import SuppressionCreateJobCreateQueryResourceObject
 from openapi_client.model.suppression_create_job_create_query_resource_object_attributes import SuppressionCreateJobCreateQueryResourceObjectAttributes
 from openapi_client.model.tag_campaign_op import TagCampaignOp
 from openapi_client.model.tag_campaign_op_data_inner import TagCampaignOpDataInner
 from openapi_client.model.tag_create_query import TagCreateQuery
@@ -231,19 +204,16 @@
 from openapi_client.model.template_enum import TemplateEnum
 from openapi_client.model.template_render_query import TemplateRenderQuery
 from openapi_client.model.template_render_query_resource_object import TemplateRenderQueryResourceObject
 from openapi_client.model.template_render_query_resource_object_attributes import TemplateRenderQueryResourceObjectAttributes
 from openapi_client.model.template_update_query import TemplateUpdateQuery
 from openapi_client.model.template_update_query_resource_object import TemplateUpdateQueryResourceObject
 from openapi_client.model.template_update_query_resource_object_attributes import TemplateUpdateQueryResourceObjectAttributes
-from openapi_client.model.test_api_analytics_sample_enum import TestApiAnalyticsSampleEnum
-from openapi_client.model.test_list_enum import TestListEnum
 from openapi_client.model.throttled_schedule_options import ThrottledScheduleOptions
 from openapi_client.model.tracking_options_sub_object import TrackingOptionsSubObject
 from openapi_client.model.utm_params_sub_object import UTMParamsSubObject
 from openapi_client.model.unsubscription_create_job_create_query import UnsubscriptionCreateJobCreateQuery
 from openapi_client.model.unsubscription_create_job_create_query_resource_object import UnsubscriptionCreateJobCreateQueryResourceObject
 from openapi_client.model.unsubscription_create_job_create_query_resource_object_attributes import UnsubscriptionCreateJobCreateQueryResourceObjectAttributes
 from openapi_client.model.unsuppression_create_job_create_query import UnsuppressionCreateJobCreateQuery
 from openapi_client.model.unsuppression_create_job_create_query_resource_object import UnsuppressionCreateJobCreateQueryResourceObject
 from openapi_client.model.unsuppression_create_job_create_query_resource_object_attributes import UnsuppressionCreateJobCreateQueryResourceObjectAttributes
-from openapi_client.model.utm_param_info import UtmParamInfo
```

### Comparing `klaviyo-api-2.0.1/src/openapi_client/rest.py` & `klaviyo-api-2.0.2/src/openapi_client/rest.py`

 * *Files identical despite different names*

