# Comparing `tmp/alibabacloud_dingtalk-2.0.19.tar.gz` & `tmp/alibabacloud_dingtalk-2.0.20.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_dingtalk-2.0.19.tar", last modified: Fri Jun  9 07:12:55 2023, max compression
+gzip compressed data, was "dist/alibabacloud_dingtalk-2.0.20.tar", last modified: Tue Jun 13 08:58:19 2023, max compression
```

## Comparing `alibabacloud_dingtalk-2.0.19.tar` & `alibabacloud_dingtalk-2.0.20.tar`

### file list

```diff
@@ -1,365 +1,369 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/
--rw-r--r--   0 root         (0) root         (0)    19882 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2309 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1021 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1106 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/algo_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/algo_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9980 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/algo_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    23314 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/algo_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/alitrip_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/alitrip_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    58254 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/alitrip_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   169621 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/alitrip_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/apaas_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/apaas_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    25166 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/apaas_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    46194 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/apaas_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/app_market_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/app_market_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    25682 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/app_market_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    27728 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/app_market_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/ats_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/ats_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    90648 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/ats_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   138912 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/ats_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/attendance_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/attendance_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   165948 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/attendance_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   323041 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/attendance_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/badge_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/badge_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    45240 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/badge_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    62246 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/badge_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/bizfinance_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/bizfinance_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   201848 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/bizfinance_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   569113 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/bizfinance_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/blackboard_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/blackboard_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4942 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/blackboard_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     3871 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/blackboard_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/calendar_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/calendar_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   138814 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/calendar_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   331545 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/calendar_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/carbon_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/carbon_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    27976 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/carbon_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    42229 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/carbon_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/card_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/card_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    35138 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/card_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   101075 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/card_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/check_in_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/check_in_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6044 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/check_in_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    10446 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/check_in_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/chengfeng_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/chengfeng_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    71632 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/chengfeng_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   123179 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/chengfeng_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/conference_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/conference_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    90334 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/conference_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   117347 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/conference_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/connector_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/connector_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    58616 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/connector_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   124904 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/connector_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/contact_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/contact_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   297108 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/contact_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   392984 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/contact_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/content_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/content_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    21270 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/content_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    42332 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/content_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/contract_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/contract_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    19674 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/contract_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    27526 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/contract_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/conv_file_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/conv_file_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    17934 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/conv_file_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    30852 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/conv_file_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/crm_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/crm_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   223914 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/crm_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   552073 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/crm_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/crm_2_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/crm_2_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4810 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/crm_2_0/client.py
--rw-r--r--   0 root         (0) root         (0)     7385 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/crm_2_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/customer_service_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/customer_service_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    32170 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/customer_service_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    46898 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/customer_service_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/datacenter_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/datacenter_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   391978 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/datacenter_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   515455 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/datacenter_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/devicemng_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/devicemng_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   112278 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/devicemng_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   152480 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/devicemng_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/dingmi_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/dingmi_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    56946 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/dingmi_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    56301 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/dingmi_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/diot_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/diot_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    50179 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/diot_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    69305 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/diot_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/doc_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/doc_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   211006 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/doc_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   267473 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/doc_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/doc_2_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/doc_2_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   150160 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/doc_2_0/client.py
--rw-r--r--   0 root         (0) root         (0)   269103 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/doc_2_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/drive_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/drive_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   140210 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/drive_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   195538 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/drive_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/edu_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/edu_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   453174 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/edu_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   705965 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/edu_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/esign_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/esign_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    72708 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/esign_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   116546 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/esign_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/esign_2_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/esign_2_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    86294 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/esign_2_0/client.py
--rw-r--r--   0 root         (0) root         (0)   123749 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/esign_2_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/event_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/event_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5096 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/event_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     6148 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/event_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/exclusive_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/exclusive_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   316592 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/exclusive_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   439557 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/exclusive_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/finance_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/finance_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   155788 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/finance_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   302125 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/finance_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/flashmeeting_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/flashmeeting_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9368 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/flashmeeting_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    12542 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/flashmeeting_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/gateway_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/gateway_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4431 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/gateway_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     4668 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/gateway_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/group_blackboard_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/group_blackboard_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10562 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/group_blackboard_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     9742 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/group_blackboard_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/h3yun_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/h3yun_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    80133 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/h3yun_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   138362 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/h3yun_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/h5package_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/h5package_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    17059 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/h5package_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    18903 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/h5package_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/hrbrain_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/hrbrain_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5382 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/hrbrain_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     4660 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/hrbrain_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/hrm_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/hrm_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    92926 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/hrm_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   137528 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/hrm_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/im_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/im_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   302532 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/im_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   378971 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/im_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/im_2_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/im_2_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    22430 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/im_2_0/client.py
--rw-r--r--   0 root         (0) root         (0)    31875 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/im_2_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/impaas_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/impaas_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    90230 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/impaas_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    92472 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/impaas_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/industry_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/industry_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   606316 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/industry_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   855474 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/industry_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/jzcrm_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/jzcrm_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    62348 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/jzcrm_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   155140 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/jzcrm_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/link_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/link_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    63194 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/link_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   108695 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/link_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/live_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/live_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    91118 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/live_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   135110 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/live_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/manufacturing_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/manufacturing_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    16181 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/manufacturing_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    23076 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/manufacturing_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/micro_app_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/micro_app_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   146899 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/micro_app_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   175146 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/micro_app_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/miniapp_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/miniapp_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    52227 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/miniapp_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    54521 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/miniapp_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/oauth2_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/oauth2_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    31076 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/oauth2_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    40802 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/oauth2_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/occupationauth_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/occupationauth_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8962 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/occupationauth_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     7507 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/occupationauth_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/okr_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/okr_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    76720 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/okr_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   137701 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/okr_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/org_culture_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/org_culture_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    77488 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/org_culture_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   123420 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/org_culture_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/package_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/package_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    56344 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/package_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    60347 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/package_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/pedia_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/pedia_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    29226 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/pedia_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    69069 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/pedia_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/project_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/project_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   260568 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/project_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   413706 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/project_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/project_integration_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/project_integration_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    17983 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/project_integration_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    11593 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/project_integration_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/rcs_call_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/rcs_call_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5368 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/rcs_call_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     4579 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/rcs_call_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/resident_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/resident_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   135300 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/resident_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   174524 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/resident_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/robot_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/robot_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    81780 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/robot_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    93746 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/robot_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/rooms_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/rooms_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    56986 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/rooms_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    83842 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/rooms_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/search_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/search_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    39248 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/search_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    46018 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/search_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/service_group_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/service_group_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   361006 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/service_group_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   503423 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/service_group_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/smart_device_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/smart_device_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    31508 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/smart_device_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    26678 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/smart_device_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/sns_storage_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/sns_storage_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    44726 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/sns_storage_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    96217 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/sns_storage_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/storage_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/storage_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   187612 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/storage_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   353698 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/storage_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/storage_2_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/storage_2_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    53470 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/storage_2_0/client.py
--rw-r--r--   0 root         (0) root         (0)    89290 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/storage_2_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/swform_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/swform_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13910 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/swform_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    28559 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/swform_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/todo_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/todo_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    65344 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/todo_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   148231 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/todo_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/trade_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/trade_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14284 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/trade_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    16170 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/trade_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/trajectory_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/trajectory_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14192 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/trajectory_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    21677 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/trajectory_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/transcribe_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/transcribe_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13676 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/transcribe_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    17519 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/transcribe_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/trip_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/trip_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    18718 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/trip_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    32237 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/trip_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/village_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/village_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    75904 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/village_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   110849 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/village_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/watt_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/watt_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4269 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/watt_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     3363 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/watt_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/wiki_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/wiki_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8278 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/wiki_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    20486 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/wiki_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/wiki_2_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/wiki_2_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    66210 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/wiki_2_0/client.py
--rw-r--r--   0 root         (0) root         (0)   130783 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/wiki_2_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/wms_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/wms_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5370 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/wms_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     8325 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/wms_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/workbench_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/workbench_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    27686 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/workbench_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    29689 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/workbench_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/workflow_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/workflow_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   179772 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/workflow_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   377816 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/workflow_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/workrecord_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/workrecord_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4774 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/workrecord_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     3772 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/workrecord_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/yida_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/yida_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   464194 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/yida_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   687148 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/yida_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/yun_shu_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/yun_shu_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5452 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/yun_shu_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     4490 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/yun_shu_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2309 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    12014 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      239 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2684 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 08:58:19.000000 alibabacloud_dingtalk-2.0.20/
+-rw-r--r--   0 root         (0) root         (0)    19947 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2309 2023-06-13 08:58:19.000000 alibabacloud_dingtalk-2.0.20/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1021 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1106 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 08:58:19.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 08:58:19.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/activity_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/activity_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8552 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/activity_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    15385 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/activity_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 08:58:19.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/algo_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/algo_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9980 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/algo_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    23314 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/algo_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 08:58:19.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/alitrip_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/alitrip_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    58254 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/alitrip_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   169621 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/alitrip_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 08:58:19.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/apaas_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/apaas_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    25166 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/apaas_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    46194 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/apaas_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 08:58:19.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/app_market_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/app_market_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    25682 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/app_market_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    27728 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/app_market_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 08:58:19.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/ats_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/ats_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    90648 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/ats_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   138912 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/ats_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 08:58:19.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/attendance_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/attendance_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   165948 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/attendance_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   323041 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/attendance_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 08:58:19.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/badge_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/badge_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    45240 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/badge_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    62246 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/badge_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 08:58:19.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/bizfinance_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/bizfinance_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   201848 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/bizfinance_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   569113 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/bizfinance_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 08:58:19.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/blackboard_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/blackboard_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4942 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/blackboard_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     3871 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/blackboard_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 08:58:19.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/calendar_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/calendar_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   139370 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/calendar_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   341471 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/calendar_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 08:58:19.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/carbon_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/carbon_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    27976 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/carbon_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    42229 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/carbon_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 08:58:19.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/card_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/card_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    35138 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/card_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   101075 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/card_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 08:58:19.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/check_in_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/check_in_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6044 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/check_in_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    10446 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/check_in_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 08:58:19.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/chengfeng_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/chengfeng_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    71632 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/chengfeng_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   123179 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/chengfeng_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 08:58:19.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/conference_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/conference_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    90334 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/conference_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   117347 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/conference_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 08:58:19.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/connector_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/connector_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    58616 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/connector_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   124904 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/connector_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 08:58:19.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/contact_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/contact_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   297108 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/contact_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   392984 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/contact_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 08:58:19.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/content_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/content_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    21270 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/content_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    42332 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/content_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 08:58:19.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/contract_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/contract_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    19674 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/contract_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    27526 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/contract_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 08:58:19.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/conv_file_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/conv_file_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    17934 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/conv_file_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    30852 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/conv_file_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 08:58:19.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/crm_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/crm_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   223914 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/crm_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   552073 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/crm_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 08:58:19.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/crm_2_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/crm_2_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4810 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/crm_2_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     7385 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/crm_2_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 08:58:19.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/customer_service_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/customer_service_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    32170 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/customer_service_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    46898 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/customer_service_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 08:58:19.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/datacenter_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/datacenter_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   391978 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/datacenter_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   515455 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/datacenter_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 08:58:19.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/devicemng_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/devicemng_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   112278 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/devicemng_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   152480 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/devicemng_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 08:58:19.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/dingmi_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/dingmi_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    56946 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/dingmi_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    56301 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/dingmi_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 08:58:19.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/diot_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/diot_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    52941 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/diot_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    71864 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/diot_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 08:58:19.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/doc_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/doc_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   211006 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/doc_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   267473 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/doc_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 08:58:19.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/doc_2_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/doc_2_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   150160 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/doc_2_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   269103 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/doc_2_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 08:58:19.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/drive_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/drive_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   140210 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/drive_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   195538 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/drive_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 08:58:19.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/edu_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/edu_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   453174 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/edu_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   705965 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/edu_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 08:58:19.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/esign_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/esign_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    72708 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/esign_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   116546 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/esign_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 08:58:19.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/esign_2_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/esign_2_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    86294 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/esign_2_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   123749 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/esign_2_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 08:58:19.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/event_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/event_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5096 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/event_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     6148 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/event_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 08:58:19.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/exclusive_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/exclusive_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   316592 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/exclusive_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   439557 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/exclusive_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 08:58:19.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/finance_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/finance_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   155788 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/finance_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   302125 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/finance_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 08:58:19.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/flashmeeting_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/flashmeeting_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9368 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/flashmeeting_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    12542 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/flashmeeting_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 08:58:19.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/gateway_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/gateway_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4633 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/gateway_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     4901 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/gateway_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 08:58:19.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/group_blackboard_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/group_blackboard_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10562 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/group_blackboard_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     9742 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/group_blackboard_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 08:58:19.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/h3yun_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/h3yun_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    80133 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/h3yun_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   138362 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/h3yun_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 08:58:19.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/h5package_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/h5package_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    17059 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/h5package_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    18903 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/h5package_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 08:58:19.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/hrbrain_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/hrbrain_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5382 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/hrbrain_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     4660 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/hrbrain_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 08:58:19.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/hrm_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/hrm_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    92926 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/hrm_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   137528 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/hrm_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 08:58:19.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/im_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/im_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   302532 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/im_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   378971 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/im_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 08:58:19.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/im_2_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/im_2_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    22430 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/im_2_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    31875 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/im_2_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 08:58:19.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/impaas_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/impaas_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    90230 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/impaas_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    92472 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/impaas_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 08:58:19.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/industry_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/industry_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   610684 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/industry_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   859772 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/industry_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 08:58:19.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/jzcrm_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/jzcrm_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    62348 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/jzcrm_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   155140 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/jzcrm_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 08:58:19.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/link_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/link_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    63194 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/link_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   108695 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/link_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 08:58:19.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/live_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/live_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    91118 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/live_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   135110 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/live_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 08:58:19.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/manufacturing_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/manufacturing_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    16181 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/manufacturing_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    23076 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/manufacturing_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 08:58:19.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/micro_app_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/micro_app_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   146899 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/micro_app_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   175146 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/micro_app_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 08:58:19.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/miniapp_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/miniapp_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    52227 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/miniapp_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    54521 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/miniapp_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 08:58:19.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/oauth2_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/oauth2_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    31076 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/oauth2_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    40802 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/oauth2_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 08:58:19.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/occupationauth_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/occupationauth_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8962 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/occupationauth_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     7507 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/occupationauth_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 08:58:19.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/okr_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/okr_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    76720 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/okr_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   137701 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/okr_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 08:58:19.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/org_culture_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/org_culture_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    77488 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/org_culture_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   123420 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/org_culture_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 08:58:19.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/package_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/package_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    56344 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/package_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    60347 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/package_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 08:58:19.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/pedia_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/pedia_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    29226 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/pedia_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    69069 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/pedia_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 08:58:19.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/project_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/project_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   260568 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/project_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   413706 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/project_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 08:58:19.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/project_integration_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/project_integration_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    17983 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/project_integration_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    11593 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/project_integration_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 08:58:19.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/rcs_call_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/rcs_call_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5368 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/rcs_call_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     4579 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/rcs_call_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 08:58:19.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/resident_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/resident_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   135300 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/resident_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   174524 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/resident_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 08:58:19.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/robot_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/robot_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    81780 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/robot_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    93746 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/robot_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 08:58:19.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/rooms_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/rooms_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    56986 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/rooms_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    83842 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/rooms_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 08:58:19.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/search_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/search_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    39248 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/search_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    46018 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/search_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 08:58:19.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/service_group_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/service_group_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   361006 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/service_group_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   503423 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/service_group_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 08:58:19.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/smart_device_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/smart_device_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    31508 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/smart_device_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    26678 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/smart_device_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 08:58:19.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/sns_storage_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/sns_storage_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    44726 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/sns_storage_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    96217 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/sns_storage_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 08:58:19.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/storage_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/storage_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   187612 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/storage_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   353698 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/storage_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 08:58:19.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/storage_2_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/storage_2_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    53470 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/storage_2_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    89290 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/storage_2_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 08:58:19.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/swform_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/swform_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13910 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/swform_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    28559 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/swform_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 08:58:19.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/todo_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/todo_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    65344 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/todo_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   148231 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/todo_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 08:58:19.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/trade_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/trade_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14284 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/trade_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    16170 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/trade_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 08:58:19.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/trajectory_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/trajectory_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14192 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/trajectory_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    21677 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/trajectory_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 08:58:19.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/transcribe_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/transcribe_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13676 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/transcribe_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    17519 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/transcribe_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 08:58:19.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/trip_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/trip_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    18718 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/trip_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    32237 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/trip_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 08:58:19.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/village_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/village_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    75904 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/village_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   110849 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/village_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 08:58:19.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/watt_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/watt_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4269 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/watt_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     3363 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/watt_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 08:58:19.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/wiki_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/wiki_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8278 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/wiki_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    20486 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/wiki_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 08:58:19.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/wiki_2_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/wiki_2_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    66210 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/wiki_2_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   130783 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/wiki_2_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 08:58:19.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/wms_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/wms_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5370 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/wms_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     8325 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/wms_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 08:58:19.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/workbench_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/workbench_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    27686 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/workbench_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    29689 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/workbench_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 08:58:19.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/workflow_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/workflow_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   179772 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/workflow_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   377816 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/workflow_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 08:58:19.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/workrecord_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/workrecord_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4774 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/workrecord_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     3772 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/workrecord_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 08:58:19.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/yida_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/yida_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   464194 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/yida_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   687148 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/yida_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 08:58:19.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/yun_shu_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/yun_shu_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5452 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/yun_shu_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     4490 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/yun_shu_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 08:58:19.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2309 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    12151 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      239 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-06-13 08:58:19.000000 alibabacloud_dingtalk-2.0.20/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2684 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/setup.py
```

### Comparing `alibabacloud_dingtalk-2.0.19/ChangeLog.md` & `alibabacloud_dingtalk-2.0.20/ChangeLog.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+2023-06-09 Version: 2.0.19
+- Update AddOfficialAccountFollower.
+
 2023-05-31 Version: 2.0.18
 - Update AddOfficialAccountFollower.
 
 2023-05-26 Version: 2.0.17
 - Update AddOfficialAccountFollower.
 
 2023-05-24 Version: 2.0.16
