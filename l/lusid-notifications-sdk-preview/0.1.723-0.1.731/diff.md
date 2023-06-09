# Comparing `tmp/lusid-notifications-sdk-preview-0.1.723.tar.gz` & `tmp/lusid-notifications-sdk-preview-0.1.731.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/lusid-notifications-sdk-preview-0.1.723.tar", last modified: Tue Jun  6 10:26:43 2023, max compression
+gzip compressed data, was "dist/lusid-notifications-sdk-preview-0.1.731.tar", last modified: Fri Jun  9 09:56:36 2023, max compression
```

## Comparing `lusid-notifications-sdk-preview-0.1.723.tar` & `lusid-notifications-sdk-preview-0.1.731.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 10:26:43.000000 lusid-notifications-sdk-preview-0.1.723/
--rw-r--r--   0 root         (0) root         (0)       54 2023-06-06 10:24:53.000000 lusid-notifications-sdk-preview-0.1.723/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      373 2023-06-06 10:26:43.000000 lusid-notifications-sdk-preview-0.1.723/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     9590 2023-06-06 10:24:53.000000 lusid-notifications-sdk-preview-0.1.723/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 10:26:43.000000 lusid-notifications-sdk-preview-0.1.723/lusid_notifications/
--rw-r--r--   0 root         (0) root         (0)     4349 2023-06-06 10:24:53.000000 lusid-notifications-sdk-preview-0.1.723/lusid_notifications/__init__.py
--rw-r--r--   0 root         (0) root         (0)       24 2023-06-06 10:24:53.000000 lusid-notifications-sdk-preview-0.1.723/lusid_notifications/__version__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 10:26:43.000000 lusid-notifications-sdk-preview-0.1.723/lusid_notifications/api/
--rw-r--r--   0 root         (0) root         (0)      501 2023-06-06 10:24:53.000000 lusid-notifications-sdk-preview-0.1.723/lusid_notifications/api/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6851 2023-06-06 10:24:53.000000 lusid-notifications-sdk-preview-0.1.723/lusid_notifications/api/application_metadata_api.py
--rw-r--r--   0 root         (0) root         (0)    10524 2023-06-06 10:24:53.000000 lusid-notifications-sdk-preview-0.1.723/lusid_notifications/api/deliveries_api.py
--rw-r--r--   0 root         (0) root         (0)    13990 2023-06-06 10:24:53.000000 lusid-notifications-sdk-preview-0.1.723/lusid_notifications/api/event_types_api.py
--rw-r--r--   0 root         (0) root         (0)     6975 2023-06-06 10:24:53.000000 lusid-notifications-sdk-preview-0.1.723/lusid_notifications/api/events_api.py
--rw-r--r--   0 root         (0) root         (0)   122660 2023-06-06 10:24:53.000000 lusid-notifications-sdk-preview-0.1.723/lusid_notifications/api/notifications_api.py
--rw-r--r--   0 root         (0) root         (0)    47811 2023-06-06 10:24:53.000000 lusid-notifications-sdk-preview-0.1.723/lusid_notifications/api/subscriptions_api.py
--rw-r--r--   0 root         (0) root         (0)    27436 2023-06-06 10:24:53.000000 lusid-notifications-sdk-preview-0.1.723/lusid_notifications/api_client.py
--rw-r--r--   0 root         (0) root         (0)    16635 2023-06-06 10:24:53.000000 lusid-notifications-sdk-preview-0.1.723/lusid_notifications/configuration.py
--rw-r--r--   0 root         (0) root         (0)     5099 2023-06-06 10:24:53.000000 lusid-notifications-sdk-preview-0.1.723/lusid_notifications/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 10:26:43.000000 lusid-notifications-sdk-preview-0.1.723/lusid_notifications/models/
--rw-r--r--   0 root         (0) root         (0)     2995 2023-06-06 10:24:53.000000 lusid-notifications-sdk-preview-0.1.723/lusid_notifications/models/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7264 2023-06-06 10:24:53.000000 lusid-notifications-sdk-preview-0.1.723/lusid_notifications/models/access_controlled_action.py
--rw-r--r--   0 root         (0) root         (0)     9027 2023-06-06 10:24:53.000000 lusid-notifications-sdk-preview-0.1.723/lusid_notifications/models/access_controlled_resource.py
--rw-r--r--   0 root         (0) root         (0)     7232 2023-06-06 10:24:53.000000 lusid-notifications-sdk-preview-0.1.723/lusid_notifications/models/action_id.py
--rw-r--r--   0 root         (0) root         (0)     6512 2023-06-06 10:24:53.000000 lusid-notifications-sdk-preview-0.1.723/lusid_notifications/models/attempt.py
--rw-r--r--   0 root         (0) root         (0)     5557 2023-06-06 10:24:53.000000 lusid-notifications-sdk-preview-0.1.723/lusid_notifications/models/attempt_status.py
--rw-r--r--   0 root         (0) root         (0)    11703 2023-06-06 10:24:53.000000 lusid-notifications-sdk-preview-0.1.723/lusid_notifications/models/create_aws_sqs_notification.py
--rw-r--r--   0 root         (0) root         (0)    16290 2023-06-06 10:24:53.000000 lusid-notifications-sdk-preview-0.1.723/lusid_notifications/models/create_email_notification.py
--rw-r--r--   0 root         (0) root         (0)     8814 2023-06-06 10:24:53.000000 lusid-notifications-sdk-preview-0.1.723/lusid_notifications/models/create_sms_notification.py
--rw-r--r--   0 root         (0) root         (0)    10822 2023-06-06 10:24:53.000000 lusid-notifications-sdk-preview-0.1.723/lusid_notifications/models/create_subscription.py
--rw-r--r--   0 root         (0) root         (0)    16161 2023-06-06 10:24:53.000000 lusid-notifications-sdk-preview-0.1.723/lusid_notifications/models/create_webhook_notification.py
--rw-r--r--   0 root         (0) root         (0)    12397 2023-06-06 10:24:53.000000 lusid-notifications-sdk-preview-0.1.723/lusid_notifications/models/delivery.py
--rw-r--r--   0 root         (0) root         (0)     4091 2023-06-06 10:24:53.000000 lusid-notifications-sdk-preview-0.1.723/lusid_notifications/models/event_details.py
--rw-r--r--   0 root         (0) root         (0)    10287 2023-06-06 10:24:53.000000 lusid-notifications-sdk-preview-0.1.723/lusid_notifications/models/event_type_schema.py
--rw-r--r--   0 root         (0) root         (0)     8025 2023-06-06 10:24:53.000000 lusid-notifications-sdk-preview-0.1.723/lusid_notifications/models/id_selector_definition.py
--rw-r--r--   0 root         (0) root         (0)     9514 2023-06-06 10:24:53.000000 lusid-notifications-sdk-preview-0.1.723/lusid_notifications/models/identifier_part_schema.py
--rw-r--r--   0 root         (0) root         (0)     6426 2023-06-06 10:24:53.000000 lusid-notifications-sdk-preview-0.1.723/lusid_notifications/models/link.py
--rw-r--r--   0 root         (0) root         (0)     9540 2023-06-06 10:24:53.000000 lusid-notifications-sdk-preview-0.1.723/lusid_notifications/models/lusid_problem_details.py
--rw-r--r--   0 root         (0) root         (0)    10705 2023-06-06 10:24:53.000000 lusid-notifications-sdk-preview-0.1.723/lusid_notifications/models/lusid_validation_problem_details.py
--rw-r--r--   0 root         (0) root         (0)     7437 2023-06-06 10:24:53.000000 lusid-notifications-sdk-preview-0.1.723/lusid_notifications/models/matching_pattern.py
--rw-r--r--   0 root         (0) root         (0)    18059 2023-06-06 10:24:53.000000 lusid-notifications-sdk-preview-0.1.723/lusid_notifications/models/notification.py
--rw-r--r--   0 root         (0) root         (0)     5155 2023-06-06 10:24:53.000000 lusid-notifications-sdk-preview-0.1.723/lusid_notifications/models/notification_status.py
--rw-r--r--   0 root         (0) root         (0)     6099 2023-06-06 10:24:53.000000 lusid-notifications-sdk-preview-0.1.723/lusid_notifications/models/resource_id.py
--rw-r--r--   0 root         (0) root         (0)     7775 2023-06-06 10:24:53.000000 lusid-notifications-sdk-preview-0.1.723/lusid_notifications/models/resource_list_of_access_controlled_resource.py
--rw-r--r--   0 root         (0) root         (0)     7327 2023-06-06 10:24:53.000000 lusid-notifications-sdk-preview-0.1.723/lusid_notifications/models/resource_list_of_delivery.py
--rw-r--r--   0 root         (0) root         (0)     7523 2023-06-06 10:24:53.000000 lusid-notifications-sdk-preview-0.1.723/lusid_notifications/models/resource_list_of_event_type_schema.py
--rw-r--r--   0 root         (0) root         (0)     7439 2023-06-06 10:24:53.000000 lusid-notifications-sdk-preview-0.1.723/lusid_notifications/models/resource_list_of_notification.py
--rw-r--r--   0 root         (0) root         (0)     7439 2023-06-06 10:24:53.000000 lusid-notifications-sdk-preview-0.1.723/lusid_notifications/models/resource_list_of_subscription.py
--rw-r--r--   0 root         (0) root         (0)    15560 2023-06-06 10:24:53.000000 lusid-notifications-sdk-preview-0.1.723/lusid_notifications/models/subscription.py
--rw-r--r--   0 root         (0) root         (0)    11703 2023-06-06 10:24:53.000000 lusid-notifications-sdk-preview-0.1.723/lusid_notifications/models/update_aws_sqs_notification.py
--rw-r--r--   0 root         (0) root         (0)    16290 2023-06-06 10:24:53.000000 lusid-notifications-sdk-preview-0.1.723/lusid_notifications/models/update_email_notification.py
--rw-r--r--   0 root         (0) root         (0)     8814 2023-06-06 10:24:53.000000 lusid-notifications-sdk-preview-0.1.723/lusid_notifications/models/update_sms_notification.py
--rw-r--r--   0 root         (0) root         (0)     9939 2023-06-06 10:24:53.000000 lusid-notifications-sdk-preview-0.1.723/lusid_notifications/models/update_subscription.py
--rw-r--r--   0 root         (0) root         (0)    16161 2023-06-06 10:24:53.000000 lusid-notifications-sdk-preview-0.1.723/lusid_notifications/models/update_webhook_notification.py
--rw-r--r--   0 root         (0) root         (0)    13561 2023-06-06 10:24:53.000000 lusid-notifications-sdk-preview-0.1.723/lusid_notifications/rest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 10:26:43.000000 lusid-notifications-sdk-preview-0.1.723/lusid_notifications/utilities/
--rw-r--r--   0 root         (0) root         (0)       65 2023-06-06 10:24:53.000000 lusid-notifications-sdk-preview-0.1.723/lusid_notifications/utilities/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1042 2023-06-06 10:24:53.000000 lusid-notifications-sdk-preview-0.1.723/lusid_notifications/utilities/config_keys.json
--rw-r--r--   0 root         (0) root         (0)      295 2023-06-06 10:24:53.000000 lusid-notifications-sdk-preview-0.1.723/lusid_notifications/utilities/config_keys.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 10:26:43.000000 lusid-notifications-sdk-preview-0.1.723/lusid_notifications_sdk_preview.egg-info/
--rw-r--r--   0 root         (0) root         (0)      373 2023-06-06 10:26:43.000000 lusid-notifications-sdk-preview-0.1.723/lusid_notifications_sdk_preview.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2692 2023-06-06 10:26:43.000000 lusid-notifications-sdk-preview-0.1.723/lusid_notifications_sdk_preview.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-06 10:26:43.000000 lusid-notifications-sdk-preview-0.1.723/lusid_notifications_sdk_preview.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      116 2023-06-06 10:26:43.000000 lusid-notifications-sdk-preview-0.1.723/lusid_notifications_sdk_preview.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       20 2023-06-06 10:26:43.000000 lusid-notifications-sdk-preview-0.1.723/lusid_notifications_sdk_preview.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-06 10:26:43.000000 lusid-notifications-sdk-preview-0.1.723/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2322 2023-06-06 10:24:53.000000 lusid-notifications-sdk-preview-0.1.723/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 09:56:36.000000 lusid-notifications-sdk-preview-0.1.731/
+-rw-r--r--   0 root         (0) root         (0)       54 2023-06-09 09:53:31.000000 lusid-notifications-sdk-preview-0.1.731/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      373 2023-06-09 09:56:36.000000 lusid-notifications-sdk-preview-0.1.731/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     9590 2023-06-09 09:53:31.000000 lusid-notifications-sdk-preview-0.1.731/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 09:56:36.000000 lusid-notifications-sdk-preview-0.1.731/lusid_notifications/
+-rw-r--r--   0 root         (0) root         (0)     4349 2023-06-09 09:53:31.000000 lusid-notifications-sdk-preview-0.1.731/lusid_notifications/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       24 2023-06-09 09:53:31.000000 lusid-notifications-sdk-preview-0.1.731/lusid_notifications/__version__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 09:56:36.000000 lusid-notifications-sdk-preview-0.1.731/lusid_notifications/api/
+-rw-r--r--   0 root         (0) root         (0)      501 2023-06-09 09:53:31.000000 lusid-notifications-sdk-preview-0.1.731/lusid_notifications/api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6851 2023-06-09 09:53:31.000000 lusid-notifications-sdk-preview-0.1.731/lusid_notifications/api/application_metadata_api.py
+-rw-r--r--   0 root         (0) root         (0)    10524 2023-06-09 09:53:31.000000 lusid-notifications-sdk-preview-0.1.731/lusid_notifications/api/deliveries_api.py
+-rw-r--r--   0 root         (0) root         (0)    13990 2023-06-09 09:53:31.000000 lusid-notifications-sdk-preview-0.1.731/lusid_notifications/api/event_types_api.py
+-rw-r--r--   0 root         (0) root         (0)     6975 2023-06-09 09:53:31.000000 lusid-notifications-sdk-preview-0.1.731/lusid_notifications/api/events_api.py
+-rw-r--r--   0 root         (0) root         (0)   122660 2023-06-09 09:53:31.000000 lusid-notifications-sdk-preview-0.1.731/lusid_notifications/api/notifications_api.py
+-rw-r--r--   0 root         (0) root         (0)    47811 2023-06-09 09:53:31.000000 lusid-notifications-sdk-preview-0.1.731/lusid_notifications/api/subscriptions_api.py
+-rw-r--r--   0 root         (0) root         (0)    27436 2023-06-09 09:53:31.000000 lusid-notifications-sdk-preview-0.1.731/lusid_notifications/api_client.py
+-rw-r--r--   0 root         (0) root         (0)    16635 2023-06-09 09:53:31.000000 lusid-notifications-sdk-preview-0.1.731/lusid_notifications/configuration.py
+-rw-r--r--   0 root         (0) root         (0)     5099 2023-06-09 09:53:31.000000 lusid-notifications-sdk-preview-0.1.731/lusid_notifications/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 09:56:36.000000 lusid-notifications-sdk-preview-0.1.731/lusid_notifications/models/
+-rw-r--r--   0 root         (0) root         (0)     2995 2023-06-09 09:53:31.000000 lusid-notifications-sdk-preview-0.1.731/lusid_notifications/models/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7264 2023-06-09 09:53:31.000000 lusid-notifications-sdk-preview-0.1.731/lusid_notifications/models/access_controlled_action.py
+-rw-r--r--   0 root         (0) root         (0)     9027 2023-06-09 09:53:31.000000 lusid-notifications-sdk-preview-0.1.731/lusid_notifications/models/access_controlled_resource.py
+-rw-r--r--   0 root         (0) root         (0)     7232 2023-06-09 09:53:31.000000 lusid-notifications-sdk-preview-0.1.731/lusid_notifications/models/action_id.py
+-rw-r--r--   0 root         (0) root         (0)     6512 2023-06-09 09:53:31.000000 lusid-notifications-sdk-preview-0.1.731/lusid_notifications/models/attempt.py
+-rw-r--r--   0 root         (0) root         (0)     5557 2023-06-09 09:53:31.000000 lusid-notifications-sdk-preview-0.1.731/lusid_notifications/models/attempt_status.py
+-rw-r--r--   0 root         (0) root         (0)    11703 2023-06-09 09:53:31.000000 lusid-notifications-sdk-preview-0.1.731/lusid_notifications/models/create_aws_sqs_notification.py
+-rw-r--r--   0 root         (0) root         (0)    16290 2023-06-09 09:53:31.000000 lusid-notifications-sdk-preview-0.1.731/lusid_notifications/models/create_email_notification.py
+-rw-r--r--   0 root         (0) root         (0)     8814 2023-06-09 09:53:31.000000 lusid-notifications-sdk-preview-0.1.731/lusid_notifications/models/create_sms_notification.py
+-rw-r--r--   0 root         (0) root         (0)    12632 2023-06-09 09:53:31.000000 lusid-notifications-sdk-preview-0.1.731/lusid_notifications/models/create_subscription.py
+-rw-r--r--   0 root         (0) root         (0)    16161 2023-06-09 09:53:31.000000 lusid-notifications-sdk-preview-0.1.731/lusid_notifications/models/create_webhook_notification.py
+-rw-r--r--   0 root         (0) root         (0)    12397 2023-06-09 09:53:31.000000 lusid-notifications-sdk-preview-0.1.731/lusid_notifications/models/delivery.py
+-rw-r--r--   0 root         (0) root         (0)     4091 2023-06-09 09:53:31.000000 lusid-notifications-sdk-preview-0.1.731/lusid_notifications/models/event_details.py
+-rw-r--r--   0 root         (0) root         (0)    10287 2023-06-09 09:53:31.000000 lusid-notifications-sdk-preview-0.1.731/lusid_notifications/models/event_type_schema.py
+-rw-r--r--   0 root         (0) root         (0)     8025 2023-06-09 09:53:31.000000 lusid-notifications-sdk-preview-0.1.731/lusid_notifications/models/id_selector_definition.py
+-rw-r--r--   0 root         (0) root         (0)     9514 2023-06-09 09:53:31.000000 lusid-notifications-sdk-preview-0.1.731/lusid_notifications/models/identifier_part_schema.py
+-rw-r--r--   0 root         (0) root         (0)     6426 2023-06-09 09:53:31.000000 lusid-notifications-sdk-preview-0.1.731/lusid_notifications/models/link.py
+-rw-r--r--   0 root         (0) root         (0)     9540 2023-06-09 09:53:31.000000 lusid-notifications-sdk-preview-0.1.731/lusid_notifications/models/lusid_problem_details.py
+-rw-r--r--   0 root         (0) root         (0)    10705 2023-06-09 09:53:31.000000 lusid-notifications-sdk-preview-0.1.731/lusid_notifications/models/lusid_validation_problem_details.py
+-rw-r--r--   0 root         (0) root         (0)     7437 2023-06-09 09:53:31.000000 lusid-notifications-sdk-preview-0.1.731/lusid_notifications/models/matching_pattern.py
+-rw-r--r--   0 root         (0) root         (0)    18059 2023-06-09 09:53:31.000000 lusid-notifications-sdk-preview-0.1.731/lusid_notifications/models/notification.py
+-rw-r--r--   0 root         (0) root         (0)     5155 2023-06-09 09:53:31.000000 lusid-notifications-sdk-preview-0.1.731/lusid_notifications/models/notification_status.py
+-rw-r--r--   0 root         (0) root         (0)     6099 2023-06-09 09:53:31.000000 lusid-notifications-sdk-preview-0.1.731/lusid_notifications/models/resource_id.py
+-rw-r--r--   0 root         (0) root         (0)     7775 2023-06-09 09:53:31.000000 lusid-notifications-sdk-preview-0.1.731/lusid_notifications/models/resource_list_of_access_controlled_resource.py
+-rw-r--r--   0 root         (0) root         (0)     7327 2023-06-09 09:53:31.000000 lusid-notifications-sdk-preview-0.1.731/lusid_notifications/models/resource_list_of_delivery.py
+-rw-r--r--   0 root         (0) root         (0)     7523 2023-06-09 09:53:31.000000 lusid-notifications-sdk-preview-0.1.731/lusid_notifications/models/resource_list_of_event_type_schema.py
+-rw-r--r--   0 root         (0) root         (0)     7439 2023-06-09 09:53:31.000000 lusid-notifications-sdk-preview-0.1.731/lusid_notifications/models/resource_list_of_notification.py
+-rw-r--r--   0 root         (0) root         (0)     7439 2023-06-09 09:53:31.000000 lusid-notifications-sdk-preview-0.1.731/lusid_notifications/models/resource_list_of_subscription.py
+-rw-r--r--   0 root         (0) root         (0)    16992 2023-06-09 09:53:31.000000 lusid-notifications-sdk-preview-0.1.731/lusid_notifications/models/subscription.py
+-rw-r--r--   0 root         (0) root         (0)    11703 2023-06-09 09:53:31.000000 lusid-notifications-sdk-preview-0.1.731/lusid_notifications/models/update_aws_sqs_notification.py
+-rw-r--r--   0 root         (0) root         (0)    16290 2023-06-09 09:53:31.000000 lusid-notifications-sdk-preview-0.1.731/lusid_notifications/models/update_email_notification.py
+-rw-r--r--   0 root         (0) root         (0)     8814 2023-06-09 09:53:31.000000 lusid-notifications-sdk-preview-0.1.731/lusid_notifications/models/update_sms_notification.py
+-rw-r--r--   0 root         (0) root         (0)    11767 2023-06-09 09:53:31.000000 lusid-notifications-sdk-preview-0.1.731/lusid_notifications/models/update_subscription.py
+-rw-r--r--   0 root         (0) root         (0)    16161 2023-06-09 09:53:31.000000 lusid-notifications-sdk-preview-0.1.731/lusid_notifications/models/update_webhook_notification.py
+-rw-r--r--   0 root         (0) root         (0)    13561 2023-06-09 09:53:31.000000 lusid-notifications-sdk-preview-0.1.731/lusid_notifications/rest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 09:56:36.000000 lusid-notifications-sdk-preview-0.1.731/lusid_notifications/utilities/
+-rw-r--r--   0 root         (0) root         (0)       65 2023-06-09 09:53:31.000000 lusid-notifications-sdk-preview-0.1.731/lusid_notifications/utilities/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1042 2023-06-09 09:53:31.000000 lusid-notifications-sdk-preview-0.1.731/lusid_notifications/utilities/config_keys.json
+-rw-r--r--   0 root         (0) root         (0)      295 2023-06-09 09:53:31.000000 lusid-notifications-sdk-preview-0.1.731/lusid_notifications/utilities/config_keys.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 09:56:36.000000 lusid-notifications-sdk-preview-0.1.731/lusid_notifications_sdk_preview.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      373 2023-06-09 09:56:36.000000 lusid-notifications-sdk-preview-0.1.731/lusid_notifications_sdk_preview.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2692 2023-06-09 09:56:36.000000 lusid-notifications-sdk-preview-0.1.731/lusid_notifications_sdk_preview.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-09 09:56:36.000000 lusid-notifications-sdk-preview-0.1.731/lusid_notifications_sdk_preview.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      116 2023-06-09 09:56:36.000000 lusid-notifications-sdk-preview-0.1.731/lusid_notifications_sdk_preview.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       20 2023-06-09 09:56:36.000000 lusid-notifications-sdk-preview-0.1.731/lusid_notifications_sdk_preview.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-09 09:56:36.000000 lusid-notifications-sdk-preview-0.1.731/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2322 2023-06-09 09:53:31.000000 lusid-notifications-sdk-preview-0.1.731/setup.py
```

### Comparing `lusid-notifications-sdk-preview-0.1.723/README.md` & `lusid-notifications-sdk-preview-0.1.731/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # lusid-notifications-sdk
 FINBOURNE Technology
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
-- API version: 0.1.723
-- Package version: 0.1.723
+- API version: 0.1.731
+- Package version: 0.1.731
 - Build package: org.openapitools.codegen.languages.PythonLegacyClientCodegen
 For more information, please visit [https://www.finbourne.com](https://www.finbourne.com)
 
 ## Requirements.
 
 Python 2.7 and 3.4+
```

### Comparing `lusid-notifications-sdk-preview-0.1.723/lusid_notifications/__init__.py` & `lusid-notifications-sdk-preview-0.1.731/lusid_notifications/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,23 +3,23 @@
 # flake8: noqa
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.723
+    The version of the OpenAPI document: 0.1.731
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
-__version__ = "0.1.723"
+__version__ = "0.1.731"
 
 # import apis into sdk package
 from lusid_notifications.api.application_metadata_api import ApplicationMetadataApi
 from lusid_notifications.api.deliveries_api import DeliveriesApi
 from lusid_notifications.api.event_types_api import EventTypesApi
 from lusid_notifications.api.events_api import EventsApi
 from lusid_notifications.api.notifications_api import NotificationsApi
```

### Comparing `lusid-notifications-sdk-preview-0.1.723/lusid_notifications/api/application_metadata_api.py` & `lusid-notifications-sdk-preview-0.1.731/lusid_notifications/api/application_metadata_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.723
+    The version of the OpenAPI document: 0.1.731
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
@@ -141,15 +141,15 @@
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.723'
+        header_params['X-LUSID-SDK-Version'] = '0.1.731'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "ResourceListOfAccessControlledResource",
         }
