# Comparing `tmp/lusid-notification-sdk-preview-0.1.717.tar.gz` & `tmp/lusid-notification-sdk-preview-0.1.741.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/lusid-notification-sdk-preview-0.1.717.tar", last modified: Thu Jun  1 09:48:44 2023, max compression
+gzip compressed data, was "dist/lusid-notification-sdk-preview-0.1.741.tar", last modified: Tue Jun 13 10:34:59 2023, max compression
```

## Comparing `lusid-notification-sdk-preview-0.1.717.tar` & `lusid-notification-sdk-preview-0.1.741.tar`

### file list

```diff
@@ -1,68 +1,68 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 09:48:44.000000 lusid-notification-sdk-preview-0.1.717/
--rw-r--r--   0 root         (0) root         (0)       53 2023-06-01 09:48:16.000000 lusid-notification-sdk-preview-0.1.717/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      379 2023-06-01 09:48:44.000000 lusid-notification-sdk-preview-0.1.717/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     8040 2023-06-01 09:48:16.000000 lusid-notification-sdk-preview-0.1.717/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 09:48:44.000000 lusid-notification-sdk-preview-0.1.717/lusid_notification/
--rw-r--r--   0 root         (0) root         (0)     4452 2023-06-01 09:48:16.000000 lusid-notification-sdk-preview-0.1.717/lusid_notification/__init__.py
--rw-r--r--   0 root         (0) root         (0)       24 2023-06-01 09:48:16.000000 lusid-notification-sdk-preview-0.1.717/lusid_notification/__version__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 09:48:44.000000 lusid-notification-sdk-preview-0.1.717/lusid_notification/api/
--rw-r--r--   0 root         (0) root         (0)      506 2023-06-01 09:48:16.000000 lusid-notification-sdk-preview-0.1.717/lusid_notification/api/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6847 2023-06-01 09:48:16.000000 lusid-notification-sdk-preview-0.1.717/lusid_notification/api/application_metadata_api.py
--rw-r--r--   0 root         (0) root         (0)    10519 2023-06-01 09:48:16.000000 lusid-notification-sdk-preview-0.1.717/lusid_notification/api/deliveries_api.py
--rw-r--r--   0 root         (0) root         (0)    13984 2023-06-01 09:48:16.000000 lusid-notification-sdk-preview-0.1.717/lusid_notification/api/event_types_api.py
--rw-r--r--   0 root         (0) root         (0)     7820 2023-06-01 09:48:16.000000 lusid-notification-sdk-preview-0.1.717/lusid_notification/api/manual_event_api.py
--rw-r--r--   0 root         (0) root         (0)    52797 2023-06-01 09:48:16.000000 lusid-notification-sdk-preview-0.1.717/lusid_notification/api/notifications_api.py
--rw-r--r--   0 root         (0) root         (0)    47803 2023-06-01 09:48:16.000000 lusid-notification-sdk-preview-0.1.717/lusid_notification/api/subscriptions_api.py
--rw-r--r--   0 root         (0) root         (0)    27431 2023-06-01 09:48:16.000000 lusid-notification-sdk-preview-0.1.717/lusid_notification/api_client.py
--rw-r--r--   0 root         (0) root         (0)    16631 2023-06-01 09:48:16.000000 lusid-notification-sdk-preview-0.1.717/lusid_notification/configuration.py
--rw-r--r--   0 root         (0) root         (0)     5099 2023-06-01 09:48:16.000000 lusid-notification-sdk-preview-0.1.717/lusid_notification/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 09:48:44.000000 lusid-notification-sdk-preview-0.1.717/lusid_notification/models/
--rw-r--r--   0 root         (0) root         (0)     3100 2023-06-01 09:48:16.000000 lusid-notification-sdk-preview-0.1.717/lusid_notification/models/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7254 2023-06-01 09:48:16.000000 lusid-notification-sdk-preview-0.1.717/lusid_notification/models/access_controlled_action.py
--rw-r--r--   0 root         (0) root         (0)     9017 2023-06-01 09:48:16.000000 lusid-notification-sdk-preview-0.1.717/lusid_notification/models/access_controlled_resource.py
--rw-r--r--   0 root         (0) root         (0)     7231 2023-06-01 09:48:16.000000 lusid-notification-sdk-preview-0.1.717/lusid_notification/models/action_id.py
--rw-r--r--   0 root         (0) root         (0)    10957 2023-06-01 09:48:16.000000 lusid-notification-sdk-preview-0.1.717/lusid_notification/models/amazon_sqs_notification_type.py
--rw-r--r--   0 root         (0) root         (0)     9234 2023-06-01 09:48:16.000000 lusid-notification-sdk-preview-0.1.717/lusid_notification/models/api_request_notification_type.py
--rw-r--r--   0 root         (0) root         (0)     6508 2023-06-01 09:48:16.000000 lusid-notification-sdk-preview-0.1.717/lusid_notification/models/attempt.py
--rw-r--r--   0 root         (0) root         (0)     5556 2023-06-01 09:48:16.000000 lusid-notification-sdk-preview-0.1.717/lusid_notification/models/attempt_status.py
--rw-r--r--   0 root         (0) root         (0)    11191 2023-06-01 09:48:16.000000 lusid-notification-sdk-preview-0.1.717/lusid_notification/models/create_notification_request.py
--rw-r--r--   0 root         (0) root         (0)    10603 2023-06-01 09:48:16.000000 lusid-notification-sdk-preview-0.1.717/lusid_notification/models/create_subscription.py
--rw-r--r--   0 root         (0) root         (0)    12390 2023-06-01 09:48:16.000000 lusid-notification-sdk-preview-0.1.717/lusid_notification/models/delivery.py
--rw-r--r--   0 root         (0) root         (0)    14935 2023-06-01 09:48:16.000000 lusid-notification-sdk-preview-0.1.717/lusid_notification/models/email_notification_type.py
--rw-r--r--   0 root         (0) root         (0)     9337 2023-06-01 09:48:16.000000 lusid-notification-sdk-preview-0.1.717/lusid_notification/models/event_type_schema.py
--rw-r--r--   0 root         (0) root         (0)     8021 2023-06-01 09:48:16.000000 lusid-notification-sdk-preview-0.1.717/lusid_notification/models/id_selector_definition.py
--rw-r--r--   0 root         (0) root         (0)     9510 2023-06-01 09:48:16.000000 lusid-notification-sdk-preview-0.1.717/lusid_notification/models/identifier_part_schema.py
--rw-r--r--   0 root         (0) root         (0)     6425 2023-06-01 09:48:16.000000 lusid-notification-sdk-preview-0.1.717/lusid_notification/models/link.py
--rw-r--r--   0 root         (0) root         (0)     9539 2023-06-01 09:48:16.000000 lusid-notification-sdk-preview-0.1.717/lusid_notification/models/lusid_problem_details.py
--rw-r--r--   0 root         (0) root         (0)    10704 2023-06-01 09:48:16.000000 lusid-notification-sdk-preview-0.1.717/lusid_notification/models/lusid_validation_problem_details.py
--rw-r--r--   0 root         (0) root         (0)     5086 2023-06-01 09:48:16.000000 lusid-notification-sdk-preview-0.1.717/lusid_notification/models/manual_event.py
--rw-r--r--   0 root         (0) root         (0)     7863 2023-06-01 09:48:16.000000 lusid-notification-sdk-preview-0.1.717/lusid_notification/models/manual_event_body.py
--rw-r--r--   0 root         (0) root         (0)     6827 2023-06-01 09:48:16.000000 lusid-notification-sdk-preview-0.1.717/lusid_notification/models/manual_event_header.py
--rw-r--r--   0 root         (0) root         (0)     4162 2023-06-01 09:48:16.000000 lusid-notification-sdk-preview-0.1.717/lusid_notification/models/manual_event_request.py
--rw-r--r--   0 root         (0) root         (0)     7436 2023-06-01 09:48:16.000000 lusid-notification-sdk-preview-0.1.717/lusid_notification/models/matching_pattern.py
--rw-r--r--   0 root         (0) root         (0)    14867 2023-06-01 09:48:16.000000 lusid-notification-sdk-preview-0.1.717/lusid_notification/models/notification.py
--rw-r--r--   0 root         (0) root         (0)     5154 2023-06-01 09:48:16.000000 lusid-notification-sdk-preview-0.1.717/lusid_notification/models/notification_status.py
--rw-r--r--   0 root         (0) root         (0)     6098 2023-06-01 09:48:16.000000 lusid-notification-sdk-preview-0.1.717/lusid_notification/models/resource_id.py
--rw-r--r--   0 root         (0) root         (0)     7768 2023-06-01 09:48:16.000000 lusid-notification-sdk-preview-0.1.717/lusid_notification/models/resource_list_of_access_controlled_resource.py
--rw-r--r--   0 root         (0) root         (0)     7320 2023-06-01 09:48:16.000000 lusid-notification-sdk-preview-0.1.717/lusid_notification/models/resource_list_of_delivery.py
--rw-r--r--   0 root         (0) root         (0)     7516 2023-06-01 09:48:16.000000 lusid-notification-sdk-preview-0.1.717/lusid_notification/models/resource_list_of_event_type_schema.py
--rw-r--r--   0 root         (0) root         (0)     7432 2023-06-01 09:48:16.000000 lusid-notification-sdk-preview-0.1.717/lusid_notification/models/resource_list_of_notification.py
--rw-r--r--   0 root         (0) root         (0)     7432 2023-06-01 09:48:16.000000 lusid-notification-sdk-preview-0.1.717/lusid_notification/models/resource_list_of_subscription.py
--rw-r--r--   0 root         (0) root         (0)     8012 2023-06-01 09:48:16.000000 lusid-notification-sdk-preview-0.1.717/lusid_notification/models/sms_notification_type.py
--rw-r--r--   0 root         (0) root         (0)    14424 2023-06-01 09:48:16.000000 lusid-notification-sdk-preview-0.1.717/lusid_notification/models/subscription.py
--rw-r--r--   0 root         (0) root         (0)     9020 2023-06-01 09:48:16.000000 lusid-notification-sdk-preview-0.1.717/lusid_notification/models/update_notification_request.py
--rw-r--r--   0 root         (0) root         (0)     9723 2023-06-01 09:48:16.000000 lusid-notification-sdk-preview-0.1.717/lusid_notification/models/update_subscription.py
--rw-r--r--   0 root         (0) root         (0)    15803 2023-06-01 09:48:16.000000 lusid-notification-sdk-preview-0.1.717/lusid_notification/models/webhook_notification_type.py
--rw-r--r--   0 root         (0) root         (0)    13560 2023-06-01 09:48:16.000000 lusid-notification-sdk-preview-0.1.717/lusid_notification/rest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 09:48:44.000000 lusid-notification-sdk-preview-0.1.717/lusid_notification/utilities/
--rw-r--r--   0 root         (0) root         (0)       64 2023-06-01 09:48:16.000000 lusid-notification-sdk-preview-0.1.717/lusid_notification/utilities/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1040 2023-06-01 09:48:16.000000 lusid-notification-sdk-preview-0.1.717/lusid_notification/utilities/config_keys.json
--rw-r--r--   0 root         (0) root         (0)      295 2023-06-01 09:48:16.000000 lusid-notification-sdk-preview-0.1.717/lusid_notification/utilities/config_keys.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 09:48:44.000000 lusid-notification-sdk-preview-0.1.717/lusid_notification_sdk_preview.egg-info/
--rw-r--r--   0 root         (0) root         (0)      379 2023-06-01 09:48:44.000000 lusid-notification-sdk-preview-0.1.717/lusid_notification_sdk_preview.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2734 2023-06-01 09:48:44.000000 lusid-notification-sdk-preview-0.1.717/lusid_notification_sdk_preview.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-01 09:48:44.000000 lusid-notification-sdk-preview-0.1.717/lusid_notification_sdk_preview.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      116 2023-06-01 09:48:44.000000 lusid-notification-sdk-preview-0.1.717/lusid_notification_sdk_preview.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       19 2023-06-01 09:48:44.000000 lusid-notification-sdk-preview-0.1.717/lusid_notification_sdk_preview.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-01 09:48:44.000000 lusid-notification-sdk-preview-0.1.717/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2327 2023-06-01 09:48:16.000000 lusid-notification-sdk-preview-0.1.717/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 10:34:59.000000 lusid-notification-sdk-preview-0.1.741/
+-rw-r--r--   0 root         (0) root         (0)       53 2023-06-13 10:32:53.000000 lusid-notification-sdk-preview-0.1.741/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      379 2023-06-13 10:34:59.000000 lusid-notification-sdk-preview-0.1.741/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     8040 2023-06-13 10:32:53.000000 lusid-notification-sdk-preview-0.1.741/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 10:34:59.000000 lusid-notification-sdk-preview-0.1.741/lusid_notification/
+-rw-r--r--   0 root         (0) root         (0)     4452 2023-06-13 10:32:53.000000 lusid-notification-sdk-preview-0.1.741/lusid_notification/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       24 2023-06-13 10:32:53.000000 lusid-notification-sdk-preview-0.1.741/lusid_notification/__version__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 10:34:59.000000 lusid-notification-sdk-preview-0.1.741/lusid_notification/api/
+-rw-r--r--   0 root         (0) root         (0)      506 2023-06-13 10:32:53.000000 lusid-notification-sdk-preview-0.1.741/lusid_notification/api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6847 2023-06-13 10:32:53.000000 lusid-notification-sdk-preview-0.1.741/lusid_notification/api/application_metadata_api.py
+-rw-r--r--   0 root         (0) root         (0)    10519 2023-06-13 10:32:53.000000 lusid-notification-sdk-preview-0.1.741/lusid_notification/api/deliveries_api.py
+-rw-r--r--   0 root         (0) root         (0)    13984 2023-06-13 10:32:53.000000 lusid-notification-sdk-preview-0.1.741/lusid_notification/api/event_types_api.py
+-rw-r--r--   0 root         (0) root         (0)     7820 2023-06-13 10:32:53.000000 lusid-notification-sdk-preview-0.1.741/lusid_notification/api/manual_event_api.py
+-rw-r--r--   0 root         (0) root         (0)    52797 2023-06-13 10:32:53.000000 lusid-notification-sdk-preview-0.1.741/lusid_notification/api/notifications_api.py
+-rw-r--r--   0 root         (0) root         (0)    47803 2023-06-13 10:32:53.000000 lusid-notification-sdk-preview-0.1.741/lusid_notification/api/subscriptions_api.py
+-rw-r--r--   0 root         (0) root         (0)    27431 2023-06-13 10:32:53.000000 lusid-notification-sdk-preview-0.1.741/lusid_notification/api_client.py
+-rw-r--r--   0 root         (0) root         (0)    16631 2023-06-13 10:32:53.000000 lusid-notification-sdk-preview-0.1.741/lusid_notification/configuration.py
+-rw-r--r--   0 root         (0) root         (0)     5099 2023-06-13 10:32:53.000000 lusid-notification-sdk-preview-0.1.741/lusid_notification/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 10:34:59.000000 lusid-notification-sdk-preview-0.1.741/lusid_notification/models/
+-rw-r--r--   0 root         (0) root         (0)     3100 2023-06-13 10:32:53.000000 lusid-notification-sdk-preview-0.1.741/lusid_notification/models/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7254 2023-06-13 10:32:53.000000 lusid-notification-sdk-preview-0.1.741/lusid_notification/models/access_controlled_action.py
+-rw-r--r--   0 root         (0) root         (0)     9017 2023-06-13 10:32:53.000000 lusid-notification-sdk-preview-0.1.741/lusid_notification/models/access_controlled_resource.py
+-rw-r--r--   0 root         (0) root         (0)     7231 2023-06-13 10:32:53.000000 lusid-notification-sdk-preview-0.1.741/lusid_notification/models/action_id.py
+-rw-r--r--   0 root         (0) root         (0)    10957 2023-06-13 10:32:53.000000 lusid-notification-sdk-preview-0.1.741/lusid_notification/models/amazon_sqs_notification_type.py
+-rw-r--r--   0 root         (0) root         (0)     9234 2023-06-13 10:32:53.000000 lusid-notification-sdk-preview-0.1.741/lusid_notification/models/api_request_notification_type.py
+-rw-r--r--   0 root         (0) root         (0)     6508 2023-06-13 10:32:53.000000 lusid-notification-sdk-preview-0.1.741/lusid_notification/models/attempt.py
+-rw-r--r--   0 root         (0) root         (0)     5556 2023-06-13 10:32:53.000000 lusid-notification-sdk-preview-0.1.741/lusid_notification/models/attempt_status.py
+-rw-r--r--   0 root         (0) root         (0)    11191 2023-06-13 10:32:53.000000 lusid-notification-sdk-preview-0.1.741/lusid_notification/models/create_notification_request.py
+-rw-r--r--   0 root         (0) root         (0)    12413 2023-06-13 10:32:53.000000 lusid-notification-sdk-preview-0.1.741/lusid_notification/models/create_subscription.py
+-rw-r--r--   0 root         (0) root         (0)    12390 2023-06-13 10:32:53.000000 lusid-notification-sdk-preview-0.1.741/lusid_notification/models/delivery.py
+-rw-r--r--   0 root         (0) root         (0)    14935 2023-06-13 10:32:53.000000 lusid-notification-sdk-preview-0.1.741/lusid_notification/models/email_notification_type.py
+-rw-r--r--   0 root         (0) root         (0)    11110 2023-06-13 10:32:53.000000 lusid-notification-sdk-preview-0.1.741/lusid_notification/models/event_type_schema.py
+-rw-r--r--   0 root         (0) root         (0)     8021 2023-06-13 10:32:53.000000 lusid-notification-sdk-preview-0.1.741/lusid_notification/models/id_selector_definition.py
+-rw-r--r--   0 root         (0) root         (0)     9510 2023-06-13 10:32:53.000000 lusid-notification-sdk-preview-0.1.741/lusid_notification/models/identifier_part_schema.py
+-rw-r--r--   0 root         (0) root         (0)     6425 2023-06-13 10:32:53.000000 lusid-notification-sdk-preview-0.1.741/lusid_notification/models/link.py
+-rw-r--r--   0 root         (0) root         (0)     9539 2023-06-13 10:32:53.000000 lusid-notification-sdk-preview-0.1.741/lusid_notification/models/lusid_problem_details.py
+-rw-r--r--   0 root         (0) root         (0)    10704 2023-06-13 10:32:53.000000 lusid-notification-sdk-preview-0.1.741/lusid_notification/models/lusid_validation_problem_details.py
+-rw-r--r--   0 root         (0) root         (0)     5086 2023-06-13 10:32:53.000000 lusid-notification-sdk-preview-0.1.741/lusid_notification/models/manual_event.py
+-rw-r--r--   0 root         (0) root         (0)     7863 2023-06-13 10:32:53.000000 lusid-notification-sdk-preview-0.1.741/lusid_notification/models/manual_event_body.py
+-rw-r--r--   0 root         (0) root         (0)     6827 2023-06-13 10:32:53.000000 lusid-notification-sdk-preview-0.1.741/lusid_notification/models/manual_event_header.py
+-rw-r--r--   0 root         (0) root         (0)     4162 2023-06-13 10:32:53.000000 lusid-notification-sdk-preview-0.1.741/lusid_notification/models/manual_event_request.py
+-rw-r--r--   0 root         (0) root         (0)     7436 2023-06-13 10:32:53.000000 lusid-notification-sdk-preview-0.1.741/lusid_notification/models/matching_pattern.py
+-rw-r--r--   0 root         (0) root         (0)    16373 2023-06-13 10:32:53.000000 lusid-notification-sdk-preview-0.1.741/lusid_notification/models/notification.py
+-rw-r--r--   0 root         (0) root         (0)     5154 2023-06-13 10:32:53.000000 lusid-notification-sdk-preview-0.1.741/lusid_notification/models/notification_status.py
+-rw-r--r--   0 root         (0) root         (0)     6098 2023-06-13 10:32:53.000000 lusid-notification-sdk-preview-0.1.741/lusid_notification/models/resource_id.py
+-rw-r--r--   0 root         (0) root         (0)     7768 2023-06-13 10:32:53.000000 lusid-notification-sdk-preview-0.1.741/lusid_notification/models/resource_list_of_access_controlled_resource.py
+-rw-r--r--   0 root         (0) root         (0)     7320 2023-06-13 10:32:53.000000 lusid-notification-sdk-preview-0.1.741/lusid_notification/models/resource_list_of_delivery.py
+-rw-r--r--   0 root         (0) root         (0)     7516 2023-06-13 10:32:53.000000 lusid-notification-sdk-preview-0.1.741/lusid_notification/models/resource_list_of_event_type_schema.py
+-rw-r--r--   0 root         (0) root         (0)     7432 2023-06-13 10:32:53.000000 lusid-notification-sdk-preview-0.1.741/lusid_notification/models/resource_list_of_notification.py
+-rw-r--r--   0 root         (0) root         (0)     7432 2023-06-13 10:32:53.000000 lusid-notification-sdk-preview-0.1.741/lusid_notification/models/resource_list_of_subscription.py
+-rw-r--r--   0 root         (0) root         (0)     8012 2023-06-13 10:32:53.000000 lusid-notification-sdk-preview-0.1.741/lusid_notification/models/sms_notification_type.py
+-rw-r--r--   0 root         (0) root         (0)    15856 2023-06-13 10:32:53.000000 lusid-notification-sdk-preview-0.1.741/lusid_notification/models/subscription.py
+-rw-r--r--   0 root         (0) root         (0)     9020 2023-06-13 10:32:53.000000 lusid-notification-sdk-preview-0.1.741/lusid_notification/models/update_notification_request.py
+-rw-r--r--   0 root         (0) root         (0)    11551 2023-06-13 10:32:53.000000 lusid-notification-sdk-preview-0.1.741/lusid_notification/models/update_subscription.py
+-rw-r--r--   0 root         (0) root         (0)    15803 2023-06-13 10:32:53.000000 lusid-notification-sdk-preview-0.1.741/lusid_notification/models/webhook_notification_type.py
+-rw-r--r--   0 root         (0) root         (0)    13560 2023-06-13 10:32:53.000000 lusid-notification-sdk-preview-0.1.741/lusid_notification/rest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 10:34:59.000000 lusid-notification-sdk-preview-0.1.741/lusid_notification/utilities/
+-rw-r--r--   0 root         (0) root         (0)       64 2023-06-13 10:32:53.000000 lusid-notification-sdk-preview-0.1.741/lusid_notification/utilities/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1040 2023-06-13 10:32:53.000000 lusid-notification-sdk-preview-0.1.741/lusid_notification/utilities/config_keys.json
+-rw-r--r--   0 root         (0) root         (0)      295 2023-06-13 10:32:53.000000 lusid-notification-sdk-preview-0.1.741/lusid_notification/utilities/config_keys.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 10:34:59.000000 lusid-notification-sdk-preview-0.1.741/lusid_notification_sdk_preview.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      379 2023-06-13 10:34:59.000000 lusid-notification-sdk-preview-0.1.741/lusid_notification_sdk_preview.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2734 2023-06-13 10:34:59.000000 lusid-notification-sdk-preview-0.1.741/lusid_notification_sdk_preview.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-13 10:34:59.000000 lusid-notification-sdk-preview-0.1.741/lusid_notification_sdk_preview.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      116 2023-06-13 10:34:59.000000 lusid-notification-sdk-preview-0.1.741/lusid_notification_sdk_preview.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       19 2023-06-13 10:34:59.000000 lusid-notification-sdk-preview-0.1.741/lusid_notification_sdk_preview.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-13 10:34:59.000000 lusid-notification-sdk-preview-0.1.741/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2327 2023-06-13 10:32:53.000000 lusid-notification-sdk-preview-0.1.741/setup.py
```

### Comparing `lusid-notification-sdk-preview-0.1.717/README.md` & `lusid-notification-sdk-preview-0.1.741/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # lusid-notification-sdk
 FINBOURNE Technology
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
-- API version: 0.1.717
-- Package version: 0.1.717
+- API version: 0.1.741
+- Package version: 0.1.741
 - Build package: org.openapitools.codegen.languages.PythonLegacyClientCodegen
 For more information, please visit [https://www.finbourne.com](https://www.finbourne.com)
 
 ## Requirements.
 
 Python 2.7 and 3.4+
```

### Comparing `lusid-notification-sdk-preview-0.1.717/lusid_notification/__init__.py` & `lusid-notification-sdk-preview-0.1.741/lusid_notification/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,23 +3,23 @@
 # flake8: noqa
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.717
+    The version of the OpenAPI document: 0.1.741
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
-__version__ = "0.1.717"
+__version__ = "0.1.741"
 
 # import apis into sdk package
 from lusid_notification.api.application_metadata_api import ApplicationMetadataApi
 from lusid_notification.api.deliveries_api import DeliveriesApi
 from lusid_notification.api.event_types_api import EventTypesApi
 from lusid_notification.api.manual_event_api import ManualEventApi
 from lusid_notification.api.notifications_api import NotificationsApi
```

### Comparing `lusid-notification-sdk-preview-0.1.717/lusid_notification/api/application_metadata_api.py` & `lusid-notification-sdk-preview-0.1.741/lusid_notification/api/application_metadata_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.717
+    The version of the OpenAPI document: 0.1.741
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
@@ -141,15 +141,15 @@
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.717'
+        header_params['X-LUSID-SDK-Version'] = '0.1.741'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "ResourceListOfAccessControlledResource",
         }