```

### Comparing `alibabacloud_dingtalk-2.0.19/LICENSE` & `alibabacloud_dingtalk-2.0.20/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.19/PKG-INFO` & `alibabacloud_dingtalk-2.0.20/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_dingtalk
-Version: 2.0.19
+Version: 2.0.20
 Summary: Alibaba Cloud Dingtalk SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_dingtalk-2.0.19/README-CN.md` & `alibabacloud_dingtalk-2.0.20/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.19/README.md` & `alibabacloud_dingtalk-2.0.20/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/algo_1_0/client.py` & `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/algo_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/algo_1_0/models.py` & `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/algo_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/alitrip_1_0/client.py` & `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/alitrip_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/alitrip_1_0/models.py` & `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/alitrip_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/apaas_1_0/client.py` & `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/apaas_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/apaas_1_0/models.py` & `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/apaas_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/app_market_1_0/client.py` & `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/app_market_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/app_market_1_0/models.py` & `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/app_market_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/ats_1_0/client.py` & `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/ats_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/ats_1_0/models.py` & `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/ats_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/attendance_1_0/client.py` & `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/attendance_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/attendance_1_0/models.py` & `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/attendance_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/badge_1_0/client.py` & `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/badge_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/badge_1_0/models.py` & `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/badge_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/bizfinance_1_0/client.py` & `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/bizfinance_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/bizfinance_1_0/models.py` & `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/bizfinance_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/blackboard_1_0/client.py` & `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/blackboard_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/blackboard_1_0/models.py` & `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/blackboard_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/calendar_1_0/client.py` & `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/calendar_1_0/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -525,14 +525,16 @@
             body['location'] = request.location
         if not UtilClient.is_unset(request.online_meeting_info):
             body['onlineMeetingInfo'] = request.online_meeting_info
         if not UtilClient.is_unset(request.recurrence):
             body['recurrence'] = request.recurrence
         if not UtilClient.is_unset(request.reminders):
             body['reminders'] = request.reminders
