# Comparing `tmp/alibabacloud_dingtalk-2.0.18.tar.gz` & `tmp/alibabacloud_dingtalk-2.0.19.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_dingtalk-2.0.18.tar", last modified: Wed May 31 06:47:25 2023, max compression
+gzip compressed data, was "dist/alibabacloud_dingtalk-2.0.19.tar", last modified: Fri Jun  9 07:12:55 2023, max compression
```

## Comparing `alibabacloud_dingtalk-2.0.18.tar` & `alibabacloud_dingtalk-2.0.19.tar`

### file list

```diff
@@ -1,365 +1,365 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/
--rw-r--r--   0 root         (0) root         (0)    19817 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2309 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1021 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1106 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/algo_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/algo_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9980 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/algo_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    23314 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/algo_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/alitrip_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/alitrip_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    58254 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/alitrip_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   169621 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/alitrip_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/apaas_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/apaas_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    25166 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/apaas_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    46194 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/apaas_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/app_market_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/app_market_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    21260 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/app_market_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    23341 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/app_market_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/ats_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/ats_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    90648 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/ats_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   138912 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/ats_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/attendance_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/attendance_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   165948 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/attendance_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   322772 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/attendance_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/badge_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/badge_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    45240 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/badge_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    62246 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/badge_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/bizfinance_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/bizfinance_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   201848 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/bizfinance_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   569113 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/bizfinance_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/blackboard_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/blackboard_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4942 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/blackboard_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     3871 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/blackboard_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/calendar_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/calendar_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   138814 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/calendar_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   331545 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/calendar_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/carbon_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/carbon_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    27976 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/carbon_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    42229 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/carbon_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/card_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/card_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    35138 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/card_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   101075 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/card_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/check_in_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/check_in_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6044 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/check_in_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    10446 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/check_in_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/chengfeng_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/chengfeng_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    71632 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/chengfeng_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   123179 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/chengfeng_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/conference_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/conference_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    90334 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/conference_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   117347 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/conference_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/connector_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/connector_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    58616 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/connector_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   124904 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/connector_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/contact_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/contact_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   297108 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/contact_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   392984 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/contact_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/content_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/content_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    21270 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/content_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    42332 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/content_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/contract_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/contract_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6576 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/contract_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    10253 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/contract_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/conv_file_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/conv_file_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    17934 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/conv_file_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    30852 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/conv_file_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/crm_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/crm_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   223914 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/crm_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   552073 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/crm_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/crm_2_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/crm_2_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4810 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/crm_2_0/client.py
--rw-r--r--   0 root         (0) root         (0)     7385 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/crm_2_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/customer_service_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/customer_service_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    32170 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/customer_service_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    46898 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/customer_service_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/datacenter_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/datacenter_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   391978 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/datacenter_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   515455 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/datacenter_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/devicemng_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/devicemng_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   112278 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/devicemng_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   152480 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/devicemng_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/dingmi_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/dingmi_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    56946 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/dingmi_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    56301 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/dingmi_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/diot_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/diot_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    48073 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/diot_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    67303 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/diot_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/doc_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/doc_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   211006 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/doc_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   267473 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/doc_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/doc_2_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/doc_2_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   150160 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/doc_2_0/client.py
--rw-r--r--   0 root         (0) root         (0)   269103 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/doc_2_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/drive_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/drive_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   140210 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/drive_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   195538 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/drive_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/edu_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/edu_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   453174 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/edu_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   705965 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/edu_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/esign_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/esign_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    72708 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/esign_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   116546 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/esign_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/esign_2_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/esign_2_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    86294 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/esign_2_0/client.py
--rw-r--r--   0 root         (0) root         (0)   123749 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/esign_2_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/event_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/event_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5096 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/event_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     6148 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/event_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/exclusive_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/exclusive_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   312544 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/exclusive_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   433417 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/exclusive_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/finance_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/finance_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   155788 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/finance_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   302125 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/finance_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/flashmeeting_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/flashmeeting_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9368 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/flashmeeting_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    12542 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/flashmeeting_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/gateway_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/gateway_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4431 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/gateway_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     4668 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/gateway_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/group_blackboard_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/group_blackboard_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10562 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/group_blackboard_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     9742 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/group_blackboard_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/h3yun_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/h3yun_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    80133 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/h3yun_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   138362 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/h3yun_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/h5package_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/h5package_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    17059 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/h5package_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    18903 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/h5package_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/hrbrain_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/hrbrain_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5382 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/hrbrain_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     4660 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/hrbrain_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/hrm_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/hrm_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    92926 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/hrm_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   137528 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/hrm_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/im_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/im_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   302532 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/im_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   378971 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/im_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/im_2_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/im_2_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    22430 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/im_2_0/client.py
--rw-r--r--   0 root         (0) root         (0)    31875 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/im_2_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/impaas_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/impaas_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    90230 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/impaas_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    92472 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/impaas_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/industry_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/industry_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   606316 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/industry_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   855474 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/industry_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/jzcrm_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/jzcrm_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    62348 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/jzcrm_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   155140 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/jzcrm_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/link_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/link_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    63194 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/link_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   108695 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/link_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/live_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/live_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    91118 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/live_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   135110 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/live_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/manufacturing_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/manufacturing_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    16181 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/manufacturing_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    23076 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/manufacturing_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/micro_app_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/micro_app_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   144945 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/micro_app_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   173192 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/micro_app_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/miniapp_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/miniapp_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    52227 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/miniapp_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    54521 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/miniapp_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/oauth2_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/oauth2_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    31076 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/oauth2_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    40802 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/oauth2_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/occupationauth_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/occupationauth_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8962 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/occupationauth_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     7507 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/occupationauth_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/okr_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/okr_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    76720 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/okr_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   137701 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/okr_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/org_culture_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/org_culture_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    77488 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/org_culture_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   123420 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/org_culture_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/package_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/package_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    56344 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/package_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    60347 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/package_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/pedia_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/pedia_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    29226 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/pedia_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    69069 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/pedia_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/project_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/project_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   260568 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/project_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   413706 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/project_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/project_integration_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/project_integration_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    17983 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/project_integration_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    11593 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/project_integration_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/rcs_call_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/rcs_call_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5368 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/rcs_call_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     4579 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/rcs_call_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/resident_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/resident_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   135300 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/resident_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   174524 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/resident_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/robot_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/robot_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    81780 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/robot_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    93746 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/robot_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/rooms_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/rooms_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    56986 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/rooms_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    83842 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/rooms_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/search_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/search_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    39248 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/search_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    46018 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/search_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/service_group_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/service_group_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   361006 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/service_group_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   503423 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/service_group_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/smart_device_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/smart_device_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    31508 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/smart_device_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    26678 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/smart_device_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/sns_storage_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/sns_storage_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    44726 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/sns_storage_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    96217 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/sns_storage_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/storage_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/storage_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   187612 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/storage_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   353698 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/storage_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/storage_2_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/storage_2_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    53470 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/storage_2_0/client.py
--rw-r--r--   0 root         (0) root         (0)    89290 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/storage_2_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/swform_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/swform_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13910 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/swform_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    28559 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/swform_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/todo_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/todo_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    65344 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/todo_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   148231 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/todo_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/trade_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/trade_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14284 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/trade_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    16170 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/trade_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/trajectory_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/trajectory_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14192 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/trajectory_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    21677 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/trajectory_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/transcribe_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/transcribe_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13676 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/transcribe_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    17519 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/transcribe_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/trip_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/trip_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    18718 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/trip_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    32237 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/trip_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/village_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/village_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    75904 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/village_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   110849 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/village_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/watt_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/watt_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4269 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/watt_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     3363 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/watt_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/wiki_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/wiki_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8278 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/wiki_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    20486 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/wiki_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/wiki_2_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/wiki_2_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    66210 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/wiki_2_0/client.py
--rw-r--r--   0 root         (0) root         (0)   130783 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/wiki_2_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/wms_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/wms_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5370 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/wms_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     8325 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/wms_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/workbench_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/workbench_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    27686 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/workbench_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    29689 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/workbench_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/workflow_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/workflow_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   179772 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/workflow_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   377816 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/workflow_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/workrecord_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/workrecord_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4774 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/workrecord_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     3772 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/workrecord_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/yida_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/yida_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   464194 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/yida_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   687148 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/yida_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/yun_shu_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/yun_shu_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5452 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/yun_shu_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     4490 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/yun_shu_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2309 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    12014 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      239 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2684 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/
+-rw-r--r--   0 root         (0) root         (0)    19882 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2309 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1021 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1106 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/algo_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/algo_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9980 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/algo_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    23314 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/algo_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/alitrip_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/alitrip_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    58254 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/alitrip_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   169621 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/alitrip_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/apaas_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/apaas_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    25166 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/apaas_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    46194 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/apaas_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/app_market_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/app_market_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    25682 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/app_market_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    27728 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/app_market_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/ats_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/ats_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    90648 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/ats_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   138912 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/ats_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/attendance_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/attendance_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   165948 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/attendance_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   323041 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/attendance_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/badge_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/badge_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    45240 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/badge_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    62246 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/badge_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/bizfinance_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/bizfinance_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   201848 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/bizfinance_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   569113 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/bizfinance_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/blackboard_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/blackboard_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4942 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/blackboard_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     3871 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/blackboard_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/calendar_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/calendar_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   138814 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/calendar_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   331545 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/calendar_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/carbon_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/carbon_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    27976 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/carbon_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    42229 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/carbon_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/card_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/card_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    35138 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/card_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   101075 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/card_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/check_in_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/check_in_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6044 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/check_in_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    10446 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/check_in_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/chengfeng_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/chengfeng_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    71632 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/chengfeng_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   123179 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/chengfeng_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/conference_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/conference_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    90334 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/conference_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   117347 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/conference_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/connector_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/connector_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    58616 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/connector_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   124904 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/connector_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/contact_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/contact_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   297108 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/contact_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   392984 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/contact_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/content_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/content_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    21270 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/content_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    42332 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/content_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/contract_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/contract_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    19674 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/contract_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    27526 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/contract_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/conv_file_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/conv_file_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    17934 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/conv_file_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    30852 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/conv_file_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/crm_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/crm_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   223914 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/crm_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   552073 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/crm_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/crm_2_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/crm_2_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4810 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/crm_2_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     7385 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/crm_2_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/customer_service_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/customer_service_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    32170 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/customer_service_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    46898 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/customer_service_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/datacenter_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/datacenter_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   391978 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/datacenter_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   515455 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/datacenter_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/devicemng_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/devicemng_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   112278 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/devicemng_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   152480 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/devicemng_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/dingmi_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/dingmi_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    56946 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/dingmi_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    56301 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/dingmi_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/diot_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/diot_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    50179 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/diot_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    69305 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/diot_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/doc_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/doc_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   211006 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/doc_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   267473 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/doc_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/doc_2_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/doc_2_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   150160 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/doc_2_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   269103 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/doc_2_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/drive_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/drive_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   140210 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/drive_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   195538 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/drive_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/edu_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/edu_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   453174 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/edu_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   705965 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/edu_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/esign_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/esign_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    72708 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/esign_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   116546 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/esign_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/esign_2_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/esign_2_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    86294 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/esign_2_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   123749 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/esign_2_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/event_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/event_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5096 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/event_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     6148 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/event_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/exclusive_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/exclusive_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   316592 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/exclusive_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   439557 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/exclusive_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/finance_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/finance_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   155788 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/finance_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   302125 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/finance_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/flashmeeting_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/flashmeeting_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9368 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/flashmeeting_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    12542 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/flashmeeting_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/gateway_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/gateway_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4431 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/gateway_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     4668 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/gateway_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/group_blackboard_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/group_blackboard_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10562 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/group_blackboard_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     9742 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/group_blackboard_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/h3yun_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/h3yun_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    80133 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/h3yun_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   138362 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/h3yun_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/h5package_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/h5package_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    17059 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/h5package_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    18903 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/h5package_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/hrbrain_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/hrbrain_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5382 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/hrbrain_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     4660 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/hrbrain_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/hrm_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/hrm_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    92926 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/hrm_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   137528 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/hrm_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/im_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/im_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   302532 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/im_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   378971 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/im_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/im_2_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/im_2_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    22430 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/im_2_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    31875 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/im_2_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/impaas_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/impaas_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    90230 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/impaas_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    92472 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/impaas_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/industry_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/industry_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   606316 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/industry_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   855474 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/industry_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/jzcrm_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/jzcrm_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    62348 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/jzcrm_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   155140 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/jzcrm_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/link_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/link_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    63194 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/link_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   108695 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/link_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/live_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/live_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    91118 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/live_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   135110 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/live_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/manufacturing_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/manufacturing_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    16181 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/manufacturing_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    23076 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/manufacturing_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/micro_app_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/micro_app_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   146899 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/micro_app_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   175146 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/micro_app_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/miniapp_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/miniapp_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    52227 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/miniapp_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    54521 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/miniapp_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/oauth2_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/oauth2_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    31076 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/oauth2_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    40802 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/oauth2_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/occupationauth_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/occupationauth_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8962 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/occupationauth_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     7507 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/occupationauth_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/okr_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/okr_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    76720 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/okr_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   137701 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/okr_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/org_culture_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/org_culture_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    77488 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/org_culture_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   123420 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/org_culture_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/package_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/package_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    56344 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/package_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    60347 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/package_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/pedia_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/pedia_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    29226 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/pedia_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    69069 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/pedia_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/project_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/project_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   260568 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/project_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   413706 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/project_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/project_integration_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/project_integration_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    17983 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/project_integration_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    11593 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/project_integration_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/rcs_call_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/rcs_call_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5368 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/rcs_call_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     4579 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/rcs_call_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/resident_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/resident_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   135300 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/resident_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   174524 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/resident_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/robot_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/robot_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    81780 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/robot_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    93746 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/robot_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/rooms_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/rooms_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    56986 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/rooms_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    83842 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/rooms_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/search_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/search_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    39248 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/search_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    46018 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/search_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/service_group_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/service_group_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   361006 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/service_group_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   503423 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/service_group_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/smart_device_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/smart_device_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    31508 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/smart_device_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    26678 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/smart_device_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/sns_storage_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/sns_storage_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    44726 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/sns_storage_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    96217 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/sns_storage_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/storage_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/storage_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   187612 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/storage_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   353698 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/storage_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/storage_2_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/storage_2_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    53470 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/storage_2_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    89290 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/storage_2_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/swform_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/swform_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13910 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/swform_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    28559 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/swform_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/todo_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/todo_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    65344 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/todo_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   148231 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/todo_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/trade_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/trade_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14284 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/trade_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    16170 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/trade_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/trajectory_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/trajectory_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14192 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/trajectory_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    21677 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/trajectory_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/transcribe_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/transcribe_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13676 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/transcribe_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    17519 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/transcribe_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/trip_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/trip_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    18718 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/trip_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    32237 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/trip_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/village_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/village_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    75904 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/village_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   110849 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/village_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/watt_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/watt_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4269 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/watt_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     3363 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/watt_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/wiki_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/wiki_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8278 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/wiki_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    20486 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/wiki_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/wiki_2_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/wiki_2_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    66210 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/wiki_2_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   130783 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/wiki_2_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/wms_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/wms_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5370 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/wms_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     8325 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/wms_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/workbench_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/workbench_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    27686 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/workbench_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    29689 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/workbench_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/workflow_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/workflow_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   179772 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/workflow_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   377816 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/workflow_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/workrecord_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/workrecord_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4774 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/workrecord_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     3772 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/workrecord_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/yida_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/yida_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   464194 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/yida_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   687148 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/yida_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/yun_shu_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/yun_shu_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5452 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/yun_shu_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     4490 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/yun_shu_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2309 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    12014 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      239 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2684 2023-06-09 07:12:55.000000 alibabacloud_dingtalk-2.0.19/setup.py
```

### Comparing `alibabacloud_dingtalk-2.0.18/ChangeLog.md` & `alibabacloud_dingtalk-2.0.19/ChangeLog.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+2023-05-31 Version: 2.0.18
+- Update AddOfficialAccountFollower.
+
 2023-05-26 Version: 2.0.17
 - Update AddOfficialAccountFollower.
 
 2023-05-24 Version: 2.0.16
 - Update AddOfficialAccountFollower.
 
 2023-05-18 Version: 2.0.15