```

### Comparing `lusid-notification-sdk-preview-0.1.717/lusid_notification/api/deliveries_api.py` & `lusid-notification-sdk-preview-0.1.741/lusid_notification/api/deliveries_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.717
+    The version of the OpenAPI document: 0.1.741
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
@@ -179,15 +179,15 @@
             ['application/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.717'
+        header_params['X-LUSID-SDK-Version'] = '0.1.741'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "ResourceListOfDelivery",
             400: "LusidValidationProblemDetails",
```

### Comparing `lusid-notification-sdk-preview-0.1.717/lusid_notification/api/event_types_api.py` & `lusid-notification-sdk-preview-0.1.741/lusid_notification/api/event_types_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.717
+    The version of the OpenAPI document: 0.1.741
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
@@ -160,15 +160,15 @@
             ['application/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.717'
+        header_params['X-LUSID-SDK-Version'] = '0.1.741'
 
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
-        header_params['X-LUSID-SDK-Version'] = '0.1.717'
+        header_params['X-LUSID-SDK-Version'] = '0.1.741'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "ResourceListOfEventTypeSchema",
             404: "str",
```

### Comparing `lusid-notification-sdk-preview-0.1.717/lusid_notification/api/manual_event_api.py` & `lusid-notification-sdk-preview-0.1.741/lusid_notification/api/manual_event_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.717
+    The version of the OpenAPI document: 0.1.741
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
@@ -155,15 +155,15 @@
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json-patch+json', 'application/json', 'text/json', 'application/*+json'])  # noqa: E501
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.717'
+        header_params['X-LUSID-SDK-Version'] = '0.1.741'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             201: "ManualEvent",
             400: "LusidValidationProblemDetails",
```

### Comparing `lusid-notification-sdk-preview-0.1.717/lusid_notification/api/notifications_api.py` & `lusid-notification-sdk-preview-0.1.741/lusid_notification/api/notifications_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.717
+    The version of the OpenAPI document: 0.1.741
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
@@ -195,15 +195,15 @@
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json-patch+json', 'application/json', 'text/json', 'application/*+json'])  # noqa: E501
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.717'
+        header_params['X-LUSID-SDK-Version'] = '0.1.741'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             201: "Notification",
             400: "LusidValidationProblemDetails",
@@ -375,15 +375,15 @@
             ['application/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.717'
+        header_params['X-LUSID-SDK-Version'] = '0.1.741'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {}
 
         return self.api_client.call_api(
@@ -552,15 +552,15 @@
             ['application/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.717'
+        header_params['X-LUSID-SDK-Version'] = '0.1.741'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "Notification",
             400: "LusidValidationProblemDetails",
@@ -722,15 +722,15 @@
             ['application/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.717'
+        header_params['X-LUSID-SDK-Version'] = '0.1.741'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "ResourceListOfNotification",
             400: "LusidValidationProblemDetails",
@@ -925,15 +925,15 @@
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json-patch+json', 'application/json', 'text/json', 'application/*+json'])  # noqa: E501
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.717'
+        header_params['X-LUSID-SDK-Version'] = '0.1.741'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "Notification",
             400: "LusidValidationProblemDetails",
```

### Comparing `lusid-notification-sdk-preview-0.1.717/lusid_notification/api/subscriptions_api.py` & `lusid-notification-sdk-preview-0.1.741/lusid_notification/api/subscriptions_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.717
+    The version of the OpenAPI document: 0.1.741
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
-        header_params['X-LUSID-SDK-Version'] = '0.1.717'
+        header_params['X-LUSID-SDK-Version'] = '0.1.741'
 
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
-        header_params['X-LUSID-SDK-Version'] = '0.1.717'
+        header_params['X-LUSID-SDK-Version'] = '0.1.741'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {}
 
         return self.api_client.call_api(
@@ -492,15 +492,15 @@
             ['application/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.717'
+        header_params['X-LUSID-SDK-Version'] = '0.1.741'
 
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
-        header_params['X-LUSID-SDK-Version'] = '0.1.717'
+        header_params['X-LUSID-SDK-Version'] = '0.1.741'
 
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
-        header_params['X-LUSID-SDK-Version'] = '0.1.717'
+        header_params['X-LUSID-SDK-Version'] = '0.1.741'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "Subscription",
             400: "LusidValidationProblemDetails",
```

### Comparing `lusid-notification-sdk-preview-0.1.717/lusid_notification/api_client.py` & `lusid-notification-sdk-preview-0.1.741/lusid_notification/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # coding: utf-8
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.717
+    The version of the OpenAPI document: 0.1.741
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
-        self.user_agent = 'OpenAPI-Generator/0.1.717/python'
+        self.user_agent = 'OpenAPI-Generator/0.1.741/python'
         self.client_side_validation = configuration.client_side_validation
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.close()
```

### Comparing `lusid-notification-sdk-preview-0.1.717/lusid_notification/configuration.py` & `lusid-notification-sdk-preview-0.1.741/lusid_notification/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.717
+    The version of the OpenAPI document: 0.1.741
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
-               "Version of the API: 0.1.717\n"\
-               "SDK Package Version: 0.1.717".\
+               "Version of the API: 0.1.741\n"\
+               "SDK Package Version: 0.1.741".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `lusid-notification-sdk-preview-0.1.717/lusid_notification/exceptions.py` & `lusid-notification-sdk-preview-0.1.741/lusid_notification/exceptions.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.717
+    The version of the OpenAPI document: 0.1.741
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import six
```

### Comparing `lusid-notification-sdk-preview-0.1.717/lusid_notification/models/__init__.py` & `lusid-notification-sdk-preview-0.1.741/lusid_notification/models/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # flake8: noqa
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.717
+    The version of the OpenAPI document: 0.1.741
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `lusid-notification-sdk-preview-0.1.717/lusid_notification/models/access_controlled_action.py` & `lusid-notification-sdk-preview-0.1.741/lusid_notification/models/access_controlled_action.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.717
+    The version of the OpenAPI document: 0.1.741
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.717/lusid_notification/models/access_controlled_resource.py` & `lusid-notification-sdk-preview-0.1.741/lusid_notification/models/access_controlled_resource.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.717
+    The version of the OpenAPI document: 0.1.741
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.717/lusid_notification/models/action_id.py` & `lusid-notification-sdk-preview-0.1.741/lusid_notification/models/action_id.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.717
+    The version of the OpenAPI document: 0.1.741
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.717/lusid_notification/models/amazon_sqs_notification_type.py` & `lusid-notification-sdk-preview-0.1.741/lusid_notification/models/amazon_sqs_notification_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.717
+    The version of the OpenAPI document: 0.1.741
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.717/lusid_notification/models/api_request_notification_type.py` & `lusid-notification-sdk-preview-0.1.741/lusid_notification/models/api_request_notification_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.717
+    The version of the OpenAPI document: 0.1.741
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.717/lusid_notification/models/attempt.py` & `lusid-notification-sdk-preview-0.1.741/lusid_notification/models/attempt.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.717
+    The version of the OpenAPI document: 0.1.741
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.717/lusid_notification/models/attempt_status.py` & `lusid-notification-sdk-preview-0.1.741/lusid_notification/models/attempt_status.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.717
+    The version of the OpenAPI document: 0.1.741
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.717/lusid_notification/models/create_notification_request.py` & `lusid-notification-sdk-preview-0.1.741/lusid_notification/models/create_notification_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.717
+    The version of the OpenAPI document: 0.1.741
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.717/lusid_notification/models/create_subscription.py` & `lusid-notification-sdk-preview-0.1.741/lusid_notification/models/update_subscription.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.717
+    The version of the OpenAPI document: 0.1.741
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
@@ -18,15 +18,15 @@
 import pprint
 import re  # noqa: F401
 import six
 
 from lusid_notification.configuration import Configuration
 
 
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
         'description': 'optional',
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
-        :type id: lusid_notification.ResourceId
         :param display_name:  The name of the subscription (required)
         :type display_name: str
         :param description:  The summary of the services provided by the subscription
         :type description: str
         :param status:  The current status of the subscription. Possible values are: Active, Inactive (required)
         :type status: str
         :param matching_pattern:  (required)
         :type matching_pattern: lusid_notification.MatchingPattern
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
-        :rtype: lusid_notification.ResourceId
-        """
-        return self._id
-
-    @id.setter
-    def id(self, id):
-        """Sets the id of this CreateSubscription.
-
-
-        :param id: The id of this CreateSubscription.  # noqa: E501
-        :type id: lusid_notification.ResourceId
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
         if (self.local_vars_configuration.client_side_validation and
                 description is not None and len(description) > 512):
             raise ValueError("Invalid value for `description`, length must be less than or equal to `512`")  # noqa: E501
         if (self.local_vars_configuration.client_side_validation and
                 description is not None and len(description) < 1):
@@ -181,63 +158,95 @@
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
         :rtype: lusid_notification.MatchingPattern
         """
         return self._matching_pattern
 
     @matching_pattern.setter
     def matching_pattern(self, matching_pattern):
-        """Sets the matching_pattern of this CreateSubscription.
+        """Sets the matching_pattern of this UpdateSubscription.
 
 
-        :param matching_pattern: The matching_pattern of this CreateSubscription.  # noqa: E501
+        :param matching_pattern: The matching_pattern of this UpdateSubscription.  # noqa: E501
         :type matching_pattern: lusid_notification.MatchingPattern
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
@@ -272,18 +281,18 @@
 
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

### Comparing `lusid-notification-sdk-preview-0.1.717/lusid_notification/models/delivery.py` & `lusid-notification-sdk-preview-0.1.741/lusid_notification/models/delivery.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.717
+    The version of the OpenAPI document: 0.1.741
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.717/lusid_notification/models/email_notification_type.py` & `lusid-notification-sdk-preview-0.1.741/lusid_notification/models/email_notification_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.717
+    The version of the OpenAPI document: 0.1.741
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.717/lusid_notification/models/event_type_schema.py` & `lusid-notification-sdk-preview-0.1.741/lusid_notification/models/event_type_schema.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.717
+    The version of the OpenAPI document: 0.1.741
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
@@ -41,75 +41,89 @@
     openapi_types = {
         'id': 'str',
         'display_name': 'str',
         'description': 'str',
         'entity': 'str',
         'application': 'str',
         'json_schema': 'object',
+        'header_schema': 'object',
+        'body_schema': 'object',
         'href': 'str'
     }
 
     attribute_map = {
         'id': 'id',
         'display_name': 'displayName',
         'description': 'description',
         'entity': 'entity',
         'application': 'application',
         'json_schema': 'jsonSchema',
+        'header_schema': 'headerSchema',
+        'body_schema': 'bodySchema',
         'href': 'href'
     }
 
     required_map = {
         'id': 'optional',
         'display_name': 'optional',
         'description': 'optional',
         'entity': 'optional',
         'application': 'optional',
-        'json_schema': 'required',
+        'json_schema': 'optional',
+        'header_schema': 'optional',
+        'body_schema': 'optional',
         'href': 'optional'
     }
 
-    def __init__(self, id=None, display_name=None, description=None, entity=None, application=None, json_schema=None, href=None, local_vars_configuration=None):  # noqa: E501
+    def __init__(self, id=None, display_name=None, description=None, entity=None, application=None, json_schema=None, header_schema=None, body_schema=None, href=None, local_vars_configuration=None):  # noqa: E501
         """EventTypeSchema - a model defined in OpenAPI"
         
         :param id:  The identifier of the event type
         :type id: str
         :param display_name:  Identifier name of the event
         :type display_name: str
         :param description:  The summary of the event
         :type description: str
         :param entity:  The entity against which the event originated
         :type entity: str
         :param application:  The application associated with the event
         :type application: str
-        :param json_schema:  The schema of the event (required)
+        :param json_schema:  The schema of the event
         :type json_schema: object
+        :param header_schema:  Header
+        :type header_schema: object
+        :param body_schema:  Body
+        :type body_schema: object
         :param href:  A URI for retrieving this schema
         :type href: str
 
         """  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration.get_default_copy()
         self.local_vars_configuration = local_vars_configuration
 
         self._id = None
         self._display_name = None
         self._description = None
         self._entity = None
         self._application = None
         self._json_schema = None
+        self._header_schema = None
+        self._body_schema = None
         self._href = None
         self.discriminator = None
 
         self.id = id
         self.display_name = display_name
         self.description = description
         self.entity = entity
         self.application = application
         self.json_schema = json_schema
+        self.header_schema = header_schema
+        self.body_schema = body_schema
         self.href = href
 
     @property
     def id(self):
         """Gets the id of this EventTypeSchema.  # noqa: E501
 
         The identifier of the event type  # noqa: E501
@@ -243,14 +257,60 @@
         :param json_schema: The json_schema of this EventTypeSchema.  # noqa: E501
         :type json_schema: object
         """
 
         self._json_schema = json_schema
 
     @property
+    def header_schema(self):
+        """Gets the header_schema of this EventTypeSchema.  # noqa: E501
+
+        Header  # noqa: E501
+
+        :return: The header_schema of this EventTypeSchema.  # noqa: E501
+        :rtype: object
+        """
+        return self._header_schema
+
+    @header_schema.setter
+    def header_schema(self, header_schema):
+        """Sets the header_schema of this EventTypeSchema.
+
+        Header  # noqa: E501
+
+        :param header_schema: The header_schema of this EventTypeSchema.  # noqa: E501
+        :type header_schema: object
+        """
+
+        self._header_schema = header_schema
+
+    @property
+    def body_schema(self):
+        """Gets the body_schema of this EventTypeSchema.  # noqa: E501
+
+        Body  # noqa: E501
+
+        :return: The body_schema of this EventTypeSchema.  # noqa: E501
+        :rtype: object
+        """
+        return self._body_schema
+
+    @body_schema.setter
+    def body_schema(self, body_schema):
+        """Sets the body_schema of this EventTypeSchema.
+
+        Body  # noqa: E501
+
+        :param body_schema: The body_schema of this EventTypeSchema.  # noqa: E501
+        :type body_schema: object
+        """
+
+        self._body_schema = body_schema
+
+    @property
     def href(self):
         """Gets the href of this EventTypeSchema.  # noqa: E501
 
         A URI for retrieving this schema  # noqa: E501
 
         :return: The href of this EventTypeSchema.  # noqa: E501
         :rtype: str
```

### Comparing `lusid-notification-sdk-preview-0.1.717/lusid_notification/models/id_selector_definition.py` & `lusid-notification-sdk-preview-0.1.741/lusid_notification/models/id_selector_definition.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.717
+    The version of the OpenAPI document: 0.1.741
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.717/lusid_notification/models/identifier_part_schema.py` & `lusid-notification-sdk-preview-0.1.741/lusid_notification/models/identifier_part_schema.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.717
+    The version of the OpenAPI document: 0.1.741
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.717/lusid_notification/models/link.py` & `lusid-notification-sdk-preview-0.1.741/lusid_notification/models/link.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.717
+    The version of the OpenAPI document: 0.1.741
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.717/lusid_notification/models/lusid_problem_details.py` & `lusid-notification-sdk-preview-0.1.741/lusid_notification/models/lusid_problem_details.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.717
+    The version of the OpenAPI document: 0.1.741
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.717/lusid_notification/models/lusid_validation_problem_details.py` & `lusid-notification-sdk-preview-0.1.741/lusid_notification/models/lusid_validation_problem_details.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.717
+    The version of the OpenAPI document: 0.1.741
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.717/lusid_notification/models/manual_event.py` & `lusid-notification-sdk-preview-0.1.741/lusid_notification/models/manual_event.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.717
+    The version of the OpenAPI document: 0.1.741
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.717/lusid_notification/models/manual_event_body.py` & `lusid-notification-sdk-preview-0.1.741/lusid_notification/models/manual_event_body.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.717
+    The version of the OpenAPI document: 0.1.741
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.717/lusid_notification/models/manual_event_header.py` & `lusid-notification-sdk-preview-0.1.741/lusid_notification/models/manual_event_header.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.717
+    The version of the OpenAPI document: 0.1.741
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.717/lusid_notification/models/manual_event_request.py` & `lusid-notification-sdk-preview-0.1.741/lusid_notification/models/manual_event_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.717
+    The version of the OpenAPI document: 0.1.741
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.717/lusid_notification/models/matching_pattern.py` & `lusid-notification-sdk-preview-0.1.741/lusid_notification/models/matching_pattern.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.717
+    The version of the OpenAPI document: 0.1.741
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.717/lusid_notification/models/notification.py` & `lusid-notification-sdk-preview-0.1.741/lusid_notification/models/notification.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.717
+    The version of the OpenAPI document: 0.1.741
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
@@ -38,86 +38,93 @@
       required_map (dict): The key is attribute name
                            and the value is whether it is 'required' or 'optional'.
     """
     openapi_types = {
         'notification_id': 'str',
         'display_name': 'str',
         'description': 'str',
-        'notification_type': 'object',
+        'notification_type': 'OneOfAmazonSqsNotificationTypeApiRequestNotificationTypeEmailNotificationTypeSmsNotificationTypeWebhookNotificationType',
         'created_at': 'datetime',
         'user_id_created': 'str',
         'modified_at': 'datetime',
-        'user_id_modified': 'str'
+        'user_id_modified': 'str',
+        'href': 'str'
     }
 
     attribute_map = {
         'notification_id': 'notificationId',
         'display_name': 'displayName',
         'description': 'description',
         'notification_type': 'notificationType',
         'created_at': 'createdAt',
         'user_id_created': 'userIdCreated',
         'modified_at': 'modifiedAt',
-        'user_id_modified': 'userIdModified'
+        'user_id_modified': 'userIdModified',
+        'href': 'href'
     }
 
     required_map = {
         'notification_id': 'required',
         'display_name': 'optional',
         'description': 'optional',
         'notification_type': 'required',
         'created_at': 'required',
         'user_id_created': 'required',
         'modified_at': 'required',
-        'user_id_modified': 'required'
+        'user_id_modified': 'required',
+        'href': 'optional'
     }
 
-    def __init__(self, notification_id=None, display_name=None, description=None, notification_type=None, created_at=None, user_id_created=None, modified_at=None, user_id_modified=None, local_vars_configuration=None):  # noqa: E501
+    def __init__(self, notification_id=None, display_name=None, description=None, notification_type=None, created_at=None, user_id_created=None, modified_at=None, user_id_modified=None, href=None, local_vars_configuration=None):  # noqa: E501
         """Notification - a model defined in OpenAPI"
         
         :param notification_id:  The identifier of the notification (required)
         :type notification_id: str
         :param display_name:  The name of the notification
         :type display_name: str
         :param description:  The summary of the services provided by the notification
         :type description: str
         :param notification_type:  The type and contents of the notification (required)
-        :type notification_type: object
+        :type notification_type: lusid_notification.OneOfAmazonSqsNotificationTypeApiRequestNotificationTypeEmailNotificationTypeSmsNotificationTypeWebhookNotificationType
         :param created_at:  The time at which the subscription was made (required)
         :type created_at: datetime
         :param user_id_created:  The user who made the subscription (required)
         :type user_id_created: str
         :param modified_at:  The time at which the subscription was last modified (required)
         :type modified_at: datetime
         :param user_id_modified:  The user who last modified the subscription (required)
         :type user_id_modified: str
+        :param href:  A URI for retrieving this notification
+        :type href: str
 
         """  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration.get_default_copy()
         self.local_vars_configuration = local_vars_configuration
 
         self._notification_id = None
         self._display_name = None
         self._description = None
         self._notification_type = None
         self._created_at = None
         self._user_id_created = None
         self._modified_at = None
         self._user_id_modified = None
+        self._href = None
         self.discriminator = None
 
         self.notification_id = notification_id
         self.display_name = display_name
         self.description = description
         self.notification_type = notification_type
         self.created_at = created_at
         self.user_id_created = user_id_created
         self.modified_at = modified_at
         self.user_id_modified = user_id_modified
+        self.href = href
 
     @property
     def notification_id(self):
         """Gets the notification_id of this Notification.  # noqa: E501
 
         The identifier of the notification  # noqa: E501
 
@@ -210,27 +217,29 @@
     @property
     def notification_type(self):
         """Gets the notification_type of this Notification.  # noqa: E501
 
         The type and contents of the notification  # noqa: E501
 
         :return: The notification_type of this Notification.  # noqa: E501
-        :rtype: object
+        :rtype: lusid_notification.OneOfAmazonSqsNotificationTypeApiRequestNotificationTypeEmailNotificationTypeSmsNotificationTypeWebhookNotificationType
         """
         return self._notification_type
 
     @notification_type.setter
     def notification_type(self, notification_type):
         """Sets the notification_type of this Notification.
 
         The type and contents of the notification  # noqa: E501
 
         :param notification_type: The notification_type of this Notification.  # noqa: E501
-        :type notification_type: object
+        :type notification_type: lusid_notification.OneOfAmazonSqsNotificationTypeApiRequestNotificationTypeEmailNotificationTypeSmsNotificationTypeWebhookNotificationType
         """
+        if self.local_vars_configuration.client_side_validation and notification_type is None:  # noqa: E501
+            raise ValueError("Invalid value for `notification_type`, must not be `None`")  # noqa: E501
 
         self._notification_type = notification_type
 
     @property
     def created_at(self):
         """Gets the created_at of this Notification.  # noqa: E501
 
@@ -332,14 +341,37 @@
             raise ValueError("Invalid value for `user_id_modified`, must not be `None`")  # noqa: E501
         if (self.local_vars_configuration.client_side_validation and
                 user_id_modified is not None and len(user_id_modified) < 1):
             raise ValueError("Invalid value for `user_id_modified`, length must be greater than or equal to `1`")  # noqa: E501
 
         self._user_id_modified = user_id_modified
 
+    @property
+    def href(self):
+        """Gets the href of this Notification.  # noqa: E501
+
+        A URI for retrieving this notification  # noqa: E501
+
+        :return: The href of this Notification.  # noqa: E501
+        :rtype: str
+        """
+        return self._href
+
+    @href.setter
+    def href(self, href):
+        """Sets the href of this Notification.
+
+        A URI for retrieving this notification  # noqa: E501
+
+        :param href: The href of this Notification.  # noqa: E501
+        :type href: str
+        """
+
+        self._href = href
+
     def to_dict(self, serialize=False):
         """Returns the model properties as a dict"""
         result = {}
 
         def convert(x):
             if hasattr(x, "to_dict"):
                 args = getfullargspec(x.to_dict).args
```

### Comparing `lusid-notification-sdk-preview-0.1.717/lusid_notification/models/notification_status.py` & `lusid-notification-sdk-preview-0.1.741/lusid_notification/models/notification_status.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.717
+    The version of the OpenAPI document: 0.1.741
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.717/lusid_notification/models/resource_id.py` & `lusid-notification-sdk-preview-0.1.741/lusid_notification/models/resource_id.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.717
+    The version of the OpenAPI document: 0.1.741
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.717/lusid_notification/models/resource_list_of_access_controlled_resource.py` & `lusid-notification-sdk-preview-0.1.741/lusid_notification/models/resource_list_of_access_controlled_resource.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.717
+    The version of the OpenAPI document: 0.1.741
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.717/lusid_notification/models/resource_list_of_delivery.py` & `lusid-notification-sdk-preview-0.1.741/lusid_notification/models/resource_list_of_delivery.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.717
+    The version of the OpenAPI document: 0.1.741
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.717/lusid_notification/models/resource_list_of_event_type_schema.py` & `lusid-notification-sdk-preview-0.1.741/lusid_notification/models/resource_list_of_event_type_schema.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.717
+    The version of the OpenAPI document: 0.1.741
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.717/lusid_notification/models/resource_list_of_notification.py` & `lusid-notification-sdk-preview-0.1.741/lusid_notification/models/resource_list_of_notification.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.717
+    The version of the OpenAPI document: 0.1.741
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.717/lusid_notification/models/resource_list_of_subscription.py` & `lusid-notification-sdk-preview-0.1.741/lusid_notification/models/resource_list_of_subscription.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.717
+    The version of the OpenAPI document: 0.1.741
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.717/lusid_notification/models/sms_notification_type.py` & `lusid-notification-sdk-preview-0.1.741/lusid_notification/models/sms_notification_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.717
+    The version of the OpenAPI document: 0.1.741
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.717/lusid_notification/models/subscription.py` & `lusid-notification-sdk-preview-0.1.741/lusid_notification/models/subscription.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.717
+    The version of the OpenAPI document: 0.1.741
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
@@ -43,42 +43,45 @@
         'display_name': 'str',
         'description': 'str',
         'status': 'str',
         'matching_pattern': 'MatchingPattern',
         'created_at': 'datetime',
         'user_id_created': 'str',
         'modified_at': 'datetime',
-        'user_id_modified': 'str'
+        'user_id_modified': 'str',
+        'use_as_auth': 'str'
     }
 
     attribute_map = {
         'id': 'id',
         'display_name': 'displayName',
         'description': 'description',
         'status': 'status',
         'matching_pattern': 'matchingPattern',
         'created_at': 'createdAt',
         'user_id_created': 'userIdCreated',
         'modified_at': 'modifiedAt',
-        'user_id_modified': 'userIdModified'
+        'user_id_modified': 'userIdModified',
+        'use_as_auth': 'useAsAuth'
     }
 
     required_map = {
         'id': 'required',
         'display_name': 'required',
         'description': 'optional',
         'status': 'required',
         'matching_pattern': 'required',
         'created_at': 'required',
         'user_id_created': 'required',
         'modified_at': 'required',
-        'user_id_modified': 'required'
+        'user_id_modified': 'required',
+        'use_as_auth': 'required'
     }
 
-    def __init__(self, id=None, display_name=None, description=None, status=None, matching_pattern=None, created_at=None, user_id_created=None, modified_at=None, user_id_modified=None, local_vars_configuration=None):  # noqa: E501
+    def __init__(self, id=None, display_name=None, description=None, status=None, matching_pattern=None, created_at=None, user_id_created=None, modified_at=None, user_id_modified=None, use_as_auth=None, local_vars_configuration=None):  # noqa: E501
         """Subscription - a model defined in OpenAPI"
         
         :param id:  (required)
         :type id: lusid_notification.ResourceId
         :param display_name:  The name of the subscription (required)
         :type display_name: str
         :param description:  The summary of the services provided by the subscription
@@ -91,14 +94,16 @@
         :type created_at: datetime
         :param user_id_created:  The user who made the subscription (required)
         :type user_id_created: str
         :param modified_at:  The time at which the subscription was last modified (required)
         :type modified_at: datetime
         :param user_id_modified:  The user who last modified the subscription (required)
         :type user_id_modified: str
+        :param use_as_auth:  The user to use as auth for the subscription (required)
+        :type use_as_auth: str
 
         """  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration.get_default_copy()
         self.local_vars_configuration = local_vars_configuration
 
         self._id = None
@@ -106,25 +111,27 @@
         self._description = None
         self._status = None
         self._matching_pattern = None
         self._created_at = None
         self._user_id_created = None
         self._modified_at = None
         self._user_id_modified = None
+        self._use_as_auth = None
         self.discriminator = None
 
         self.id = id
         self.display_name = display_name
         self.description = description
         self.status = status
         self.matching_pattern = matching_pattern
         self.created_at = created_at
         self.user_id_created = user_id_created
         self.modified_at = modified_at
         self.user_id_modified = user_id_modified
+        self.use_as_auth = use_as_auth
 
     @property
     def id(self):
         """Gets the id of this Subscription.  # noqa: E501
 
 
         :return: The id of this Subscription.  # noqa: E501
@@ -349,14 +356,42 @@
             raise ValueError("Invalid value for `user_id_modified`, must not be `None`")  # noqa: E501
         if (self.local_vars_configuration.client_side_validation and
                 user_id_modified is not None and len(user_id_modified) < 1):
             raise ValueError("Invalid value for `user_id_modified`, length must be greater than or equal to `1`")  # noqa: E501
 
         self._user_id_modified = user_id_modified
 
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

### Comparing `lusid-notification-sdk-preview-0.1.717/lusid_notification/models/update_notification_request.py` & `lusid-notification-sdk-preview-0.1.741/lusid_notification/models/update_notification_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.717
+    The version of the OpenAPI document: 0.1.741
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.717/lusid_notification/models/update_subscription.py` & `lusid-notification-sdk-preview-0.1.741/lusid_notification/models/create_subscription.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.717
+    The version of the OpenAPI document: 0.1.741
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
@@ -18,15 +18,15 @@
 import pprint
 import re  # noqa: F401
 import six
 
 from lusid_notification.configuration import Configuration
 
 
-class UpdateSubscription(object):
+class CreateSubscription(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     """
@@ -35,80 +35,117 @@
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
       required_map (dict): The key is attribute name
                            and the value is whether it is 'required' or 'optional'.
     """
     openapi_types = {
+        'id': 'ResourceId',
         'display_name': 'str',
         'description': 'str',
         'status': 'str',
-        'matching_pattern': 'MatchingPattern'
+        'matching_pattern': 'MatchingPattern',
+        'use_as_auth': 'str'
     }
 
     attribute_map = {
+        'id': 'id',
         'display_name': 'displayName',
         'description': 'description',
         'status': 'status',
-        'matching_pattern': 'matchingPattern'
+        'matching_pattern': 'matchingPattern',
+        'use_as_auth': 'useAsAuth'
     }
 
     required_map = {
+        'id': 'required',
         'display_name': 'required',
         'description': 'optional',
         'status': 'required',
-        'matching_pattern': 'required'
+        'matching_pattern': 'required',
+        'use_as_auth': 'optional'
     }
 
-    def __init__(self, display_name=None, description=None, status=None, matching_pattern=None, local_vars_configuration=None):  # noqa: E501
-        """UpdateSubscription - a model defined in OpenAPI"
+    def __init__(self, id=None, display_name=None, description=None, status=None, matching_pattern=None, use_as_auth=None, local_vars_configuration=None):  # noqa: E501
+        """CreateSubscription - a model defined in OpenAPI"
         
+        :param id:  (required)
+        :type id: lusid_notification.ResourceId
         :param display_name:  The name of the subscription (required)
         :type display_name: str
         :param description:  The summary of the services provided by the subscription
         :type description: str
         :param status:  The current status of the subscription. Possible values are: Active, Inactive (required)
         :type status: str
         :param matching_pattern:  (required)
         :type matching_pattern: lusid_notification.MatchingPattern
+        :param use_as_auth:  The user to authenticate the subscription
+        :type use_as_auth: str
 
         """  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration.get_default_copy()
         self.local_vars_configuration = local_vars_configuration
 
+        self._id = None
         self._display_name = None
         self._description = None
         self._status = None
         self._matching_pattern = None
+        self._use_as_auth = None
         self.discriminator = None
 
+        self.id = id
         self.display_name = display_name
         self.description = description
         self.status = status
         self.matching_pattern = matching_pattern
+        self.use_as_auth = use_as_auth
+
+    @property
+    def id(self):
+        """Gets the id of this CreateSubscription.  # noqa: E501
+
+
+        :return: The id of this CreateSubscription.  # noqa: E501
+        :rtype: lusid_notification.ResourceId
+        """
+        return self._id
+
+    @id.setter
+    def id(self, id):
+        """Sets the id of this CreateSubscription.
+
+
+        :param id: The id of this CreateSubscription.  # noqa: E501
+        :type id: lusid_notification.ResourceId
+        """
+        if self.local_vars_configuration.client_side_validation and id is None:  # noqa: E501
+            raise ValueError("Invalid value for `id`, must not be `None`")  # noqa: E501
+
+        self._id = id
 
     @property
     def display_name(self):
-        """Gets the display_name of this UpdateSubscription.  # noqa: E501
+        """Gets the display_name of this CreateSubscription.  # noqa: E501
 
         The name of the subscription  # noqa: E501
 
-        :return: The display_name of this UpdateSubscription.  # noqa: E501
+        :return: The display_name of this CreateSubscription.  # noqa: E501
         :rtype: str
         """
         return self._display_name
 
     @display_name.setter
     def display_name(self, display_name):
-        """Sets the display_name of this UpdateSubscription.
+        """Sets the display_name of this CreateSubscription.
 
         The name of the subscription  # noqa: E501
 
-        :param display_name: The display_name of this UpdateSubscription.  # noqa: E501
+        :param display_name: The display_name of this CreateSubscription.  # noqa: E501
         :type display_name: str
         """
         if self.local_vars_configuration.client_side_validation and display_name is None:  # noqa: E501
             raise ValueError("Invalid value for `display_name`, must not be `None`")  # noqa: E501
         if (self.local_vars_configuration.client_side_validation and
                 display_name is not None and len(display_name) > 64):
             raise ValueError("Invalid value for `display_name`, length must be less than or equal to `64`")  # noqa: E501
@@ -119,30 +156,30 @@
                 display_name is not None and not re.search(r'^[\s\S]*$', display_name)):  # noqa: E501
             raise ValueError(r"Invalid value for `display_name`, must be a follow pattern or equal to `/^[\s\S]*$/`")  # noqa: E501
 
         self._display_name = display_name
 
     @property
     def description(self):
-        """Gets the description of this UpdateSubscription.  # noqa: E501
+        """Gets the description of this CreateSubscription.  # noqa: E501
 
         The summary of the services provided by the subscription  # noqa: E501
 
-        :return: The description of this UpdateSubscription.  # noqa: E501
+        :return: The description of this CreateSubscription.  # noqa: E501
         :rtype: str
         """
         return self._description
 
     @description.setter
     def description(self, description):
-        """Sets the description of this UpdateSubscription.
+        """Sets the description of this CreateSubscription.
 
         The summary of the services provided by the subscription  # noqa: E501
 
-        :param description: The description of this UpdateSubscription.  # noqa: E501
+        :param description: The description of this CreateSubscription.  # noqa: E501
         :type description: str
         """
         if (self.local_vars_configuration.client_side_validation and
                 description is not None and len(description) > 512):
             raise ValueError("Invalid value for `description`, length must be less than or equal to `512`")  # noqa: E501
         if (self.local_vars_configuration.client_side_validation and
                 description is not None and len(description) < 1):
@@ -151,63 +188,95 @@
                 description is not None and not re.search(r'^[\s\S]*$', description)):  # noqa: E501
             raise ValueError(r"Invalid value for `description`, must be a follow pattern or equal to `/^[\s\S]*$/`")  # noqa: E501
 
         self._description = description
 
     @property
     def status(self):
-        """Gets the status of this UpdateSubscription.  # noqa: E501
+        """Gets the status of this CreateSubscription.  # noqa: E501
 
         The current status of the subscription. Possible values are: Active, Inactive  # noqa: E501
 
-        :return: The status of this UpdateSubscription.  # noqa: E501
+        :return: The status of this CreateSubscription.  # noqa: E501
         :rtype: str
         """
         return self._status
 
     @status.setter
     def status(self, status):
-        """Sets the status of this UpdateSubscription.
+        """Sets the status of this CreateSubscription.
 
         The current status of the subscription. Possible values are: Active, Inactive  # noqa: E501
 
-        :param status: The status of this UpdateSubscription.  # noqa: E501
+        :param status: The status of this CreateSubscription.  # noqa: E501
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
-        """Gets the matching_pattern of this UpdateSubscription.  # noqa: E501
+        """Gets the matching_pattern of this CreateSubscription.  # noqa: E501
 
 
-        :return: The matching_pattern of this UpdateSubscription.  # noqa: E501
+        :return: The matching_pattern of this CreateSubscription.  # noqa: E501
         :rtype: lusid_notification.MatchingPattern
         """
         return self._matching_pattern
 
     @matching_pattern.setter
     def matching_pattern(self, matching_pattern):
-        """Sets the matching_pattern of this UpdateSubscription.
+        """Sets the matching_pattern of this CreateSubscription.
 
 
-        :param matching_pattern: The matching_pattern of this UpdateSubscription.  # noqa: E501
+        :param matching_pattern: The matching_pattern of this CreateSubscription.  # noqa: E501
         :type matching_pattern: lusid_notification.MatchingPattern
         """
         if self.local_vars_configuration.client_side_validation and matching_pattern is None:  # noqa: E501
             raise ValueError("Invalid value for `matching_pattern`, must not be `None`")  # noqa: E501
 
         self._matching_pattern = matching_pattern
 
+    @property
+    def use_as_auth(self):
+        """Gets the use_as_auth of this CreateSubscription.  # noqa: E501
+
+        The user to authenticate the subscription  # noqa: E501
+
+        :return: The use_as_auth of this CreateSubscription.  # noqa: E501
+        :rtype: str
+        """
+        return self._use_as_auth
+
+    @use_as_auth.setter
+    def use_as_auth(self, use_as_auth):
+        """Sets the use_as_auth of this CreateSubscription.
+
+        The user to authenticate the subscription  # noqa: E501
+
+        :param use_as_auth: The use_as_auth of this CreateSubscription.  # noqa: E501
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
@@ -242,18 +311,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, UpdateSubscription):
+        if not isinstance(other, CreateSubscription):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, UpdateSubscription):
+        if not isinstance(other, CreateSubscription):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `lusid-notification-sdk-preview-0.1.717/lusid_notification/models/webhook_notification_type.py` & `lusid-notification-sdk-preview-0.1.741/lusid_notification/models/webhook_notification_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.717
+    The version of the OpenAPI document: 0.1.741
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.717/lusid_notification/rest.py` & `lusid-notification-sdk-preview-0.1.741/lusid_notification/rest.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.717
+    The version of the OpenAPI document: 0.1.741
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `lusid-notification-sdk-preview-0.1.717/lusid_notification/utilities/config_keys.json` & `lusid-notification-sdk-preview-0.1.741/lusid_notification/utilities/config_keys.json`

 * *Files identical despite different names*

### Comparing `lusid-notification-sdk-preview-0.1.717/lusid_notification_sdk_preview.egg-info/SOURCES.txt` & `lusid-notification-sdk-preview-0.1.741/lusid_notification_sdk_preview.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lusid-notification-sdk-preview-0.1.717/setup.py` & `lusid-notification-sdk-preview-0.1.741/setup.py`

 * *Files identical despite different names*