+        if not UtilClient.is_unset(request.rich_text_description):
+            body['richTextDescription'] = request.rich_text_description
         if not UtilClient.is_unset(request.start):
             body['start'] = request.start
         if not UtilClient.is_unset(request.summary):
             body['summary'] = request.summary
         if not UtilClient.is_unset(request.ui_configs):
             body['uiConfigs'] = request.ui_configs
         real_headers = {}
@@ -584,14 +586,16 @@
             body['location'] = request.location
         if not UtilClient.is_unset(request.online_meeting_info):
             body['onlineMeetingInfo'] = request.online_meeting_info
         if not UtilClient.is_unset(request.recurrence):
             body['recurrence'] = request.recurrence
         if not UtilClient.is_unset(request.reminders):
             body['reminders'] = request.reminders
+        if not UtilClient.is_unset(request.rich_text_description):
+            body['richTextDescription'] = request.rich_text_description
         if not UtilClient.is_unset(request.start):
             body['start'] = request.start
         if not UtilClient.is_unset(request.summary):
             body['summary'] = request.summary
         if not UtilClient.is_unset(request.ui_configs):
             body['uiConfigs'] = request.ui_configs
         real_headers = {}
@@ -2406,14 +2410,16 @@
             body['location'] = request.location
         if not UtilClient.is_unset(request.online_meeting_info):
             body['onlineMeetingInfo'] = request.online_meeting_info
         if not UtilClient.is_unset(request.recurrence):
             body['recurrence'] = request.recurrence
         if not UtilClient.is_unset(request.reminders):
             body['reminders'] = request.reminders
+        if not UtilClient.is_unset(request.rich_text_description):
+            body['richTextDescription'] = request.rich_text_description
         if not UtilClient.is_unset(request.start):
             body['start'] = request.start
         if not UtilClient.is_unset(request.summary):
             body['summary'] = request.summary
         real_headers = {}
         if not UtilClient.is_unset(headers.common_headers):
             real_headers = headers.common_headers
@@ -2466,14 +2472,16 @@
             body['location'] = request.location
         if not UtilClient.is_unset(request.online_meeting_info):
             body['onlineMeetingInfo'] = request.online_meeting_info
         if not UtilClient.is_unset(request.recurrence):
             body['recurrence'] = request.recurrence
         if not UtilClient.is_unset(request.reminders):
             body['reminders'] = request.reminders
+        if not UtilClient.is_unset(request.rich_text_description):
+            body['richTextDescription'] = request.rich_text_description
         if not UtilClient.is_unset(request.start):
             body['start'] = request.start
         if not UtilClient.is_unset(request.summary):
             body['summary'] = request.summary
         real_headers = {}
         if not UtilClient.is_unset(headers.common_headers):
             real_headers = headers.common_headers
```

### Comparing `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/calendar_1_0/models.py` & `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/calendar_1_0/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -1081,14 +1081,41 @@
         if m.get('method') is not None:
             self.method = m.get('method')
         if m.get('minutes') is not None:
             self.minutes = m.get('minutes')
         return self
 
 
+class CreateEventRequestRichTextDescription(TeaModel):
+    def __init__(
+        self,
+        text: str = None,
+    ):
+        self.text = text
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.text is not None:
+            result['text'] = self.text
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('text') is not None:
+            self.text = m.get('text')
+        return self
+
+
 class CreateEventRequestStart(TeaModel):
     def __init__(
         self,
         date: str = None,
         date_time: str = None,
         time_zone: str = None,
     ):
@@ -1165,27 +1192,29 @@
         end: CreateEventRequestEnd = None,
         extra: Dict[str, str] = None,
         is_all_day: bool = None,
         location: CreateEventRequestLocation = None,
         online_meeting_info: CreateEventRequestOnlineMeetingInfo = None,
         recurrence: CreateEventRequestRecurrence = None,
         reminders: List[CreateEventRequestReminders] = None,
+        rich_text_description: CreateEventRequestRichTextDescription = None,
         start: CreateEventRequestStart = None,
         summary: str = None,
         ui_configs: List[CreateEventRequestUiConfigs] = None,
     ):
         self.attendees = attendees
         self.description = description
         self.end = end
         self.extra = extra
         self.is_all_day = is_all_day
         self.location = location
         self.online_meeting_info = online_meeting_info
         self.recurrence = recurrence
         self.reminders = reminders
+        self.rich_text_description = rich_text_description
         self.start = start
         self.summary = summary
         self.ui_configs = ui_configs
 
     def validate(self):
         if self.attendees:
             for k in self.attendees:
@@ -1199,14 +1228,16 @@
             self.online_meeting_info.validate()
         if self.recurrence:
             self.recurrence.validate()
         if self.reminders:
             for k in self.reminders:
                 if k:
                     k.validate()
+        if self.rich_text_description:
+            self.rich_text_description.validate()
         if self.start:
             self.start.validate()
         if self.ui_configs:
             for k in self.ui_configs:
                 if k:
                     k.validate()
 
@@ -1234,14 +1265,16 @@
             result['onlineMeetingInfo'] = self.online_meeting_info.to_map()
         if self.recurrence is not None:
             result['recurrence'] = self.recurrence.to_map()
         result['reminders'] = []
         if self.reminders is not None:
             for k in self.reminders:
                 result['reminders'].append(k.to_map() if k else None)
+        if self.rich_text_description is not None:
+            result['richTextDescription'] = self.rich_text_description.to_map()
         if self.start is not None:
             result['start'] = self.start.to_map()
         if self.summary is not None:
             result['summary'] = self.summary
         result['uiConfigs'] = []
         if self.ui_configs is not None:
             for k in self.ui_configs:
@@ -1274,14 +1307,17 @@
             temp_model = CreateEventRequestRecurrence()
             self.recurrence = temp_model.from_map(m['recurrence'])
         self.reminders = []
         if m.get('reminders') is not None:
             for k in m.get('reminders'):
                 temp_model = CreateEventRequestReminders()
                 self.reminders.append(temp_model.from_map(k))
+        if m.get('richTextDescription') is not None:
+            temp_model = CreateEventRequestRichTextDescription()
+            self.rich_text_description = temp_model.from_map(m['richTextDescription'])
         if m.get('start') is not None:
             temp_model = CreateEventRequestStart()
             self.start = temp_model.from_map(m['start'])
         if m.get('summary') is not None:
             self.summary = m.get('summary')
         self.ui_configs = []
         if m.get('uiConfigs') is not None:
@@ -1655,14 +1691,41 @@
         if m.get('method') is not None:
             self.method = m.get('method')
         if m.get('minutes') is not None:
             self.minutes = m.get('minutes')
         return self
 
 
+class CreateEventResponseBodyRichTextDescription(TeaModel):
+    def __init__(
+        self,
+        text: str = None,
+    ):
+        self.text = text
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.text is not None:
+            result['text'] = self.text
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('text') is not None:
+            self.text = m.get('text')
+        return self
+
+
 class CreateEventResponseBodyStart(TeaModel):
     def __init__(
         self,
         date: str = None,
         date_time: str = None,
         time_zone: str = None,
     ):
@@ -1741,14 +1804,15 @@
         id: str = None,
         is_all_day: bool = None,
         location: CreateEventResponseBodyLocation = None,
         online_meeting_info: CreateEventResponseBodyOnlineMeetingInfo = None,
         organizer: CreateEventResponseBodyOrganizer = None,
         recurrence: CreateEventResponseBodyRecurrence = None,
         reminders: List[CreateEventResponseBodyReminders] = None,
+        rich_text_description: CreateEventResponseBodyRichTextDescription = None,
         start: CreateEventResponseBodyStart = None,
         summary: str = None,
         ui_configs: List[CreateEventResponseBodyUiConfigs] = None,
         update_time: str = None,
     ):
         self.attendees = attendees
         self.create_time = create_time
@@ -1757,14 +1821,15 @@
         self.id = id
         self.is_all_day = is_all_day
         self.location = location
         self.online_meeting_info = online_meeting_info
         self.organizer = organizer
         self.recurrence = recurrence
         self.reminders = reminders
+        self.rich_text_description = rich_text_description
         self.start = start
         self.summary = summary
         self.ui_configs = ui_configs
         self.update_time = update_time
 
     def validate(self):
         if self.attendees:
@@ -1781,14 +1846,16 @@
             self.organizer.validate()
         if self.recurrence:
             self.recurrence.validate()
         if self.reminders:
             for k in self.reminders:
                 if k:
                     k.validate()
+        if self.rich_text_description:
+            self.rich_text_description.validate()
         if self.start:
             self.start.validate()
         if self.ui_configs:
             for k in self.ui_configs:
                 if k:
                     k.validate()
 
@@ -1820,14 +1887,16 @@
             result['organizer'] = self.organizer.to_map()
         if self.recurrence is not None:
             result['recurrence'] = self.recurrence.to_map()
         result['reminders'] = []
         if self.reminders is not None:
             for k in self.reminders:
                 result['reminders'].append(k.to_map() if k else None)
+        if self.rich_text_description is not None:
+            result['richTextDescription'] = self.rich_text_description.to_map()
         if self.start is not None:
             result['start'] = self.start.to_map()
         if self.summary is not None:
             result['summary'] = self.summary
         result['uiConfigs'] = []
         if self.ui_configs is not None:
             for k in self.ui_configs:
@@ -1867,14 +1936,17 @@
             temp_model = CreateEventResponseBodyRecurrence()
             self.recurrence = temp_model.from_map(m['recurrence'])
         self.reminders = []
         if m.get('reminders') is not None:
             for k in m.get('reminders'):
                 temp_model = CreateEventResponseBodyReminders()
                 self.reminders.append(temp_model.from_map(k))
+        if m.get('richTextDescription') is not None:
+            temp_model = CreateEventResponseBodyRichTextDescription()
+            self.rich_text_description = temp_model.from_map(m['richTextDescription'])
         if m.get('start') is not None:
             temp_model = CreateEventResponseBodyStart()
             self.start = temp_model.from_map(m['start'])
         if m.get('summary') is not None:
             self.summary = m.get('summary')
         self.ui_configs = []
         if m.get('uiConfigs') is not None:
@@ -3092,14 +3164,41 @@
         if m.get('method') is not None:
             self.method = m.get('method')
         if m.get('minutes') is not None:
             self.minutes = m.get('minutes')
         return self
 
 
+class GetEventResponseBodyRichTextDescription(TeaModel):
+    def __init__(
+        self,
+        text: str = None,
+    ):
+        self.text = text
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.text is not None:
+            result['text'] = self.text
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('text') is not None:
+            self.text = m.get('text')
+        return self
+
+
 class GetEventResponseBodyStart(TeaModel):
     def __init__(
         self,
         date: str = None,
         date_time: str = None,
         time_zone: str = None,
     ):
@@ -3149,14 +3248,15 @@
         location: GetEventResponseBodyLocation = None,
         meeting_rooms: List[GetEventResponseBodyMeetingRooms] = None,
         online_meeting_info: GetEventResponseBodyOnlineMeetingInfo = None,
         organizer: GetEventResponseBodyOrganizer = None,
         origin_start: GetEventResponseBodyOriginStart = None,
         recurrence: GetEventResponseBodyRecurrence = None,
         reminders: List[GetEventResponseBodyReminders] = None,
+        rich_text_description: GetEventResponseBodyRichTextDescription = None,
         series_master_id: str = None,
         start: GetEventResponseBodyStart = None,
         status: str = None,
         summary: str = None,
         update_time: str = None,
     ):
         self.attendees = attendees
@@ -3170,14 +3270,15 @@
         self.location = location
         self.meeting_rooms = meeting_rooms
         self.online_meeting_info = online_meeting_info
         self.organizer = organizer
         self.origin_start = origin_start
         self.recurrence = recurrence
         self.reminders = reminders
+        self.rich_text_description = rich_text_description
         self.series_master_id = series_master_id
         self.start = start
         self.status = status
         self.summary = summary
         self.update_time = update_time
 
     def validate(self):
@@ -3207,14 +3308,16 @@
             self.origin_start.validate()
         if self.recurrence:
             self.recurrence.validate()
         if self.reminders:
             for k in self.reminders:
                 if k:
                     k.validate()
+        if self.rich_text_description:
+            self.rich_text_description.validate()
         if self.start:
             self.start.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -3254,14 +3357,16 @@
             result['originStart'] = self.origin_start.to_map()
         if self.recurrence is not None:
             result['recurrence'] = self.recurrence.to_map()
         result['reminders'] = []
         if self.reminders is not None:
             for k in self.reminders:
                 result['reminders'].append(k.to_map() if k else None)
+        if self.rich_text_description is not None:
+            result['richTextDescription'] = self.rich_text_description.to_map()
         if self.series_master_id is not None:
             result['seriesMasterId'] = self.series_master_id
         if self.start is not None:
             result['start'] = self.start.to_map()
         if self.status is not None:
             result['status'] = self.status
         if self.summary is not None:
@@ -3317,14 +3422,17 @@
             temp_model = GetEventResponseBodyRecurrence()
             self.recurrence = temp_model.from_map(m['recurrence'])
         self.reminders = []
         if m.get('reminders') is not None:
             for k in m.get('reminders'):
                 temp_model = GetEventResponseBodyReminders()
                 self.reminders.append(temp_model.from_map(k))
+        if m.get('richTextDescription') is not None:
+            temp_model = GetEventResponseBodyRichTextDescription()
+            self.rich_text_description = temp_model.from_map(m['richTextDescription'])
         if m.get('seriesMasterId') is not None:
             self.series_master_id = m.get('seriesMasterId')
         if m.get('start') is not None:
             temp_model = GetEventResponseBodyStart()
             self.start = temp_model.from_map(m['start'])
         if m.get('status') is not None:
             self.status = m.get('status')
@@ -5835,14 +5943,41 @@
         if m.get('method') is not None:
             self.method = m.get('method')
         if m.get('minutes') is not None:
             self.minutes = m.get('minutes')
         return self
 
 
+class ListEventsResponseBodyEventsRichTextDescription(TeaModel):
+    def __init__(
+        self,
+        text: str = None,
+    ):
+        self.text = text
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.text is not None:
+            result['text'] = self.text
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('text') is not None:
+            self.text = m.get('text')
+        return self
+
+
 class ListEventsResponseBodyEventsStart(TeaModel):
     def __init__(
         self,
         date: str = None,
         date_time: str = None,
         time_zone: str = None,
     ):
@@ -5892,14 +6027,15 @@
         location: ListEventsResponseBodyEventsLocation = None,
         meeting_rooms: List[ListEventsResponseBodyEventsMeetingRooms] = None,
         online_meeting_info: ListEventsResponseBodyEventsOnlineMeetingInfo = None,
         organizer: ListEventsResponseBodyEventsOrganizer = None,
         origin_start: ListEventsResponseBodyEventsOriginStart = None,
         recurrence: ListEventsResponseBodyEventsRecurrence = None,
         reminders: List[ListEventsResponseBodyEventsReminders] = None,
+        rich_text_description: ListEventsResponseBodyEventsRichTextDescription = None,
         series_master_id: str = None,
         start: ListEventsResponseBodyEventsStart = None,
         status: str = None,
         summary: str = None,
         update_time: str = None,
     ):
         self.attendees = attendees
@@ -5913,14 +6049,15 @@
         self.location = location
         self.meeting_rooms = meeting_rooms
         self.online_meeting_info = online_meeting_info
         self.organizer = organizer
         self.origin_start = origin_start
         self.recurrence = recurrence
         self.reminders = reminders
+        self.rich_text_description = rich_text_description
         self.series_master_id = series_master_id
         self.start = start
         self.status = status
         self.summary = summary
         self.update_time = update_time
 
     def validate(self):
@@ -5950,14 +6087,16 @@
             self.origin_start.validate()
         if self.recurrence:
             self.recurrence.validate()
         if self.reminders:
             for k in self.reminders:
                 if k:
                     k.validate()
+        if self.rich_text_description:
+            self.rich_text_description.validate()
         if self.start:
             self.start.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -5997,14 +6136,16 @@
             result['originStart'] = self.origin_start.to_map()
         if self.recurrence is not None:
             result['recurrence'] = self.recurrence.to_map()
         result['reminders'] = []
         if self.reminders is not None:
             for k in self.reminders:
                 result['reminders'].append(k.to_map() if k else None)
+        if self.rich_text_description is not None:
+            result['richTextDescription'] = self.rich_text_description.to_map()
         if self.series_master_id is not None:
             result['seriesMasterId'] = self.series_master_id
         if self.start is not None:
             result['start'] = self.start.to_map()
         if self.status is not None:
             result['status'] = self.status
         if self.summary is not None:
@@ -6060,14 +6201,17 @@
             temp_model = ListEventsResponseBodyEventsRecurrence()
             self.recurrence = temp_model.from_map(m['recurrence'])
         self.reminders = []
         if m.get('reminders') is not None:
             for k in m.get('reminders'):
                 temp_model = ListEventsResponseBodyEventsReminders()
                 self.reminders.append(temp_model.from_map(k))
+        if m.get('richTextDescription') is not None:
+            temp_model = ListEventsResponseBodyEventsRichTextDescription()
+            self.rich_text_description = temp_model.from_map(m['richTextDescription'])
         if m.get('seriesMasterId') is not None:
             self.series_master_id = m.get('seriesMasterId')
         if m.get('start') is not None:
             temp_model = ListEventsResponseBodyEventsStart()
             self.start = temp_model.from_map(m['start'])
         if m.get('status') is not None:
             self.status = m.get('status')