```

### Comparing `alibabacloud_dingtalk-2.0.18/LICENSE` & `alibabacloud_dingtalk-2.0.19/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.18/PKG-INFO` & `alibabacloud_dingtalk-2.0.19/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_dingtalk
-Version: 2.0.18
+Version: 2.0.19
 Summary: Alibaba Cloud Dingtalk SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_dingtalk-2.0.18/README-CN.md` & `alibabacloud_dingtalk-2.0.19/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.18/README.md` & `alibabacloud_dingtalk-2.0.19/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/algo_1_0/client.py` & `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/algo_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/algo_1_0/models.py` & `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/algo_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/alitrip_1_0/client.py` & `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/alitrip_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/alitrip_1_0/models.py` & `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/alitrip_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/apaas_1_0/client.py` & `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/apaas_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/apaas_1_0/models.py` & `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/apaas_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/app_market_1_0/client.py` & `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/app_market_1_0/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -209,14 +209,112 @@
         self,
         request: dingtalkapp_market__1__0_models.GetCoolAppAccessStatusRequest,
     ) -> dingtalkapp_market__1__0_models.GetCoolAppAccessStatusResponse:
         runtime = util_models.RuntimeOptions()
         headers = dingtalkapp_market__1__0_models.GetCoolAppAccessStatusHeaders()
         return await self.get_cool_app_access_status_with_options_async(request, headers, runtime)
 