```

### Comparing `lusid-notifications-sdk-preview-0.1.723/lusid_notifications/api/deliveries_api.py` & `lusid-notifications-sdk-preview-0.1.731/lusid_notifications/api/deliveries_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.723
+    The version of the OpenAPI document: 0.1.731
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
@@ -179,15 +179,15 @@
             ['application/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.723'
+        header_params['X-LUSID-SDK-Version'] = '0.1.731'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "ResourceListOfDelivery",
             400: "LusidValidationProblemDetails",
```

### Comparing `lusid-notifications-sdk-preview-0.1.723/lusid_notifications/api/event_types_api.py` & `lusid-notifications-sdk-preview-0.1.731/lusid_notifications/api/event_types_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.723
+    The version of the OpenAPI document: 0.1.731
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
@@ -160,15 +160,15 @@
             ['application/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.723'
+        header_params['X-LUSID-SDK-Version'] = '0.1.731'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "EventTypeSchema",
             400: "LusidValidationProblemDetails",
@@ -292,15 +292,15 @@
             ['application/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.723'
+        header_params['X-LUSID-SDK-Version'] = '0.1.731'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "ResourceListOfEventTypeSchema",
             404: "str",
```

### Comparing `lusid-notifications-sdk-preview-0.1.723/lusid_notifications/api/events_api.py` & `lusid-notifications-sdk-preview-0.1.731/lusid_notifications/api/events_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.723
+    The version of the OpenAPI document: 0.1.731
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
@@ -150,15 +150,15 @@
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json-patch+json', 'application/json', 'text/json', 'application/*+json'])  # noqa: E501
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.723'
+        header_params['X-LUSID-SDK-Version'] = '0.1.731'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             201: "EventDetails",
             400: "LusidValidationProblemDetails",
```

### Comparing `lusid-notifications-sdk-preview-0.1.723/lusid_notifications/api/notifications_api.py` & `lusid-notifications-sdk-preview-0.1.731/lusid_notifications/api/notifications_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.723
+    The version of the OpenAPI document: 0.1.731
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
@@ -201,15 +201,15 @@
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json-patch+json', 'application/json', 'text/json', 'application/*+json'])  # noqa: E501
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.723'
+        header_params['X-LUSID-SDK-Version'] = '0.1.731'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             201: "Notification",
             400: "LusidValidationProblemDetails",
@@ -384,15 +384,15 @@
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json-patch+json', 'application/json', 'text/json', 'application/*+json'])  # noqa: E501
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.723'
+        header_params['X-LUSID-SDK-Version'] = '0.1.731'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             201: "Notification",
             400: "LusidValidationProblemDetails",
@@ -567,15 +567,15 @@
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json-patch+json', 'application/json', 'text/json', 'application/*+json'])  # noqa: E501
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.723'
+        header_params['X-LUSID-SDK-Version'] = '0.1.731'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             201: "Notification",
             400: "LusidValidationProblemDetails",
@@ -750,15 +750,15 @@
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json-patch+json', 'application/json', 'text/json', 'application/*+json'])  # noqa: E501
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.723'
+        header_params['X-LUSID-SDK-Version'] = '0.1.731'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             201: "Notification",
             400: "LusidValidationProblemDetails",
@@ -930,15 +930,15 @@
             ['application/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.723'
+        header_params['X-LUSID-SDK-Version'] = '0.1.731'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {}
 
         return self.api_client.call_api(
@@ -1107,15 +1107,15 @@
             ['application/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.723'
+        header_params['X-LUSID-SDK-Version'] = '0.1.731'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "Notification",
             400: "LusidValidationProblemDetails",
@@ -1277,15 +1277,15 @@
             ['application/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.723'
+        header_params['X-LUSID-SDK-Version'] = '0.1.731'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "ResourceListOfNotification",
             400: "LusidValidationProblemDetails",
@@ -1480,15 +1480,15 @@
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json-patch+json', 'application/json', 'text/json', 'application/*+json'])  # noqa: E501
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.723'
+        header_params['X-LUSID-SDK-Version'] = '0.1.731'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "Notification",
             400: "LusidValidationProblemDetails",
@@ -1683,15 +1683,15 @@
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json-patch+json', 'application/json', 'text/json', 'application/*+json'])  # noqa: E501
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.723'
+        header_params['X-LUSID-SDK-Version'] = '0.1.731'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "Notification",
             400: "LusidValidationProblemDetails",
@@ -1886,15 +1886,15 @@
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json-patch+json', 'application/json', 'text/json', 'application/*+json'])  # noqa: E501
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.723'
+        header_params['X-LUSID-SDK-Version'] = '0.1.731'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "Notification",
             400: "LusidValidationProblemDetails",
@@ -2089,15 +2089,15 @@
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json-patch+json', 'application/json', 'text/json', 'application/*+json'])  # noqa: E501
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.723'
+        header_params['X-LUSID-SDK-Version'] = '0.1.731'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "Notification",
             400: "LusidValidationProblemDetails",
```

### Comparing `lusid-notifications-sdk-preview-0.1.723/lusid_notifications/api/subscriptions_api.py` & `lusid-notifications-sdk-preview-0.1.731/lusid_notifications/api/subscriptions_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.723
+    The version of the OpenAPI document: 0.1.731
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
@@ -157,15 +157,15 @@
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json-patch+json', 'application/json', 'text/json', 'application/*+json'])  # noqa: E501
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.723'
+        header_params['X-LUSID-SDK-Version'] = '0.1.731'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             201: "Subscription",
             400: "LusidValidationProblemDetails",
@@ -326,15 +326,15 @@
             ['application/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.723'
+        header_params['X-LUSID-SDK-Version'] = '0.1.731'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {}
 
         return self.api_client.call_api(
@@ -492,15 +492,15 @@
             ['application/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.723'
+        header_params['X-LUSID-SDK-Version'] = '0.1.731'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "Subscription",
             400: "LusidValidationProblemDetails",
@@ -680,15 +680,15 @@
             ['application/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.723'
+        header_params['X-LUSID-SDK-Version'] = '0.1.731'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "ResourceListOfSubscription",
             400: "LusidValidationProblemDetails",
@@ -863,15 +863,15 @@
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json-patch+json', 'application/json', 'text/json', 'application/*+json'])  # noqa: E501
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.723'
+        header_params['X-LUSID-SDK-Version'] = '0.1.731'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "Subscription",
             400: "LusidValidationProblemDetails",
```

### Comparing `lusid-notifications-sdk-preview-0.1.723/lusid_notifications/api_client.py` & `lusid-notifications-sdk-preview-0.1.731/lusid_notifications/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # coding: utf-8
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.723
+    The version of the OpenAPI document: 0.1.731
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 from __future__ import absolute_import
 
 import atexit
@@ -75,15 +75,15 @@
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'OpenAPI-Generator/0.1.723/python'
+        self.user_agent = 'OpenAPI-Generator/0.1.731/python'
         self.client_side_validation = configuration.client_side_validation
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.close()
```

### Comparing `lusid-notifications-sdk-preview-0.1.723/lusid_notifications/configuration.py` & `lusid-notifications-sdk-preview-0.1.731/lusid_notifications/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.723
+    The version of the OpenAPI document: 0.1.731
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
@@ -392,16 +392,16 @@
         """Gets the essential information for debugging.
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
-               "Version of the API: 0.1.723\n"\
-               "SDK Package Version: 0.1.723".\
+               "Version of the API: 0.1.731\n"\
+               "SDK Package Version: 0.1.731".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `lusid-notifications-sdk-preview-0.1.723/lusid_notifications/exceptions.py` & `lusid-notifications-sdk-preview-0.1.731/lusid_notifications/exceptions.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.723
+    The version of the OpenAPI document: 0.1.731
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import six
```

### Comparing `lusid-notifications-sdk-preview-0.1.723/lusid_notifications/models/__init__.py` & `lusid-notifications-sdk-preview-0.1.731/lusid_notifications/models/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # flake8: noqa
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.723
+    The version of the OpenAPI document: 0.1.731
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `lusid-notifications-sdk-preview-0.1.723/lusid_notifications/models/access_controlled_action.py` & `lusid-notifications-sdk-preview-0.1.731/lusid_notifications/models/access_controlled_action.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.723
+    The version of the OpenAPI document: 0.1.731
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notifications-sdk-preview-0.1.723/lusid_notifications/models/access_controlled_resource.py` & `lusid-notifications-sdk-preview-0.1.731/lusid_notifications/models/access_controlled_resource.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.723
+    The version of the OpenAPI document: 0.1.731
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notifications-sdk-preview-0.1.723/lusid_notifications/models/action_id.py` & `lusid-notifications-sdk-preview-0.1.731/lusid_notifications/models/action_id.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.723
+    The version of the OpenAPI document: 0.1.731
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notifications-sdk-preview-0.1.723/lusid_notifications/models/attempt.py` & `lusid-notifications-sdk-preview-0.1.731/lusid_notifications/models/attempt.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.723
+    The version of the OpenAPI document: 0.1.731
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notifications-sdk-preview-0.1.723/lusid_notifications/models/attempt_status.py` & `lusid-notifications-sdk-preview-0.1.731/lusid_notifications/models/attempt_status.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.723
+    The version of the OpenAPI document: 0.1.731
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notifications-sdk-preview-0.1.723/lusid_notifications/models/create_aws_sqs_notification.py` & `lusid-notifications-sdk-preview-0.1.731/lusid_notifications/models/create_aws_sqs_notification.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.723
+    The version of the OpenAPI document: 0.1.731
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notifications-sdk-preview-0.1.723/lusid_notifications/models/create_email_notification.py` & `lusid-notifications-sdk-preview-0.1.731/lusid_notifications/models/create_email_notification.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.723
+    The version of the OpenAPI document: 0.1.731
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notifications-sdk-preview-0.1.723/lusid_notifications/models/create_sms_notification.py` & `lusid-notifications-sdk-preview-0.1.731/lusid_notifications/models/create_sms_notification.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.723
+    The version of the OpenAPI document: 0.1.731
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notifications-sdk-preview-0.1.723/lusid_notifications/models/create_subscription.py` & `lusid-notifications-sdk-preview-0.1.731/lusid_notifications/models/update_subscription.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.723
+    The version of the OpenAPI document: 0.1.731
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
@@ -18,15 +18,15 @@
 import pprint
 import re  # noqa: F401
 import six
 
 from lusid_notifications.configuration import Configuration
 
 
-class CreateSubscription(object):
+class UpdateSubscription(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     """
@@ -35,110 +35,87 @@
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
       required_map (dict): The key is attribute name
                            and the value is whether it is 'required' or 'optional'.
     """
     openapi_types = {
-        'id': 'ResourceId',
         'display_name': 'str',
         'description': 'str',
         'status': 'str',
-        'matching_pattern': 'MatchingPattern'
+        'matching_pattern': 'MatchingPattern',
+        'use_as_auth': 'str'
     }
 
     attribute_map = {
-        'id': 'id',
         'display_name': 'displayName',
         'description': 'description',
         'status': 'status',
-        'matching_pattern': 'matchingPattern'
+        'matching_pattern': 'matchingPattern',
+        'use_as_auth': 'useAsAuth'
     }
 
     required_map = {
-        'id': 'required',
         'display_name': 'required',
         'description': 'required',
         'status': 'required',
-        'matching_pattern': 'required'
+        'matching_pattern': 'required',
+        'use_as_auth': 'optional'
     }
 
-    def __init__(self, id=None, display_name=None, description=None, status=None, matching_pattern=None, local_vars_configuration=None):  # noqa: E501
-        """CreateSubscription - a model defined in OpenAPI"
+    def __init__(self, display_name=None, description=None, status=None, matching_pattern=None, use_as_auth=None, local_vars_configuration=None):  # noqa: E501
+        """UpdateSubscription - a model defined in OpenAPI"
         
-        :param id:  (required)
-        :type id: lusid_notifications.ResourceId
         :param display_name:  The name of the subscription (required)
         :type display_name: str
         :param description:  The summary of the services provided by the subscription (required)
         :type description: str
         :param status:  The current status of the subscription. Possible values are: Active, Inactive (required)
         :type status: str
         :param matching_pattern:  (required)
         :type matching_pattern: lusid_notifications.MatchingPattern
+        :param use_as_auth:  The user to authenticate with for subscriptions
+        :type use_as_auth: str
 
         """  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration.get_default_copy()
         self.local_vars_configuration = local_vars_configuration
 
-        self._id = None
         self._display_name = None
         self._description = None
         self._status = None
         self._matching_pattern = None
+        self._use_as_auth = None
         self.discriminator = None
 
-        self.id = id
         self.display_name = display_name
         self.description = description
         self.status = status
         self.matching_pattern = matching_pattern
-
-    @property
-    def id(self):
-        """Gets the id of this CreateSubscription.  # noqa: E501
-
-
-        :return: The id of this CreateSubscription.  # noqa: E501
-        :rtype: lusid_notifications.ResourceId
-        """
-        return self._id
-
-    @id.setter
-    def id(self, id):
-        """Sets the id of this CreateSubscription.
-
-
-        :param id: The id of this CreateSubscription.  # noqa: E501
-        :type id: lusid_notifications.ResourceId
-        """
-        if self.local_vars_configuration.client_side_validation and id is None:  # noqa: E501
-            raise ValueError("Invalid value for `id`, must not be `None`")  # noqa: E501
-
-        self._id = id
+        self.use_as_auth = use_as_auth
 
     @property
     def display_name(self):
-        """Gets the display_name of this CreateSubscription.  # noqa: E501
+        """Gets the display_name of this UpdateSubscription.  # noqa: E501
 
         The name of the subscription  # noqa: E501
 
-        :return: The display_name of this CreateSubscription.  # noqa: E501
+        :return: The display_name of this UpdateSubscription.  # noqa: E501
         :rtype: str
         """
         return self._display_name
 
     @display_name.setter
     def display_name(self, display_name):
-        """Sets the display_name of this CreateSubscription.
+        """Sets the display_name of this UpdateSubscription.
 
         The name of the subscription  # noqa: E501
 
-        :param display_name: The display_name of this CreateSubscription.  # noqa: E501
+        :param display_name: The display_name of this UpdateSubscription.  # noqa: E501
         :type display_name: str
         """
         if self.local_vars_configuration.client_side_validation and display_name is None:  # noqa: E501
             raise ValueError("Invalid value for `display_name`, must not be `None`")  # noqa: E501
         if (self.local_vars_configuration.client_side_validation and
                 display_name is not None and len(display_name) > 64):
             raise ValueError("Invalid value for `display_name`, length must be less than or equal to `64`")  # noqa: E501
@@ -149,30 +126,30 @@
                 display_name is not None and not re.search(r'^[\s\S]*$', display_name)):  # noqa: E501
             raise ValueError(r"Invalid value for `display_name`, must be a follow pattern or equal to `/^[\s\S]*$/`")  # noqa: E501
 
         self._display_name = display_name
 
     @property
     def description(self):
-        """Gets the description of this CreateSubscription.  # noqa: E501
+        """Gets the description of this UpdateSubscription.  # noqa: E501
 
         The summary of the services provided by the subscription  # noqa: E501
 
-        :return: The description of this CreateSubscription.  # noqa: E501
+        :return: The description of this UpdateSubscription.  # noqa: E501
         :rtype: str
         """
         return self._description
 
     @description.setter
     def description(self, description):
-        """Sets the description of this CreateSubscription.
+        """Sets the description of this UpdateSubscription.
 
         The summary of the services provided by the subscription  # noqa: E501
 
-        :param description: The description of this CreateSubscription.  # noqa: E501
+        :param description: The description of this UpdateSubscription.  # noqa: E501
         :type description: str
         """
         if self.local_vars_configuration.client_side_validation and description is None:  # noqa: E501
             raise ValueError("Invalid value for `description`, must not be `None`")  # noqa: E501
         if (self.local_vars_configuration.client_side_validation and
                 description is not None and len(description) > 512):
             raise ValueError("Invalid value for `description`, length must be less than or equal to `512`")  # noqa: E501
@@ -183,63 +160,95 @@
                 description is not None and not re.search(r'^[\s\S]*$', description)):  # noqa: E501
             raise ValueError(r"Invalid value for `description`, must be a follow pattern or equal to `/^[\s\S]*$/`")  # noqa: E501
 
         self._description = description
 
     @property
     def status(self):
-        """Gets the status of this CreateSubscription.  # noqa: E501
+        """Gets the status of this UpdateSubscription.  # noqa: E501
 
         The current status of the subscription. Possible values are: Active, Inactive  # noqa: E501
 
-        :return: The status of this CreateSubscription.  # noqa: E501
+        :return: The status of this UpdateSubscription.  # noqa: E501
         :rtype: str
         """
         return self._status
 
     @status.setter
     def status(self, status):
-        """Sets the status of this CreateSubscription.
+        """Sets the status of this UpdateSubscription.
 
         The current status of the subscription. Possible values are: Active, Inactive  # noqa: E501
 
-        :param status: The status of this CreateSubscription.  # noqa: E501
+        :param status: The status of this UpdateSubscription.  # noqa: E501
         :type status: str
         """
         if self.local_vars_configuration.client_side_validation and status is None:  # noqa: E501
             raise ValueError("Invalid value for `status`, must not be `None`")  # noqa: E501
         if (self.local_vars_configuration.client_side_validation and
                 status is not None and len(status) < 1):
             raise ValueError("Invalid value for `status`, length must be greater than or equal to `1`")  # noqa: E501
 
         self._status = status
 
     @property
     def matching_pattern(self):
-        """Gets the matching_pattern of this CreateSubscription.  # noqa: E501
+        """Gets the matching_pattern of this UpdateSubscription.  # noqa: E501
 
 
-        :return: The matching_pattern of this CreateSubscription.  # noqa: E501
+        :return: The matching_pattern of this UpdateSubscription.  # noqa: E501
         :rtype: lusid_notifications.MatchingPattern
         """
         return self._matching_pattern
 
     @matching_pattern.setter
     def matching_pattern(self, matching_pattern):
-        """Sets the matching_pattern of this CreateSubscription.
+        """Sets the matching_pattern of this UpdateSubscription.
 
 
-        :param matching_pattern: The matching_pattern of this CreateSubscription.  # noqa: E501
+        :param matching_pattern: The matching_pattern of this UpdateSubscription.  # noqa: E501
         :type matching_pattern: lusid_notifications.MatchingPattern
         """
         if self.local_vars_configuration.client_side_validation and matching_pattern is None:  # noqa: E501
             raise ValueError("Invalid value for `matching_pattern`, must not be `None`")  # noqa: E501
 
         self._matching_pattern = matching_pattern
 
+    @property
+    def use_as_auth(self):
+        """Gets the use_as_auth of this UpdateSubscription.  # noqa: E501
+
+        The user to authenticate with for subscriptions  # noqa: E501
+
+        :return: The use_as_auth of this UpdateSubscription.  # noqa: E501
+        :rtype: str
+        """
+        return self._use_as_auth
+
+    @use_as_auth.setter
+    def use_as_auth(self, use_as_auth):
+        """Sets the use_as_auth of this UpdateSubscription.
+
+        The user to authenticate with for subscriptions  # noqa: E501
+
+        :param use_as_auth: The use_as_auth of this UpdateSubscription.  # noqa: E501
+        :type use_as_auth: str
+        """
+        if (self.local_vars_configuration.client_side_validation and
+                use_as_auth is not None and len(use_as_auth) > 64):
+            raise ValueError("Invalid value for `use_as_auth`, length must be less than or equal to `64`")  # noqa: E501
+        if (self.local_vars_configuration.client_side_validation and
+                use_as_auth is not None and len(use_as_auth) < 1):
+            raise ValueError("Invalid value for `use_as_auth`, length must be greater than or equal to `1`")  # noqa: E501
+        if (self.local_vars_configuration.client_side_validation and
+                use_as_auth is not None and not re.search(r'^[a-zA-Z0-9\-_]+$', use_as_auth)):  # noqa: E501
+            raise ValueError(r"Invalid value for `use_as_auth`, must be a follow pattern or equal to `/^[a-zA-Z0-9\-_]+$/`")  # noqa: E501
+
+        self._use_as_auth = use_as_auth
+
     def to_dict(self, serialize=False):
         """Returns the model properties as a dict"""
         result = {}
 
         def convert(x):
             if hasattr(x, "to_dict"):
                 args = getfullargspec(x.to_dict).args
@@ -274,18 +283,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, CreateSubscription):
+        if not isinstance(other, UpdateSubscription):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, CreateSubscription):
+        if not isinstance(other, UpdateSubscription):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `lusid-notifications-sdk-preview-0.1.723/lusid_notifications/models/create_webhook_notification.py` & `lusid-notifications-sdk-preview-0.1.731/lusid_notifications/models/create_webhook_notification.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.723
+    The version of the OpenAPI document: 0.1.731
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notifications-sdk-preview-0.1.723/lusid_notifications/models/delivery.py` & `lusid-notifications-sdk-preview-0.1.731/lusid_notifications/models/delivery.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.723
+    The version of the OpenAPI document: 0.1.731
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notifications-sdk-preview-0.1.723/lusid_notifications/models/event_details.py` & `lusid-notifications-sdk-preview-0.1.731/lusid_notifications/models/event_details.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.723
+    The version of the OpenAPI document: 0.1.731
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notifications-sdk-preview-0.1.723/lusid_notifications/models/event_type_schema.py` & `lusid-notifications-sdk-preview-0.1.731/lusid_notifications/models/event_type_schema.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.723
+    The version of the OpenAPI document: 0.1.731
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notifications-sdk-preview-0.1.723/lusid_notifications/models/id_selector_definition.py` & `lusid-notifications-sdk-preview-0.1.731/lusid_notifications/models/id_selector_definition.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.723
+    The version of the OpenAPI document: 0.1.731
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notifications-sdk-preview-0.1.723/lusid_notifications/models/identifier_part_schema.py` & `lusid-notifications-sdk-preview-0.1.731/lusid_notifications/models/identifier_part_schema.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.723
+    The version of the OpenAPI document: 0.1.731
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notifications-sdk-preview-0.1.723/lusid_notifications/models/link.py` & `lusid-notifications-sdk-preview-0.1.731/lusid_notifications/models/link.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.723
+    The version of the OpenAPI document: 0.1.731
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notifications-sdk-preview-0.1.723/lusid_notifications/models/lusid_problem_details.py` & `lusid-notifications-sdk-preview-0.1.731/lusid_notifications/models/lusid_problem_details.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.723
+    The version of the OpenAPI document: 0.1.731
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notifications-sdk-preview-0.1.723/lusid_notifications/models/lusid_validation_problem_details.py` & `lusid-notifications-sdk-preview-0.1.731/lusid_notifications/models/lusid_validation_problem_details.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.723
+    The version of the OpenAPI document: 0.1.731
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notifications-sdk-preview-0.1.723/lusid_notifications/models/matching_pattern.py` & `lusid-notifications-sdk-preview-0.1.731/lusid_notifications/models/matching_pattern.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.723
+    The version of the OpenAPI document: 0.1.731
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notifications-sdk-preview-0.1.723/lusid_notifications/models/notification.py` & `lusid-notifications-sdk-preview-0.1.731/lusid_notifications/models/notification.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.723
+    The version of the OpenAPI document: 0.1.731
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notifications-sdk-preview-0.1.723/lusid_notifications/models/notification_status.py` & `lusid-notifications-sdk-preview-0.1.731/lusid_notifications/models/notification_status.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.723
+    The version of the OpenAPI document: 0.1.731
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notifications-sdk-preview-0.1.723/lusid_notifications/models/resource_id.py` & `lusid-notifications-sdk-preview-0.1.731/lusid_notifications/models/resource_id.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.723
+    The version of the OpenAPI document: 0.1.731
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notifications-sdk-preview-0.1.723/lusid_notifications/models/resource_list_of_access_controlled_resource.py` & `lusid-notifications-sdk-preview-0.1.731/lusid_notifications/models/resource_list_of_access_controlled_resource.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.723
+    The version of the OpenAPI document: 0.1.731
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notifications-sdk-preview-0.1.723/lusid_notifications/models/resource_list_of_delivery.py` & `lusid-notifications-sdk-preview-0.1.731/lusid_notifications/models/resource_list_of_delivery.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.723
+    The version of the OpenAPI document: 0.1.731
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notifications-sdk-preview-0.1.723/lusid_notifications/models/resource_list_of_event_type_schema.py` & `lusid-notifications-sdk-preview-0.1.731/lusid_notifications/models/resource_list_of_event_type_schema.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.723
+    The version of the OpenAPI document: 0.1.731
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notifications-sdk-preview-0.1.723/lusid_notifications/models/resource_list_of_notification.py` & `lusid-notifications-sdk-preview-0.1.731/lusid_notifications/models/resource_list_of_notification.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.723
+    The version of the OpenAPI document: 0.1.731
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notifications-sdk-preview-0.1.723/lusid_notifications/models/resource_list_of_subscription.py` & `lusid-notifications-sdk-preview-0.1.731/lusid_notifications/models/resource_list_of_subscription.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.723
+    The version of the OpenAPI document: 0.1.731
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notifications-sdk-preview-0.1.723/lusid_notifications/models/subscription.py` & `lusid-notifications-sdk-preview-0.1.731/lusid_notifications/models/subscription.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.723
+    The version of the OpenAPI document: 0.1.731
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
@@ -44,44 +44,47 @@
         'display_name': 'str',
         'description': 'str',
         'status': 'str',
         'matching_pattern': 'MatchingPattern',
         'created_at': 'datetime',
         'created_by': 'str',
         'last_modified_at': 'datetime',
-        'last_modified_by': 'str'
+        'last_modified_by': 'str',
+        'use_as_auth': 'str'
     }
 
     attribute_map = {
         'notifications': 'notifications',
         'id': 'id',
         'display_name': 'displayName',
         'description': 'description',
         'status': 'status',
         'matching_pattern': 'matchingPattern',
         'created_at': 'createdAt',
         'created_by': 'createdBy',
         'last_modified_at': 'lastModifiedAt',
-        'last_modified_by': 'lastModifiedBy'
+        'last_modified_by': 'lastModifiedBy',
+        'use_as_auth': 'useAsAuth'
     }
 
     required_map = {
         'notifications': 'optional',
         'id': 'required',
         'display_name': 'required',
         'description': 'optional',
         'status': 'required',
         'matching_pattern': 'required',
         'created_at': 'required',
         'created_by': 'required',
         'last_modified_at': 'required',
-        'last_modified_by': 'required'
+        'last_modified_by': 'required',
+        'use_as_auth': 'required'
     }
 
-    def __init__(self, notifications=None, id=None, display_name=None, description=None, status=None, matching_pattern=None, created_at=None, created_by=None, last_modified_at=None, last_modified_by=None, local_vars_configuration=None):  # noqa: E501
+    def __init__(self, notifications=None, id=None, display_name=None, description=None, status=None, matching_pattern=None, created_at=None, created_by=None, last_modified_at=None, last_modified_by=None, use_as_auth=None, local_vars_configuration=None):  # noqa: E501
         """Subscription - a model defined in OpenAPI"
         
         :param notifications:  List of notifications belonging to a subscription
         :type notifications: list[lusid_notifications.Notification]
         :param id:  (required)
         :type id: lusid_notifications.ResourceId
         :param display_name:  The name of the subscription (required)
@@ -96,14 +99,16 @@
         :type created_at: datetime
         :param created_by:  The user who made the subscription (required)
         :type created_by: str
         :param last_modified_at:  The time at which the subscription was last modified (required)
         :type last_modified_at: datetime
         :param last_modified_by:  The user who last modified the subscription (required)
         :type last_modified_by: str
+        :param use_as_auth:  The user to use as auth for the subscription (required)
+        :type use_as_auth: str
 
         """  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration.get_default_copy()
         self.local_vars_configuration = local_vars_configuration
 
         self._notifications = None
@@ -112,26 +117,28 @@
         self._description = None
         self._status = None
         self._matching_pattern = None
         self._created_at = None
         self._created_by = None
         self._last_modified_at = None
         self._last_modified_by = None
+        self._use_as_auth = None
         self.discriminator = None
 
         self.notifications = notifications
         self.id = id
         self.display_name = display_name
         self.description = description
         self.status = status
         self.matching_pattern = matching_pattern
         self.created_at = created_at
         self.created_by = created_by
         self.last_modified_at = last_modified_at
         self.last_modified_by = last_modified_by
+        self.use_as_auth = use_as_auth
 
     @property
     def notifications(self):
         """Gets the notifications of this Subscription.  # noqa: E501
 
         List of notifications belonging to a subscription  # noqa: E501
 
@@ -379,14 +386,42 @@
             raise ValueError("Invalid value for `last_modified_by`, must not be `None`")  # noqa: E501
         if (self.local_vars_configuration.client_side_validation and
                 last_modified_by is not None and len(last_modified_by) < 1):
             raise ValueError("Invalid value for `last_modified_by`, length must be greater than or equal to `1`")  # noqa: E501
 
         self._last_modified_by = last_modified_by
 
+    @property
+    def use_as_auth(self):
+        """Gets the use_as_auth of this Subscription.  # noqa: E501
+
+        The user to use as auth for the subscription  # noqa: E501
+
+        :return: The use_as_auth of this Subscription.  # noqa: E501
+        :rtype: str
+        """
+        return self._use_as_auth
+
+    @use_as_auth.setter
+    def use_as_auth(self, use_as_auth):
+        """Sets the use_as_auth of this Subscription.
+
+        The user to use as auth for the subscription  # noqa: E501
+
+        :param use_as_auth: The use_as_auth of this Subscription.  # noqa: E501
+        :type use_as_auth: str
+        """
+        if self.local_vars_configuration.client_side_validation and use_as_auth is None:  # noqa: E501
+            raise ValueError("Invalid value for `use_as_auth`, must not be `None`")  # noqa: E501
+        if (self.local_vars_configuration.client_side_validation and
+                use_as_auth is not None and len(use_as_auth) < 1):
+            raise ValueError("Invalid value for `use_as_auth`, length must be greater than or equal to `1`")  # noqa: E501
+
+        self._use_as_auth = use_as_auth
+
     def to_dict(self, serialize=False):
         """Returns the model properties as a dict"""
         result = {}
 
         def convert(x):
             if hasattr(x, "to_dict"):
                 args = getfullargspec(x.to_dict).args
```

### Comparing `lusid-notifications-sdk-preview-0.1.723/lusid_notifications/models/update_aws_sqs_notification.py` & `lusid-notifications-sdk-preview-0.1.731/lusid_notifications/models/update_aws_sqs_notification.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.723
+    The version of the OpenAPI document: 0.1.731
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notifications-sdk-preview-0.1.723/lusid_notifications/models/update_email_notification.py` & `lusid-notifications-sdk-preview-0.1.731/lusid_notifications/models/update_email_notification.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.723
+    The version of the OpenAPI document: 0.1.731
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notifications-sdk-preview-0.1.723/lusid_notifications/models/update_sms_notification.py` & `lusid-notifications-sdk-preview-0.1.731/lusid_notifications/models/update_sms_notification.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.723
+    The version of the OpenAPI document: 0.1.731
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notifications-sdk-preview-0.1.723/lusid_notifications/models/update_webhook_notification.py` & `lusid-notifications-sdk-preview-0.1.731/lusid_notifications/models/update_webhook_notification.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.723
+    The version of the OpenAPI document: 0.1.731
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notifications-sdk-preview-0.1.723/lusid_notifications/rest.py` & `lusid-notifications-sdk-preview-0.1.731/lusid_notifications/rest.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.723
+    The version of the OpenAPI document: 0.1.731
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `lusid-notifications-sdk-preview-0.1.723/lusid_notifications/utilities/config_keys.json` & `lusid-notifications-sdk-preview-0.1.731/lusid_notifications/utilities/config_keys.json`

 * *Files identical despite different names*

### Comparing `lusid-notifications-sdk-preview-0.1.723/lusid_notifications_sdk_preview.egg-info/SOURCES.txt` & `lusid-notifications-sdk-preview-0.1.731/lusid_notifications_sdk_preview.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lusid-notifications-sdk-preview-0.1.723/setup.py` & `lusid-notifications-sdk-preview-0.1.731/setup.py`

 * *Files identical despite different names*