@@ -7242,14 +7386,53 @@
         if m.get('displayName') is not None:
             self.display_name = m.get('displayName')
         if m.get('meetingRooms') is not None:
             self.meeting_rooms = m.get('meetingRooms')
         return self
 
 
+class ListEventsViewResponseBodyEventsMeetingRooms(TeaModel):
+    def __init__(
+        self,
+        display_name: str = None,
+        response_status: str = None,
+        room_id: str = None,
+    ):
+        self.display_name = display_name
+        self.response_status = response_status
+        self.room_id = room_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.display_name is not None:
+            result['displayName'] = self.display_name
+        if self.response_status is not None:
+            result['responseStatus'] = self.response_status
+        if self.room_id is not None:
+            result['roomId'] = self.room_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('displayName') is not None:
+            self.display_name = m.get('displayName')
+        if m.get('responseStatus') is not None:
+            self.response_status = m.get('responseStatus')
+        if m.get('roomId') is not None:
+            self.room_id = m.get('roomId')
+        return self
+
+
 class ListEventsViewResponseBodyEventsOnlineMeetingInfo(TeaModel):
     def __init__(
         self,
         conference_id: str = None,
         extra_info: Dict[str, Any] = None,
         type: str = None,
         url: str = None,
@@ -7487,14 +7670,41 @@
             self.pattern = temp_model.from_map(m['pattern'])
         if m.get('range') is not None:
             temp_model = ListEventsViewResponseBodyEventsRecurrenceRange()
             self.range = temp_model.from_map(m['range'])
         return self
 
 
+class ListEventsViewResponseBodyEventsRichTextDescription(TeaModel):
+    def __init__(
+        self,
+        text: str = None,
+    ):
+        self.text = text
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.text is not None:
+            result['text'] = self.text
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('text') is not None:
+            self.text = m.get('text')
+        return self
+
+
 class ListEventsViewResponseBodyEventsStart(TeaModel):
     def __init__(
         self,
         date: str = None,
         date_time: str = None,
         time_zone: str = None,
     ):
@@ -7538,18 +7748,20 @@
         create_time: str = None,
         description: str = None,
         end: ListEventsViewResponseBodyEventsEnd = None,
         extended_properties: ListEventsViewResponseBodyEventsExtendedProperties = None,
         id: str = None,
         is_all_day: bool = None,
         location: ListEventsViewResponseBodyEventsLocation = None,
+        meeting_rooms: List[ListEventsViewResponseBodyEventsMeetingRooms] = None,
         online_meeting_info: ListEventsViewResponseBodyEventsOnlineMeetingInfo = None,
         organizer: ListEventsViewResponseBodyEventsOrganizer = None,
         origin_start: ListEventsViewResponseBodyEventsOriginStart = None,
         recurrence: ListEventsViewResponseBodyEventsRecurrence = None,
+        rich_text_description: ListEventsViewResponseBodyEventsRichTextDescription = None,
         series_master_id: str = None,
         start: ListEventsViewResponseBodyEventsStart = None,
         status: str = None,
         summary: str = None,
         update_time: str = None,
     ):
         self.attendees = attendees
@@ -7557,18 +7769,20 @@
         self.create_time = create_time
         self.description = description
         self.end = end
         self.extended_properties = extended_properties
         self.id = id
         self.is_all_day = is_all_day
         self.location = location
+        self.meeting_rooms = meeting_rooms
         self.online_meeting_info = online_meeting_info
         self.organizer = organizer
         self.origin_start = origin_start
         self.recurrence = recurrence
+        self.rich_text_description = rich_text_description
         self.series_master_id = series_master_id
         self.start = start
         self.status = status
         self.summary = summary
         self.update_time = update_time
 
     def validate(self):
@@ -7582,22 +7796,28 @@
                     k.validate()
         if self.end:
             self.end.validate()
         if self.extended_properties:
             self.extended_properties.validate()
         if self.location:
             self.location.validate()
+        if self.meeting_rooms:
+            for k in self.meeting_rooms:
+                if k:
+                    k.validate()
         if self.online_meeting_info:
             self.online_meeting_info.validate()
         if self.organizer:
             self.organizer.validate()
         if self.origin_start:
             self.origin_start.validate()
         if self.recurrence:
             self.recurrence.validate()
+        if self.rich_text_description:
+            self.rich_text_description.validate()
         if self.start:
             self.start.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -7621,22 +7841,28 @@
             result['extendedProperties'] = self.extended_properties.to_map()
         if self.id is not None:
             result['id'] = self.id
         if self.is_all_day is not None:
             result['isAllDay'] = self.is_all_day
         if self.location is not None:
             result['location'] = self.location.to_map()
+        result['meetingRooms'] = []
+        if self.meeting_rooms is not None:
+            for k in self.meeting_rooms:
+                result['meetingRooms'].append(k.to_map() if k else None)
         if self.online_meeting_info is not None:
             result['onlineMeetingInfo'] = self.online_meeting_info.to_map()
         if self.organizer is not None:
             result['organizer'] = self.organizer.to_map()
         if self.origin_start is not None:
             result['originStart'] = self.origin_start.to_map()
         if self.recurrence is not None:
             result['recurrence'] = self.recurrence.to_map()
+        if self.rich_text_description is not None:
+            result['richTextDescription'] = self.rich_text_description.to_map()
         if self.series_master_id is not None:
             result['seriesMasterId'] = self.series_master_id
         if self.start is not None:
             result['start'] = self.start.to_map()
         if self.status is not None:
             result['status'] = self.status
         if self.summary is not None:
@@ -7670,26 +7896,34 @@
         if m.get('id') is not None:
             self.id = m.get('id')
         if m.get('isAllDay') is not None:
             self.is_all_day = m.get('isAllDay')
         if m.get('location') is not None:
             temp_model = ListEventsViewResponseBodyEventsLocation()
             self.location = temp_model.from_map(m['location'])
+        self.meeting_rooms = []
+        if m.get('meetingRooms') is not None:
+            for k in m.get('meetingRooms'):
+                temp_model = ListEventsViewResponseBodyEventsMeetingRooms()
+                self.meeting_rooms.append(temp_model.from_map(k))
         if m.get('onlineMeetingInfo') is not None:
             temp_model = ListEventsViewResponseBodyEventsOnlineMeetingInfo()
             self.online_meeting_info = temp_model.from_map(m['onlineMeetingInfo'])
         if m.get('organizer') is not None:
             temp_model = ListEventsViewResponseBodyEventsOrganizer()
             self.organizer = temp_model.from_map(m['organizer'])
         if m.get('originStart') is not None:
             temp_model = ListEventsViewResponseBodyEventsOriginStart()
             self.origin_start = temp_model.from_map(m['originStart'])
         if m.get('recurrence') is not None:
             temp_model = ListEventsViewResponseBodyEventsRecurrence()
             self.recurrence = temp_model.from_map(m['recurrence'])
+        if m.get('richTextDescription') is not None:
+            temp_model = ListEventsViewResponseBodyEventsRichTextDescription()
+            self.rich_text_description = temp_model.from_map(m['richTextDescription'])
         if m.get('seriesMasterId') is not None:
             self.series_master_id = m.get('seriesMasterId')
         if m.get('start') is not None:
             temp_model = ListEventsViewResponseBodyEventsStart()
             self.start = temp_model.from_map(m['start'])
         if m.get('status') is not None:
             self.status = m.get('status')
@@ -8954,14 +9188,41 @@
         if m.get('method') is not None:
             self.method = m.get('method')
         if m.get('minutes') is not None:
             self.minutes = m.get('minutes')
         return self
 
 
+class PatchEventRequestRichTextDescription(TeaModel):
+    def __init__(
+        self,
+        text: str = None,
+    ):
+        self.text = text
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.text is not None:
+            result['text'] = self.text
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('text') is not None:
+            self.text = m.get('text')
+        return self
+
+
 class PatchEventRequestStart(TeaModel):
     def __init__(
         self,
         date: str = None,
         date_time: str = None,
         time_zone: str = None,
     ):
@@ -9006,27 +9267,29 @@
         extra: Dict[str, str] = None,
         id: str = None,
         is_all_day: bool = None,
         location: PatchEventRequestLocation = None,
         online_meeting_info: PatchEventRequestOnlineMeetingInfo = None,
         recurrence: PatchEventRequestRecurrence = None,
         reminders: List[PatchEventRequestReminders] = None,
+        rich_text_description: PatchEventRequestRichTextDescription = None,
         start: PatchEventRequestStart = None,
         summary: str = None,
     ):
         self.attendees = attendees
         self.description = description
         self.end = end
         self.extra = extra
         self.id = id
         self.is_all_day = is_all_day
         self.location = location
         self.online_meeting_info = online_meeting_info
         self.recurrence = recurrence
         self.reminders = reminders
+        self.rich_text_description = rich_text_description
         self.start = start
         self.summary = summary
 
     def validate(self):
         if self.attendees:
             for k in self.attendees:
                 if k:
@@ -9039,14 +9302,16 @@
             self.online_meeting_info.validate()
         if self.recurrence:
             self.recurrence.validate()
         if self.reminders:
             for k in self.reminders:
                 if k:
                     k.validate()
+        if self.rich_text_description:
+            self.rich_text_description.validate()
         if self.start:
             self.start.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -9072,14 +9337,16 @@
             result['onlineMeetingInfo'] = self.online_meeting_info.to_map()
         if self.recurrence is not None:
             result['recurrence'] = self.recurrence.to_map()
         result['reminders'] = []
         if self.reminders is not None:
             for k in self.reminders:
                 result['reminders'].append(k.to_map() if k else None)