+    def get_in_app_sku_url_with_options(
+        self,
+        request: dingtalkapp_market__1__0_models.GetInAppSkuUrlRequest,
+        headers: dingtalkapp_market__1__0_models.GetInAppSkuUrlHeaders,
+        runtime: util_models.RuntimeOptions,
+    ) -> dingtalkapp_market__1__0_models.GetInAppSkuUrlResponse:
+        UtilClient.validate_model(request)
+        body = {}
+        if not UtilClient.is_unset(request.callback_page):
+            body['callbackPage'] = request.callback_page
+        if not UtilClient.is_unset(request.extend_param):
+            body['extendParam'] = request.extend_param
+        if not UtilClient.is_unset(request.goods_code):
+            body['goodsCode'] = request.goods_code
+        if not UtilClient.is_unset(request.item_code):
+            body['itemCode'] = request.item_code
+        real_headers = {}
+        if not UtilClient.is_unset(headers.common_headers):
+            real_headers = headers.common_headers
+        if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
+            real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
+        req = open_api_models.OpenApiRequest(
+            headers=real_headers,
+            body=OpenApiUtilClient.parse_to_map(body)
+        )
+        params = open_api_models.Params(
+            action='GetInAppSkuUrl',
+            version='appMarket_1.0',
+            protocol='HTTP',
+            pathname=f'/v1.0/appMarket/internals/skuPages/query',
+            method='POST',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='none',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dingtalkapp_market__1__0_models.GetInAppSkuUrlResponse(),
+            self.execute(params, req, runtime)
+        )
+
+    async def get_in_app_sku_url_with_options_async(
+        self,
+        request: dingtalkapp_market__1__0_models.GetInAppSkuUrlRequest,
+        headers: dingtalkapp_market__1__0_models.GetInAppSkuUrlHeaders,
+        runtime: util_models.RuntimeOptions,
+    ) -> dingtalkapp_market__1__0_models.GetInAppSkuUrlResponse:
+        UtilClient.validate_model(request)
+        body = {}
+        if not UtilClient.is_unset(request.callback_page):
+            body['callbackPage'] = request.callback_page
+        if not UtilClient.is_unset(request.extend_param):
+            body['extendParam'] = request.extend_param
+        if not UtilClient.is_unset(request.goods_code):
+            body['goodsCode'] = request.goods_code
+        if not UtilClient.is_unset(request.item_code):
+            body['itemCode'] = request.item_code
+        real_headers = {}
+        if not UtilClient.is_unset(headers.common_headers):
+            real_headers = headers.common_headers
+        if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
+            real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
+        req = open_api_models.OpenApiRequest(
+            headers=real_headers,
+            body=OpenApiUtilClient.parse_to_map(body)
+        )
+        params = open_api_models.Params(
+            action='GetInAppSkuUrl',
+            version='appMarket_1.0',
+            protocol='HTTP',
+            pathname=f'/v1.0/appMarket/internals/skuPages/query',
+            method='POST',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='none',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dingtalkapp_market__1__0_models.GetInAppSkuUrlResponse(),
+            await self.execute_async(params, req, runtime)
+        )
+
+    def get_in_app_sku_url(
+        self,
+        request: dingtalkapp_market__1__0_models.GetInAppSkuUrlRequest,
+    ) -> dingtalkapp_market__1__0_models.GetInAppSkuUrlResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = dingtalkapp_market__1__0_models.GetInAppSkuUrlHeaders()
+        return self.get_in_app_sku_url_with_options(request, headers, runtime)
+
+    async def get_in_app_sku_url_async(
+        self,
+        request: dingtalkapp_market__1__0_models.GetInAppSkuUrlRequest,
+    ) -> dingtalkapp_market__1__0_models.GetInAppSkuUrlResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = dingtalkapp_market__1__0_models.GetInAppSkuUrlHeaders()
+        return await self.get_in_app_sku_url_with_options_async(request, headers, runtime)
+
     def get_personal_experience_info_with_options(
         self,
         request: dingtalkapp_market__1__0_models.GetPersonalExperienceInfoRequest,
         headers: dingtalkapp_market__1__0_models.GetPersonalExperienceInfoHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> dingtalkapp_market__1__0_models.GetPersonalExperienceInfoResponse:
         UtilClient.validate_model(request)
```

### Comparing `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/app_market_1_0/models.py` & `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/app_market_1_0/models.py`

 * *Files 10% similar despite different names*

```diff
@@ -286,14 +286,163 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = GetCoolAppAccessStatusResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class GetInAppSkuUrlHeaders(TeaModel):
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
+class GetInAppSkuUrlRequest(TeaModel):
+    def __init__(
+        self,
+        callback_page: str = None,
+        extend_param: str = None,
+        goods_code: str = None,
+        item_code: str = None,
+    ):
+        self.callback_page = callback_page
+        self.extend_param = extend_param
+        self.goods_code = goods_code
+        self.item_code = item_code
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
+        if self.callback_page is not None:
+            result['callbackPage'] = self.callback_page
+        if self.extend_param is not None:
+            result['extendParam'] = self.extend_param
+        if self.goods_code is not None:
+            result['goodsCode'] = self.goods_code
+        if self.item_code is not None:
+            result['itemCode'] = self.item_code
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('callbackPage') is not None:
+            self.callback_page = m.get('callbackPage')
+        if m.get('extendParam') is not None:
+            self.extend_param = m.get('extendParam')
+        if m.get('goodsCode') is not None:
+            self.goods_code = m.get('goodsCode')
+        if m.get('itemCode') is not None:
+            self.item_code = m.get('itemCode')
+        return self
+
+
+class GetInAppSkuUrlResponseBody(TeaModel):
+    def __init__(
+        self,
+        url: str = None,
+    ):
+        self.url = url
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
+        if self.url is not None:
+            result['url'] = self.url
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('url') is not None:
+            self.url = m.get('url')
+        return self
+
+
+class GetInAppSkuUrlResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: GetInAppSkuUrlResponseBody = None,
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
+            temp_model = GetInAppSkuUrlResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class GetPersonalExperienceInfoHeaders(TeaModel):
     def __init__(
         self,
         common_headers: Dict[str, str] = None,
         x_acs_dingtalk_access_token: str = None,
     ):
         self.common_headers = common_headers
```

### Comparing `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/ats_1_0/client.py` & `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/ats_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/ats_1_0/models.py` & `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/ats_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/attendance_1_0/client.py` & `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/attendance_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/attendance_1_0/models.py` & `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/attendance_1_0/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -5470,26 +5470,28 @@
         self,
         absenteeism_late_minutes: int = None,
         across: int = None,
         begin_min: int = None,
         check_time: str = None,
         check_type: str = None,
         end_min: int = None,
+        flex_minutes: List[int] = None,
         free_check: bool = None,
         late_back_setting: GetShiftResponseBodyResultSectionsPunchesLateBackSetting = None,
         permit_minutes: int = None,
         punche_id: int = None,
         serious_late_minutes: int = None,
     ):
         self.absenteeism_late_minutes = absenteeism_late_minutes
         self.across = across
         self.begin_min = begin_min
         self.check_time = check_time
         self.check_type = check_type
         self.end_min = end_min
+        self.flex_minutes = flex_minutes
         self.free_check = free_check
         self.late_back_setting = late_back_setting
         self.permit_minutes = permit_minutes
         self.punche_id = punche_id
         self.serious_late_minutes = serious_late_minutes
 
     def validate(self):
@@ -5509,15 +5511,17 @@
         if self.begin_min is not None:
             result['beginMin'] = self.begin_min
         if self.check_time is not None:
             result['checkTime'] = self.check_time
         if self.check_type is not None:
             result['checkType'] = self.check_type
         if self.end_min is not None:
-            result['end_min'] = self.end_min
+            result['endMin'] = self.end_min
+        if self.flex_minutes is not None:
+            result['flexMinutes'] = self.flex_minutes
         if self.free_check is not None:
             result['freeCheck'] = self.free_check
         if self.late_back_setting is not None:
             result['lateBackSetting'] = self.late_back_setting.to_map()
         if self.permit_minutes is not None:
             result['permitMinutes'] = self.permit_minutes
         if self.punche_id is not None:
@@ -5534,16 +5538,18 @@
             self.across = m.get('across')
         if m.get('beginMin') is not None:
             self.begin_min = m.get('beginMin')
         if m.get('checkTime') is not None:
             self.check_time = m.get('checkTime')
         if m.get('checkType') is not None:
             self.check_type = m.get('checkType')
-        if m.get('end_min') is not None:
-            self.end_min = m.get('end_min')
+        if m.get('endMin') is not None:
+            self.end_min = m.get('endMin')
+        if m.get('flexMinutes') is not None:
+            self.flex_minutes = m.get('flexMinutes')
         if m.get('freeCheck') is not None:
             self.free_check = m.get('freeCheck')
         if m.get('lateBackSetting') is not None:
             temp_model = GetShiftResponseBodyResultSectionsPunchesLateBackSetting()
             self.late_back_setting = temp_model.from_map(m['lateBackSetting'])
         if m.get('permitMinutes') is not None:
             self.permit_minutes = m.get('permitMinutes')