+        if self.rich_text_description is not None:
+            result['richTextDescription'] = self.rich_text_description.to_map()
         if self.start is not None:
             result['start'] = self.start.to_map()
         if self.summary is not None:
             result['summary'] = self.summary
         return result
 
     def from_map(self, m: dict = None):
@@ -9110,14 +9377,17 @@
             temp_model = PatchEventRequestRecurrence()
             self.recurrence = temp_model.from_map(m['recurrence'])
         self.reminders = []
         if m.get('reminders') is not None:
             for k in m.get('reminders'):
                 temp_model = PatchEventRequestReminders()
                 self.reminders.append(temp_model.from_map(k))
+        if m.get('richTextDescription') is not None:
+            temp_model = PatchEventRequestRichTextDescription()
+            self.rich_text_description = temp_model.from_map(m['richTextDescription'])
         if m.get('start') is not None:
             temp_model = PatchEventRequestStart()
             self.start = temp_model.from_map(m['start'])
         if m.get('summary') is not None:
             self.summary = m.get('summary')
         return self
 
@@ -9486,14 +9756,41 @@
         if m.get('method') is not None:
             self.method = m.get('method')
         if m.get('minutes') is not None:
             self.minutes = m.get('minutes')
         return self
 
 
+class PatchEventResponseBodyRichTextDescription(TeaModel):
+    def __init__(
+        self,
+        text: str = None,
+    ):
+        self.text = text
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.text is not None:
+            result['text'] = self.text
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('text') is not None:
+            self.text = m.get('text')
+        return self
+
+
 class PatchEventResponseBodyStart(TeaModel):
     def __init__(
         self,
         date: str = None,
         date_time: str = None,
         time_zone: str = None,
     ):
@@ -9539,14 +9836,15 @@
         id: str = None,
         is_all_day: bool = None,
         location: PatchEventResponseBodyLocation = None,
         online_meeting_info: PatchEventResponseBodyOnlineMeetingInfo = None,
         organizer: PatchEventResponseBodyOrganizer = None,
         recurrence: PatchEventResponseBodyRecurrence = None,
         reminders: List[PatchEventResponseBodyReminders] = None,
+        rich_text_description: PatchEventResponseBodyRichTextDescription = None,
         start: PatchEventResponseBodyStart = None,
         summary: str = None,
         update_time: str = None,
     ):
         self.attendees = attendees
         self.create_time = create_time
         self.description = description
@@ -9554,14 +9852,15 @@
         self.id = id
         self.is_all_day = is_all_day
         self.location = location
         self.online_meeting_info = online_meeting_info
         self.organizer = organizer
         self.recurrence = recurrence
         self.reminders = reminders
+        self.rich_text_description = rich_text_description
         self.start = start
         self.summary = summary
         self.update_time = update_time
 
     def validate(self):
         if self.attendees:
             for k in self.attendees:
@@ -9577,14 +9876,16 @@
             self.organizer.validate()
         if self.recurrence:
             self.recurrence.validate()
         if self.reminders:
             for k in self.reminders:
                 if k:
                     k.validate()
+        if self.rich_text_description:
+            self.rich_text_description.validate()
         if self.start:
             self.start.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -9612,14 +9913,16 @@
             result['organizer'] = self.organizer.to_map()
         if self.recurrence is not None:
             result['recurrence'] = self.recurrence.to_map()
         result['reminders'] = []
         if self.reminders is not None:
             for k in self.reminders:
                 result['reminders'].append(k.to_map() if k else None)
+        if self.rich_text_description is not None:
+            result['richTextDescription'] = self.rich_text_description.to_map()
         if self.start is not None:
             result['start'] = self.start.to_map()
         if self.summary is not None:
             result['summary'] = self.summary
         if self.update_time is not None:
             result['updateTime'] = self.update_time
         return result
@@ -9655,14 +9958,17 @@
             temp_model = PatchEventResponseBodyRecurrence()
             self.recurrence = temp_model.from_map(m['recurrence'])
         self.reminders = []
         if m.get('reminders') is not None:
             for k in m.get('reminders'):
                 temp_model = PatchEventResponseBodyReminders()
                 self.reminders.append(temp_model.from_map(k))
+        if m.get('richTextDescription') is not None:
+            temp_model = PatchEventResponseBodyRichTextDescription()
+            self.rich_text_description = temp_model.from_map(m['richTextDescription'])
         if m.get('start') is not None:
             temp_model = PatchEventResponseBodyStart()
             self.start = temp_model.from_map(m['start'])
         if m.get('summary') is not None:
             self.summary = m.get('summary')
         if m.get('updateTime') is not None:
             self.update_time = m.get('updateTime')
```

### Comparing `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/carbon_1_0/client.py` & `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/carbon_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/carbon_1_0/models.py` & `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/carbon_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/card_1_0/client.py` & `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/card_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/card_1_0/models.py` & `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/card_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/check_in_1_0/client.py` & `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/check_in_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/check_in_1_0/models.py` & `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/check_in_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/chengfeng_1_0/client.py` & `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/chengfeng_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/chengfeng_1_0/models.py` & `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/chengfeng_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/conference_1_0/client.py` & `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/conference_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/conference_1_0/models.py` & `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/conference_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/connector_1_0/client.py` & `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/connector_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/connector_1_0/models.py` & `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/connector_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/contact_1_0/client.py` & `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/contact_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/contact_1_0/models.py` & `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/contact_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/content_1_0/client.py` & `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/content_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/content_1_0/models.py` & `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/content_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/contract_1_0/client.py` & `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/contract_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/contract_1_0/models.py` & `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/contract_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/conv_file_1_0/client.py` & `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/conv_file_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/conv_file_1_0/models.py` & `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/conv_file_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/crm_1_0/client.py` & `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/crm_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/crm_1_0/models.py` & `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/crm_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/crm_2_0/client.py` & `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/crm_2_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/crm_2_0/models.py` & `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/crm_2_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/customer_service_1_0/client.py` & `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/customer_service_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/customer_service_1_0/models.py` & `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/customer_service_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/datacenter_1_0/client.py` & `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/datacenter_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/datacenter_1_0/models.py` & `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/datacenter_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/devicemng_1_0/client.py` & `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/devicemng_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/devicemng_1_0/models.py` & `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/devicemng_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/dingmi_1_0/client.py` & `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/dingmi_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/dingmi_1_0/models.py` & `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/dingmi_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/diot_1_0/client.py` & `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/diot_1_0/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 # This file is auto-generated, don't edit it. Thanks.
-from Tea.core import TeaCore
 from typing import Dict
+from Tea.core import TeaCore
 
 from alibabacloud_gateway_spi.client import Client as SPIClient
 from alibabacloud_tea_openapi.client import Client as OpenApiClient
 from alibabacloud_tea_openapi import models as open_api_models
 from alibabacloud_gateway_dingtalk.client import Client as GatewayClientClient
 from alibabacloud_tea_util.client import Client as UtilClient
 from alibabacloud_dingtalk.diot_1_0 import models as dingtalkdiot__1__0_models
@@ -27,14 +27,90 @@
         self._client = GatewayClientClient()
         self._spi = self._client
         self._signature_algorithm = 'v2'
         self._endpoint_rule = ''
         if UtilClient.empty(self._endpoint):
             self._endpoint = 'api.dingtalk.com'
 