@@ -5577,27 +5583,27 @@
 
         result = dict()
         if self.across is not None:
             result['across'] = self.across
         if self.check_time is not None:
             result['checkTime'] = self.check_time
         if self.check_type is not None:
-            result['check_type'] = self.check_type
+            result['checkType'] = self.check_type
         if self.rest_id is not None:
             result['restId'] = self.rest_id
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('across') is not None:
             self.across = m.get('across')
         if m.get('checkTime') is not None:
             self.check_time = m.get('checkTime')
-        if m.get('check_type') is not None:
-            self.check_type = m.get('check_type')
+        if m.get('checkType') is not None:
+            self.check_type = m.get('checkType')
         if m.get('restId') is not None:
             self.rest_id = m.get('restId')
         return self
 
 
 class GetShiftResponseBodyResultSections(TeaModel):
     def __init__(
```

### Comparing `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/badge_1_0/client.py` & `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/badge_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/badge_1_0/models.py` & `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/badge_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/bizfinance_1_0/client.py` & `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/bizfinance_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/bizfinance_1_0/models.py` & `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/bizfinance_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/blackboard_1_0/client.py` & `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/blackboard_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/blackboard_1_0/models.py` & `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/blackboard_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/calendar_1_0/client.py` & `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/calendar_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/calendar_1_0/models.py` & `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/calendar_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/carbon_1_0/client.py` & `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/carbon_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/carbon_1_0/models.py` & `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/carbon_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/card_1_0/client.py` & `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/card_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/card_1_0/models.py` & `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/card_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/check_in_1_0/client.py` & `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/check_in_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/check_in_1_0/models.py` & `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/check_in_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/chengfeng_1_0/client.py` & `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/chengfeng_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/chengfeng_1_0/models.py` & `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/chengfeng_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/conference_1_0/client.py` & `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/conference_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/conference_1_0/models.py` & `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/conference_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/connector_1_0/client.py` & `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/connector_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/connector_1_0/models.py` & `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/connector_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/contact_1_0/client.py` & `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/contact_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/contact_1_0/models.py` & `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/contact_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/content_1_0/client.py` & `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/content_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/content_1_0/models.py` & `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/content_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/contract_1_0/models.py` & `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/group_blackboard_1_0/models.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*-
 # This file is auto-generated, don't edit it. Thanks.
 from Tea.model import TeaModel
-from typing import Dict, List
+from typing import Dict
 
 
-class SendContractCardHeaders(TeaModel):
+class CreateGroupBlackboardHeaders(TeaModel):
     def __init__(
         self,
         common_headers: Dict[str, str] = None,
         x_acs_dingtalk_access_token: str = None,
     ):
         self.common_headers = common_headers
         self.x_acs_dingtalk_access_token = x_acs_dingtalk_access_token
@@ -33,259 +33,259 @@
         if m.get('commonHeaders') is not None:
             self.common_headers = m.get('commonHeaders')
         if m.get('x-acs-dingtalk-access-token') is not None:
             self.x_acs_dingtalk_access_token = m.get('x-acs-dingtalk-access-token')
         return self
 
 
-class SendContractCardRequestContractInfo(TeaModel):
+class CreateGroupBlackboardRequest(TeaModel):
     def __init__(
         self,
-        contract_code: str = None,
-        contract_name: str = None,
-        create_time: int = None,
-        sign_user_name: str = None,
+        content: str = None,
+        open_conversation_id: str = None,
+        send_ding: bool = None,
+        sticky: bool = None,
+        unique_id: str = None,
+        user_id: str = None,
     ):
-        self.contract_code = contract_code
-        self.contract_name = contract_name
-        self.create_time = create_time
-        self.sign_user_name = sign_user_name
+        self.content = content
+        self.open_conversation_id = open_conversation_id
+        self.send_ding = send_ding
+        self.sticky = sticky
+        self.unique_id = unique_id
+        self.user_id = user_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.contract_code is not None:
-            result['contractCode'] = self.contract_code
-        if self.contract_name is not None:
-            result['contractName'] = self.contract_name
-        if self.create_time is not None:
-            result['createTime'] = self.create_time
-        if self.sign_user_name is not None:
-            result['signUserName'] = self.sign_user_name
+        if self.content is not None:
+            result['content'] = self.content
+        if self.open_conversation_id is not None:
+            result['openConversationId'] = self.open_conversation_id
+        if self.send_ding is not None:
+            result['sendDing'] = self.send_ding
+        if self.sticky is not None:
+            result['sticky'] = self.sticky
+        if self.unique_id is not None:
+            result['uniqueId'] = self.unique_id
+        if self.user_id is not None:
+            result['userId'] = self.user_id
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('contractCode') is not None:
-            self.contract_code = m.get('contractCode')
-        if m.get('contractName') is not None:
-            self.contract_name = m.get('contractName')
-        if m.get('createTime') is not None:
-            self.create_time = m.get('createTime')
-        if m.get('signUserName') is not None:
-            self.sign_user_name = m.get('signUserName')
+        if m.get('content') is not None:
+            self.content = m.get('content')
+        if m.get('openConversationId') is not None:
+            self.open_conversation_id = m.get('openConversationId')
+        if m.get('sendDing') is not None:
+            self.send_ding = m.get('sendDing')
+        if m.get('sticky') is not None:
+            self.sticky = m.get('sticky')
+        if m.get('uniqueId') is not None:
+            self.unique_id = m.get('uniqueId')
+        if m.get('userId') is not None:
+            self.user_id = m.get('userId')
         return self
 
 
-class SendContractCardRequestReceivers(TeaModel):
+class CreateGroupBlackboardResponseBody(TeaModel):
     def __init__(
         self,
-        corp_id: str = None,
-        user_id: str = None,
-        user_type: str = None,
+        data_id: str = None,
+        success: bool = None,
     ):
-        self.corp_id = corp_id
-        self.user_id = user_id
-        self.user_type = user_type
+        self.data_id = data_id
+        self.success = success
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.corp_id is not None:
-            result['corpId'] = self.corp_id
-        if self.user_id is not None:
-            result['userId'] = self.user_id
-        if self.user_type is not None:
-            result['userType'] = self.user_type
+        if self.data_id is not None:
+            result['dataId'] = self.data_id
+        if self.success is not None:
+            result['success'] = self.success
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('corpId') is not None:
-            self.corp_id = m.get('corpId')
-        if m.get('userId') is not None:
-            self.user_id = m.get('userId')
-        if m.get('userType') is not None:
-            self.user_type = m.get('userType')
+        if m.get('dataId') is not None:
+            self.data_id = m.get('dataId')
+        if m.get('success') is not None:
+            self.success = m.get('success')
         return self
 
 
-class SendContractCardRequestSender(TeaModel):
+class CreateGroupBlackboardResponse(TeaModel):
     def __init__(
         self,
-        corp_id: str = None,
-        user_id: str = None,
-        user_type: str = None,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: CreateGroupBlackboardResponseBody = None,
     ):
-        self.corp_id = corp_id
-        self.user_id = user_id
-        self.user_type = user_type
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
+            temp_model = CreateGroupBlackboardResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
+class DeleteGroupBlackboardHeaders(TeaModel):
+    def __init__(
+        self,
+        common_headers: Dict[str, str] = None,
+        x_acs_dingtalk_access_token: str = None,
+    ):
+        self.common_headers = common_headers
+        self.x_acs_dingtalk_access_token = x_acs_dingtalk_access_token
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.corp_id is not None:
-            result['corpId'] = self.corp_id
-        if self.user_id is not None:
-            result['userId'] = self.user_id
-        if self.user_type is not None:
-            result['userType'] = self.user_type
+        if self.common_headers is not None:
+            result['commonHeaders'] = self.common_headers
+        if self.x_acs_dingtalk_access_token is not None:
+            result['x-acs-dingtalk-access-token'] = self.x_acs_dingtalk_access_token
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('corpId') is not None:
-            self.corp_id = m.get('corpId')
-        if m.get('userId') is not None:
-            self.user_id = m.get('userId')
-        if m.get('userType') is not None:
-            self.user_type = m.get('userType')
+        if m.get('commonHeaders') is not None:
+            self.common_headers = m.get('commonHeaders')
+        if m.get('x-acs-dingtalk-access-token') is not None:
+            self.x_acs_dingtalk_access_token = m.get('x-acs-dingtalk-access-token')
         return self
 
 
-class SendContractCardRequest(TeaModel):
+class DeleteGroupBlackboardRequest(TeaModel):
     def __init__(
         self,
-        card_type: str = None,
-        contract_info: SendContractCardRequestContractInfo = None,
-        corp_id: str = None,
-        extension: Dict[str, str] = None,
-        process_instance_id: str = None,
-        receive_groups: List[str] = None,
-        receivers: List[SendContractCardRequestReceivers] = None,
-        sender: SendContractCardRequestSender = None,
-        sync_single_chat: bool = None,
+        data_id: str = None,
+        open_conversation_id: str = None,
+        user_id: str = None,
     ):
-        self.card_type = card_type
-        self.contract_info = contract_info
-        self.corp_id = corp_id
-        self.extension = extension
-        self.process_instance_id = process_instance_id
-        self.receive_groups = receive_groups
-        self.receivers = receivers
-        self.sender = sender
-        self.sync_single_chat = sync_single_chat
+        self.data_id = data_id
+        self.open_conversation_id = open_conversation_id
+        self.user_id = user_id
 
     def validate(self):
-        if self.contract_info:
-            self.contract_info.validate()
-        if self.receivers:
-            for k in self.receivers:
-                if k:
-                    k.validate()
-        if self.sender:
-            self.sender.validate()
+        pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.card_type is not None:
-            result['cardType'] = self.card_type
-        if self.contract_info is not None:
-            result['contractInfo'] = self.contract_info.to_map()
-        if self.corp_id is not None:
-            result['corpId'] = self.corp_id
-        if self.extension is not None:
-            result['extension'] = self.extension
-        if self.process_instance_id is not None:
-            result['processInstanceId'] = self.process_instance_id
-        if self.receive_groups is not None:
-            result['receiveGroups'] = self.receive_groups
-        result['receivers'] = []
-        if self.receivers is not None:
-            for k in self.receivers:
-                result['receivers'].append(k.to_map() if k else None)
-        if self.sender is not None:
-            result['sender'] = self.sender.to_map()
-        if self.sync_single_chat is not None:
-            result['syncSingleChat'] = self.sync_single_chat
+        if self.data_id is not None:
+            result['dataId'] = self.data_id
+        if self.open_conversation_id is not None:
+            result['openConversationId'] = self.open_conversation_id
+        if self.user_id is not None:
+            result['userId'] = self.user_id
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('cardType') is not None:
-            self.card_type = m.get('cardType')
-        if m.get('contractInfo') is not None:
-            temp_model = SendContractCardRequestContractInfo()
-            self.contract_info = temp_model.from_map(m['contractInfo'])
-        if m.get('corpId') is not None:
-            self.corp_id = m.get('corpId')
-        if m.get('extension') is not None:
-            self.extension = m.get('extension')
-        if m.get('processInstanceId') is not None:
-            self.process_instance_id = m.get('processInstanceId')
-        if m.get('receiveGroups') is not None:
-            self.receive_groups = m.get('receiveGroups')
-        self.receivers = []
-        if m.get('receivers') is not None:
-            for k in m.get('receivers'):
-                temp_model = SendContractCardRequestReceivers()
-                self.receivers.append(temp_model.from_map(k))
-        if m.get('sender') is not None:
-            temp_model = SendContractCardRequestSender()
-            self.sender = temp_model.from_map(m['sender'])
-        if m.get('syncSingleChat') is not None:
-            self.sync_single_chat = m.get('syncSingleChat')
+        if m.get('dataId') is not None:
+            self.data_id = m.get('dataId')
+        if m.get('openConversationId') is not None:
+            self.open_conversation_id = m.get('openConversationId')
+        if m.get('userId') is not None:
+            self.user_id = m.get('userId')
         return self
 
 
-class SendContractCardResponseBody(TeaModel):
+class DeleteGroupBlackboardResponseBody(TeaModel):
     def __init__(
         self,
+        is_deleted: bool = None,
         success: bool = None,
     ):
+        self.is_deleted = is_deleted
         self.success = success
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
+        if self.is_deleted is not None:
+            result['isDeleted'] = self.is_deleted
         if self.success is not None:
             result['success'] = self.success
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
+        if m.get('isDeleted') is not None:
+            self.is_deleted = m.get('isDeleted')
         if m.get('success') is not None:
             self.success = m.get('success')
         return self
 
 
-class SendContractCardResponse(TeaModel):
+class DeleteGroupBlackboardResponse(TeaModel):
     def __init__(
         self,
         headers: Dict[str, str] = None,
         status_code: int = None,
-        body: SendContractCardResponseBody = None,
+        body: DeleteGroupBlackboardResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
@@ -311,12 +311,12 @@
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('headers') is not None:
             self.headers = m.get('headers')
         if m.get('statusCode') is not None:
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
-            temp_model = SendContractCardResponseBody()
+            temp_model = DeleteGroupBlackboardResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
```

### Comparing `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/conv_file_1_0/client.py` & `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/conv_file_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/conv_file_1_0/models.py` & `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/conv_file_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/crm_1_0/client.py` & `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/crm_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/crm_1_0/models.py` & `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/crm_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/crm_2_0/client.py` & `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/crm_2_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/crm_2_0/models.py` & `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/crm_2_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/customer_service_1_0/client.py` & `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/customer_service_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/customer_service_1_0/models.py` & `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/customer_service_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/datacenter_1_0/client.py` & `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/datacenter_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/datacenter_1_0/models.py` & `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/datacenter_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/devicemng_1_0/client.py` & `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/devicemng_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/devicemng_1_0/models.py` & `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/devicemng_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/dingmi_1_0/client.py` & `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/dingmi_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/dingmi_1_0/models.py` & `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/dingmi_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/diot_1_0/client.py` & `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/diot_1_0/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -587,14 +587,72 @@
         self,
         request: dingtalkdiot__1__0_models.DeviceConferenceRequest,
     ) -> dingtalkdiot__1__0_models.DeviceConferenceResponse:
         runtime = util_models.RuntimeOptions()
         headers = dingtalkdiot__1__0_models.DeviceConferenceHeaders()
         return await self.device_conference_with_options_async(request, headers, runtime)
 
+    def diot_system_mark_test_with_options(
+        self,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> dingtalkdiot__1__0_models.DiotSystemMarkTestResponse:
+        req = open_api_models.OpenApiRequest(
+            headers=headers
+        )
+        params = open_api_models.Params(
+            action='DiotSystemMarkTest',
+            version='diot_1.0',
+            protocol='HTTP',
+            pathname=f'/v1.0/diot/sys/mark/test',
+            method='GET',
+            auth_type='Anonymous',
+            style='ROA',
+            req_body_type='none',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dingtalkdiot__1__0_models.DiotSystemMarkTestResponse(),
+            self.execute(params, req, runtime)
+        )
+
+    async def diot_system_mark_test_with_options_async(
+        self,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> dingtalkdiot__1__0_models.DiotSystemMarkTestResponse:
+        req = open_api_models.OpenApiRequest(
+            headers=headers
+        )
+        params = open_api_models.Params(
+            action='DiotSystemMarkTest',
+            version='diot_1.0',
+            protocol='HTTP',
+            pathname=f'/v1.0/diot/sys/mark/test',
+            method='GET',
+            auth_type='Anonymous',
+            style='ROA',
+            req_body_type='none',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dingtalkdiot__1__0_models.DiotSystemMarkTestResponse(),
+            await self.execute_async(params, req, runtime)
+        )
+
+    def diot_system_mark_test(self) -> dingtalkdiot__1__0_models.DiotSystemMarkTestResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.diot_system_mark_test_with_options(headers, runtime)
+
+    async def diot_system_mark_test_async(self) -> dingtalkdiot__1__0_models.DiotSystemMarkTestResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.diot_system_mark_test_with_options_async(headers, runtime)
+
     def push_event_with_options(
         self,
         request: dingtalkdiot__1__0_models.PushEventRequest,
         headers: dingtalkdiot__1__0_models.PushEventHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> dingtalkdiot__1__0_models.PushEventResponse:
         UtilClient.validate_model(request)
```

### Comparing `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/diot_1_0/models.py` & `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/diot_1_0/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -1135,14 +1135,85 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = DeviceConferenceResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class DiotSystemMarkTestResponseBody(TeaModel):
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
+class DiotSystemMarkTestResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: DiotSystemMarkTestResponseBody = None,
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
+            temp_model = DiotSystemMarkTestResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class PushEventHeaders(TeaModel):
     def __init__(
         self,
         common_headers: Dict[str, str] = None,
         x_acs_dingtalk_access_token: str = None,
     ):
         self.common_headers = common_headers
```

### Comparing `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/doc_1_0/client.py` & `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/doc_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/doc_1_0/models.py` & `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/doc_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/doc_2_0/client.py` & `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/doc_2_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/doc_2_0/models.py` & `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/doc_2_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/drive_1_0/client.py` & `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/drive_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/drive_1_0/models.py` & `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/drive_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/edu_1_0/client.py` & `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/edu_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/edu_1_0/models.py` & `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/edu_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/esign_1_0/client.py` & `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/esign_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/esign_1_0/models.py` & `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/esign_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/esign_2_0/client.py` & `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/esign_2_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/esign_2_0/models.py` & `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/esign_2_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/event_1_0/client.py` & `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/event_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/event_1_0/models.py` & `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/event_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/exclusive_1_0/client.py` & `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/exclusive_1_0/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -3145,14 +3145,104 @@
         self,
         request: dingtalkexclusive__1__0_models.GetOaOperatorLogListRequest,
     ) -> dingtalkexclusive__1__0_models.GetOaOperatorLogListResponse:
         runtime = util_models.RuntimeOptions()
         headers = dingtalkexclusive__1__0_models.GetOaOperatorLogListHeaders()
         return await self.get_oa_operator_log_list_with_options_async(request, headers, runtime)
 
+    def get_out_groups_by_page_with_options(
+        self,
+        request: dingtalkexclusive__1__0_models.GetOutGroupsByPageRequest,
+        headers: dingtalkexclusive__1__0_models.GetOutGroupsByPageHeaders,
+        runtime: util_models.RuntimeOptions,
+    ) -> dingtalkexclusive__1__0_models.GetOutGroupsByPageResponse:
+        UtilClient.validate_model(request)
+        body = {}
+        if not UtilClient.is_unset(request.page_number):
+            body['pageNumber'] = request.page_number
+        if not UtilClient.is_unset(request.page_size):
+            body['pageSize'] = request.page_size
+        real_headers = {}
+        if not UtilClient.is_unset(headers.common_headers):
+            real_headers = headers.common_headers
+        if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
+            real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
+        req = open_api_models.OpenApiRequest(
+            headers=real_headers,
+            body=OpenApiUtilClient.parse_to_map(body)
+        )
+        params = open_api_models.Params(
+            action='GetOutGroupsByPage',
+            version='exclusive_1.0',
+            protocol='HTTP',
+            pathname=f'/v1.0/exclusive/audits/outsideGroups/query',
+            method='POST',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='none',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dingtalkexclusive__1__0_models.GetOutGroupsByPageResponse(),
+            self.execute(params, req, runtime)
+        )
+
+    async def get_out_groups_by_page_with_options_async(
+        self,
+        request: dingtalkexclusive__1__0_models.GetOutGroupsByPageRequest,
+        headers: dingtalkexclusive__1__0_models.GetOutGroupsByPageHeaders,
+        runtime: util_models.RuntimeOptions,
+    ) -> dingtalkexclusive__1__0_models.GetOutGroupsByPageResponse:
+        UtilClient.validate_model(request)
+        body = {}
+        if not UtilClient.is_unset(request.page_number):
+            body['pageNumber'] = request.page_number
+        if not UtilClient.is_unset(request.page_size):
+            body['pageSize'] = request.page_size
+        real_headers = {}
+        if not UtilClient.is_unset(headers.common_headers):
+            real_headers = headers.common_headers
+        if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
+            real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
+        req = open_api_models.OpenApiRequest(
+            headers=real_headers,
+            body=OpenApiUtilClient.parse_to_map(body)
+        )
+        params = open_api_models.Params(
+            action='GetOutGroupsByPage',
+            version='exclusive_1.0',
+            protocol='HTTP',
+            pathname=f'/v1.0/exclusive/audits/outsideGroups/query',
+            method='POST',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='none',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dingtalkexclusive__1__0_models.GetOutGroupsByPageResponse(),
+            await self.execute_async(params, req, runtime)
+        )
+
+    def get_out_groups_by_page(
+        self,
+        request: dingtalkexclusive__1__0_models.GetOutGroupsByPageRequest,
+    ) -> dingtalkexclusive__1__0_models.GetOutGroupsByPageResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = dingtalkexclusive__1__0_models.GetOutGroupsByPageHeaders()
+        return self.get_out_groups_by_page_with_options(request, headers, runtime)
+
+    async def get_out_groups_by_page_async(
+        self,
+        request: dingtalkexclusive__1__0_models.GetOutGroupsByPageRequest,
+    ) -> dingtalkexclusive__1__0_models.GetOutGroupsByPageResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = dingtalkexclusive__1__0_models.GetOutGroupsByPageHeaders()
+        return await self.get_out_groups_by_page_with_options_async(request, headers, runtime)
+
     def get_outside_audit_group_message_by_page_with_options(
         self,
         request: dingtalkexclusive__1__0_models.GetOutsideAuditGroupMessageByPageRequest,
         headers: dingtalkexclusive__1__0_models.GetOutsideAuditGroupMessageByPageHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> dingtalkexclusive__1__0_models.GetOutsideAuditGroupMessageByPageResponse:
         UtilClient.validate_model(request)
```

### Comparing `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/exclusive_1_0/models.py` & `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/exclusive_1_0/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -6132,14 +6132,221 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = GetOaOperatorLogListResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class GetOutGroupsByPageHeaders(TeaModel):
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
+class GetOutGroupsByPageRequest(TeaModel):
+    def __init__(
+        self,
+        page_number: int = None,
+        page_size: int = None,
+    ):
+        self.page_number = page_number
+        self.page_size = page_size
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
+        if self.page_number is not None:
+            result['pageNumber'] = self.page_number
+        if self.page_size is not None:
+            result['pageSize'] = self.page_size
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('pageNumber') is not None:
+            self.page_number = m.get('pageNumber')
+        if m.get('pageSize') is not None:
+            self.page_size = m.get('pageSize')
+        return self
+
+
+class GetOutGroupsByPageResponseBodyResponseBodyGroupList(TeaModel):
+    def __init__(
+        self,
+        open_conversation_id: str = None,
+    ):
+        self.open_conversation_id = open_conversation_id
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
+        if self.open_conversation_id is not None:
+            result['openConversationId'] = self.open_conversation_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('openConversationId') is not None:
+            self.open_conversation_id = m.get('openConversationId')
+        return self
+
+
+class GetOutGroupsByPageResponseBodyResponseBody(TeaModel):
+    def __init__(
+        self,
+        group_list: List[GetOutGroupsByPageResponseBodyResponseBodyGroupList] = None,
+        total: int = None,
+    ):
+        self.group_list = group_list
+        self.total = total
+
+    def validate(self):
+        if self.group_list:
+            for k in self.group_list:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        result['groupList'] = []
+        if self.group_list is not None:
+            for k in self.group_list:
+                result['groupList'].append(k.to_map() if k else None)
+        if self.total is not None:
+            result['total'] = self.total
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        self.group_list = []
+        if m.get('groupList') is not None:
+            for k in m.get('groupList'):
+                temp_model = GetOutGroupsByPageResponseBodyResponseBodyGroupList()
+                self.group_list.append(temp_model.from_map(k))
+        if m.get('total') is not None:
+            self.total = m.get('total')
+        return self
+
+
+class GetOutGroupsByPageResponseBody(TeaModel):
+    def __init__(
+        self,
+        response_body: GetOutGroupsByPageResponseBodyResponseBody = None,
+    ):
+        self.response_body = response_body
+
+    def validate(self):
+        if self.response_body:
+            self.response_body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.response_body is not None:
+            result['responseBody'] = self.response_body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('responseBody') is not None:
+            temp_model = GetOutGroupsByPageResponseBodyResponseBody()
+            self.response_body = temp_model.from_map(m['responseBody'])
+        return self
+
+
+class GetOutGroupsByPageResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: GetOutGroupsByPageResponseBody = None,
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
+            temp_model = GetOutGroupsByPageResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class GetOutsideAuditGroupMessageByPageHeaders(TeaModel):
     def __init__(
         self,
         common_headers: Dict[str, str] = None,
         x_acs_dingtalk_access_token: str = None,
     ):
         self.common_headers = common_headers
```

### Comparing `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/finance_1_0/client.py` & `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/finance_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/finance_1_0/models.py` & `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/finance_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/flashmeeting_1_0/client.py` & `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/flashmeeting_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/flashmeeting_1_0/models.py` & `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/flashmeeting_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/gateway_1_0/client.py` & `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/gateway_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/gateway_1_0/models.py` & `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/gateway_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/group_blackboard_1_0/client.py` & `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/group_blackboard_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/group_blackboard_1_0/models.py` & `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/wms_1_0/models.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*-
 # This file is auto-generated, don't edit it. Thanks.
 from Tea.model import TeaModel
-from typing import Dict
+from typing import Dict, List
 
 
-class CreateGroupBlackboardHeaders(TeaModel):
+class QueryGoodsListHeaders(TeaModel):
     def __init__(
         self,
         common_headers: Dict[str, str] = None,
         x_acs_dingtalk_access_token: str = None,
     ):
         self.common_headers = common_headers
         self.x_acs_dingtalk_access_token = x_acs_dingtalk_access_token
@@ -33,259 +33,204 @@
         if m.get('commonHeaders') is not None:
             self.common_headers = m.get('commonHeaders')
         if m.get('x-acs-dingtalk-access-token') is not None:
             self.x_acs_dingtalk_access_token = m.get('x-acs-dingtalk-access-token')
         return self
 
 
-class CreateGroupBlackboardRequest(TeaModel):
+class QueryGoodsListRequest(TeaModel):
     def __init__(
         self,
-        content: str = None,
-        open_conversation_id: str = None,
-        send_ding: bool = None,
-        sticky: bool = None,
-        unique_id: str = None,
-        user_id: str = None,
+        end_time_in_mills: int = None,
+        max_results: int = None,
+        next_token: int = None,
+        start_time_in_mills: int = None,
     ):
-        self.content = content
-        self.open_conversation_id = open_conversation_id
-        self.send_ding = send_ding
-        self.sticky = sticky
-        self.unique_id = unique_id
-        self.user_id = user_id
+        self.end_time_in_mills = end_time_in_mills
+        self.max_results = max_results
+        self.next_token = next_token
+        self.start_time_in_mills = start_time_in_mills
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.content is not None:
-            result['content'] = self.content
-        if self.open_conversation_id is not None:
-            result['openConversationId'] = self.open_conversation_id
-        if self.send_ding is not None:
-            result['sendDing'] = self.send_ding
-        if self.sticky is not None:
-            result['sticky'] = self.sticky
-        if self.unique_id is not None:
-            result['uniqueId'] = self.unique_id
-        if self.user_id is not None:
-            result['userId'] = self.user_id
+        if self.end_time_in_mills is not None:
+            result['endTimeInMills'] = self.end_time_in_mills
+        if self.max_results is not None:
+            result['maxResults'] = self.max_results
+        if self.next_token is not None:
+            result['nextToken'] = self.next_token
+        if self.start_time_in_mills is not None:
+            result['startTimeInMills'] = self.start_time_in_mills
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('content') is not None:
-            self.content = m.get('content')
-        if m.get('openConversationId') is not None:
-            self.open_conversation_id = m.get('openConversationId')
-        if m.get('sendDing') is not None:
-            self.send_ding = m.get('sendDing')
-        if m.get('sticky') is not None:
-            self.sticky = m.get('sticky')
-        if m.get('uniqueId') is not None:
-            self.unique_id = m.get('uniqueId')
-        if m.get('userId') is not None:
-            self.user_id = m.get('userId')
+        if m.get('endTimeInMills') is not None:
+            self.end_time_in_mills = m.get('endTimeInMills')
+        if m.get('maxResults') is not None:
+            self.max_results = m.get('maxResults')
+        if m.get('nextToken') is not None:
+            self.next_token = m.get('nextToken')
+        if m.get('startTimeInMills') is not None:
+            self.start_time_in_mills = m.get('startTimeInMills')
         return self
 
 
-class CreateGroupBlackboardResponseBody(TeaModel):
+class QueryGoodsListResponseBodyResultList(TeaModel):
     def __init__(
         self,
-        data_id: str = None,
-        success: bool = None,
+        goods_name: str = None,
+        goods_no: str = None,
+        instance_id: str = None,
+        product_specs: str = None,
+        unit: str = None,
     ):
-        self.data_id = data_id
-        self.success = success
+        self.goods_name = goods_name
+        self.goods_no = goods_no
+        self.instance_id = instance_id
+        self.product_specs = product_specs
+        self.unit = unit
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.data_id is not None:
-            result['dataId'] = self.data_id
-        if self.success is not None:
-            result['success'] = self.success
+        if self.goods_name is not None:
+            result['goodsName'] = self.goods_name
+        if self.goods_no is not None:
+            result['goodsNo'] = self.goods_no
+        if self.instance_id is not None:
+            result['instanceId'] = self.instance_id
+        if self.product_specs is not None:
+            result['productSpecs'] = self.product_specs
+        if self.unit is not None:
+            result['unit'] = self.unit
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('dataId') is not None:
-            self.data_id = m.get('dataId')
-        if m.get('success') is not None:
-            self.success = m.get('success')
+        if m.get('goodsName') is not None:
+            self.goods_name = m.get('goodsName')
+        if m.get('goodsNo') is not None:
+            self.goods_no = m.get('goodsNo')
+        if m.get('instanceId') is not None:
+            self.instance_id = m.get('instanceId')
+        if m.get('productSpecs') is not None:
+            self.product_specs = m.get('productSpecs')
+        if m.get('unit') is not None:
+            self.unit = m.get('unit')
         return self
 
 
-class CreateGroupBlackboardResponse(TeaModel):
+class QueryGoodsListResponseBodyResult(TeaModel):
     def __init__(
         self,
-        headers: Dict[str, str] = None,
-        status_code: int = None,
-        body: CreateGroupBlackboardResponseBody = None,
+        has_more: bool = None,
+        list: List[QueryGoodsListResponseBodyResultList] = None,
+        max_results: int = None,
+        next_token: str = None,
     ):
-        self.headers = headers
-        self.status_code = status_code
-        self.body = body
+        self.has_more = has_more
+        self.list = list
+        self.max_results = max_results
+        self.next_token = next_token
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
-        if self.body:
-            self.body.validate()
+        if self.list:
+            for k in self.list:
+                if k:
+                    k.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.headers is not None:
-            result['headers'] = self.headers
-        if self.status_code is not None:
-            result['statusCode'] = self.status_code
-        if self.body is not None:
-            result['body'] = self.body.to_map()
+        if self.has_more is not None:
+            result['hasMore'] = self.has_more
+        result['list'] = []
+        if self.list is not None:
+            for k in self.list:
+                result['list'].append(k.to_map() if k else None)
+        if self.max_results is not None:
+            result['maxResults'] = self.max_results
+        if self.next_token is not None:
+            result['nextToken'] = self.next_token
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('headers') is not None:
-            self.headers = m.get('headers')
-        if m.get('statusCode') is not None:
-            self.status_code = m.get('statusCode')
-        if m.get('body') is not None:
-            temp_model = CreateGroupBlackboardResponseBody()
-            self.body = temp_model.from_map(m['body'])
+        if m.get('hasMore') is not None:
+            self.has_more = m.get('hasMore')
+        self.list = []
+        if m.get('list') is not None:
+            for k in m.get('list'):
+                temp_model = QueryGoodsListResponseBodyResultList()
+                self.list.append(temp_model.from_map(k))
+        if m.get('maxResults') is not None:
+            self.max_results = m.get('maxResults')
+        if m.get('nextToken') is not None:
+            self.next_token = m.get('nextToken')
         return self
 
 
-class DeleteGroupBlackboardHeaders(TeaModel):
+class QueryGoodsListResponseBody(TeaModel):
     def __init__(
         self,
-        common_headers: Dict[str, str] = None,
-        x_acs_dingtalk_access_token: str = None,
-    ):
-        self.common_headers = common_headers
-        self.x_acs_dingtalk_access_token = x_acs_dingtalk_access_token
-
-    def validate(self):
-        pass
-
-    def to_map(self):
-        _map = super().to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.common_headers is not None:
-            result['commonHeaders'] = self.common_headers
-        if self.x_acs_dingtalk_access_token is not None:
-            result['x-acs-dingtalk-access-token'] = self.x_acs_dingtalk_access_token
-        return result
-
-    def from_map(self, m: dict = None):
-        m = m or dict()
-        if m.get('commonHeaders') is not None:
-            self.common_headers = m.get('commonHeaders')
-        if m.get('x-acs-dingtalk-access-token') is not None:
-            self.x_acs_dingtalk_access_token = m.get('x-acs-dingtalk-access-token')
-        return self
-
-
-class DeleteGroupBlackboardRequest(TeaModel):
-    def __init__(
-        self,
-        data_id: str = None,
-        open_conversation_id: str = None,
-        user_id: str = None,
-    ):
-        self.data_id = data_id
-        self.open_conversation_id = open_conversation_id
-        self.user_id = user_id
-
-    def validate(self):
-        pass
-
-    def to_map(self):
-        _map = super().to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.data_id is not None:
-            result['dataId'] = self.data_id
-        if self.open_conversation_id is not None:
-            result['openConversationId'] = self.open_conversation_id
-        if self.user_id is not None:
-            result['userId'] = self.user_id
-        return result
-
-    def from_map(self, m: dict = None):
-        m = m or dict()
-        if m.get('dataId') is not None:
-            self.data_id = m.get('dataId')
-        if m.get('openConversationId') is not None:
-            self.open_conversation_id = m.get('openConversationId')
-        if m.get('userId') is not None:
-            self.user_id = m.get('userId')
-        return self
-
-
-class DeleteGroupBlackboardResponseBody(TeaModel):
-    def __init__(
-        self,
-        is_deleted: bool = None,
+        result: QueryGoodsListResponseBodyResult = None,
         success: bool = None,
     ):
-        self.is_deleted = is_deleted
+        self.result = result
         self.success = success
 
     def validate(self):
-        pass
+        if self.result:
+            self.result.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.is_deleted is not None:
-            result['isDeleted'] = self.is_deleted
+        if self.result is not None:
+            result['result'] = self.result.to_map()
         if self.success is not None:
             result['success'] = self.success
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('isDeleted') is not None:
-            self.is_deleted = m.get('isDeleted')
+        if m.get('result') is not None:
+            temp_model = QueryGoodsListResponseBodyResult()
+            self.result = temp_model.from_map(m['result'])
         if m.get('success') is not None:
             self.success = m.get('success')
         return self
 
 
-class DeleteGroupBlackboardResponse(TeaModel):
+class QueryGoodsListResponse(TeaModel):
     def __init__(
         self,
         headers: Dict[str, str] = None,
         status_code: int = None,
-        body: DeleteGroupBlackboardResponseBody = None,
+        body: QueryGoodsListResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
@@ -311,12 +256,12 @@
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('headers') is not None:
             self.headers = m.get('headers')
         if m.get('statusCode') is not None:
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
-            temp_model = DeleteGroupBlackboardResponseBody()
+            temp_model = QueryGoodsListResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
```

### Comparing `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/h3yun_1_0/client.py` & `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/h3yun_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/h3yun_1_0/models.py` & `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/h3yun_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/h5package_1_0/client.py` & `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/h5package_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/h5package_1_0/models.py` & `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/h5package_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/hrbrain_1_0/client.py` & `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/hrbrain_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/hrbrain_1_0/models.py` & `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/hrbrain_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/hrm_1_0/client.py` & `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/hrm_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/hrm_1_0/models.py` & `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/hrm_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/im_1_0/client.py` & `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/im_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/im_1_0/models.py` & `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/im_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/im_2_0/client.py` & `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/im_2_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/im_2_0/models.py` & `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/im_2_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/impaas_1_0/client.py` & `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/impaas_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/impaas_1_0/models.py` & `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/impaas_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/industry_1_0/client.py` & `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/industry_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/industry_1_0/models.py` & `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/industry_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/jzcrm_1_0/client.py` & `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/jzcrm_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/jzcrm_1_0/models.py` & `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/jzcrm_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/link_1_0/client.py` & `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/link_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/link_1_0/models.py` & `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/link_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/live_1_0/client.py` & `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/live_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/live_1_0/models.py` & `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/live_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/manufacturing_1_0/client.py` & `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/manufacturing_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/manufacturing_1_0/models.py` & `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/manufacturing_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/micro_app_1_0/client.py` & `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/micro_app_1_0/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -333,14 +333,72 @@
         role_id: str,
         request: dingtalkmicro_app__1__0_models.AddMemberToAppRoleRequest,
     ) -> dingtalkmicro_app__1__0_models.AddMemberToAppRoleResponse:
         runtime = util_models.RuntimeOptions()
         headers = dingtalkmicro_app__1__0_models.AddMemberToAppRoleHeaders()
         return await self.add_member_to_app_role_with_options_async(agent_id, role_id, request, headers, runtime)
 
+    def anhei_pwith_options(
+        self,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> dingtalkmicro_app__1__0_models.AnheiPResponse:
+        req = open_api_models.OpenApiRequest(
+            headers=headers
+        )
+        params = open_api_models.Params(
+            action='AnheiP',
+            version='microApp_1.0',
+            protocol='HTTP',
+            pathname=f'/v1.0/microApp/anheiP',
+            method='GET',
+            auth_type='Anonymous',
+            style='ROA',
+            req_body_type='none',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dingtalkmicro_app__1__0_models.AnheiPResponse(),
+            self.execute(params, req, runtime)
+        )
+
+    async def anhei_pwith_options_async(
+        self,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> dingtalkmicro_app__1__0_models.AnheiPResponse:
+        req = open_api_models.OpenApiRequest(
+            headers=headers
+        )
+        params = open_api_models.Params(
+            action='AnheiP',
+            version='microApp_1.0',
+            protocol='HTTP',
+            pathname=f'/v1.0/microApp/anheiP',
+            method='GET',
+            auth_type='Anonymous',
+            style='ROA',
+            req_body_type='none',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dingtalkmicro_app__1__0_models.AnheiPResponse(),
+            await self.execute_async(params, req, runtime)
+        )
+
+    def anhei_p(self) -> dingtalkmicro_app__1__0_models.AnheiPResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.anhei_pwith_options(headers, runtime)
+
+    async def anhei_p_async(self) -> dingtalkmicro_app__1__0_models.AnheiPResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.anhei_pwith_options_async(headers, runtime)
+
     def anhei_test_888with_options(
         self,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> dingtalkmicro_app__1__0_models.AnheiTest888Response:
         req = open_api_models.OpenApiRequest(
             headers=headers
```

### Comparing `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/micro_app_1_0/models.py` & `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/micro_app_1_0/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -541,14 +541,85 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = AddMemberToAppRoleResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class AnheiPResponseBody(TeaModel):
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
+class AnheiPResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: AnheiPResponseBody = None,
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
+            temp_model = AnheiPResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class AnheiTest888ResponseBody(TeaModel):
     def __init__(
         self,
         request_id: str = None,
     ):
         self.request_id = request_id
```

### Comparing `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/miniapp_1_0/client.py` & `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/miniapp_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/miniapp_1_0/models.py` & `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/miniapp_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/oauth2_1_0/client.py` & `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/oauth2_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/oauth2_1_0/models.py` & `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/oauth2_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/occupationauth_1_0/client.py` & `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/occupationauth_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/occupationauth_1_0/models.py` & `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/occupationauth_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/okr_1_0/client.py` & `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/okr_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/okr_1_0/models.py` & `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/okr_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/org_culture_1_0/client.py` & `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/org_culture_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/org_culture_1_0/models.py` & `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/org_culture_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/package_1_0/client.py` & `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/package_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/package_1_0/models.py` & `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/package_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/pedia_1_0/client.py` & `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/pedia_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/pedia_1_0/models.py` & `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/pedia_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/project_1_0/client.py` & `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/project_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/project_1_0/models.py` & `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/project_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/project_integration_1_0/client.py` & `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/project_integration_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/project_integration_1_0/models.py` & `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/project_integration_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/rcs_call_1_0/client.py` & `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/rcs_call_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/rcs_call_1_0/models.py` & `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/rcs_call_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/resident_1_0/client.py` & `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/resident_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/resident_1_0/models.py` & `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/resident_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/robot_1_0/client.py` & `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/robot_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/robot_1_0/models.py` & `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/robot_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/rooms_1_0/client.py` & `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/rooms_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/rooms_1_0/models.py` & `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/rooms_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/search_1_0/client.py` & `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/search_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/search_1_0/models.py` & `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/search_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/service_group_1_0/client.py` & `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/service_group_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/service_group_1_0/models.py` & `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/service_group_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/smart_device_1_0/client.py` & `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/smart_device_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/smart_device_1_0/models.py` & `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/smart_device_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/sns_storage_1_0/client.py` & `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/sns_storage_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/sns_storage_1_0/models.py` & `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/sns_storage_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/storage_1_0/client.py` & `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/storage_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/storage_1_0/models.py` & `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/storage_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/storage_2_0/client.py` & `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/storage_2_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/storage_2_0/models.py` & `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/storage_2_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/swform_1_0/client.py` & `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/swform_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/swform_1_0/models.py` & `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/swform_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/todo_1_0/client.py` & `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/todo_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/todo_1_0/models.py` & `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/todo_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/trade_1_0/client.py` & `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/trade_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/trade_1_0/models.py` & `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/trade_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/trajectory_1_0/client.py` & `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/trajectory_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/trajectory_1_0/models.py` & `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/trajectory_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/transcribe_1_0/client.py` & `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/transcribe_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/transcribe_1_0/models.py` & `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/transcribe_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/trip_1_0/client.py` & `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/trip_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/trip_1_0/models.py` & `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/trip_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/village_1_0/client.py` & `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/village_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/village_1_0/models.py` & `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/village_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/watt_1_0/client.py` & `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/watt_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/watt_1_0/models.py` & `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/watt_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/wiki_1_0/client.py` & `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/wiki_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/wiki_1_0/models.py` & `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/wiki_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/wiki_2_0/client.py` & `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/wiki_2_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/wiki_2_0/models.py` & `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/wiki_2_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/wms_1_0/client.py` & `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/wms_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/workbench_1_0/client.py` & `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/workbench_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/workbench_1_0/models.py` & `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/workbench_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/workflow_1_0/client.py` & `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/workflow_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/workflow_1_0/models.py` & `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/workflow_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/workrecord_1_0/client.py` & `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/workrecord_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/workrecord_1_0/models.py` & `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/workrecord_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/yida_1_0/client.py` & `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/yida_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/yida_1_0/models.py` & `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/yida_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/yun_shu_1_0/client.py` & `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/yun_shu_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/yun_shu_1_0/models.py` & `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk/yun_shu_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk.egg-info/PKG-INFO` & `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-dingtalk
-Version: 2.0.18
+Version: 2.0.19
 Summary: Alibaba Cloud Dingtalk SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk.egg-info/SOURCES.txt` & `alibabacloud_dingtalk-2.0.19/alibabacloud_dingtalk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.18/setup.py` & `alibabacloud_dingtalk-2.0.19/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_dingtalk.
 
-Created on 31/05/2023
+Created on 09/06/2023
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_dingtalk"
 NAME = "alibabacloud_dingtalk" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud Dingtalk SDK Library for Python"
```