+    def ayun_onlien_test_with_options(
+        self,
+        request: dingtalkdiot__1__0_models.AyunOnlienTestRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> dingtalkdiot__1__0_models.AyunOnlienTestResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.req_id):
+            query['reqId'] = request.req_id
+        req = open_api_models.OpenApiRequest(
+            headers=headers,
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='AyunOnlienTest',
+            version='diot_1.0',
+            protocol='HTTP',
+            pathname=f'/v1.0/diot/ayunTest',
+            method='GET',
+            auth_type='Anonymous',
+            style='ROA',
+            req_body_type='none',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dingtalkdiot__1__0_models.AyunOnlienTestResponse(),
+            self.execute(params, req, runtime)
+        )
+
+    async def ayun_onlien_test_with_options_async(
+        self,
+        request: dingtalkdiot__1__0_models.AyunOnlienTestRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> dingtalkdiot__1__0_models.AyunOnlienTestResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.req_id):
+            query['reqId'] = request.req_id
+        req = open_api_models.OpenApiRequest(
+            headers=headers,
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='AyunOnlienTest',
+            version='diot_1.0',
+            protocol='HTTP',
+            pathname=f'/v1.0/diot/ayunTest',
+            method='GET',
+            auth_type='Anonymous',
+            style='ROA',
+            req_body_type='none',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dingtalkdiot__1__0_models.AyunOnlienTestResponse(),
+            await self.execute_async(params, req, runtime)
+        )
+
+    def ayun_onlien_test(
+        self,
+        request: dingtalkdiot__1__0_models.AyunOnlienTestRequest,
+    ) -> dingtalkdiot__1__0_models.AyunOnlienTestResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.ayun_onlien_test_with_options(request, headers, runtime)
+
+    async def ayun_onlien_test_async(
+        self,
+        request: dingtalkdiot__1__0_models.AyunOnlienTestRequest,
+    ) -> dingtalkdiot__1__0_models.AyunOnlienTestResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.ayun_onlien_test_with_options_async(request, headers, runtime)
+
     def batch_delete_device_with_options(
         self,
         request: dingtalkdiot__1__0_models.BatchDeleteDeviceRequest,
         headers: dingtalkdiot__1__0_models.BatchDeleteDeviceHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> dingtalkdiot__1__0_models.BatchDeleteDeviceResponse:
         UtilClient.validate_model(request)
```

### Comparing `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/diot_1_0/models.py` & `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/diot_1_0/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,111 @@
 # -*- coding: utf-8 -*-
 # This file is auto-generated, don't edit it. Thanks.
 from Tea.model import TeaModel
 from typing import Dict, List, Any
 
 
+class AyunOnlienTestRequest(TeaModel):
+    def __init__(
+        self,
+        req_id: str = None,
+    ):
+        self.req_id = req_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.req_id is not None:
+            result['reqId'] = self.req_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('reqId') is not None:
+            self.req_id = m.get('reqId')
+        return self
+
+
+class AyunOnlienTestResponseBody(TeaModel):
+    def __init__(
+        self,
+        request_id: str = None,
+    ):
+        self.request_id = request_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.request_id is not None:
+            result['requestId'] = self.request_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('requestId') is not None:
+            self.request_id = m.get('requestId')
+        return self
+
+
+class AyunOnlienTestResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: AyunOnlienTestResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = AyunOnlienTestResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class BatchDeleteDeviceHeaders(TeaModel):
     def __init__(
         self,
         common_headers: Dict[str, str] = None,
         x_acs_dingtalk_access_token: str = None,
     ):
         self.common_headers = common_headers
```

### Comparing `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/doc_1_0/client.py` & `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/doc_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/doc_1_0/models.py` & `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/doc_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/doc_2_0/client.py` & `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/doc_2_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/doc_2_0/models.py` & `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/doc_2_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/drive_1_0/client.py` & `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/drive_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/drive_1_0/models.py` & `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/drive_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/edu_1_0/client.py` & `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/edu_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/edu_1_0/models.py` & `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/edu_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/esign_1_0/client.py` & `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/esign_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/esign_1_0/models.py` & `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/esign_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/esign_2_0/client.py` & `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/esign_2_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/esign_2_0/models.py` & `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/esign_2_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/event_1_0/client.py` & `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/event_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/event_1_0/models.py` & `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/event_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/exclusive_1_0/client.py` & `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/exclusive_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/exclusive_1_0/models.py` & `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/exclusive_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/finance_1_0/client.py` & `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/finance_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/finance_1_0/models.py` & `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/finance_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/flashmeeting_1_0/client.py` & `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/flashmeeting_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/flashmeeting_1_0/models.py` & `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/flashmeeting_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/gateway_1_0/client.py` & `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/gateway_1_0/client.py`

 * *Files 9% similar despite different names*

```diff
@@ -39,14 +39,16 @@
     ) -> dingtalkgateway__1__0_models.OpenConnectionResponse:
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.client_id):
             body['clientId'] = request.client_id
         if not UtilClient.is_unset(request.client_secret):
             body['clientSecret'] = request.client_secret
+        if not UtilClient.is_unset(request.local_ip):
+            body['localIp'] = request.local_ip
         if not UtilClient.is_unset(request.subscriptions):
             body['subscriptions'] = request.subscriptions
         req = open_api_models.OpenApiRequest(
             headers=headers,
             body=OpenApiUtilClient.parse_to_map(body)
         )
         params = open_api_models.Params(
@@ -73,14 +75,16 @@
     ) -> dingtalkgateway__1__0_models.OpenConnectionResponse:
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.client_id):
             body['clientId'] = request.client_id
         if not UtilClient.is_unset(request.client_secret):
             body['clientSecret'] = request.client_secret
+        if not UtilClient.is_unset(request.local_ip):
+            body['localIp'] = request.local_ip
         if not UtilClient.is_unset(request.subscriptions):
             body['subscriptions'] = request.subscriptions
         req = open_api_models.OpenApiRequest(
             headers=headers,
             body=OpenApiUtilClient.parse_to_map(body)
         )
         params = open_api_models.Params(
```

### Comparing `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/gateway_1_0/models.py` & `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/gateway_1_0/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,18 +38,20 @@
 
 
 class OpenConnectionRequest(TeaModel):
     def __init__(
         self,
         client_id: str = None,
         client_secret: str = None,
+        local_ip: str = None,
         subscriptions: List[OpenConnectionRequestSubscriptions] = None,
     ):
         self.client_id = client_id
         self.client_secret = client_secret
+        self.local_ip = local_ip
         self.subscriptions = subscriptions
 
     def validate(self):
         if self.subscriptions:
             for k in self.subscriptions:
                 if k:
                     k.validate()
@@ -60,26 +62,30 @@
             return _map
 
         result = dict()
         if self.client_id is not None:
             result['clientId'] = self.client_id
         if self.client_secret is not None:
             result['clientSecret'] = self.client_secret
+        if self.local_ip is not None:
+            result['localIp'] = self.local_ip
         result['subscriptions'] = []
         if self.subscriptions is not None:
             for k in self.subscriptions:
                 result['subscriptions'].append(k.to_map() if k else None)
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('clientId') is not None:
             self.client_id = m.get('clientId')
         if m.get('clientSecret') is not None:
             self.client_secret = m.get('clientSecret')
+        if m.get('localIp') is not None:
+            self.local_ip = m.get('localIp')
         self.subscriptions = []
         if m.get('subscriptions') is not None:
             for k in m.get('subscriptions'):
                 temp_model = OpenConnectionRequestSubscriptions()
                 self.subscriptions.append(temp_model.from_map(k))
         return self
```

### Comparing `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/group_blackboard_1_0/client.py` & `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/group_blackboard_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/group_blackboard_1_0/models.py` & `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/group_blackboard_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/h3yun_1_0/client.py` & `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/h3yun_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/h3yun_1_0/models.py` & `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/h3yun_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/h5package_1_0/client.py` & `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/h5package_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/h5package_1_0/models.py` & `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/h5package_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/hrbrain_1_0/client.py` & `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/hrbrain_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/hrbrain_1_0/models.py` & `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/hrbrain_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/hrm_1_0/client.py` & `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/hrm_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/hrm_1_0/models.py` & `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/hrm_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/im_1_0/client.py` & `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/im_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/im_1_0/models.py` & `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/im_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/im_2_0/client.py` & `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/im_2_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/im_2_0/models.py` & `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/im_2_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/impaas_1_0/client.py` & `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/impaas_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/impaas_1_0/models.py` & `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/impaas_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/industry_1_0/client.py` & `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/industry_1_0/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -11607,14 +11607,112 @@
         self,
         request: dingtalkindustry__1__0_models.SupplyChainUpdateDeptInfoRequest,
     ) -> dingtalkindustry__1__0_models.SupplyChainUpdateDeptInfoResponse:
         runtime = util_models.RuntimeOptions()
         headers = dingtalkindustry__1__0_models.SupplyChainUpdateDeptInfoHeaders()
         return await self.supply_chain_update_dept_info_with_options_async(request, headers, runtime)
 
+    def supply_delete_member_with_options(
+        self,
+        request: dingtalkindustry__1__0_models.SupplyDeleteMemberRequest,
+        headers: dingtalkindustry__1__0_models.SupplyDeleteMemberHeaders,
+        runtime: util_models.RuntimeOptions,
+    ) -> dingtalkindustry__1__0_models.SupplyDeleteMemberResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.dept_id):
+            query['deptId'] = request.dept_id
+        if not UtilClient.is_unset(request.mobile):
+            query['mobile'] = request.mobile
+        if not UtilClient.is_unset(request.union_id):
+            query['unionId'] = request.union_id
+        if not UtilClient.is_unset(request.user_id):
+            query['userId'] = request.user_id
+        real_headers = {}
+        if not UtilClient.is_unset(headers.common_headers):
+            real_headers = headers.common_headers
+        if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
+            real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
+        req = open_api_models.OpenApiRequest(
+            headers=real_headers,
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='SupplyDeleteMember',
+            version='industry_1.0',
+            protocol='HTTP',
+            pathname=f'/v1.0/industry/supplyChains/members',
+            method='DELETE',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='none',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dingtalkindustry__1__0_models.SupplyDeleteMemberResponse(),
+            self.execute(params, req, runtime)
+        )
+
+    async def supply_delete_member_with_options_async(
+        self,
+        request: dingtalkindustry__1__0_models.SupplyDeleteMemberRequest,
+        headers: dingtalkindustry__1__0_models.SupplyDeleteMemberHeaders,
+        runtime: util_models.RuntimeOptions,
+    ) -> dingtalkindustry__1__0_models.SupplyDeleteMemberResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.dept_id):
+            query['deptId'] = request.dept_id
+        if not UtilClient.is_unset(request.mobile):
+            query['mobile'] = request.mobile
+        if not UtilClient.is_unset(request.union_id):
+            query['unionId'] = request.union_id
+        if not UtilClient.is_unset(request.user_id):
+            query['userId'] = request.user_id
+        real_headers = {}
+        if not UtilClient.is_unset(headers.common_headers):
+            real_headers = headers.common_headers
+        if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
+            real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
+        req = open_api_models.OpenApiRequest(
+            headers=real_headers,
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='SupplyDeleteMember',
+            version='industry_1.0',
+            protocol='HTTP',
+            pathname=f'/v1.0/industry/supplyChains/members',
+            method='DELETE',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='none',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dingtalkindustry__1__0_models.SupplyDeleteMemberResponse(),
+            await self.execute_async(params, req, runtime)
+        )
+
+    def supply_delete_member(
+        self,
+        request: dingtalkindustry__1__0_models.SupplyDeleteMemberRequest,
+    ) -> dingtalkindustry__1__0_models.SupplyDeleteMemberResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = dingtalkindustry__1__0_models.SupplyDeleteMemberHeaders()
+        return self.supply_delete_member_with_options(request, headers, runtime)
+
+    async def supply_delete_member_async(
+        self,
+        request: dingtalkindustry__1__0_models.SupplyDeleteMemberRequest,
+    ) -> dingtalkindustry__1__0_models.SupplyDeleteMemberResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = dingtalkindustry__1__0_models.SupplyDeleteMemberHeaders()
+        return await self.supply_delete_member_with_options_async(request, headers, runtime)
+
     def supply_delete_partner_admins_with_options(
         self,
         request: dingtalkindustry__1__0_models.SupplyDeletePartnerAdminsRequest,
         headers: dingtalkindustry__1__0_models.SupplyDeletePartnerAdminsHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> dingtalkindustry__1__0_models.SupplyDeletePartnerAdminsResponse:
         UtilClient.validate_model(request)
```

### Comparing `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/industry_1_0/models.py` & `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/industry_1_0/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -24426,14 +24426,163 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = SupplyChainUpdateDeptInfoResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class SupplyDeleteMemberHeaders(TeaModel):
+    def __init__(
+        self,
+        common_headers: Dict[str, str] = None,
+        x_acs_dingtalk_access_token: str = None,
+    ):
+        self.common_headers = common_headers
+        self.x_acs_dingtalk_access_token = x_acs_dingtalk_access_token
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.common_headers is not None:
+            result['commonHeaders'] = self.common_headers
+        if self.x_acs_dingtalk_access_token is not None:
+            result['x-acs-dingtalk-access-token'] = self.x_acs_dingtalk_access_token
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('commonHeaders') is not None:
+            self.common_headers = m.get('commonHeaders')
+        if m.get('x-acs-dingtalk-access-token') is not None:
+            self.x_acs_dingtalk_access_token = m.get('x-acs-dingtalk-access-token')
+        return self
+
+
+class SupplyDeleteMemberRequest(TeaModel):
+    def __init__(
+        self,
+        dept_id: int = None,
+        mobile: str = None,
+        union_id: str = None,
+        user_id: str = None,
+    ):
+        self.dept_id = dept_id
+        self.mobile = mobile
+        self.union_id = union_id
+        self.user_id = user_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.dept_id is not None:
+            result['deptId'] = self.dept_id
+        if self.mobile is not None:
+            result['mobile'] = self.mobile
+        if self.union_id is not None:
+            result['unionId'] = self.union_id
+        if self.user_id is not None:
+            result['userId'] = self.user_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('deptId') is not None:
+            self.dept_id = m.get('deptId')
+        if m.get('mobile') is not None:
+            self.mobile = m.get('mobile')
+        if m.get('unionId') is not None:
+            self.union_id = m.get('unionId')
+        if m.get('userId') is not None:
+            self.user_id = m.get('userId')
+        return self
+
+
+class SupplyDeleteMemberResponseBody(TeaModel):
+    def __init__(
+        self,
+        result: bool = None,
+    ):
+        self.result = result
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.result is not None:
+            result['result'] = self.result
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('result') is not None:
+            self.result = m.get('result')
+        return self
+
+
+class SupplyDeleteMemberResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: SupplyDeleteMemberResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = SupplyDeleteMemberResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class SupplyDeletePartnerAdminsHeaders(TeaModel):
     def __init__(
         self,
         common_headers: Dict[str, str] = None,
         x_acs_dingtalk_access_token: str = None,
     ):
         self.common_headers = common_headers
```

### Comparing `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/jzcrm_1_0/client.py` & `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/jzcrm_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/jzcrm_1_0/models.py` & `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/jzcrm_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/link_1_0/client.py` & `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/link_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/link_1_0/models.py` & `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/link_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/live_1_0/client.py` & `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/live_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/live_1_0/models.py` & `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/live_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/manufacturing_1_0/client.py` & `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/manufacturing_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/manufacturing_1_0/models.py` & `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/manufacturing_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/micro_app_1_0/client.py` & `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/micro_app_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/micro_app_1_0/models.py` & `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/micro_app_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/miniapp_1_0/client.py` & `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/miniapp_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/miniapp_1_0/models.py` & `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/miniapp_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/oauth2_1_0/client.py` & `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/oauth2_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/oauth2_1_0/models.py` & `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/oauth2_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/occupationauth_1_0/client.py` & `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/occupationauth_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/occupationauth_1_0/models.py` & `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/occupationauth_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/okr_1_0/client.py` & `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/okr_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/okr_1_0/models.py` & `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/okr_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/org_culture_1_0/client.py` & `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/org_culture_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/org_culture_1_0/models.py` & `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/org_culture_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/package_1_0/client.py` & `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/package_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/package_1_0/models.py` & `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/package_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/pedia_1_0/client.py` & `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/pedia_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/pedia_1_0/models.py` & `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/pedia_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/project_1_0/client.py` & `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/project_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/project_1_0/models.py` & `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/project_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/project_integration_1_0/client.py` & `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/project_integration_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/project_integration_1_0/models.py` & `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/project_integration_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/rcs_call_1_0/client.py` & `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/rcs_call_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/rcs_call_1_0/models.py` & `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/rcs_call_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/resident_1_0/client.py` & `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/resident_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/resident_1_0/models.py` & `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/resident_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/robot_1_0/client.py` & `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/robot_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/robot_1_0/models.py` & `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/robot_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/rooms_1_0/client.py` & `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/rooms_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/rooms_1_0/models.py` & `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/rooms_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/search_1_0/client.py` & `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/search_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/search_1_0/models.py` & `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/search_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/service_group_1_0/client.py` & `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/service_group_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/service_group_1_0/models.py` & `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/service_group_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/smart_device_1_0/client.py` & `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/smart_device_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/smart_device_1_0/models.py` & `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/smart_device_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/sns_storage_1_0/client.py` & `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/sns_storage_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/sns_storage_1_0/models.py` & `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/sns_storage_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/storage_1_0/client.py` & `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/storage_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/storage_1_0/models.py` & `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/storage_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/storage_2_0/client.py` & `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/storage_2_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/storage_2_0/models.py` & `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/storage_2_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/swform_1_0/client.py` & `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/swform_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/swform_1_0/models.py` & `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/swform_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/todo_1_0/client.py` & `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/todo_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/todo_1_0/models.py` & `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/todo_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/trade_1_0/client.py` & `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/trade_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/trade_1_0/models.py` & `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/trade_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/trajectory_1_0/client.py` & `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/trajectory_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/trajectory_1_0/models.py` & `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/trajectory_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/transcribe_1_0/client.py` & `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/transcribe_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/transcribe_1_0/models.py` & `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/transcribe_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/trip_1_0/client.py` & `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/trip_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/trip_1_0/models.py` & `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/trip_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/village_1_0/client.py` & `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/village_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/village_1_0/models.py` & `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/village_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/watt_1_0/client.py` & `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/watt_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/watt_1_0/models.py` & `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/watt_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/wiki_1_0/client.py` & `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/wiki_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/wiki_1_0/models.py` & `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/wiki_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/wiki_2_0/client.py` & `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/wiki_2_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/wiki_2_0/models.py` & `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/wiki_2_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/wms_1_0/client.py` & `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/wms_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/wms_1_0/models.py` & `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/wms_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/workbench_1_0/client.py` & `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/workbench_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/workbench_1_0/models.py` & `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/workbench_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/workflow_1_0/client.py` & `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/workflow_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/workflow_1_0/models.py` & `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/workflow_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/workrecord_1_0/client.py` & `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/workrecord_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/workrecord_1_0/models.py` & `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/workrecord_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/yida_1_0/client.py` & `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/yida_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/yida_1_0/models.py` & `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/yida_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/yun_shu_1_0/client.py` & `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/yun_shu_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/yun_shu_1_0/models.py` & `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/yun_shu_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk.egg-info/PKG-INFO` & `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-dingtalk
-Version: 2.0.19
+Version: 2.0.20
 Summary: Alibaba Cloud Dingtalk SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk.egg-info/SOURCES.txt` & `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -7,14 +7,17 @@
 setup.py
 alibabacloud_dingtalk/__init__.py
 alibabacloud_dingtalk.egg-info/PKG-INFO
 alibabacloud_dingtalk.egg-info/SOURCES.txt
 alibabacloud_dingtalk.egg-info/dependency_links.txt
 alibabacloud_dingtalk.egg-info/requires.txt
 alibabacloud_dingtalk.egg-info/top_level.txt
+alibabacloud_dingtalk/activity_1_0/__init__.py
+alibabacloud_dingtalk/activity_1_0/client.py
+alibabacloud_dingtalk/activity_1_0/models.py
 alibabacloud_dingtalk/algo_1_0/__init__.py
 alibabacloud_dingtalk/algo_1_0/client.py
 alibabacloud_dingtalk/algo_1_0/models.py
 alibabacloud_dingtalk/alitrip_1_0/__init__.py
 alibabacloud_dingtalk/alitrip_1_0/client.py
 alibabacloud_dingtalk/alitrip_1_0/models.py
 alibabacloud_dingtalk/apaas_1_0/__init__.py
```

### Comparing `alibabacloud_dingtalk-2.0.19/setup.py` & `alibabacloud_dingtalk-2.0.20/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_dingtalk.
 
-Created on 09/06/2023
+Created on 13/06/2023
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_dingtalk"
 NAME = "alibabacloud_dingtalk" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud Dingtalk SDK Library for Python"
```

