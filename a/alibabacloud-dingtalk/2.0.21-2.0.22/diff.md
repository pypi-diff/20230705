# Comparing `tmp/alibabacloud_dingtalk-2.0.21.tar.gz` & `tmp/alibabacloud_dingtalk-2.0.22.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_dingtalk-2.0.21.tar", last modified: Fri Jun 16 07:09:03 2023, max compression
+gzip compressed data, was "dist/alibabacloud_dingtalk-2.0.22.tar", last modified: Wed Jul  5 01:54:58 2023, max compression
```

## Comparing `alibabacloud_dingtalk-2.0.21.tar` & `alibabacloud_dingtalk-2.0.22.tar`

### file list

```diff
@@ -1,373 +1,377 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 07:09:03.000000 alibabacloud_dingtalk-2.0.21/
--rw-r--r--   0 root         (0) root         (0)    20012 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2309 2023-06-16 07:09:03.000000 alibabacloud_dingtalk-2.0.21/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1021 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1106 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 07:09:03.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 07:09:03.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/activity_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/activity_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8552 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/activity_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    15385 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/activity_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 07:09:03.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/algo_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/algo_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9980 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/algo_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    23314 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/algo_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 07:09:03.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/alitrip_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/alitrip_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    58254 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/alitrip_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   169621 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/alitrip_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 07:09:03.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/apaas_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/apaas_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    25166 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/apaas_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    46194 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/apaas_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 07:09:03.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/app_market_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/app_market_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    25682 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/app_market_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    27728 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/app_market_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 07:09:03.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/ats_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/ats_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    90648 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/ats_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   138912 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/ats_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 07:09:03.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/attendance_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/attendance_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   165948 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/attendance_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   323041 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/attendance_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 07:09:03.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/badge_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/badge_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    45240 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/badge_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    62246 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/badge_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 07:09:03.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/bizfinance_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/bizfinance_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   202090 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/bizfinance_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   571964 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/bizfinance_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 07:09:03.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/blackboard_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/blackboard_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4942 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/blackboard_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     3871 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/blackboard_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 07:09:03.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/calendar_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/calendar_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   139370 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/calendar_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   341471 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/calendar_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 07:09:03.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/carbon_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/carbon_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    27976 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/carbon_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    42229 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/carbon_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 07:09:03.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/card_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/card_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    35138 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/card_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   101075 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/card_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 07:09:03.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/check_in_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/check_in_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6044 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/check_in_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    10446 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/check_in_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 07:09:03.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/chengfeng_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/chengfeng_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    71632 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/chengfeng_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   123179 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/chengfeng_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 07:09:03.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/conference_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/conference_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   108908 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/conference_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   152805 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/conference_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 07:09:03.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/connector_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/connector_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    58616 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/connector_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   124904 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/connector_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 07:09:03.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/contact_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/contact_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   297108 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/contact_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   392984 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/contact_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 07:09:03.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/content_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/content_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    21270 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/content_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    42332 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/content_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 07:09:03.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/contract_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/contract_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    19674 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/contract_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    27526 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/contract_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 07:09:03.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/conv_file_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/conv_file_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    17934 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/conv_file_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    30852 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/conv_file_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 07:09:03.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/crm_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/crm_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   223914 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/crm_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   552073 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/crm_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 07:09:03.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/crm_2_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/crm_2_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4810 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/crm_2_0/client.py
--rw-r--r--   0 root         (0) root         (0)     7385 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/crm_2_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 07:09:03.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/customer_service_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/customer_service_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    32170 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/customer_service_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    46898 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/customer_service_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 07:09:03.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/datacenter_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/datacenter_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   391978 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/datacenter_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   515455 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/datacenter_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 07:09:03.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/devicemng_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/devicemng_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   112278 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/devicemng_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   152480 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/devicemng_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 07:09:03.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/ding_phone_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/ding_phone_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13874 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/ding_phone_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    16265 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/ding_phone_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 07:09:03.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/dingmi_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/dingmi_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    56946 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/dingmi_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    56301 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/dingmi_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 07:09:03.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/diot_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/diot_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    52941 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/diot_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    71864 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/diot_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 07:09:03.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/doc_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/doc_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   211006 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/doc_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   267473 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/doc_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 07:09:03.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/doc_2_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/doc_2_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   150160 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/doc_2_0/client.py
--rw-r--r--   0 root         (0) root         (0)   269351 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/doc_2_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 07:09:03.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/drive_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/drive_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   140210 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/drive_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   195538 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/drive_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 07:09:03.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/edu_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/edu_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   472940 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/edu_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   731141 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/edu_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 07:09:03.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/esign_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/esign_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    72708 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/esign_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   116546 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/esign_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 07:09:03.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/esign_2_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/esign_2_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    86294 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/esign_2_0/client.py
--rw-r--r--   0 root         (0) root         (0)   123749 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/esign_2_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 07:09:03.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/event_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/event_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5096 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/event_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     6148 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/event_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 07:09:03.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/exclusive_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/exclusive_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   316592 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/exclusive_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   439557 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/exclusive_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 07:09:03.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/finance_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/finance_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   155788 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/finance_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   302125 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/finance_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 07:09:03.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/flashmeeting_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/flashmeeting_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13914 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/flashmeeting_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    21540 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/flashmeeting_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 07:09:03.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/gateway_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/gateway_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4633 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/gateway_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     4901 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/gateway_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 07:09:03.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/group_blackboard_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/group_blackboard_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10562 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/group_blackboard_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     9742 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/group_blackboard_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 07:09:03.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/h3yun_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/h3yun_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    80133 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/h3yun_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   138362 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/h3yun_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 07:09:03.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/h5package_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/h5package_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    17059 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/h5package_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    18903 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/h5package_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 07:09:03.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/hrbrain_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/hrbrain_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5382 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/hrbrain_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     4660 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/hrbrain_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 07:09:03.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/hrm_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/hrm_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    92926 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/hrm_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   137528 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/hrm_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 07:09:03.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/im_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/im_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   302532 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/im_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   378971 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/im_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 07:09:03.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/im_2_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/im_2_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    22430 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/im_2_0/client.py
--rw-r--r--   0 root         (0) root         (0)    31875 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/im_2_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 07:09:03.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/impaas_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/impaas_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    90230 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/impaas_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    92472 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/impaas_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 07:09:03.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/industry_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/industry_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   610684 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/industry_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   859772 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/industry_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 07:09:03.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/jzcrm_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/jzcrm_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    62348 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/jzcrm_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   155140 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/jzcrm_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 07:09:03.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/link_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/link_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    63194 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/link_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   108695 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/link_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 07:09:03.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/live_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/live_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    91118 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/live_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   135110 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/live_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 07:09:03.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/manufacturing_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/manufacturing_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    16181 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/manufacturing_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    23076 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/manufacturing_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 07:09:03.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/micro_app_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/micro_app_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   146899 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/micro_app_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   175146 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/micro_app_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 07:09:03.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/miniapp_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/miniapp_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    52227 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/miniapp_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    54521 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/miniapp_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 07:09:03.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/oauth2_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/oauth2_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    31076 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/oauth2_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    40802 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/oauth2_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 07:09:03.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/occupationauth_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/occupationauth_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8962 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/occupationauth_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     7507 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/occupationauth_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 07:09:03.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/okr_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/okr_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    76720 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/okr_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   137701 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/okr_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 07:09:03.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/org_culture_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/org_culture_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    77488 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/org_culture_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   123420 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/org_culture_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 07:09:03.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/package_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/package_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    56344 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/package_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    60347 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/package_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 07:09:03.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/pedia_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/pedia_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    29226 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/pedia_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    69069 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/pedia_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 07:09:03.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/project_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/project_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   264898 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/project_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   418571 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/project_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 07:09:03.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/project_integration_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/project_integration_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    17983 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/project_integration_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    11593 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/project_integration_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 07:09:03.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/rcs_call_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/rcs_call_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5368 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/rcs_call_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     4579 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/rcs_call_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 07:09:03.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/resident_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/resident_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   135300 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/resident_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   174524 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/resident_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 07:09:03.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/robot_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/robot_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    81780 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/robot_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    93746 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/robot_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 07:09:03.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/rooms_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/rooms_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    56986 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/rooms_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    83842 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/rooms_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 07:09:03.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/search_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/search_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    39248 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/search_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    46018 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/search_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 07:09:03.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/service_group_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/service_group_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   361006 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/service_group_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   503423 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/service_group_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 07:09:03.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/smart_device_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/smart_device_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    31508 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/smart_device_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    26678 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/smart_device_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 07:09:03.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/sns_storage_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/sns_storage_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    44726 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/sns_storage_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    96217 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/sns_storage_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 07:09:03.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/storage_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/storage_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   187612 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/storage_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   353698 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/storage_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 07:09:03.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/storage_2_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/storage_2_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    53470 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/storage_2_0/client.py
--rw-r--r--   0 root         (0) root         (0)    89290 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/storage_2_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 07:09:03.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/swform_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/swform_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13910 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/swform_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    28559 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/swform_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 07:09:03.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/todo_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/todo_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    65344 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/todo_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   148231 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/todo_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 07:09:03.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/trade_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/trade_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14284 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/trade_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    16170 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/trade_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 07:09:03.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/trajectory_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/trajectory_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14192 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/trajectory_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    21677 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/trajectory_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 07:09:03.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/transcribe_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/transcribe_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13676 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/transcribe_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    17519 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/transcribe_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 07:09:03.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/trip_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/trip_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    18718 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/trip_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    32237 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/trip_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 07:09:03.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/village_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/village_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    75904 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/village_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   110849 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/village_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 07:09:03.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/watt_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/watt_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4269 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/watt_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     3363 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/watt_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 07:09:03.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/wiki_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/wiki_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8278 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/wiki_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    20486 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/wiki_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 07:09:03.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/wiki_2_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/wiki_2_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    66210 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/wiki_2_0/client.py
--rw-r--r--   0 root         (0) root         (0)   130783 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/wiki_2_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 07:09:03.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/wms_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/wms_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5370 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/wms_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     8325 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/wms_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 07:09:03.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/workbench_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/workbench_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    27686 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/workbench_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    29689 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/workbench_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 07:09:03.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/workflow_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/workflow_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   179772 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/workflow_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   377816 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/workflow_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 07:09:03.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/workrecord_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/workrecord_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4774 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/workrecord_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     3772 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/workrecord_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 07:09:03.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/yida_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/yida_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   464194 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/yida_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   687148 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/yida_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 07:09:03.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/yun_shu_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/yun_shu_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5452 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/yun_shu_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     4490 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/yun_shu_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 07:09:03.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2309 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    12294 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      239 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-06-16 07:09:03.000000 alibabacloud_dingtalk-2.0.21/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2684 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/
+-rw-r--r--   0 root         (0) root         (0)    20077 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2309 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1021 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1106 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/activity_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/activity_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8552 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/activity_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    15385 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/activity_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/algo_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/algo_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9980 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/algo_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    23314 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/algo_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/alitrip_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/alitrip_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    58254 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/alitrip_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   169621 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/alitrip_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/apaas_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/apaas_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    25166 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/apaas_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    46194 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/apaas_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/app_market_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/app_market_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    25682 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/app_market_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    27728 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/app_market_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/ats_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/ats_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    90914 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/ats_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   139242 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/ats_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/attendance_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/attendance_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   165948 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/attendance_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   323041 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/attendance_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/badge_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/badge_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    45240 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/badge_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    62246 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/badge_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/bizfinance_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/bizfinance_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   202090 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/bizfinance_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   575598 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/bizfinance_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/blackboard_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/blackboard_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9614 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/blackboard_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    10132 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/blackboard_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/calendar_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/calendar_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   142048 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/calendar_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   346941 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/calendar_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/carbon_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/carbon_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    27976 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/carbon_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    42229 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/carbon_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/card_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/card_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    35138 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/card_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   101075 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/card_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/check_in_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/check_in_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6044 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/check_in_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    10446 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/check_in_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/chengfeng_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/chengfeng_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    71632 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/chengfeng_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   123179 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/chengfeng_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/conference_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/conference_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   126888 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/conference_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   172646 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/conference_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/connector_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/connector_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    58616 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/connector_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   124904 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/connector_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/contact_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/contact_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   297108 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/contact_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   392984 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/contact_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/content_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/content_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    21270 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/content_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    42332 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/content_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/contract_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/contract_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    19674 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/contract_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    27526 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/contract_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/conv_file_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/conv_file_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    17934 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/conv_file_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    30852 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/conv_file_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/crm_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/crm_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   223914 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/crm_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   552073 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/crm_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/crm_2_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/crm_2_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4810 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/crm_2_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     7385 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/crm_2_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/customer_service_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/customer_service_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    32170 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/customer_service_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    46898 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/customer_service_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/datacenter_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/datacenter_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   391978 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/datacenter_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   515455 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/datacenter_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/devicemng_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/devicemng_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   112278 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/devicemng_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   152480 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/devicemng_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/ding_phone_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/ding_phone_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13874 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/ding_phone_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    16265 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/ding_phone_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/dingmi_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/dingmi_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    56946 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/dingmi_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    56301 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/dingmi_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/diot_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/diot_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    52941 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/diot_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    71831 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/diot_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/doc_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/doc_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   219916 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/doc_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   278738 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/doc_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/doc_2_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/doc_2_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   150160 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/doc_2_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   269893 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/doc_2_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/drive_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/drive_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   140210 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/drive_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   195538 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/drive_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/edu_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/edu_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   472940 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/edu_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   731141 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/edu_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/esign_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/esign_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    72708 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/esign_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   116546 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/esign_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/esign_2_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/esign_2_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    86294 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/esign_2_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   123749 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/esign_2_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/event_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/event_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8259 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/event_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     8976 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/event_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/exclusive_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/exclusive_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   316592 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/exclusive_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   439557 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/exclusive_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/finance_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/finance_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   155788 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/finance_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   302125 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/finance_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/flashmeeting_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/flashmeeting_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13914 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/flashmeeting_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    21801 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/flashmeeting_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/gateway_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/gateway_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4633 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/gateway_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     4901 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/gateway_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/group_blackboard_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/group_blackboard_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10562 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/group_blackboard_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     9742 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/group_blackboard_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/h3yun_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/h3yun_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    80133 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/h3yun_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   138362 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/h3yun_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/h5package_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/h5package_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    17059 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/h5package_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    18903 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/h5package_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/hrbrain_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/hrbrain_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5382 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/hrbrain_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     4660 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/hrbrain_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/hrm_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/hrm_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    92926 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/hrm_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   137528 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/hrm_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/im_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/im_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   302740 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/im_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   379213 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/im_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/im_2_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/im_2_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    22430 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/im_2_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    31875 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/im_2_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/impaas_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/impaas_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    90230 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/impaas_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    92472 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/impaas_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/industry_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/industry_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   610684 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/industry_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   859772 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/industry_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/jzcrm_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/jzcrm_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    62348 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/jzcrm_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   155140 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/jzcrm_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/link_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/link_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    63194 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/link_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   108695 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/link_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/live_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/live_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    91118 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/live_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   135110 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/live_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/live_activities_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/live_activities_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5464 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/live_activities_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     7253 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/live_activities_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/manufacturing_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/manufacturing_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    16181 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/manufacturing_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    23076 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/manufacturing_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/micro_app_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/micro_app_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   148979 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/micro_app_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   177099 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/micro_app_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/miniapp_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/miniapp_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    52227 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/miniapp_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    54521 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/miniapp_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/oauth2_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/oauth2_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    31076 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/oauth2_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    40802 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/oauth2_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/occupationauth_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/occupationauth_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8962 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/occupationauth_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     7507 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/occupationauth_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/okr_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/okr_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    76720 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/okr_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   137701 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/okr_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/org_culture_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/org_culture_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    77488 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/org_culture_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   123420 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/org_culture_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/package_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/package_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    56344 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/package_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    60347 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/package_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/pedia_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/pedia_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    29226 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/pedia_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    69069 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/pedia_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/project_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/project_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   264898 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/project_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   419073 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/project_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/project_integration_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/project_integration_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    17983 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/project_integration_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    11593 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/project_integration_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/rcs_call_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/rcs_call_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5368 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/rcs_call_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     4579 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/rcs_call_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/resident_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/resident_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   135300 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/resident_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   174524 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/resident_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/robot_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/robot_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    81780 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/robot_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    93746 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/robot_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/rooms_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/rooms_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    56986 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/rooms_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    83842 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/rooms_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/search_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/search_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    39248 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/search_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    46018 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/search_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/service_group_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/service_group_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   361006 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/service_group_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   503423 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/service_group_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/smart_device_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/smart_device_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    31508 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/smart_device_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    26678 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/smart_device_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/sns_storage_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/sns_storage_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    44726 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/sns_storage_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    96217 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/sns_storage_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/storage_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/storage_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   187612 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/storage_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   353698 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/storage_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/storage_2_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/storage_2_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    53470 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/storage_2_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    89290 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/storage_2_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/swform_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/swform_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13910 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/swform_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    28559 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/swform_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/todo_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/todo_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    65344 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/todo_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   148231 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/todo_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/trade_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/trade_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14284 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/trade_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    16170 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/trade_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/trajectory_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/trajectory_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14192 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/trajectory_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    21677 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/trajectory_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/transcribe_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/transcribe_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13676 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/transcribe_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    17519 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/transcribe_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/trip_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/trip_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    18718 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/trip_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    32237 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/trip_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/village_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/village_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    75904 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/village_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   110849 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/village_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/watt_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/watt_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4269 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/watt_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     3363 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/watt_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/wiki_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/wiki_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8278 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/wiki_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    20486 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/wiki_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/wiki_2_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/wiki_2_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    66210 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/wiki_2_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   130783 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/wiki_2_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/wms_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/wms_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5370 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/wms_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     8325 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/wms_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/workbench_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/workbench_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    32014 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/workbench_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    34941 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/workbench_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/workflow_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/workflow_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   179772 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/workflow_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   377816 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/workflow_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/workrecord_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/workrecord_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4774 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/workrecord_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     3772 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/workrecord_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/yida_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/yida_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   464194 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/yida_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   687148 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/yida_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/yun_shu_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/yun_shu_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5452 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/yun_shu_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     4490 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/yun_shu_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2309 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    12452 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      239 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2684 2023-07-05 01:54:58.000000 alibabacloud_dingtalk-2.0.22/setup.py
```

### Comparing `alibabacloud_dingtalk-2.0.21/ChangeLog.md` & `alibabacloud_dingtalk-2.0.22/ChangeLog.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+2023-06-16 Version: 2.0.21
+- Update AddOfficialAccountFollower.
+
 2023-06-13 Version: 2.0.20
 - Update AddOfficialAccountFollower.
 
 2023-06-09 Version: 2.0.19
 - Update AddOfficialAccountFollower.
 
 2023-05-31 Version: 2.0.18
```

### Comparing `alibabacloud_dingtalk-2.0.21/LICENSE` & `alibabacloud_dingtalk-2.0.22/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.21/PKG-INFO` & `alibabacloud_dingtalk-2.0.22/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_dingtalk
-Version: 2.0.21
+Version: 2.0.22
 Summary: Alibaba Cloud Dingtalk SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_dingtalk-2.0.21/README-CN.md` & `alibabacloud_dingtalk-2.0.22/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.21/README.md` & `alibabacloud_dingtalk-2.0.22/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/activity_1_0/client.py` & `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/activity_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/activity_1_0/models.py` & `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/activity_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/algo_1_0/client.py` & `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/algo_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/algo_1_0/models.py` & `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/algo_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/alitrip_1_0/client.py` & `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/alitrip_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/alitrip_1_0/models.py` & `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/alitrip_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/apaas_1_0/client.py` & `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/apaas_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/apaas_1_0/models.py` & `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/apaas_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/app_market_1_0/client.py` & `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/app_market_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/app_market_1_0/models.py` & `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/app_market_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/ats_1_0/client.py` & `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/ats_1_0/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -600,14 +600,16 @@
         body = {}
         if not UtilClient.is_unset(request.channel_code):
             body['channelCode'] = request.channel_code
         if not UtilClient.is_unset(request.deliver_job_id):
             body['deliverJobId'] = request.deliver_job_id
         if not UtilClient.is_unset(request.from_mail_address):
             body['fromMailAddress'] = request.from_mail_address
+        if not UtilClient.is_unset(request.history_mail_import):
+            body['historyMailImport'] = request.history_mail_import
         if not UtilClient.is_unset(request.mail_id):
             body['mailId'] = request.mail_id
         if not UtilClient.is_unset(request.mail_title):
             body['mailTitle'] = request.mail_title
         if not UtilClient.is_unset(request.opt_user_id):
             body['optUserId'] = request.opt_user_id
         if not UtilClient.is_unset(request.receive_mail_address):
@@ -659,14 +661,16 @@
         body = {}
         if not UtilClient.is_unset(request.channel_code):
             body['channelCode'] = request.channel_code
         if not UtilClient.is_unset(request.deliver_job_id):
             body['deliverJobId'] = request.deliver_job_id
         if not UtilClient.is_unset(request.from_mail_address):
             body['fromMailAddress'] = request.from_mail_address
+        if not UtilClient.is_unset(request.history_mail_import):
+            body['historyMailImport'] = request.history_mail_import
         if not UtilClient.is_unset(request.mail_id):
             body['mailId'] = request.mail_id
         if not UtilClient.is_unset(request.mail_title):
             body['mailTitle'] = request.mail_title
         if not UtilClient.is_unset(request.opt_user_id):
             body['optUserId'] = request.opt_user_id
         if not UtilClient.is_unset(request.receive_mail_address):
```

### Comparing `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/ats_1_0/models.py` & `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/ats_1_0/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -1870,27 +1870,29 @@
 class CollectResumeMailRequest(TeaModel):
     def __init__(
         self,
         biz_code: str = None,
         channel_code: str = None,
         deliver_job_id: str = None,
         from_mail_address: str = None,
+        history_mail_import: bool = None,
         mail_id: str = None,
         mail_title: str = None,
         opt_user_id: str = None,
         receive_mail_address: str = None,
         receive_mail_type: int = None,
         received_time: int = None,
         resume_channel_url: str = None,
         resume_file: CollectResumeMailRequestResumeFile = None,
     ):
         self.biz_code = biz_code
         self.channel_code = channel_code
         self.deliver_job_id = deliver_job_id
         self.from_mail_address = from_mail_address
+        self.history_mail_import = history_mail_import
         self.mail_id = mail_id
         self.mail_title = mail_title
         self.opt_user_id = opt_user_id
         self.receive_mail_address = receive_mail_address
         self.receive_mail_type = receive_mail_type
         self.received_time = received_time
         self.resume_channel_url = resume_channel_url
@@ -1910,14 +1912,16 @@
             result['bizCode'] = self.biz_code
         if self.channel_code is not None:
             result['channelCode'] = self.channel_code
         if self.deliver_job_id is not None:
             result['deliverJobId'] = self.deliver_job_id
         if self.from_mail_address is not None:
             result['fromMailAddress'] = self.from_mail_address
+        if self.history_mail_import is not None:
+            result['historyMailImport'] = self.history_mail_import
         if self.mail_id is not None:
             result['mailId'] = self.mail_id
         if self.mail_title is not None:
             result['mailTitle'] = self.mail_title
         if self.opt_user_id is not None:
             result['optUserId'] = self.opt_user_id
         if self.receive_mail_address is not None:
@@ -1938,14 +1942,16 @@
             self.biz_code = m.get('bizCode')
         if m.get('channelCode') is not None:
             self.channel_code = m.get('channelCode')
         if m.get('deliverJobId') is not None:
             self.deliver_job_id = m.get('deliverJobId')
         if m.get('fromMailAddress') is not None:
             self.from_mail_address = m.get('fromMailAddress')
+        if m.get('historyMailImport') is not None:
+            self.history_mail_import = m.get('historyMailImport')
         if m.get('mailId') is not None:
             self.mail_id = m.get('mailId')
         if m.get('mailTitle') is not None:
             self.mail_title = m.get('mailTitle')
         if m.get('optUserId') is not None:
             self.opt_user_id = m.get('optUserId')
         if m.get('receiveMailAddress') is not None:
```

### Comparing `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/attendance_1_0/client.py` & `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/attendance_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/attendance_1_0/models.py` & `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/attendance_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/badge_1_0/client.py` & `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/badge_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/badge_1_0/models.py` & `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/badge_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/bizfinance_1_0/client.py` & `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/bizfinance_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/bizfinance_1_0/models.py` & `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/bizfinance_1_0/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -8892,44 +8892,92 @@
         if m.get('invoiceKeyVOList') is not None:
             for k in m.get('invoiceKeyVOList'):
                 temp_model = UnbindApplyReceiptAndInvoiceRelatedResponseBodyBatchUpdateInvoiceResponseInvoiceKeyVOList()
                 self.invoice_key_volist.append(temp_model.from_map(k))
         return self
 
 
+class UnbindApplyReceiptAndInvoiceRelatedResponseBodyErrorInvoiceKeyVOList(TeaModel):
+    def __init__(
+        self,
+        invoice_code: str = None,
+        invoice_no: str = None,
+    ):
+        self.invoice_code = invoice_code
+        self.invoice_no = invoice_no
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
+        if self.invoice_code is not None:
+            result['invoiceCode'] = self.invoice_code
+        if self.invoice_no is not None:
+            result['invoiceNo'] = self.invoice_no
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('invoiceCode') is not None:
+            self.invoice_code = m.get('invoiceCode')
+        if m.get('invoiceNo') is not None:
+            self.invoice_no = m.get('invoiceNo')
+        return self
+
+
 class UnbindApplyReceiptAndInvoiceRelatedResponseBody(TeaModel):
     def __init__(
         self,
         batch_update_invoice_response: UnbindApplyReceiptAndInvoiceRelatedResponseBodyBatchUpdateInvoiceResponse = None,
+        error_invoice_key_volist: List[UnbindApplyReceiptAndInvoiceRelatedResponseBodyErrorInvoiceKeyVOList] = None,
         success: bool = None,
     ):
         self.batch_update_invoice_response = batch_update_invoice_response
+        self.error_invoice_key_volist = error_invoice_key_volist
         self.success = success
 
     def validate(self):
         if self.batch_update_invoice_response:
             self.batch_update_invoice_response.validate()
+        if self.error_invoice_key_volist:
+            for k in self.error_invoice_key_volist:
+                if k:
+                    k.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.batch_update_invoice_response is not None:
             result['batchUpdateInvoiceResponse'] = self.batch_update_invoice_response.to_map()
+        result['errorInvoiceKeyVOList'] = []
+        if self.error_invoice_key_volist is not None:
+            for k in self.error_invoice_key_volist:
+                result['errorInvoiceKeyVOList'].append(k.to_map() if k else None)
         if self.success is not None:
             result['success'] = self.success
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('batchUpdateInvoiceResponse') is not None:
             temp_model = UnbindApplyReceiptAndInvoiceRelatedResponseBodyBatchUpdateInvoiceResponse()
             self.batch_update_invoice_response = temp_model.from_map(m['batchUpdateInvoiceResponse'])
+        self.error_invoice_key_volist = []
+        if m.get('errorInvoiceKeyVOList') is not None:
+            for k in m.get('errorInvoiceKeyVOList'):
+                temp_model = UnbindApplyReceiptAndInvoiceRelatedResponseBodyErrorInvoiceKeyVOList()
+                self.error_invoice_key_volist.append(temp_model.from_map(k))
         if m.get('success') is not None:
             self.success = m.get('success')
         return self
 
 
 class UnbindApplyReceiptAndInvoiceRelatedResponse(TeaModel):
     def __init__(
@@ -9829,44 +9877,92 @@
         if m.get('invoiceKeyVOList') is not None:
             for k in m.get('invoiceKeyVOList'):
                 temp_model = UpdateApplyReceiptAndInvoiceRelatedResponseBodyBatchUpdateInvoiceResponseInvoiceKeyVOList()
                 self.invoice_key_volist.append(temp_model.from_map(k))
         return self
 
 
+class UpdateApplyReceiptAndInvoiceRelatedResponseBodyErrorInvoiceKeyVOList(TeaModel):
+    def __init__(
+        self,
+        invoice_code: str = None,
+        invoice_no: str = None,
+    ):
+        self.invoice_code = invoice_code
+        self.invoice_no = invoice_no
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
+        if self.invoice_code is not None:
+            result['invoiceCode'] = self.invoice_code
+        if self.invoice_no is not None:
+            result['invoiceNo'] = self.invoice_no
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('invoiceCode') is not None:
+            self.invoice_code = m.get('invoiceCode')
+        if m.get('invoiceNo') is not None:
+            self.invoice_no = m.get('invoiceNo')
+        return self
+
+
 class UpdateApplyReceiptAndInvoiceRelatedResponseBody(TeaModel):
     def __init__(
         self,
         batch_update_invoice_response: UpdateApplyReceiptAndInvoiceRelatedResponseBodyBatchUpdateInvoiceResponse = None,
+        error_invoice_key_volist: List[UpdateApplyReceiptAndInvoiceRelatedResponseBodyErrorInvoiceKeyVOList] = None,
         success: bool = None,
     ):
         self.batch_update_invoice_response = batch_update_invoice_response
+        self.error_invoice_key_volist = error_invoice_key_volist
         self.success = success
 
     def validate(self):
         if self.batch_update_invoice_response:
             self.batch_update_invoice_response.validate()
+        if self.error_invoice_key_volist:
+            for k in self.error_invoice_key_volist:
+                if k:
+                    k.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.batch_update_invoice_response is not None:
             result['batchUpdateInvoiceResponse'] = self.batch_update_invoice_response.to_map()
+        result['errorInvoiceKeyVOList'] = []
+        if self.error_invoice_key_volist is not None:
+            for k in self.error_invoice_key_volist:
+                result['errorInvoiceKeyVOList'].append(k.to_map() if k else None)
         if self.success is not None:
             result['success'] = self.success
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('batchUpdateInvoiceResponse') is not None:
             temp_model = UpdateApplyReceiptAndInvoiceRelatedResponseBodyBatchUpdateInvoiceResponse()
             self.batch_update_invoice_response = temp_model.from_map(m['batchUpdateInvoiceResponse'])
+        self.error_invoice_key_volist = []
+        if m.get('errorInvoiceKeyVOList') is not None:
+            for k in m.get('errorInvoiceKeyVOList'):
+                temp_model = UpdateApplyReceiptAndInvoiceRelatedResponseBodyErrorInvoiceKeyVOList()
+                self.error_invoice_key_volist.append(temp_model.from_map(k))
         if m.get('success') is not None:
             self.success = m.get('success')
         return self
 
 
 class UpdateApplyReceiptAndInvoiceRelatedResponse(TeaModel):
     def __init__(
```

### Comparing `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/blackboard_1_0/client.py` & `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/wms_1_0/client.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from Tea.core import TeaCore
 
 from alibabacloud_gateway_spi.client import Client as SPIClient
 from alibabacloud_tea_openapi.client import Client as OpenApiClient
 from alibabacloud_tea_openapi import models as open_api_models
 from alibabacloud_gateway_dingtalk.client import Client as GatewayClientClient
 from alibabacloud_tea_util.client import Client as UtilClient
-from alibabacloud_dingtalk.blackboard_1_0 import models as dingtalkblackboard__1__0_models
+from alibabacloud_dingtalk.wms_1_0 import models as dingtalkwms__1__0_models
 from alibabacloud_tea_util import models as util_models
 from alibabacloud_openapi_util.client import Client as OpenApiUtilClient
 
 
 class Client(OpenApiClient):
     """
     *\
@@ -25,92 +25,104 @@
         super().__init__(config)
         self._client = GatewayClientClient()
         self._spi = self._client
         self._endpoint_rule = ''
         if UtilClient.empty(self._endpoint):
             self._endpoint = 'api.dingtalk.com'
 
-    def query_blackboard_space_with_options(
+    def query_goods_list_with_options(
         self,
-        request: dingtalkblackboard__1__0_models.QueryBlackboardSpaceRequest,
-        headers: dingtalkblackboard__1__0_models.QueryBlackboardSpaceHeaders,
+        request: dingtalkwms__1__0_models.QueryGoodsListRequest,
+        headers: dingtalkwms__1__0_models.QueryGoodsListHeaders,
         runtime: util_models.RuntimeOptions,
-    ) -> dingtalkblackboard__1__0_models.QueryBlackboardSpaceResponse:
+    ) -> dingtalkwms__1__0_models.QueryGoodsListResponse:
         UtilClient.validate_model(request)
         query = {}
-        if not UtilClient.is_unset(request.operation_user_id):
-            query['operationUserId'] = request.operation_user_id
+        if not UtilClient.is_unset(request.end_time_in_mills):
+            query['endTimeInMills'] = request.end_time_in_mills
+        if not UtilClient.is_unset(request.max_results):
+            query['maxResults'] = request.max_results
+        if not UtilClient.is_unset(request.next_token):
+            query['nextToken'] = request.next_token
+        if not UtilClient.is_unset(request.start_time_in_mills):
+            query['startTimeInMills'] = request.start_time_in_mills
         real_headers = {}
         if not UtilClient.is_unset(headers.common_headers):
             real_headers = headers.common_headers
         if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
             real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
         req = open_api_models.OpenApiRequest(
             headers=real_headers,
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
-            action='QueryBlackboardSpace',
-            version='blackboard_1.0',
+            action='QueryGoodsList',
+            version='wms_1.0',
             protocol='HTTP',
-            pathname=f'/v1.0/blackboard/spaces',
+            pathname=f'/v1.0/wms/goods',
             method='GET',
             auth_type='AK',
             style='ROA',
             req_body_type='none',
             body_type='json'
         )
         return TeaCore.from_map(
-            dingtalkblackboard__1__0_models.QueryBlackboardSpaceResponse(),
+            dingtalkwms__1__0_models.QueryGoodsListResponse(),
             self.execute(params, req, runtime)
         )
 
-    async def query_blackboard_space_with_options_async(
+    async def query_goods_list_with_options_async(
         self,
-        request: dingtalkblackboard__1__0_models.QueryBlackboardSpaceRequest,
-        headers: dingtalkblackboard__1__0_models.QueryBlackboardSpaceHeaders,
+        request: dingtalkwms__1__0_models.QueryGoodsListRequest,
+        headers: dingtalkwms__1__0_models.QueryGoodsListHeaders,
         runtime: util_models.RuntimeOptions,
-    ) -> dingtalkblackboard__1__0_models.QueryBlackboardSpaceResponse:
+    ) -> dingtalkwms__1__0_models.QueryGoodsListResponse:
         UtilClient.validate_model(request)
         query = {}
-        if not UtilClient.is_unset(request.operation_user_id):
-            query['operationUserId'] = request.operation_user_id
+        if not UtilClient.is_unset(request.end_time_in_mills):
+            query['endTimeInMills'] = request.end_time_in_mills
+        if not UtilClient.is_unset(request.max_results):
+            query['maxResults'] = request.max_results
+        if not UtilClient.is_unset(request.next_token):
+            query['nextToken'] = request.next_token
+        if not UtilClient.is_unset(request.start_time_in_mills):
+            query['startTimeInMills'] = request.start_time_in_mills
         real_headers = {}
         if not UtilClient.is_unset(headers.common_headers):
             real_headers = headers.common_headers
         if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
             real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
         req = open_api_models.OpenApiRequest(
             headers=real_headers,
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
-            action='QueryBlackboardSpace',
-            version='blackboard_1.0',
+            action='QueryGoodsList',
+            version='wms_1.0',
             protocol='HTTP',
-            pathname=f'/v1.0/blackboard/spaces',
+            pathname=f'/v1.0/wms/goods',
             method='GET',
             auth_type='AK',
             style='ROA',
             req_body_type='none',
             body_type='json'
         )
         return TeaCore.from_map(
-            dingtalkblackboard__1__0_models.QueryBlackboardSpaceResponse(),
+            dingtalkwms__1__0_models.QueryGoodsListResponse(),
             await self.execute_async(params, req, runtime)
         )
 
-    def query_blackboard_space(
+    def query_goods_list(
         self,
-        request: dingtalkblackboard__1__0_models.QueryBlackboardSpaceRequest,
-    ) -> dingtalkblackboard__1__0_models.QueryBlackboardSpaceResponse:
+        request: dingtalkwms__1__0_models.QueryGoodsListRequest,
+    ) -> dingtalkwms__1__0_models.QueryGoodsListResponse:
         runtime = util_models.RuntimeOptions()
-        headers = dingtalkblackboard__1__0_models.QueryBlackboardSpaceHeaders()
-        return self.query_blackboard_space_with_options(request, headers, runtime)
+        headers = dingtalkwms__1__0_models.QueryGoodsListHeaders()
+        return self.query_goods_list_with_options(request, headers, runtime)
 
-    async def query_blackboard_space_async(
+    async def query_goods_list_async(
         self,
-        request: dingtalkblackboard__1__0_models.QueryBlackboardSpaceRequest,
-    ) -> dingtalkblackboard__1__0_models.QueryBlackboardSpaceResponse:
+        request: dingtalkwms__1__0_models.QueryGoodsListRequest,
+    ) -> dingtalkwms__1__0_models.QueryGoodsListResponse:
         runtime = util_models.RuntimeOptions()
-        headers = dingtalkblackboard__1__0_models.QueryBlackboardSpaceHeaders()
-        return await self.query_blackboard_space_with_options_async(request, headers, runtime)
+        headers = dingtalkwms__1__0_models.QueryGoodsListHeaders()
+        return await self.query_goods_list_with_options_async(request, headers, runtime)
```

### Comparing `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/blackboard_1_0/models.py` & `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/workrecord_1_0/models.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*-
 # This file is auto-generated, don't edit it. Thanks.
 from Tea.model import TeaModel
 from typing import Dict
 
 
-class QueryBlackboardSpaceHeaders(TeaModel):
+class CountWorkRecordHeaders(TeaModel):
     def __init__(
         self,
         common_headers: Dict[str, str] = None,
         x_acs_dingtalk_access_token: str = None,
     ):
         self.common_headers = common_headers
         self.x_acs_dingtalk_access_token = x_acs_dingtalk_access_token
@@ -33,74 +33,74 @@
         if m.get('commonHeaders') is not None:
             self.common_headers = m.get('commonHeaders')
         if m.get('x-acs-dingtalk-access-token') is not None:
             self.x_acs_dingtalk_access_token = m.get('x-acs-dingtalk-access-token')
         return self
 
 
-class QueryBlackboardSpaceRequest(TeaModel):
+class CountWorkRecordRequest(TeaModel):
     def __init__(
         self,
-        operation_user_id: str = None,
+        user_id: str = None,
     ):
-        self.operation_user_id = operation_user_id
+        self.user_id = user_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.operation_user_id is not None:
-            result['operationUserId'] = self.operation_user_id
+        if self.user_id is not None:
+            result['userId'] = self.user_id
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('operationUserId') is not None:
-            self.operation_user_id = m.get('operationUserId')
+        if m.get('userId') is not None:
+            self.user_id = m.get('userId')
         return self
 
 
-class QueryBlackboardSpaceResponseBody(TeaModel):
+class CountWorkRecordResponseBody(TeaModel):
     def __init__(
         self,
-        space_id: str = None,
+        undo_count: int = None,
     ):
-        self.space_id = space_id
+        self.undo_count = undo_count
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.space_id is not None:
-            result['spaceId'] = self.space_id
+        if self.undo_count is not None:
+            result['undoCount'] = self.undo_count
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('spaceId') is not None:
-            self.space_id = m.get('spaceId')
+        if m.get('undoCount') is not None:
+            self.undo_count = m.get('undoCount')
         return self
 
 
-class QueryBlackboardSpaceResponse(TeaModel):
+class CountWorkRecordResponse(TeaModel):
     def __init__(
         self,
         headers: Dict[str, str] = None,
         status_code: int = None,
-        body: QueryBlackboardSpaceResponseBody = None,
+        body: CountWorkRecordResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
@@ -126,12 +126,12 @@
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('headers') is not None:
             self.headers = m.get('headers')
         if m.get('statusCode') is not None:
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
-            temp_model = QueryBlackboardSpaceResponseBody()
+            temp_model = CountWorkRecordResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
```

### Comparing `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/calendar_1_0/client.py` & `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/calendar_1_0/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,14 +41,16 @@
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.attendees_to_add):
             body['attendeesToAdd'] = request.attendees_to_add
         real_headers = {}
         if not UtilClient.is_unset(headers.common_headers):
             real_headers = headers.common_headers
+        if not UtilClient.is_unset(headers.x_client_token):
+            real_headers['x-client-token'] = UtilClient.to_jsonstring(headers.x_client_token)
         if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
             real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
         req = open_api_models.OpenApiRequest(
             headers=real_headers,
             body=OpenApiUtilClient.parse_to_map(body)
         )
         params = open_api_models.Params(
@@ -79,14 +81,16 @@
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.attendees_to_add):
             body['attendeesToAdd'] = request.attendees_to_add
         real_headers = {}
         if not UtilClient.is_unset(headers.common_headers):
             real_headers = headers.common_headers
+        if not UtilClient.is_unset(headers.x_client_token):
+            real_headers['x-client-token'] = UtilClient.to_jsonstring(headers.x_client_token)
         if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
             real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
         req = open_api_models.OpenApiRequest(
             headers=real_headers,
             body=OpenApiUtilClient.parse_to_map(body)
         )
         params = open_api_models.Params(
@@ -139,14 +143,16 @@
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.meeting_rooms_to_add):
             body['meetingRoomsToAdd'] = request.meeting_rooms_to_add
         real_headers = {}
         if not UtilClient.is_unset(headers.common_headers):
             real_headers = headers.common_headers
+        if not UtilClient.is_unset(headers.x_client_token):
+            real_headers['x-client-token'] = UtilClient.to_jsonstring(headers.x_client_token)
         if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
             real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
         req = open_api_models.OpenApiRequest(
             headers=real_headers,
             body=OpenApiUtilClient.parse_to_map(body)
         )
         params = open_api_models.Params(
@@ -177,14 +183,16 @@
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.meeting_rooms_to_add):
             body['meetingRoomsToAdd'] = request.meeting_rooms_to_add
         real_headers = {}
         if not UtilClient.is_unset(headers.common_headers):
             real_headers = headers.common_headers
+        if not UtilClient.is_unset(headers.x_client_token):
+            real_headers['x-client-token'] = UtilClient.to_jsonstring(headers.x_client_token)
         if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
             real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
         req = open_api_models.OpenApiRequest(
             headers=real_headers,
             body=OpenApiUtilClient.parse_to_map(body)
         )
         params = open_api_models.Params(
@@ -536,14 +544,16 @@
         if not UtilClient.is_unset(request.summary):
             body['summary'] = request.summary
         if not UtilClient.is_unset(request.ui_configs):
             body['uiConfigs'] = request.ui_configs
         real_headers = {}
         if not UtilClient.is_unset(headers.common_headers):
             real_headers = headers.common_headers
+        if not UtilClient.is_unset(headers.x_client_token):
+            real_headers['x-client-token'] = UtilClient.to_jsonstring(headers.x_client_token)
         if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
             real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
         req = open_api_models.OpenApiRequest(
             headers=real_headers,
             body=OpenApiUtilClient.parse_to_map(body)
         )
         params = open_api_models.Params(
@@ -597,14 +607,16 @@
         if not UtilClient.is_unset(request.summary):
             body['summary'] = request.summary
         if not UtilClient.is_unset(request.ui_configs):
             body['uiConfigs'] = request.ui_configs
         real_headers = {}
         if not UtilClient.is_unset(headers.common_headers):
             real_headers = headers.common_headers
+        if not UtilClient.is_unset(headers.x_client_token):
+            real_headers['x-client-token'] = UtilClient.to_jsonstring(headers.x_client_token)
         if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
             real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
         req = open_api_models.OpenApiRequest(
             headers=real_headers,
             body=OpenApiUtilClient.parse_to_map(body)
         )
         params = open_api_models.Params(
@@ -836,14 +848,16 @@
         event_id: str,
         headers: dingtalkcalendar__1__0_models.DeleteEventHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> dingtalkcalendar__1__0_models.DeleteEventResponse:
         real_headers = {}
         if not UtilClient.is_unset(headers.common_headers):
             real_headers = headers.common_headers
+        if not UtilClient.is_unset(headers.x_client_token):
+            real_headers['x-client-token'] = UtilClient.to_jsonstring(headers.x_client_token)
         if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
             real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
         req = open_api_models.OpenApiRequest(
             headers=real_headers
         )
         params = open_api_models.Params(
             action='DeleteEvent',
@@ -868,14 +882,16 @@
         event_id: str,
         headers: dingtalkcalendar__1__0_models.DeleteEventHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> dingtalkcalendar__1__0_models.DeleteEventResponse:
         real_headers = {}
         if not UtilClient.is_unset(headers.common_headers):
             real_headers = headers.common_headers
+        if not UtilClient.is_unset(headers.x_client_token):
+            real_headers['x-client-token'] = UtilClient.to_jsonstring(headers.x_client_token)
         if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
             real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
         req = open_api_models.OpenApiRequest(
             headers=real_headers
         )
         params = open_api_models.Params(
             action='DeleteEvent',
@@ -2416,17 +2432,21 @@
             body['reminders'] = request.reminders
         if not UtilClient.is_unset(request.rich_text_description):
             body['richTextDescription'] = request.rich_text_description
         if not UtilClient.is_unset(request.start):
             body['start'] = request.start
         if not UtilClient.is_unset(request.summary):
             body['summary'] = request.summary
+        if not UtilClient.is_unset(request.ui_configs):
+            body['uiConfigs'] = request.ui_configs
         real_headers = {}
         if not UtilClient.is_unset(headers.common_headers):
             real_headers = headers.common_headers
+        if not UtilClient.is_unset(headers.x_client_token):
+            real_headers['x-client-token'] = UtilClient.to_jsonstring(headers.x_client_token)
         if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
             real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
         req = open_api_models.OpenApiRequest(
             headers=real_headers,
             body=OpenApiUtilClient.parse_to_map(body)
         )
         params = open_api_models.Params(
@@ -2478,17 +2498,21 @@
             body['reminders'] = request.reminders
         if not UtilClient.is_unset(request.rich_text_description):
             body['richTextDescription'] = request.rich_text_description
         if not UtilClient.is_unset(request.start):
             body['start'] = request.start
         if not UtilClient.is_unset(request.summary):
             body['summary'] = request.summary
+        if not UtilClient.is_unset(request.ui_configs):
+            body['uiConfigs'] = request.ui_configs
         real_headers = {}
         if not UtilClient.is_unset(headers.common_headers):
             real_headers = headers.common_headers
+        if not UtilClient.is_unset(headers.x_client_token):
+            real_headers['x-client-token'] = UtilClient.to_jsonstring(headers.x_client_token)
         if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
             real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
         req = open_api_models.OpenApiRequest(
             headers=real_headers,
             body=OpenApiUtilClient.parse_to_map(body)
         )
         params = open_api_models.Params(
@@ -2541,14 +2565,16 @@
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.attendees_to_remove):
             body['attendeesToRemove'] = request.attendees_to_remove
         real_headers = {}
         if not UtilClient.is_unset(headers.common_headers):
             real_headers = headers.common_headers
+        if not UtilClient.is_unset(headers.x_client_token):
+            real_headers['x-client-token'] = UtilClient.to_jsonstring(headers.x_client_token)
         if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
             real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
         req = open_api_models.OpenApiRequest(
             headers=real_headers,
             body=OpenApiUtilClient.parse_to_map(body)
         )
         params = open_api_models.Params(
@@ -2579,14 +2605,16 @@
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.attendees_to_remove):
             body['attendeesToRemove'] = request.attendees_to_remove
         real_headers = {}
         if not UtilClient.is_unset(headers.common_headers):
             real_headers = headers.common_headers
+        if not UtilClient.is_unset(headers.x_client_token):
+            real_headers['x-client-token'] = UtilClient.to_jsonstring(headers.x_client_token)
         if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
             real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
         req = open_api_models.OpenApiRequest(
             headers=real_headers,
             body=OpenApiUtilClient.parse_to_map(body)
         )
         params = open_api_models.Params(
@@ -2639,14 +2667,16 @@
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.meeting_rooms_to_remove):
             body['meetingRoomsToRemove'] = request.meeting_rooms_to_remove
         real_headers = {}
         if not UtilClient.is_unset(headers.common_headers):
             real_headers = headers.common_headers
+        if not UtilClient.is_unset(headers.x_client_token):
+            real_headers['x-client-token'] = UtilClient.to_jsonstring(headers.x_client_token)
         if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
             real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
         req = open_api_models.OpenApiRequest(
             headers=real_headers,
             body=OpenApiUtilClient.parse_to_map(body)
         )
         params = open_api_models.Params(
@@ -2677,14 +2707,16 @@
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.meeting_rooms_to_remove):
             body['meetingRoomsToRemove'] = request.meeting_rooms_to_remove
         real_headers = {}
         if not UtilClient.is_unset(headers.common_headers):
             real_headers = headers.common_headers
+        if not UtilClient.is_unset(headers.x_client_token):
+            real_headers['x-client-token'] = UtilClient.to_jsonstring(headers.x_client_token)
         if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
             real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
         req = open_api_models.OpenApiRequest(
             headers=real_headers,
             body=OpenApiUtilClient.parse_to_map(body)
         )
         params = open_api_models.Params(
@@ -2737,14 +2769,16 @@
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.response_status):
             body['responseStatus'] = request.response_status
         real_headers = {}
         if not UtilClient.is_unset(headers.common_headers):
             real_headers = headers.common_headers
+        if not UtilClient.is_unset(headers.x_client_token):
+            real_headers['x-client-token'] = UtilClient.to_jsonstring(headers.x_client_token)
         if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
             real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
         req = open_api_models.OpenApiRequest(
             headers=real_headers,
             body=OpenApiUtilClient.parse_to_map(body)
         )
         params = open_api_models.Params(
@@ -2775,14 +2809,16 @@
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.response_status):
             body['responseStatus'] = request.response_status
         real_headers = {}
         if not UtilClient.is_unset(headers.common_headers):
             real_headers = headers.common_headers
+        if not UtilClient.is_unset(headers.x_client_token):
+            real_headers['x-client-token'] = UtilClient.to_jsonstring(headers.x_client_token)
         if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
             real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
         req = open_api_models.OpenApiRequest(
             headers=real_headers,
             body=OpenApiUtilClient.parse_to_map(body)
         )
         params = open_api_models.Params(
```

### Comparing `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/calendar_1_0/models.py` & `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/calendar_1_0/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,38 +4,44 @@
 from typing import Dict, List, Any
 
 
 class AddAttendeeHeaders(TeaModel):
     def __init__(
         self,
         common_headers: Dict[str, str] = None,
+        x_client_token: str = None,
         x_acs_dingtalk_access_token: str = None,
     ):
         self.common_headers = common_headers
+        self.x_client_token = x_client_token
         self.x_acs_dingtalk_access_token = x_acs_dingtalk_access_token
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.common_headers is not None:
             result['commonHeaders'] = self.common_headers
+        if self.x_client_token is not None:
+            result['x-client-token'] = self.x_client_token
         if self.x_acs_dingtalk_access_token is not None:
             result['x-acs-dingtalk-access-token'] = self.x_acs_dingtalk_access_token
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('commonHeaders') is not None:
             self.common_headers = m.get('commonHeaders')
+        if m.get('x-client-token') is not None:
+            self.x_client_token = m.get('x-client-token')
         if m.get('x-acs-dingtalk-access-token') is not None:
             self.x_acs_dingtalk_access_token = m.get('x-acs-dingtalk-access-token')
         return self
 
 
 class AddAttendeeRequestAttendeesToAdd(TeaModel):
     def __init__(
@@ -139,38 +145,44 @@
         return self
 
 
 class AddMeetingRoomsHeaders(TeaModel):
     def __init__(
         self,
         common_headers: Dict[str, str] = None,
+        x_client_token: str = None,
         x_acs_dingtalk_access_token: str = None,
     ):
         self.common_headers = common_headers
+        self.x_client_token = x_client_token
         self.x_acs_dingtalk_access_token = x_acs_dingtalk_access_token
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.common_headers is not None:
             result['commonHeaders'] = self.common_headers
+        if self.x_client_token is not None:
+            result['x-client-token'] = self.x_client_token
         if self.x_acs_dingtalk_access_token is not None:
             result['x-acs-dingtalk-access-token'] = self.x_acs_dingtalk_access_token
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('commonHeaders') is not None:
             self.common_headers = m.get('commonHeaders')
+        if m.get('x-client-token') is not None:
+            self.x_client_token = m.get('x-client-token')
         if m.get('x-acs-dingtalk-access-token') is not None:
             self.x_acs_dingtalk_access_token = m.get('x-acs-dingtalk-access-token')
         return self
 
 
 class AddMeetingRoomsRequestMeetingRoomsToAdd(TeaModel):
     def __init__(
@@ -765,38 +777,44 @@
         return self
 
 
 class CreateEventHeaders(TeaModel):
     def __init__(
         self,
         common_headers: Dict[str, str] = None,
+        x_client_token: str = None,
         x_acs_dingtalk_access_token: str = None,
     ):
         self.common_headers = common_headers
+        self.x_client_token = x_client_token
         self.x_acs_dingtalk_access_token = x_acs_dingtalk_access_token
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.common_headers is not None:
             result['commonHeaders'] = self.common_headers
+        if self.x_client_token is not None:
+            result['x-client-token'] = self.x_client_token
         if self.x_acs_dingtalk_access_token is not None:
             result['x-acs-dingtalk-access-token'] = self.x_acs_dingtalk_access_token
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('commonHeaders') is not None:
             self.common_headers = m.get('commonHeaders')
+        if m.get('x-client-token') is not None:
+            self.x_client_token = m.get('x-client-token')
         if m.get('x-acs-dingtalk-access-token') is not None:
             self.x_acs_dingtalk_access_token = m.get('x-acs-dingtalk-access-token')
         return self
 
 
 class CreateEventRequestAttendees(TeaModel):
     def __init__(
@@ -2259,38 +2277,44 @@
         return self
 
 
 class DeleteEventHeaders(TeaModel):
     def __init__(
         self,
         common_headers: Dict[str, str] = None,
+        x_client_token: str = None,
         x_acs_dingtalk_access_token: str = None,
     ):
         self.common_headers = common_headers
+        self.x_client_token = x_client_token
         self.x_acs_dingtalk_access_token = x_acs_dingtalk_access_token
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.common_headers is not None:
             result['commonHeaders'] = self.common_headers
+        if self.x_client_token is not None:
+            result['x-client-token'] = self.x_client_token
         if self.x_acs_dingtalk_access_token is not None:
             result['x-acs-dingtalk-access-token'] = self.x_acs_dingtalk_access_token
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('commonHeaders') is not None:
             self.common_headers = m.get('commonHeaders')
+        if m.get('x-client-token') is not None:
+            self.x_client_token = m.get('x-client-token')
         if m.get('x-acs-dingtalk-access-token') is not None:
             self.x_acs_dingtalk_access_token = m.get('x-acs-dingtalk-access-token')
         return self
 
 
 class DeleteEventResponse(TeaModel):
     def __init__(
@@ -8872,69 +8896,81 @@
         return self
 
 
 class PatchEventHeaders(TeaModel):
     def __init__(
         self,
         common_headers: Dict[str, str] = None,
+        x_client_token: str = None,
         x_acs_dingtalk_access_token: str = None,
     ):
         self.common_headers = common_headers
+        self.x_client_token = x_client_token
         self.x_acs_dingtalk_access_token = x_acs_dingtalk_access_token
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.common_headers is not None:
             result['commonHeaders'] = self.common_headers
+        if self.x_client_token is not None:
+            result['x-client-token'] = self.x_client_token
         if self.x_acs_dingtalk_access_token is not None:
             result['x-acs-dingtalk-access-token'] = self.x_acs_dingtalk_access_token
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('commonHeaders') is not None:
             self.common_headers = m.get('commonHeaders')
+        if m.get('x-client-token') is not None:
+            self.x_client_token = m.get('x-client-token')
         if m.get('x-acs-dingtalk-access-token') is not None:
             self.x_acs_dingtalk_access_token = m.get('x-acs-dingtalk-access-token')
         return self
 
 
 class PatchEventRequestAttendees(TeaModel):
     def __init__(
         self,
+        email: str = None,
         id: str = None,
         is_optional: bool = None,
     ):
+        self.email = email
         self.id = id
         self.is_optional = is_optional
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
+        if self.email is not None:
+            result['email'] = self.email
         if self.id is not None:
             result['id'] = self.id
         if self.is_optional is not None:
             result['isOptional'] = self.is_optional
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
+        if m.get('email') is not None:
+            self.email = m.get('email')
         if m.get('id') is not None:
             self.id = m.get('id')
         if m.get('isOptional') is not None:
             self.is_optional = m.get('isOptional')
         return self
 
 
@@ -9254,14 +9290,47 @@
         if m.get('dateTime') is not None:
             self.date_time = m.get('dateTime')
         if m.get('timeZone') is not None:
             self.time_zone = m.get('timeZone')
         return self
 
 
+class PatchEventRequestUiConfigs(TeaModel):
+    def __init__(
+        self,
+        ui_name: str = None,
+        ui_status: str = None,
+    ):
+        self.ui_name = ui_name
+        self.ui_status = ui_status
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
+        if self.ui_name is not None:
+            result['uiName'] = self.ui_name
+        if self.ui_status is not None:
+            result['uiStatus'] = self.ui_status
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('uiName') is not None:
+            self.ui_name = m.get('uiName')
+        if m.get('uiStatus') is not None:
+            self.ui_status = m.get('uiStatus')
+        return self
+
+
 class PatchEventRequest(TeaModel):
     def __init__(
         self,
         attendees: List[PatchEventRequestAttendees] = None,
         description: str = None,
         end: PatchEventRequestEnd = None,
         extra: Dict[str, str] = None,
@@ -9270,28 +9339,30 @@
         location: PatchEventRequestLocation = None,
         online_meeting_info: PatchEventRequestOnlineMeetingInfo = None,
         recurrence: PatchEventRequestRecurrence = None,
         reminders: List[PatchEventRequestReminders] = None,
         rich_text_description: PatchEventRequestRichTextDescription = None,
         start: PatchEventRequestStart = None,
         summary: str = None,
+        ui_configs: List[PatchEventRequestUiConfigs] = None,
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
         self.rich_text_description = rich_text_description
         self.start = start
         self.summary = summary
+        self.ui_configs = ui_configs
 
     def validate(self):
         if self.attendees:
             for k in self.attendees:
                 if k:
                     k.validate()
         if self.end:
@@ -9306,14 +9377,18 @@
             for k in self.reminders:
                 if k:
                     k.validate()
         if self.rich_text_description:
             self.rich_text_description.validate()
         if self.start:
             self.start.validate()
+        if self.ui_configs:
+            for k in self.ui_configs:
+                if k:
+                    k.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
@@ -9343,14 +9418,18 @@
                 result['reminders'].append(k.to_map() if k else None)
         if self.rich_text_description is not None:
             result['richTextDescription'] = self.rich_text_description.to_map()
         if self.start is not None:
             result['start'] = self.start.to_map()
         if self.summary is not None:
             result['summary'] = self.summary
+        result['uiConfigs'] = []
+        if self.ui_configs is not None:
+            for k in self.ui_configs:
+                result['uiConfigs'].append(k.to_map() if k else None)
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         self.attendees = []
         if m.get('attendees') is not None:
             for k in m.get('attendees'):
@@ -9385,14 +9464,19 @@
             temp_model = PatchEventRequestRichTextDescription()
             self.rich_text_description = temp_model.from_map(m['richTextDescription'])
         if m.get('start') is not None:
             temp_model = PatchEventRequestStart()
             self.start = temp_model.from_map(m['start'])
         if m.get('summary') is not None:
             self.summary = m.get('summary')
+        self.ui_configs = []
+        if m.get('uiConfigs') is not None:
+            for k in m.get('uiConfigs'):
+                temp_model = PatchEventRequestUiConfigs()
+                self.ui_configs.append(temp_model.from_map(k))
         return self
 
 
 class PatchEventResponseBodyAttendees(TeaModel):
     def __init__(
         self,
         display_name: str = None,
@@ -9822,14 +9906,47 @@
         if m.get('dateTime') is not None:
             self.date_time = m.get('dateTime')
         if m.get('timeZone') is not None:
             self.time_zone = m.get('timeZone')
         return self
 
 
+class PatchEventResponseBodyUiConfigs(TeaModel):
+    def __init__(
+        self,
+        ui_name: str = None,
+        ui_status: str = None,
+    ):
+        self.ui_name = ui_name
+        self.ui_status = ui_status
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
+        if self.ui_name is not None:
+            result['uiName'] = self.ui_name
+        if self.ui_status is not None:
+            result['uiStatus'] = self.ui_status
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('uiName') is not None:
+            self.ui_name = m.get('uiName')
+        if m.get('uiStatus') is not None:
+            self.ui_status = m.get('uiStatus')
+        return self
+
+
 class PatchEventResponseBody(TeaModel):
     def __init__(
         self,
         attendees: List[PatchEventResponseBodyAttendees] = None,
         create_time: str = None,
         description: str = None,
         end: PatchEventResponseBodyEnd = None,
@@ -9839,14 +9956,15 @@
         online_meeting_info: PatchEventResponseBodyOnlineMeetingInfo = None,
         organizer: PatchEventResponseBodyOrganizer = None,
         recurrence: PatchEventResponseBodyRecurrence = None,
         reminders: List[PatchEventResponseBodyReminders] = None,
         rich_text_description: PatchEventResponseBodyRichTextDescription = None,
         start: PatchEventResponseBodyStart = None,
         summary: str = None,
+        ui_configs: List[PatchEventResponseBodyUiConfigs] = None,
         update_time: str = None,
     ):
         self.attendees = attendees
         self.create_time = create_time
         self.description = description
         self.end = end
         self.id = id
@@ -9855,14 +9973,15 @@
         self.online_meeting_info = online_meeting_info
         self.organizer = organizer
         self.recurrence = recurrence
         self.reminders = reminders
         self.rich_text_description = rich_text_description
         self.start = start
         self.summary = summary
+        self.ui_configs = ui_configs
         self.update_time = update_time
 
     def validate(self):
         if self.attendees:
             for k in self.attendees:
                 if k:
                     k.validate()
@@ -9880,14 +9999,18 @@
             for k in self.reminders:
                 if k:
                     k.validate()
         if self.rich_text_description:
             self.rich_text_description.validate()
         if self.start:
             self.start.validate()
+        if self.ui_configs:
+            for k in self.ui_configs:
+                if k:
+                    k.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
@@ -9919,14 +10042,18 @@
                 result['reminders'].append(k.to_map() if k else None)
         if self.rich_text_description is not None:
             result['richTextDescription'] = self.rich_text_description.to_map()
         if self.start is not None:
             result['start'] = self.start.to_map()
         if self.summary is not None:
             result['summary'] = self.summary
+        result['uiConfigs'] = []
+        if self.ui_configs is not None:
+            for k in self.ui_configs:
+                result['uiConfigs'].append(k.to_map() if k else None)
         if self.update_time is not None:
             result['updateTime'] = self.update_time
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         self.attendees = []
@@ -9966,14 +10093,19 @@
             temp_model = PatchEventResponseBodyRichTextDescription()
             self.rich_text_description = temp_model.from_map(m['richTextDescription'])
         if m.get('start') is not None:
             temp_model = PatchEventResponseBodyStart()
             self.start = temp_model.from_map(m['start'])
         if m.get('summary') is not None:
             self.summary = m.get('summary')
+        self.ui_configs = []
+        if m.get('uiConfigs') is not None:
+            for k in m.get('uiConfigs'):
+                temp_model = PatchEventResponseBodyUiConfigs()
+                self.ui_configs.append(temp_model.from_map(k))
         if m.get('updateTime') is not None:
             self.update_time = m.get('updateTime')
         return self
 
 
 class PatchEventResponse(TeaModel):
     def __init__(
@@ -10019,38 +10151,44 @@
         return self
 
 
 class RemoveAttendeeHeaders(TeaModel):
     def __init__(
         self,
         common_headers: Dict[str, str] = None,
+        x_client_token: str = None,
         x_acs_dingtalk_access_token: str = None,
     ):
         self.common_headers = common_headers
+        self.x_client_token = x_client_token
         self.x_acs_dingtalk_access_token = x_acs_dingtalk_access_token
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.common_headers is not None:
             result['commonHeaders'] = self.common_headers
+        if self.x_client_token is not None:
+            result['x-client-token'] = self.x_client_token
         if self.x_acs_dingtalk_access_token is not None:
             result['x-acs-dingtalk-access-token'] = self.x_acs_dingtalk_access_token
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('commonHeaders') is not None:
             self.common_headers = m.get('commonHeaders')
+        if m.get('x-client-token') is not None:
+            self.x_client_token = m.get('x-client-token')
         if m.get('x-acs-dingtalk-access-token') is not None:
             self.x_acs_dingtalk_access_token = m.get('x-acs-dingtalk-access-token')
         return self
 
 
 class RemoveAttendeeRequestAttendeesToRemove(TeaModel):
     def __init__(
@@ -10148,38 +10286,44 @@
         return self
 
 
 class RemoveMeetingRoomsHeaders(TeaModel):
     def __init__(
         self,
         common_headers: Dict[str, str] = None,
+        x_client_token: str = None,
         x_acs_dingtalk_access_token: str = None,
     ):
         self.common_headers = common_headers
+        self.x_client_token = x_client_token
         self.x_acs_dingtalk_access_token = x_acs_dingtalk_access_token
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.common_headers is not None:
             result['commonHeaders'] = self.common_headers
+        if self.x_client_token is not None:
+            result['x-client-token'] = self.x_client_token
         if self.x_acs_dingtalk_access_token is not None:
             result['x-acs-dingtalk-access-token'] = self.x_acs_dingtalk_access_token
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('commonHeaders') is not None:
             self.common_headers = m.get('commonHeaders')
+        if m.get('x-client-token') is not None:
+            self.x_client_token = m.get('x-client-token')
         if m.get('x-acs-dingtalk-access-token') is not None:
             self.x_acs_dingtalk_access_token = m.get('x-acs-dingtalk-access-token')
         return self
 
 
 class RemoveMeetingRoomsRequestMeetingRoomsToRemove(TeaModel):
     def __init__(
@@ -10314,38 +10458,44 @@
         return self
 
 
 class RespondEventHeaders(TeaModel):
     def __init__(
         self,
         common_headers: Dict[str, str] = None,
+        x_client_token: str = None,
         x_acs_dingtalk_access_token: str = None,
     ):
         self.common_headers = common_headers
+        self.x_client_token = x_client_token
         self.x_acs_dingtalk_access_token = x_acs_dingtalk_access_token
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.common_headers is not None:
             result['commonHeaders'] = self.common_headers
+        if self.x_client_token is not None:
+            result['x-client-token'] = self.x_client_token
         if self.x_acs_dingtalk_access_token is not None:
             result['x-acs-dingtalk-access-token'] = self.x_acs_dingtalk_access_token
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('commonHeaders') is not None:
             self.common_headers = m.get('commonHeaders')
+        if m.get('x-client-token') is not None:
+            self.x_client_token = m.get('x-client-token')
         if m.get('x-acs-dingtalk-access-token') is not None:
             self.x_acs_dingtalk_access_token = m.get('x-acs-dingtalk-access-token')
         return self
 
 
 class RespondEventRequest(TeaModel):
     def __init__(
```

### Comparing `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/carbon_1_0/client.py` & `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/carbon_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/carbon_1_0/models.py` & `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/carbon_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/card_1_0/client.py` & `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/card_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/card_1_0/models.py` & `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/card_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/check_in_1_0/client.py` & `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/check_in_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/check_in_1_0/models.py` & `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/check_in_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/chengfeng_1_0/client.py` & `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/chengfeng_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/chengfeng_1_0/models.py` & `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/chengfeng_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/conference_1_0/client.py` & `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/conference_1_0/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,14 +25,104 @@
         super().__init__(config)
         self._client = GatewayClientClient()
         self._spi = self._client
         self._endpoint_rule = ''
         if UtilClient.empty(self._endpoint):
             self._endpoint = 'api.dingtalk.com'
 
+    def cancel_schedule_conference_with_options(
+        self,
+        request: dingtalkconference__1__0_models.CancelScheduleConferenceRequest,
+        headers: dingtalkconference__1__0_models.CancelScheduleConferenceHeaders,
+        runtime: util_models.RuntimeOptions,
+    ) -> dingtalkconference__1__0_models.CancelScheduleConferenceResponse:
+        UtilClient.validate_model(request)
+        body = {}
+        if not UtilClient.is_unset(request.creator_union_id):
+            body['creatorUnionId'] = request.creator_union_id
+        if not UtilClient.is_unset(request.schedule_conference_id):
+            body['scheduleConferenceId'] = request.schedule_conference_id
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
+            action='CancelScheduleConference',
+            version='conference_1.0',
+            protocol='HTTP',
+            pathname=f'/v1.0/conference/scheduleConferences/cancel',
+            method='POST',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='none',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dingtalkconference__1__0_models.CancelScheduleConferenceResponse(),
+            self.execute(params, req, runtime)
+        )
+
+    async def cancel_schedule_conference_with_options_async(
+        self,
+        request: dingtalkconference__1__0_models.CancelScheduleConferenceRequest,
+        headers: dingtalkconference__1__0_models.CancelScheduleConferenceHeaders,
+        runtime: util_models.RuntimeOptions,
+    ) -> dingtalkconference__1__0_models.CancelScheduleConferenceResponse:
+        UtilClient.validate_model(request)
+        body = {}
+        if not UtilClient.is_unset(request.creator_union_id):
+            body['creatorUnionId'] = request.creator_union_id
+        if not UtilClient.is_unset(request.schedule_conference_id):
+            body['scheduleConferenceId'] = request.schedule_conference_id
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
+            action='CancelScheduleConference',
+            version='conference_1.0',
+            protocol='HTTP',
+            pathname=f'/v1.0/conference/scheduleConferences/cancel',
+            method='POST',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='none',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dingtalkconference__1__0_models.CancelScheduleConferenceResponse(),
+            await self.execute_async(params, req, runtime)
+        )
+
+    def cancel_schedule_conference(
+        self,
+        request: dingtalkconference__1__0_models.CancelScheduleConferenceRequest,
+    ) -> dingtalkconference__1__0_models.CancelScheduleConferenceResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = dingtalkconference__1__0_models.CancelScheduleConferenceHeaders()
+        return self.cancel_schedule_conference_with_options(request, headers, runtime)
+
+    async def cancel_schedule_conference_async(
+        self,
+        request: dingtalkconference__1__0_models.CancelScheduleConferenceRequest,
+    ) -> dingtalkconference__1__0_models.CancelScheduleConferenceResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = dingtalkconference__1__0_models.CancelScheduleConferenceHeaders()
+        return await self.cancel_schedule_conference_with_options_async(request, headers, runtime)
+
     def close_video_conference_with_options(
         self,
         conference_id: str,
         request: dingtalkconference__1__0_models.CloseVideoConferenceRequest,
         headers: dingtalkconference__1__0_models.CloseVideoConferenceHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> dingtalkconference__1__0_models.CloseVideoConferenceResponse:
@@ -209,14 +299,112 @@
         conference_id: str,
         request: dingtalkconference__1__0_models.CohostsRequest,
     ) -> dingtalkconference__1__0_models.CohostsResponse:
         runtime = util_models.RuntimeOptions()
         headers = dingtalkconference__1__0_models.CohostsHeaders()
         return await self.cohosts_with_options_async(conference_id, request, headers, runtime)
 
+    def create_schedule_conference_with_options(
+        self,
+        request: dingtalkconference__1__0_models.CreateScheduleConferenceRequest,
+        headers: dingtalkconference__1__0_models.CreateScheduleConferenceHeaders,
+        runtime: util_models.RuntimeOptions,
+    ) -> dingtalkconference__1__0_models.CreateScheduleConferenceResponse:
+        UtilClient.validate_model(request)
+        body = {}
+        if not UtilClient.is_unset(request.creator_union_id):
+            body['creatorUnionId'] = request.creator_union_id
+        if not UtilClient.is_unset(request.end_time):
+            body['endTime'] = request.end_time
+        if not UtilClient.is_unset(request.start_time):
+            body['startTime'] = request.start_time
+        if not UtilClient.is_unset(request.title):
+            body['title'] = request.title
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
+            action='CreateScheduleConference',
+            version='conference_1.0',
+            protocol='HTTP',
+            pathname=f'/v1.0/conference/scheduleConferences',
+            method='POST',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='none',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dingtalkconference__1__0_models.CreateScheduleConferenceResponse(),
+            self.execute(params, req, runtime)
+        )
+
+    async def create_schedule_conference_with_options_async(
+        self,
+        request: dingtalkconference__1__0_models.CreateScheduleConferenceRequest,
+        headers: dingtalkconference__1__0_models.CreateScheduleConferenceHeaders,
+        runtime: util_models.RuntimeOptions,
+    ) -> dingtalkconference__1__0_models.CreateScheduleConferenceResponse:
+        UtilClient.validate_model(request)
+        body = {}
+        if not UtilClient.is_unset(request.creator_union_id):
+            body['creatorUnionId'] = request.creator_union_id
+        if not UtilClient.is_unset(request.end_time):
+            body['endTime'] = request.end_time
+        if not UtilClient.is_unset(request.start_time):
+            body['startTime'] = request.start_time
+        if not UtilClient.is_unset(request.title):
+            body['title'] = request.title
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
+            action='CreateScheduleConference',
+            version='conference_1.0',
+            protocol='HTTP',
+            pathname=f'/v1.0/conference/scheduleConferences',
+            method='POST',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='none',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dingtalkconference__1__0_models.CreateScheduleConferenceResponse(),
+            await self.execute_async(params, req, runtime)
+        )
+
+    def create_schedule_conference(
+        self,
+        request: dingtalkconference__1__0_models.CreateScheduleConferenceRequest,
+    ) -> dingtalkconference__1__0_models.CreateScheduleConferenceResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = dingtalkconference__1__0_models.CreateScheduleConferenceHeaders()
+        return self.create_schedule_conference_with_options(request, headers, runtime)
+
+    async def create_schedule_conference_async(
+        self,
+        request: dingtalkconference__1__0_models.CreateScheduleConferenceRequest,
+    ) -> dingtalkconference__1__0_models.CreateScheduleConferenceResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = dingtalkconference__1__0_models.CreateScheduleConferenceHeaders()
+        return await self.create_schedule_conference_with_options_async(request, headers, runtime)
+
     def create_video_conference_with_options(
         self,
         request: dingtalkconference__1__0_models.CreateVideoConferenceRequest,
         headers: dingtalkconference__1__0_models.CreateVideoConferenceHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> dingtalkconference__1__0_models.CreateVideoConferenceResponse:
         UtilClient.validate_model(request)
@@ -1731,14 +1919,104 @@
         conference_id: str,
         request: dingtalkconference__1__0_models.QueryConferenceMembersRequest,
     ) -> dingtalkconference__1__0_models.QueryConferenceMembersResponse:
         runtime = util_models.RuntimeOptions()
         headers = dingtalkconference__1__0_models.QueryConferenceMembersHeaders()
         return await self.query_conference_members_with_options_async(conference_id, request, headers, runtime)
 
+    def query_schedule_conference_with_options(
+        self,
+        schedule_conference_id: str,
+        request: dingtalkconference__1__0_models.QueryScheduleConferenceRequest,
+        headers: dingtalkconference__1__0_models.QueryScheduleConferenceHeaders,
+        runtime: util_models.RuntimeOptions,
+    ) -> dingtalkconference__1__0_models.QueryScheduleConferenceResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.request_union_id):
+            query['requestUnionId'] = request.request_union_id
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
+            action='QueryScheduleConference',
+            version='conference_1.0',
+            protocol='HTTP',
+            pathname=f'/v1.0/conference/scheduleConferences/{schedule_conference_id}/infos',
+            method='GET',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='none',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dingtalkconference__1__0_models.QueryScheduleConferenceResponse(),
+            self.execute(params, req, runtime)
+        )
+
+    async def query_schedule_conference_with_options_async(
+        self,
+        schedule_conference_id: str,
+        request: dingtalkconference__1__0_models.QueryScheduleConferenceRequest,
+        headers: dingtalkconference__1__0_models.QueryScheduleConferenceHeaders,
+        runtime: util_models.RuntimeOptions,
+    ) -> dingtalkconference__1__0_models.QueryScheduleConferenceResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.request_union_id):
+            query['requestUnionId'] = request.request_union_id
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
+            action='QueryScheduleConference',
+            version='conference_1.0',
+            protocol='HTTP',
+            pathname=f'/v1.0/conference/scheduleConferences/{schedule_conference_id}/infos',
+            method='GET',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='none',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dingtalkconference__1__0_models.QueryScheduleConferenceResponse(),
+            await self.execute_async(params, req, runtime)
+        )
+
+    def query_schedule_conference(
+        self,
+        schedule_conference_id: str,
+        request: dingtalkconference__1__0_models.QueryScheduleConferenceRequest,
+    ) -> dingtalkconference__1__0_models.QueryScheduleConferenceResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = dingtalkconference__1__0_models.QueryScheduleConferenceHeaders()
+        return self.query_schedule_conference_with_options(schedule_conference_id, request, headers, runtime)
+
+    async def query_schedule_conference_async(
+        self,
+        schedule_conference_id: str,
+        request: dingtalkconference__1__0_models.QueryScheduleConferenceRequest,
+    ) -> dingtalkconference__1__0_models.QueryScheduleConferenceResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = dingtalkconference__1__0_models.QueryScheduleConferenceHeaders()
+        return await self.query_schedule_conference_with_options_async(schedule_conference_id, request, headers, runtime)
+
     def query_schedule_conference_info_with_options(
         self,
         schedule_conference_id: str,
         request: dingtalkconference__1__0_models.QueryScheduleConferenceInfoRequest,
         headers: dingtalkconference__1__0_models.QueryScheduleConferenceInfoHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> dingtalkconference__1__0_models.QueryScheduleConferenceInfoResponse:
@@ -2221,14 +2499,116 @@
         conference_id: str,
         request: dingtalkconference__1__0_models.StopStreamOutRequest,
     ) -> dingtalkconference__1__0_models.StopStreamOutResponse:
         runtime = util_models.RuntimeOptions()
         headers = dingtalkconference__1__0_models.StopStreamOutHeaders()
         return await self.stop_stream_out_with_options_async(conference_id, request, headers, runtime)
 
+    def update_schedule_conference_with_options(
+        self,
+        request: dingtalkconference__1__0_models.UpdateScheduleConferenceRequest,
+        headers: dingtalkconference__1__0_models.UpdateScheduleConferenceHeaders,
+        runtime: util_models.RuntimeOptions,
+    ) -> dingtalkconference__1__0_models.UpdateScheduleConferenceResponse:
+        UtilClient.validate_model(request)
+        body = {}
+        if not UtilClient.is_unset(request.creator_union_id):
+            body['creatorUnionId'] = request.creator_union_id
+        if not UtilClient.is_unset(request.end_time):
+            body['endTime'] = request.end_time
+        if not UtilClient.is_unset(request.schedule_conference_id):
+            body['scheduleConferenceId'] = request.schedule_conference_id
+        if not UtilClient.is_unset(request.start_time):
+            body['startTime'] = request.start_time
+        if not UtilClient.is_unset(request.title):
+            body['title'] = request.title
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
+            action='UpdateScheduleConference',
+            version='conference_1.0',
+            protocol='HTTP',
+            pathname=f'/v1.0/conference/scheduleConferences',
+            method='PUT',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='none',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dingtalkconference__1__0_models.UpdateScheduleConferenceResponse(),
+            self.execute(params, req, runtime)
+        )
+
+    async def update_schedule_conference_with_options_async(
+        self,
+        request: dingtalkconference__1__0_models.UpdateScheduleConferenceRequest,
+        headers: dingtalkconference__1__0_models.UpdateScheduleConferenceHeaders,
+        runtime: util_models.RuntimeOptions,
+    ) -> dingtalkconference__1__0_models.UpdateScheduleConferenceResponse:
+        UtilClient.validate_model(request)
+        body = {}
+        if not UtilClient.is_unset(request.creator_union_id):
+            body['creatorUnionId'] = request.creator_union_id
+        if not UtilClient.is_unset(request.end_time):
+            body['endTime'] = request.end_time
+        if not UtilClient.is_unset(request.schedule_conference_id):
+            body['scheduleConferenceId'] = request.schedule_conference_id
+        if not UtilClient.is_unset(request.start_time):
+            body['startTime'] = request.start_time
+        if not UtilClient.is_unset(request.title):
+            body['title'] = request.title
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
+            action='UpdateScheduleConference',
+            version='conference_1.0',
+            protocol='HTTP',
+            pathname=f'/v1.0/conference/scheduleConferences',
+            method='PUT',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='none',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dingtalkconference__1__0_models.UpdateScheduleConferenceResponse(),
+            await self.execute_async(params, req, runtime)
+        )
+
+    def update_schedule_conference(
+        self,
+        request: dingtalkconference__1__0_models.UpdateScheduleConferenceRequest,
+    ) -> dingtalkconference__1__0_models.UpdateScheduleConferenceResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = dingtalkconference__1__0_models.UpdateScheduleConferenceHeaders()
+        return self.update_schedule_conference_with_options(request, headers, runtime)
+
+    async def update_schedule_conference_async(
+        self,
+        request: dingtalkconference__1__0_models.UpdateScheduleConferenceRequest,
+    ) -> dingtalkconference__1__0_models.UpdateScheduleConferenceResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = dingtalkconference__1__0_models.UpdateScheduleConferenceHeaders()
+        return await self.update_schedule_conference_with_options_async(request, headers, runtime)
+
     def update_video_conference_ext_info_with_options(
         self,
         conference_id: str,
         headers: dingtalkconference__1__0_models.UpdateVideoConferenceExtInfoHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> dingtalkconference__1__0_models.UpdateVideoConferenceExtInfoResponse:
         real_headers = {}
```

### Comparing `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/conference_1_0/models.py` & `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/conference_1_0/models.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,150 @@
 # -*- coding: utf-8 -*-
 # This file is auto-generated, don't edit it. Thanks.
 from Tea.model import TeaModel
 from typing import Dict, List, Any
 
 
+class CancelScheduleConferenceHeaders(TeaModel):
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
+class CancelScheduleConferenceRequest(TeaModel):
+    def __init__(
+        self,
+        creator_union_id: str = None,
+        schedule_conference_id: str = None,
+    ):
+        self.creator_union_id = creator_union_id
+        self.schedule_conference_id = schedule_conference_id
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
+        if self.creator_union_id is not None:
+            result['creatorUnionId'] = self.creator_union_id
+        if self.schedule_conference_id is not None:
+            result['scheduleConferenceId'] = self.schedule_conference_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('creatorUnionId') is not None:
+            self.creator_union_id = m.get('creatorUnionId')
+        if m.get('scheduleConferenceId') is not None:
+            self.schedule_conference_id = m.get('scheduleConferenceId')
+        return self
+
+
+class CancelScheduleConferenceResponseBody(TeaModel):
+    def __init__(
+        self,
+        success: bool = None,
+    ):
+        self.success = success
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
+        if self.success is not None:
+            result['success'] = self.success
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('success') is not None:
+            self.success = m.get('success')
+        return self
+
+
+class CancelScheduleConferenceResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: CancelScheduleConferenceResponseBody = None,
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
+            temp_model = CancelScheduleConferenceResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class CloseVideoConferenceHeaders(TeaModel):
     def __init__(
         self,
         common_headers: Dict[str, str] = None,
         x_acs_dingtalk_access_token: str = None,
     ):
         self.common_headers = common_headers
@@ -309,14 +446,187 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = CohostsResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class CreateScheduleConferenceHeaders(TeaModel):
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
+class CreateScheduleConferenceRequest(TeaModel):
+    def __init__(
+        self,
+        creator_union_id: str = None,
+        end_time: int = None,
+        start_time: int = None,
+        title: str = None,
+    ):
+        self.creator_union_id = creator_union_id
+        self.end_time = end_time
+        self.start_time = start_time
+        self.title = title
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
+        if self.creator_union_id is not None:
+            result['creatorUnionId'] = self.creator_union_id
+        if self.end_time is not None:
+            result['endTime'] = self.end_time
+        if self.start_time is not None:
+            result['startTime'] = self.start_time
+        if self.title is not None:
+            result['title'] = self.title
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('creatorUnionId') is not None:
+            self.creator_union_id = m.get('creatorUnionId')
+        if m.get('endTime') is not None:
+            self.end_time = m.get('endTime')
+        if m.get('startTime') is not None:
+            self.start_time = m.get('startTime')
+        if m.get('title') is not None:
+            self.title = m.get('title')
+        return self
+
+
+class CreateScheduleConferenceResponseBody(TeaModel):
+    def __init__(
+        self,
+        phones: List[str] = None,
+        request_id: str = None,
+        room_code: str = None,
+        schedule_conference_id: str = None,
+        url: str = None,
+    ):
+        self.phones = phones
+        self.request_id = request_id
+        self.room_code = room_code
+        self.schedule_conference_id = schedule_conference_id
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
+        if self.phones is not None:
+            result['phones'] = self.phones
+        if self.request_id is not None:
+            result['requestId'] = self.request_id
+        if self.room_code is not None:
+            result['roomCode'] = self.room_code
+        if self.schedule_conference_id is not None:
+            result['scheduleConferenceId'] = self.schedule_conference_id
+        if self.url is not None:
+            result['url'] = self.url
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('phones') is not None:
+            self.phones = m.get('phones')
+        if m.get('requestId') is not None:
+            self.request_id = m.get('requestId')
+        if m.get('roomCode') is not None:
+            self.room_code = m.get('roomCode')
+        if m.get('scheduleConferenceId') is not None:
+            self.schedule_conference_id = m.get('scheduleConferenceId')
+        if m.get('url') is not None:
+            self.url = m.get('url')
+        return self
+
+
+class CreateScheduleConferenceResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: CreateScheduleConferenceResponseBody = None,
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
+            temp_model = CreateScheduleConferenceResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class CreateVideoConferenceHeaders(TeaModel):
     def __init__(
         self,
         common_headers: Dict[str, str] = None,
         x_acs_dingtalk_access_token: str = None,
     ):
         self.common_headers = common_headers
@@ -3768,14 +4078,187 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = QueryConferenceMembersResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class QueryScheduleConferenceHeaders(TeaModel):
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
+class QueryScheduleConferenceRequest(TeaModel):
+    def __init__(
+        self,
+        request_union_id: str = None,
+    ):
+        self.request_union_id = request_union_id
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
+        if self.request_union_id is not None:
+            result['requestUnionId'] = self.request_union_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('requestUnionId') is not None:
+            self.request_union_id = m.get('requestUnionId')
+        return self
+
+
+class QueryScheduleConferenceResponseBody(TeaModel):
+    def __init__(
+        self,
+        end_time: int = None,
+        phones: List[str] = None,
+        request_id: str = None,
+        room_code: str = None,
+        schedule_conference_id: str = None,
+        start_time: int = None,
+        title: str = None,
+        url: str = None,
+    ):
+        self.end_time = end_time
+        self.phones = phones
+        self.request_id = request_id
+        self.room_code = room_code
+        self.schedule_conference_id = schedule_conference_id
+        self.start_time = start_time
+        self.title = title
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
+        if self.end_time is not None:
+            result['endTime'] = self.end_time
+        if self.phones is not None:
+            result['phones'] = self.phones
+        if self.request_id is not None:
+            result['requestId'] = self.request_id
+        if self.room_code is not None:
+            result['roomCode'] = self.room_code
+        if self.schedule_conference_id is not None:
+            result['scheduleConferenceId'] = self.schedule_conference_id
+        if self.start_time is not None:
+            result['startTime'] = self.start_time
+        if self.title is not None:
+            result['title'] = self.title
+        if self.url is not None:
+            result['url'] = self.url
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('endTime') is not None:
+            self.end_time = m.get('endTime')
+        if m.get('phones') is not None:
+            self.phones = m.get('phones')
+        if m.get('requestId') is not None:
+            self.request_id = m.get('requestId')
+        if m.get('roomCode') is not None:
+            self.room_code = m.get('roomCode')
+        if m.get('scheduleConferenceId') is not None:
+            self.schedule_conference_id = m.get('scheduleConferenceId')
+        if m.get('startTime') is not None:
+            self.start_time = m.get('startTime')
+        if m.get('title') is not None:
+            self.title = m.get('title')
+        if m.get('url') is not None:
+            self.url = m.get('url')
+        return self
+
+
+class QueryScheduleConferenceResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: QueryScheduleConferenceResponseBody = None,
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
+            temp_model = QueryScheduleConferenceResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class QueryScheduleConferenceInfoHeaders(TeaModel):
     def __init__(
         self,
         common_headers: Dict[str, str] = None,
         x_acs_dingtalk_access_token: str = None,
     ):
         self.common_headers = common_headers
@@ -4566,14 +5049,169 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = StopStreamOutResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class UpdateScheduleConferenceHeaders(TeaModel):
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
+class UpdateScheduleConferenceRequest(TeaModel):
+    def __init__(
+        self,
+        creator_union_id: str = None,
+        end_time: int = None,
+        schedule_conference_id: str = None,
+        start_time: int = None,
+        title: str = None,
+    ):
+        self.creator_union_id = creator_union_id
+        self.end_time = end_time
+        self.schedule_conference_id = schedule_conference_id
+        self.start_time = start_time
+        self.title = title
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
+        if self.creator_union_id is not None:
+            result['creatorUnionId'] = self.creator_union_id
+        if self.end_time is not None:
+            result['endTime'] = self.end_time
+        if self.schedule_conference_id is not None:
+            result['scheduleConferenceId'] = self.schedule_conference_id
+        if self.start_time is not None:
+            result['startTime'] = self.start_time
+        if self.title is not None:
+            result['title'] = self.title
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('creatorUnionId') is not None:
+            self.creator_union_id = m.get('creatorUnionId')
+        if m.get('endTime') is not None:
+            self.end_time = m.get('endTime')
+        if m.get('scheduleConferenceId') is not None:
+            self.schedule_conference_id = m.get('scheduleConferenceId')
+        if m.get('startTime') is not None:
+            self.start_time = m.get('startTime')
+        if m.get('title') is not None:
+            self.title = m.get('title')
+        return self
+
+
+class UpdateScheduleConferenceResponseBody(TeaModel):
+    def __init__(
+        self,
+        success: bool = None,
+    ):
+        self.success = success
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
+        if self.success is not None:
+            result['success'] = self.success
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('success') is not None:
+            self.success = m.get('success')
+        return self
+
+
+class UpdateScheduleConferenceResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: UpdateScheduleConferenceResponseBody = None,
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
+            temp_model = UpdateScheduleConferenceResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class UpdateVideoConferenceExtInfoHeaders(TeaModel):
     def __init__(
         self,
         common_headers: Dict[str, str] = None,
         x_acs_dingtalk_access_token: str = None,
     ):
         self.common_headers = common_headers
```

### Comparing `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/connector_1_0/client.py` & `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/connector_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/connector_1_0/models.py` & `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/connector_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/contact_1_0/client.py` & `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/contact_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/contact_1_0/models.py` & `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/contact_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/content_1_0/client.py` & `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/content_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/content_1_0/models.py` & `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/content_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/contract_1_0/client.py` & `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/contract_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/contract_1_0/models.py` & `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/contract_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/conv_file_1_0/client.py` & `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/conv_file_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/conv_file_1_0/models.py` & `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/conv_file_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/crm_1_0/client.py` & `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/crm_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/crm_1_0/models.py` & `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/crm_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/crm_2_0/client.py` & `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/crm_2_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/crm_2_0/models.py` & `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/crm_2_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/customer_service_1_0/client.py` & `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/customer_service_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/customer_service_1_0/models.py` & `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/customer_service_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/datacenter_1_0/client.py` & `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/datacenter_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/datacenter_1_0/models.py` & `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/datacenter_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/devicemng_1_0/client.py` & `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/devicemng_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/devicemng_1_0/models.py` & `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/devicemng_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/ding_phone_1_0/client.py` & `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/ding_phone_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/ding_phone_1_0/models.py` & `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/ding_phone_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/dingmi_1_0/client.py` & `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/dingmi_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/dingmi_1_0/models.py` & `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/dingmi_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/diot_1_0/client.py` & `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/diot_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/diot_1_0/models.py` & `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/diot_1_0/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,35 +30,35 @@
             self.req_id = m.get('reqId')
         return self
 
 
 class AyunOnlienTestResponseBody(TeaModel):
     def __init__(
         self,
-        request_id: str = None,
+        result: str = None,
     ):
-        self.request_id = request_id
+        self.result = result
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.request_id is not None:
-            result['requestId'] = self.request_id
+        if self.result is not None:
+            result['result'] = self.result
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('requestId') is not None:
-            self.request_id = m.get('requestId')
+        if m.get('result') is not None:
+            self.result = m.get('result')
         return self
 
 
 class AyunOnlienTestResponse(TeaModel):
     def __init__(
         self,
         headers: Dict[str, str] = None,
```

### Comparing `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/doc_1_0/client.py` & `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/doc_1_0/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,14 +25,120 @@
         super().__init__(config)
         self._client = GatewayClientClient()
         self._spi = self._client
         self._endpoint_rule = ''
         if UtilClient.empty(self._endpoint):
             self._endpoint = 'api.dingtalk.com'
 
+    def add_comment_with_options(
+        self,
+        doc_id: str,
+        request: dingtalkdoc__1__0_models.AddCommentRequest,
+        headers: dingtalkdoc__1__0_models.AddCommentHeaders,
+        runtime: util_models.RuntimeOptions,
+    ) -> dingtalkdoc__1__0_models.AddCommentResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.operator_id):
+            query['operatorId'] = request.operator_id
+        body = {}
+        if not UtilClient.is_unset(request.comment_content):
+            body['commentContent'] = request.comment_content
+        if not UtilClient.is_unset(request.comment_type):
+            body['commentType'] = request.comment_type
+        if not UtilClient.is_unset(request.option):
+            body['option'] = request.option
+        real_headers = {}
+        if not UtilClient.is_unset(headers.common_headers):
+            real_headers = headers.common_headers
+        if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
+            real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
+        req = open_api_models.OpenApiRequest(
+            headers=real_headers,
+            query=OpenApiUtilClient.query(query),
+            body=OpenApiUtilClient.parse_to_map(body)
+        )
+        params = open_api_models.Params(
+            action='AddComment',
+            version='doc_1.0',
+            protocol='HTTP',
+            pathname=f'/v1.0/doc/docs/{doc_id}/comments',
+            method='POST',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='none',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dingtalkdoc__1__0_models.AddCommentResponse(),
+            self.execute(params, req, runtime)
+        )
+
+    async def add_comment_with_options_async(
+        self,
+        doc_id: str,
+        request: dingtalkdoc__1__0_models.AddCommentRequest,
+        headers: dingtalkdoc__1__0_models.AddCommentHeaders,
+        runtime: util_models.RuntimeOptions,
+    ) -> dingtalkdoc__1__0_models.AddCommentResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.operator_id):
+            query['operatorId'] = request.operator_id
+        body = {}
+        if not UtilClient.is_unset(request.comment_content):
+            body['commentContent'] = request.comment_content
+        if not UtilClient.is_unset(request.comment_type):
+            body['commentType'] = request.comment_type
+        if not UtilClient.is_unset(request.option):
+            body['option'] = request.option
+        real_headers = {}
+        if not UtilClient.is_unset(headers.common_headers):
+            real_headers = headers.common_headers
+        if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
+            real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
+        req = open_api_models.OpenApiRequest(
+            headers=real_headers,
+            query=OpenApiUtilClient.query(query),
+            body=OpenApiUtilClient.parse_to_map(body)
+        )
+        params = open_api_models.Params(
+            action='AddComment',
+            version='doc_1.0',
+            protocol='HTTP',
+            pathname=f'/v1.0/doc/docs/{doc_id}/comments',
+            method='POST',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='none',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dingtalkdoc__1__0_models.AddCommentResponse(),
+            await self.execute_async(params, req, runtime)
+        )
+
+    def add_comment(
+        self,
+        doc_id: str,
+        request: dingtalkdoc__1__0_models.AddCommentRequest,
+    ) -> dingtalkdoc__1__0_models.AddCommentResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = dingtalkdoc__1__0_models.AddCommentHeaders()
+        return self.add_comment_with_options(doc_id, request, headers, runtime)
+
+    async def add_comment_async(
+        self,
+        doc_id: str,
+        request: dingtalkdoc__1__0_models.AddCommentRequest,
+    ) -> dingtalkdoc__1__0_models.AddCommentResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = dingtalkdoc__1__0_models.AddCommentHeaders()
+        return await self.add_comment_with_options_async(doc_id, request, headers, runtime)
+
     def add_workspace_doc_members_with_options(
         self,
         workspace_id: str,
         node_id: str,
         request: dingtalkdoc__1__0_models.AddWorkspaceDocMembersRequest,
         headers: dingtalkdoc__1__0_models.AddWorkspaceDocMembersHeaders,
         runtime: util_models.RuntimeOptions,
@@ -3139,14 +3245,120 @@
         node_id: str,
         request: dingtalkdoc__1__0_models.GetWorkspaceNodeRequest,
     ) -> dingtalkdoc__1__0_models.GetWorkspaceNodeResponse:
         runtime = util_models.RuntimeOptions()
         headers = dingtalkdoc__1__0_models.GetWorkspaceNodeHeaders()
         return await self.get_workspace_node_with_options_async(workspace_id, node_id, request, headers, runtime)
 
+    def init_document_with_options(
+        self,
+        doc_id: str,
+        request: dingtalkdoc__1__0_models.InitDocumentRequest,
+        headers: dingtalkdoc__1__0_models.InitDocumentHeaders,
+        runtime: util_models.RuntimeOptions,
+    ) -> dingtalkdoc__1__0_models.InitDocumentResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.operator_id):
+            query['operatorId'] = request.operator_id
+        body = {}
+        if not UtilClient.is_unset(request.attachments_map):
+            body['attachmentsMap'] = request.attachments_map
+        if not UtilClient.is_unset(request.import_type):
+            body['importType'] = request.import_type
+        if not UtilClient.is_unset(request.links_key):
+            body['linksKey'] = request.links_key
+        real_headers = {}
+        if not UtilClient.is_unset(headers.common_headers):
+            real_headers = headers.common_headers
+        if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
+            real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
+        req = open_api_models.OpenApiRequest(
+            headers=real_headers,
+            query=OpenApiUtilClient.query(query),
+            body=OpenApiUtilClient.parse_to_map(body)
+        )
+        params = open_api_models.Params(
+            action='InitDocument',
+            version='doc_1.0',
+            protocol='HTTP',
+            pathname=f'/v1.0/doc/docs/{doc_id}/init',
+            method='POST',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='none',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dingtalkdoc__1__0_models.InitDocumentResponse(),
+            self.execute(params, req, runtime)
+        )
+
+    async def init_document_with_options_async(
+        self,
+        doc_id: str,
+        request: dingtalkdoc__1__0_models.InitDocumentRequest,
+        headers: dingtalkdoc__1__0_models.InitDocumentHeaders,
+        runtime: util_models.RuntimeOptions,
+    ) -> dingtalkdoc__1__0_models.InitDocumentResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.operator_id):
+            query['operatorId'] = request.operator_id
+        body = {}
+        if not UtilClient.is_unset(request.attachments_map):
+            body['attachmentsMap'] = request.attachments_map
+        if not UtilClient.is_unset(request.import_type):
+            body['importType'] = request.import_type
+        if not UtilClient.is_unset(request.links_key):
+            body['linksKey'] = request.links_key
+        real_headers = {}
+        if not UtilClient.is_unset(headers.common_headers):
+            real_headers = headers.common_headers
+        if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
+            real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
+        req = open_api_models.OpenApiRequest(
+            headers=real_headers,
+            query=OpenApiUtilClient.query(query),
+            body=OpenApiUtilClient.parse_to_map(body)
+        )
+        params = open_api_models.Params(
+            action='InitDocument',
+            version='doc_1.0',
+            protocol='HTTP',
+            pathname=f'/v1.0/doc/docs/{doc_id}/init',
+            method='POST',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='none',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dingtalkdoc__1__0_models.InitDocumentResponse(),
+            await self.execute_async(params, req, runtime)
+        )
+
+    def init_document(
+        self,
+        doc_id: str,
+        request: dingtalkdoc__1__0_models.InitDocumentRequest,
+    ) -> dingtalkdoc__1__0_models.InitDocumentResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = dingtalkdoc__1__0_models.InitDocumentHeaders()
+        return self.init_document_with_options(doc_id, request, headers, runtime)
+
+    async def init_document_async(
+        self,
+        doc_id: str,
+        request: dingtalkdoc__1__0_models.InitDocumentRequest,
+    ) -> dingtalkdoc__1__0_models.InitDocumentResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = dingtalkdoc__1__0_models.InitDocumentHeaders()
+        return await self.init_document_with_options_async(doc_id, request, headers, runtime)
+
     def insert_blocks_with_options(
         self,
         document_id: str,
         request: dingtalkdoc__1__0_models.InsertBlocksRequest,
         headers: dingtalkdoc__1__0_models.InsertBlocksHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> dingtalkdoc__1__0_models.InsertBlocksResponse:
```

### Comparing `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/doc_1_0/models.py` & `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/doc_1_0/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,236 @@
 # -*- coding: utf-8 -*-
 # This file is auto-generated, don't edit it. Thanks.
 from Tea.model import TeaModel
 from typing import Dict, List, Any
 
 
+class AttachmentsMapValue(TeaModel):
+    def __init__(
+        self,
+        upload_key: str = None,
+        name: str = None,
+        media_type: str = None,
+    ):
+        self.upload_key = upload_key
+        self.name = name
+        self.media_type = media_type
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
+        if self.upload_key is not None:
+            result['uploadKey'] = self.upload_key
+        if self.name is not None:
+            result['name'] = self.name
+        if self.media_type is not None:
+            result['mediaType'] = self.media_type
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('uploadKey') is not None:
+            self.upload_key = m.get('uploadKey')
+        if m.get('name') is not None:
+            self.name = m.get('name')
+        if m.get('mediaType') is not None:
+            self.media_type = m.get('mediaType')
+        return self
+
+
+class AddCommentHeaders(TeaModel):
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
+class AddCommentRequestOption(TeaModel):
+    def __init__(
+        self,
+        create_time: str = None,
+        extra: Dict[str, str] = None,
+    ):
+        self.create_time = create_time
+        self.extra = extra
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
+        if self.create_time is not None:
+            result['createTime'] = self.create_time
+        if self.extra is not None:
+            result['extra'] = self.extra
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('createTime') is not None:
+            self.create_time = m.get('createTime')
+        if m.get('extra') is not None:
+            self.extra = m.get('extra')
+        return self
+
+
+class AddCommentRequest(TeaModel):
+    def __init__(
+        self,
+        comment_content: str = None,
+        comment_type: str = None,
+        option: AddCommentRequestOption = None,
+        operator_id: str = None,
+    ):
+        self.comment_content = comment_content
+        self.comment_type = comment_type
+        self.option = option
+        self.operator_id = operator_id
+
+    def validate(self):
+        if self.option:
+            self.option.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.comment_content is not None:
+            result['commentContent'] = self.comment_content
+        if self.comment_type is not None:
+            result['commentType'] = self.comment_type
+        if self.option is not None:
+            result['option'] = self.option.to_map()
+        if self.operator_id is not None:
+            result['operatorId'] = self.operator_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('commentContent') is not None:
+            self.comment_content = m.get('commentContent')
+        if m.get('commentType') is not None:
+            self.comment_type = m.get('commentType')
+        if m.get('option') is not None:
+            temp_model = AddCommentRequestOption()
+            self.option = temp_model.from_map(m['option'])
+        if m.get('operatorId') is not None:
+            self.operator_id = m.get('operatorId')
+        return self
+
+
+class AddCommentResponseBody(TeaModel):
+    def __init__(
+        self,
+        success: bool = None,
+    ):
+        self.success = success
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
+        if self.success is not None:
+            result['success'] = self.success
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('success') is not None:
+            self.success = m.get('success')
+        return self
+
+
+class AddCommentResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: AddCommentResponseBody = None,
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
+            temp_model = AddCommentResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class AddWorkspaceDocMembersHeaders(TeaModel):
     def __init__(
         self,
         common_headers: Dict[str, str] = None,
         x_acs_dingtalk_access_token: str = None,
     ):
         self.common_headers = common_headers
@@ -5765,14 +5988,171 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = GetWorkspaceNodeResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class InitDocumentHeaders(TeaModel):
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
+class InitDocumentRequest(TeaModel):
+    def __init__(
+        self,
+        attachments_map: Dict[str, AttachmentsMapValue] = None,
+        import_type: int = None,
+        links_key: str = None,
+        operator_id: str = None,
+    ):
+        self.attachments_map = attachments_map
+        self.import_type = import_type
+        self.links_key = links_key
+        self.operator_id = operator_id
+
+    def validate(self):
+        if self.attachments_map:
+            for v in self.attachments_map.values():
+                if v:
+                    v.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        result['attachmentsMap'] = {}
+        if self.attachments_map is not None:
+            for k, v in self.attachments_map.items():
+                result['attachmentsMap'][k] = v.to_map()
+        if self.import_type is not None:
+            result['importType'] = self.import_type
+        if self.links_key is not None:
+            result['linksKey'] = self.links_key
+        if self.operator_id is not None:
+            result['operatorId'] = self.operator_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        self.attachments_map = {}
+        if m.get('attachmentsMap') is not None:
+            for k, v in m.get('attachmentsMap').items():
+                temp_model = AttachmentsMapValue()
+                self.attachments_map[k] = temp_model.from_map(v)
+        if m.get('importType') is not None:
+            self.import_type = m.get('importType')
+        if m.get('linksKey') is not None:
+            self.links_key = m.get('linksKey')
+        if m.get('operatorId') is not None:
+            self.operator_id = m.get('operatorId')
+        return self
+
+
+class InitDocumentResponseBody(TeaModel):
+    def __init__(
+        self,
+        success: bool = None,
+    ):
+        self.success = success
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
+        if self.success is not None:
+            result['success'] = self.success
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('success') is not None:
+            self.success = m.get('success')
+        return self
+
+
+class InitDocumentResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: InitDocumentResponseBody = None,
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
+            temp_model = InitDocumentResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class InsertBlocksHeaders(TeaModel):
     def __init__(
         self,
         common_headers: Dict[str, str] = None,
         x_acs_dingtalk_access_token: str = None,
     ):
         self.common_headers = common_headers
```

### Comparing `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/doc_2_0/client.py` & `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/doc_2_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/doc_2_0/models.py` & `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/doc_2_0/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -4821,27 +4821,31 @@
             self.x_acs_dingtalk_access_token = m.get('x-acs-dingtalk-access-token')
         return self
 
 
 class ListStarsRequestOption(TeaModel):
     def __init__(
         self,
+        content_type_list: List[str] = None,
         filter_doc_types: List[str] = None,
+        list_v2: bool = None,
         max_results: int = None,
         next_token: str = None,
         order: str = None,
         order_by: str = None,
         with_dentry_creator_info: bool = None,
         with_dentry_modifier_info: bool = None,
         with_dentry_permission_role: bool = None,
         with_space_detail: bool = None,
         with_space_permission_role: bool = None,
         with_team_detail: bool = None,
     ):
+        self.content_type_list = content_type_list
         self.filter_doc_types = filter_doc_types
+        self.list_v2 = list_v2
         self.max_results = max_results
         self.next_token = next_token
         self.order = order
         self.order_by = order_by
         self.with_dentry_creator_info = with_dentry_creator_info
         self.with_dentry_modifier_info = with_dentry_modifier_info
         self.with_dentry_permission_role = with_dentry_permission_role
@@ -4854,16 +4858,20 @@
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
+        if self.content_type_list is not None:
+            result['contentTypeList'] = self.content_type_list
         if self.filter_doc_types is not None:
             result['filterDocTypes'] = self.filter_doc_types
+        if self.list_v2 is not None:
+            result['listV2'] = self.list_v2
         if self.max_results is not None:
             result['maxResults'] = self.max_results
         if self.next_token is not None:
             result['nextToken'] = self.next_token
         if self.order is not None:
             result['order'] = self.order
         if self.order_by is not None:
@@ -4880,16 +4888,20 @@
             result['withSpacePermissionRole'] = self.with_space_permission_role
         if self.with_team_detail is not None:
             result['withTeamDetail'] = self.with_team_detail
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
+        if m.get('contentTypeList') is not None:
+            self.content_type_list = m.get('contentTypeList')
         if m.get('filterDocTypes') is not None:
             self.filter_doc_types = m.get('filterDocTypes')
+        if m.get('listV2') is not None:
+            self.list_v2 = m.get('listV2')
         if m.get('maxResults') is not None:
             self.max_results = m.get('maxResults')
         if m.get('nextToken') is not None:
             self.next_token = m.get('nextToken')
         if m.get('order') is not None:
             self.order = m.get('order')
         if m.get('orderBy') is not None:
```

### Comparing `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/drive_1_0/client.py` & `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/drive_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/drive_1_0/models.py` & `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/drive_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/edu_1_0/client.py` & `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/edu_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/edu_1_0/models.py` & `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/edu_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/esign_1_0/client.py` & `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/esign_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/esign_1_0/models.py` & `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/esign_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/esign_2_0/client.py` & `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/esign_2_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/esign_2_0/models.py` & `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/esign_2_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/event_1_0/client.py` & `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/yun_shu_1_0/client.py`

 * *Files 22% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from Tea.core import TeaCore
 
 from alibabacloud_gateway_spi.client import Client as SPIClient
 from alibabacloud_tea_openapi.client import Client as OpenApiClient
 from alibabacloud_tea_openapi import models as open_api_models
 from alibabacloud_gateway_dingtalk.client import Client as GatewayClientClient
 from alibabacloud_tea_util.client import Client as UtilClient
-from alibabacloud_dingtalk.event_1_0 import models as dingtalkevent__1__0_models
+from alibabacloud_dingtalk.yun_shu_1_0 import models as dingtalkyun_shu__1__0_models
 from alibabacloud_tea_util import models as util_models
 from alibabacloud_openapi_util.client import Client as OpenApiUtilClient
 
 
 class Client(OpenApiClient):
     """
     *\
@@ -25,96 +25,104 @@
         super().__init__(config)
         self._client = GatewayClientClient()
         self._spi = self._client
         self._endpoint_rule = ''
         if UtilClient.empty(self._endpoint):
             self._endpoint = 'api.dingtalk.com'
 
-    def get_call_back_faile_result_with_options(
+    def save_open_external_log_with_options(
         self,
-        request: dingtalkevent__1__0_models.GetCallBackFaileResultRequest,
-        headers: dingtalkevent__1__0_models.GetCallBackFaileResultHeaders,
+        request: dingtalkyun_shu__1__0_models.SaveOpenExternalLogRequest,
+        headers: dingtalkyun_shu__1__0_models.SaveOpenExternalLogHeaders,
         runtime: util_models.RuntimeOptions,
-    ) -> dingtalkevent__1__0_models.GetCallBackFaileResultResponse:
+    ) -> dingtalkyun_shu__1__0_models.SaveOpenExternalLogResponse:
         UtilClient.validate_model(request)
-        query = {}
-        if not UtilClient.is_unset(request.begin_time):
-            query['beginTime'] = request.begin_time
-        if not UtilClient.is_unset(request.end_time):
-            query['endTime'] = request.end_time
+        body = {}
+        if not UtilClient.is_unset(request.corp_id):
+            body['corpId'] = request.corp_id
+        if not UtilClient.is_unset(request.log_source):
+            body['logSource'] = request.log_source
+        if not UtilClient.is_unset(request.log_type):
+            body['logType'] = request.log_type
+        if not UtilClient.is_unset(request.open_ext):
+            body['openExt'] = request.open_ext
         real_headers = {}
         if not UtilClient.is_unset(headers.common_headers):
             real_headers = headers.common_headers
         if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
             real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
         req = open_api_models.OpenApiRequest(
             headers=real_headers,
-            query=OpenApiUtilClient.query(query)
+            body=OpenApiUtilClient.parse_to_map(body)
         )
         params = open_api_models.Params(
-            action='GetCallBackFaileResult',
-            version='event_1.0',
+            action='SaveOpenExternalLog',
+            version='yunShu_1.0',
             protocol='HTTP',
-            pathname=f'/v1.0/event/callbacks/failedResults',
-            method='GET',
+            pathname=f'/v1.0/yunShu/externalLogs/save',
+            method='POST',
             auth_type='AK',
             style='ROA',
             req_body_type='none',
             body_type='json'
         )
         return TeaCore.from_map(
-            dingtalkevent__1__0_models.GetCallBackFaileResultResponse(),
+            dingtalkyun_shu__1__0_models.SaveOpenExternalLogResponse(),
             self.execute(params, req, runtime)
         )
 
-    async def get_call_back_faile_result_with_options_async(
+    async def save_open_external_log_with_options_async(
         self,
-        request: dingtalkevent__1__0_models.GetCallBackFaileResultRequest,
-        headers: dingtalkevent__1__0_models.GetCallBackFaileResultHeaders,
+        request: dingtalkyun_shu__1__0_models.SaveOpenExternalLogRequest,
+        headers: dingtalkyun_shu__1__0_models.SaveOpenExternalLogHeaders,
         runtime: util_models.RuntimeOptions,
-    ) -> dingtalkevent__1__0_models.GetCallBackFaileResultResponse:
+    ) -> dingtalkyun_shu__1__0_models.SaveOpenExternalLogResponse:
         UtilClient.validate_model(request)
-        query = {}
-        if not UtilClient.is_unset(request.begin_time):
-            query['beginTime'] = request.begin_time
-        if not UtilClient.is_unset(request.end_time):
-            query['endTime'] = request.end_time
+        body = {}
+        if not UtilClient.is_unset(request.corp_id):
+            body['corpId'] = request.corp_id
+        if not UtilClient.is_unset(request.log_source):
+            body['logSource'] = request.log_source
+        if not UtilClient.is_unset(request.log_type):
+            body['logType'] = request.log_type
+        if not UtilClient.is_unset(request.open_ext):
+            body['openExt'] = request.open_ext
         real_headers = {}
         if not UtilClient.is_unset(headers.common_headers):
             real_headers = headers.common_headers
         if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
             real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
         req = open_api_models.OpenApiRequest(
             headers=real_headers,
-            query=OpenApiUtilClient.query(query)
+            body=OpenApiUtilClient.parse_to_map(body)
         )
         params = open_api_models.Params(
-            action='GetCallBackFaileResult',
-            version='event_1.0',
+            action='SaveOpenExternalLog',
+            version='yunShu_1.0',
             protocol='HTTP',
-            pathname=f'/v1.0/event/callbacks/failedResults',
-            method='GET',
+            pathname=f'/v1.0/yunShu/externalLogs/save',
+            method='POST',
             auth_type='AK',
             style='ROA',
             req_body_type='none',
             body_type='json'
         )
         return TeaCore.from_map(
-            dingtalkevent__1__0_models.GetCallBackFaileResultResponse(),
+            dingtalkyun_shu__1__0_models.SaveOpenExternalLogResponse(),
             await self.execute_async(params, req, runtime)
         )
 
-    def get_call_back_faile_result(
+    def save_open_external_log(
         self,
-        request: dingtalkevent__1__0_models.GetCallBackFaileResultRequest,
-    ) -> dingtalkevent__1__0_models.GetCallBackFaileResultResponse:
+        request: dingtalkyun_shu__1__0_models.SaveOpenExternalLogRequest,
+    ) -> dingtalkyun_shu__1__0_models.SaveOpenExternalLogResponse:
         runtime = util_models.RuntimeOptions()
-        headers = dingtalkevent__1__0_models.GetCallBackFaileResultHeaders()
-        return self.get_call_back_faile_result_with_options(request, headers, runtime)
+        headers = dingtalkyun_shu__1__0_models.SaveOpenExternalLogHeaders()
+        return self.save_open_external_log_with_options(request, headers, runtime)
 
-    async def get_call_back_faile_result_async(
+    async def save_open_external_log_async(
         self,
-        request: dingtalkevent__1__0_models.GetCallBackFaileResultRequest,
-    ) -> dingtalkevent__1__0_models.GetCallBackFaileResultResponse:
+        request: dingtalkyun_shu__1__0_models.SaveOpenExternalLogRequest,
+    ) -> dingtalkyun_shu__1__0_models.SaveOpenExternalLogResponse:
         runtime = util_models.RuntimeOptions()
-        headers = dingtalkevent__1__0_models.GetCallBackFaileResultHeaders()
-        return await self.get_call_back_faile_result_with_options_async(request, headers, runtime)
+        headers = dingtalkyun_shu__1__0_models.SaveOpenExternalLogHeaders()
+        return await self.save_open_external_log_with_options_async(request, headers, runtime)
```

### Comparing `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/event_1_0/models.py` & `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/event_1_0/models.py`

 * *Files 22% similar despite different names*

```diff
@@ -196,7 +196,111 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = GetCallBackFaileResultResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class RePushSuiteTicketRequest(TeaModel):
+    def __init__(
+        self,
+        suite_id: int = None,
+        suite_secret: str = None,
+    ):
+        self.suite_id = suite_id
+        self.suite_secret = suite_secret
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
+        if self.suite_id is not None:
+            result['suiteId'] = self.suite_id
+        if self.suite_secret is not None:
+            result['suiteSecret'] = self.suite_secret
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('suiteId') is not None:
+            self.suite_id = m.get('suiteId')
+        if m.get('suiteSecret') is not None:
+            self.suite_secret = m.get('suiteSecret')
+        return self
+
+
+class RePushSuiteTicketResponseBody(TeaModel):
+    def __init__(
+        self,
+        result: str = None,
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
+class RePushSuiteTicketResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: RePushSuiteTicketResponseBody = None,
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
+            temp_model = RePushSuiteTicketResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
```

### Comparing `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/exclusive_1_0/client.py` & `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/exclusive_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/exclusive_1_0/models.py` & `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/exclusive_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/finance_1_0/client.py` & `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/finance_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/finance_1_0/models.py` & `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/finance_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/flashmeeting_1_0/client.py` & `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/flashmeeting_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/flashmeeting_1_0/models.py` & `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/flashmeeting_1_0/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -271,21 +271,23 @@
 
 
 class GetShanhuiByCalendarResponseBodyResult(TeaModel):
     def __init__(
         self,
         end_time: int = None,
         flashmeeting_key: str = None,
+        has_summary: bool = None,
         start_time: int = None,
         summary_doc_key: str = None,
         title: str = None,
         topics: List[GetShanhuiByCalendarResponseBodyResultTopics] = None,
     ):
         self.end_time = end_time
         self.flashmeeting_key = flashmeeting_key
+        self.has_summary = has_summary
         self.start_time = start_time
         self.summary_doc_key = summary_doc_key
         self.title = title
         self.topics = topics
 
     def validate(self):
         if self.topics:
@@ -299,14 +301,16 @@
             return _map
 
         result = dict()
         if self.end_time is not None:
             result['endTime'] = self.end_time
         if self.flashmeeting_key is not None:
             result['flashmeetingKey'] = self.flashmeeting_key
+        if self.has_summary is not None:
+            result['hasSummary'] = self.has_summary
         if self.start_time is not None:
             result['startTime'] = self.start_time
         if self.summary_doc_key is not None:
             result['summaryDocKey'] = self.summary_doc_key
         if self.title is not None:
             result['title'] = self.title
         result['topics'] = []
@@ -317,14 +321,16 @@
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('endTime') is not None:
             self.end_time = m.get('endTime')
         if m.get('flashmeetingKey') is not None:
             self.flashmeeting_key = m.get('flashmeetingKey')
+        if m.get('hasSummary') is not None:
+            self.has_summary = m.get('hasSummary')
         if m.get('startTime') is not None:
             self.start_time = m.get('startTime')
         if m.get('summaryDocKey') is not None:
             self.summary_doc_key = m.get('summaryDocKey')
         if m.get('title') is not None:
             self.title = m.get('title')
         self.topics = []
```

### Comparing `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/gateway_1_0/client.py` & `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/gateway_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/gateway_1_0/models.py` & `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/gateway_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/group_blackboard_1_0/client.py` & `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/group_blackboard_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/group_blackboard_1_0/models.py` & `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/group_blackboard_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/h3yun_1_0/client.py` & `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/h3yun_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/h3yun_1_0/models.py` & `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/h3yun_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/h5package_1_0/client.py` & `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/h5package_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/h5package_1_0/models.py` & `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/h5package_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/hrbrain_1_0/client.py` & `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/hrbrain_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/hrbrain_1_0/models.py` & `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/hrbrain_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/hrm_1_0/client.py` & `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/hrm_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/hrm_1_0/models.py` & `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/hrm_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/im_1_0/client.py` & `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/im_1_0/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1643,14 +1643,16 @@
     ) -> dingtalkim__1__0_models.GetConversationUrlResponse:
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.app_user_id):
             body['appUserId'] = request.app_user_id
         if not UtilClient.is_unset(request.channel_code):
             body['channelCode'] = request.channel_code
+        if not UtilClient.is_unset(request.device_id):
+            body['deviceId'] = request.device_id
         if not UtilClient.is_unset(request.open_conversation_id):
             body['openConversationId'] = request.open_conversation_id
         if not UtilClient.is_unset(request.user_id):
             body['userId'] = request.user_id
         real_headers = {}
         if not UtilClient.is_unset(headers.common_headers):
             real_headers = headers.common_headers
@@ -1684,14 +1686,16 @@
     ) -> dingtalkim__1__0_models.GetConversationUrlResponse:
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.app_user_id):
             body['appUserId'] = request.app_user_id
         if not UtilClient.is_unset(request.channel_code):
             body['channelCode'] = request.channel_code
+        if not UtilClient.is_unset(request.device_id):
+            body['deviceId'] = request.device_id
         if not UtilClient.is_unset(request.open_conversation_id):
             body['openConversationId'] = request.open_conversation_id
         if not UtilClient.is_unset(request.user_id):
             body['userId'] = request.user_id
         real_headers = {}
         if not UtilClient.is_unset(headers.common_headers):
             real_headers = headers.common_headers
```

### Comparing `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/im_1_0/models.py` & `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/im_1_0/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -2892,19 +2892,21 @@
 
 
 class GetConversationUrlRequest(TeaModel):
     def __init__(
         self,
         app_user_id: str = None,
         channel_code: str = None,
+        device_id: str = None,
         open_conversation_id: str = None,
         user_id: str = None,
     ):
         self.app_user_id = app_user_id
         self.channel_code = channel_code
+        self.device_id = device_id
         self.open_conversation_id = open_conversation_id
         self.user_id = user_id
 
     def validate(self):
         pass
 
     def to_map(self):
@@ -2913,26 +2915,30 @@
             return _map
 
         result = dict()
         if self.app_user_id is not None:
             result['appUserId'] = self.app_user_id
         if self.channel_code is not None:
             result['channelCode'] = self.channel_code
+        if self.device_id is not None:
+            result['deviceId'] = self.device_id
         if self.open_conversation_id is not None:
             result['openConversationId'] = self.open_conversation_id
         if self.user_id is not None:
             result['userId'] = self.user_id
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('appUserId') is not None:
             self.app_user_id = m.get('appUserId')
         if m.get('channelCode') is not None:
             self.channel_code = m.get('channelCode')
+        if m.get('deviceId') is not None:
+            self.device_id = m.get('deviceId')
         if m.get('openConversationId') is not None:
             self.open_conversation_id = m.get('openConversationId')
         if m.get('userId') is not None:
             self.user_id = m.get('userId')
         return self
```

### Comparing `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/im_2_0/client.py` & `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/im_2_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/im_2_0/models.py` & `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/im_2_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/impaas_1_0/client.py` & `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/impaas_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/impaas_1_0/models.py` & `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/impaas_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/industry_1_0/client.py` & `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/industry_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/industry_1_0/models.py` & `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/industry_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/jzcrm_1_0/client.py` & `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/jzcrm_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/jzcrm_1_0/models.py` & `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/jzcrm_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/link_1_0/client.py` & `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/link_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/link_1_0/models.py` & `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/link_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/live_1_0/client.py` & `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/live_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/live_1_0/models.py` & `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/live_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/manufacturing_1_0/client.py` & `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/manufacturing_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/manufacturing_1_0/models.py` & `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/manufacturing_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/micro_app_1_0/client.py` & `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/micro_app_1_0/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -699,14 +699,72 @@
         return self.ayun_test_with_options(headers, runtime)
 
     async def ayun_test_async(self) -> dingtalkmicro_app__1__0_models.AyunTestResponse:
         runtime = util_models.RuntimeOptions()
         headers = {}
         return await self.ayun_test_with_options_async(headers, runtime)
 
+    def ayun_test_online_with_options(
+        self,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> dingtalkmicro_app__1__0_models.AyunTestOnlineResponse:
+        req = open_api_models.OpenApiRequest(
+            headers=headers
+        )
+        params = open_api_models.Params(
+            action='AyunTestOnline',
+            version='microApp_1.0',
+            protocol='HTTP',
+            pathname=f'/v1.0/microApp/ayunTest',
+            method='GET',
+            auth_type='Anonymous',
+            style='ROA',
+            req_body_type='none',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dingtalkmicro_app__1__0_models.AyunTestOnlineResponse(),
+            self.execute(params, req, runtime)
+        )
+
+    async def ayun_test_online_with_options_async(
+        self,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> dingtalkmicro_app__1__0_models.AyunTestOnlineResponse:
+        req = open_api_models.OpenApiRequest(
+            headers=headers
+        )
+        params = open_api_models.Params(
+            action='AyunTestOnline',
+            version='microApp_1.0',
+            protocol='HTTP',
+            pathname=f'/v1.0/microApp/ayunTest',
+            method='GET',
+            auth_type='Anonymous',
+            style='ROA',
+            req_body_type='none',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dingtalkmicro_app__1__0_models.AyunTestOnlineResponse(),
+            await self.execute_async(params, req, runtime)
+        )
+
+    def ayun_test_online(self) -> dingtalkmicro_app__1__0_models.AyunTestOnlineResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.ayun_test_online_with_options(headers, runtime)
+
+    async def ayun_test_online_async(self) -> dingtalkmicro_app__1__0_models.AyunTestOnlineResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.ayun_test_online_with_options_async(headers, runtime)
+
     def create_apaas_app_with_options(
         self,
         request: dingtalkmicro_app__1__0_models.CreateApaasAppRequest,
         headers: dingtalkmicro_app__1__0_models.CreateApaasAppHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> dingtalkmicro_app__1__0_models.CreateApaasAppResponse:
         UtilClient.validate_model(request)
```

### Comparing `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/micro_app_1_0/models.py` & `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/micro_app_1_0/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -544,35 +544,35 @@
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class AnheiPResponseBody(TeaModel):
     def __init__(
         self,
-        request_id: str = None,
+        result: str = None,
     ):
-        self.request_id = request_id
+        self.result = result
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.request_id is not None:
-            result['requestId'] = self.request_id
+        if self.result is not None:
+            result['result'] = self.result
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('requestId') is not None:
-            self.request_id = m.get('requestId')
+        if m.get('result') is not None:
+            self.result = m.get('result')
         return self
 
 
 class AnheiPResponse(TeaModel):
     def __init__(
         self,
         headers: Dict[str, str] = None,
@@ -994,14 +994,85 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = AyunTestResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class AyunTestOnlineResponseBody(TeaModel):
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
+class AyunTestOnlineResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: AyunTestOnlineResponseBody = None,
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
+            temp_model = AyunTestOnlineResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class CreateApaasAppHeaders(TeaModel):
     def __init__(
         self,
         common_headers: Dict[str, str] = None,
         x_acs_dingtalk_access_token: str = None,
     ):
         self.common_headers = common_headers
```

### Comparing `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/miniapp_1_0/client.py` & `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/miniapp_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/miniapp_1_0/models.py` & `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/miniapp_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/oauth2_1_0/client.py` & `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/oauth2_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/oauth2_1_0/models.py` & `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/oauth2_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/occupationauth_1_0/client.py` & `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/occupationauth_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/occupationauth_1_0/models.py` & `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/occupationauth_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/okr_1_0/client.py` & `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/okr_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/okr_1_0/models.py` & `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/okr_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/org_culture_1_0/client.py` & `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/org_culture_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/org_culture_1_0/models.py` & `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/org_culture_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/package_1_0/client.py` & `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/package_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/package_1_0/models.py` & `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/package_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/pedia_1_0/client.py` & `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/pedia_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/pedia_1_0/models.py` & `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/pedia_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/project_1_0/client.py` & `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/project_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/project_1_0/models.py` & `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/project_1_0/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -6560,38 +6560,50 @@
             self.visibility = m.get('visibility')
         return self
 
 
 class QueryProjectResponseBody(TeaModel):
     def __init__(
         self,
+        next_token: str = None,
+        request_id: str = None,
         result: List[QueryProjectResponseBodyResult] = None,
     ):
+        self.next_token = next_token
+        self.request_id = request_id
         self.result = result
 
     def validate(self):
         if self.result:
             for k in self.result:
                 if k:
                     k.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
+        if self.next_token is not None:
+            result['nextToken'] = self.next_token
+        if self.request_id is not None:
+            result['requestId'] = self.request_id
         result['result'] = []
         if self.result is not None:
             for k in self.result:
                 result['result'].append(k.to_map() if k else None)
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
+        if m.get('nextToken') is not None:
+            self.next_token = m.get('nextToken')
+        if m.get('requestId') is not None:
+            self.request_id = m.get('requestId')
         self.result = []
         if m.get('result') is not None:
             for k in m.get('result'):
                 temp_model = QueryProjectResponseBodyResult()
                 self.result.append(temp_model.from_map(k))
         return self
```

### Comparing `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/project_integration_1_0/client.py` & `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/project_integration_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/project_integration_1_0/models.py` & `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/project_integration_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/rcs_call_1_0/client.py` & `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/rcs_call_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/rcs_call_1_0/models.py` & `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/rcs_call_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/resident_1_0/client.py` & `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/resident_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/resident_1_0/models.py` & `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/resident_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/robot_1_0/client.py` & `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/robot_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/robot_1_0/models.py` & `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/robot_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/rooms_1_0/client.py` & `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/rooms_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/rooms_1_0/models.py` & `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/rooms_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/search_1_0/client.py` & `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/search_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/search_1_0/models.py` & `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/search_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/service_group_1_0/client.py` & `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/service_group_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/service_group_1_0/models.py` & `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/service_group_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/smart_device_1_0/client.py` & `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/smart_device_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/smart_device_1_0/models.py` & `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/smart_device_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/sns_storage_1_0/client.py` & `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/sns_storage_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/sns_storage_1_0/models.py` & `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/sns_storage_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/storage_1_0/client.py` & `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/storage_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/storage_1_0/models.py` & `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/storage_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/storage_2_0/client.py` & `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/storage_2_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/storage_2_0/models.py` & `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/storage_2_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/swform_1_0/client.py` & `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/swform_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/swform_1_0/models.py` & `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/swform_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/todo_1_0/client.py` & `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/todo_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/todo_1_0/models.py` & `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/todo_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/trade_1_0/client.py` & `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/trade_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/trade_1_0/models.py` & `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/trade_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/trajectory_1_0/client.py` & `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/trajectory_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/trajectory_1_0/models.py` & `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/trajectory_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/transcribe_1_0/client.py` & `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/transcribe_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/transcribe_1_0/models.py` & `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/transcribe_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/trip_1_0/client.py` & `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/trip_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/trip_1_0/models.py` & `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/trip_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/village_1_0/client.py` & `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/village_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/village_1_0/models.py` & `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/village_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/watt_1_0/client.py` & `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/watt_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/watt_1_0/models.py` & `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/watt_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/wiki_1_0/client.py` & `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/wiki_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/wiki_1_0/models.py` & `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/wiki_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/wiki_2_0/client.py` & `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/wiki_2_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/wiki_2_0/models.py` & `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/wiki_2_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/wms_1_0/models.py` & `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/wms_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/workbench_1_0/client.py` & `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/workbench_1_0/client.py`

 * *Files 9% similar despite different names*

```diff
@@ -25,14 +25,108 @@
         super().__init__(config)
         self._client = GatewayClientClient()
         self._spi = self._client
         self._endpoint_rule = ''
         if UtilClient.empty(self._endpoint):
             self._endpoint = 'api.dingtalk.com'
 
+    def add_recent_user_app_list_with_options(
+        self,
+        request: dingtalkworkbench__1__0_models.AddRecentUserAppListRequest,
+        headers: dingtalkworkbench__1__0_models.AddRecentUserAppListHeaders,
+        runtime: util_models.RuntimeOptions,
+    ) -> dingtalkworkbench__1__0_models.AddRecentUserAppListResponse:
+        UtilClient.validate_model(request)
+        body = {}
+        if not UtilClient.is_unset(request.corp_id):
+            body['corpId'] = request.corp_id
+        if not UtilClient.is_unset(request.used_app_detail_list):
+            body['usedAppDetailList'] = request.used_app_detail_list
+        if not UtilClient.is_unset(request.user_id):
+            body['userId'] = request.user_id
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
+            action='AddRecentUserAppList',
+            version='workbench_1.0',
+            protocol='HTTP',
+            pathname=f'/v1.0/workbench/components/recentUsed/batch',
+            method='POST',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='none',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dingtalkworkbench__1__0_models.AddRecentUserAppListResponse(),
+            self.execute(params, req, runtime)
+        )
+
+    async def add_recent_user_app_list_with_options_async(
+        self,
+        request: dingtalkworkbench__1__0_models.AddRecentUserAppListRequest,
+        headers: dingtalkworkbench__1__0_models.AddRecentUserAppListHeaders,
+        runtime: util_models.RuntimeOptions,
+    ) -> dingtalkworkbench__1__0_models.AddRecentUserAppListResponse:
+        UtilClient.validate_model(request)
+        body = {}
+        if not UtilClient.is_unset(request.corp_id):
+            body['corpId'] = request.corp_id
+        if not UtilClient.is_unset(request.used_app_detail_list):
+            body['usedAppDetailList'] = request.used_app_detail_list
+        if not UtilClient.is_unset(request.user_id):
+            body['userId'] = request.user_id
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
+            action='AddRecentUserAppList',
+            version='workbench_1.0',
+            protocol='HTTP',
+            pathname=f'/v1.0/workbench/components/recentUsed/batch',
+            method='POST',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='none',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dingtalkworkbench__1__0_models.AddRecentUserAppListResponse(),
+            await self.execute_async(params, req, runtime)
+        )
+
+    def add_recent_user_app_list(
+        self,
+        request: dingtalkworkbench__1__0_models.AddRecentUserAppListRequest,
+    ) -> dingtalkworkbench__1__0_models.AddRecentUserAppListResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = dingtalkworkbench__1__0_models.AddRecentUserAppListHeaders()
+        return self.add_recent_user_app_list_with_options(request, headers, runtime)
+
+    async def add_recent_user_app_list_async(
+        self,
+        request: dingtalkworkbench__1__0_models.AddRecentUserAppListRequest,
+    ) -> dingtalkworkbench__1__0_models.AddRecentUserAppListResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = dingtalkworkbench__1__0_models.AddRecentUserAppListHeaders()
+        return await self.add_recent_user_app_list_with_options_async(request, headers, runtime)
+
     def get_ding_portal_detail_with_options(
         self,
         app_uuid: str,
         headers: dingtalkworkbench__1__0_models.GetDingPortalDetailHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> dingtalkworkbench__1__0_models.GetDingPortalDetailResponse:
         real_headers = {}
```

### Comparing `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/workbench_1_0/models.py` & `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/workbench_1_0/models.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,191 @@
 # -*- coding: utf-8 -*-
 # This file is auto-generated, don't edit it. Thanks.
 from Tea.model import TeaModel
 from typing import Dict, List
 
 
+class AddRecentUserAppListHeaders(TeaModel):
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
+class AddRecentUserAppListRequestUsedAppDetailList(TeaModel):
+    def __init__(
+        self,
+        agent_id: str = None,
+    ):
+        self.agent_id = agent_id
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
+        if self.agent_id is not None:
+            result['agentId'] = self.agent_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('agentId') is not None:
+            self.agent_id = m.get('agentId')
+        return self
+
+
+class AddRecentUserAppListRequest(TeaModel):
+    def __init__(
+        self,
+        corp_id: str = None,
+        used_app_detail_list: List[AddRecentUserAppListRequestUsedAppDetailList] = None,
+        user_id: str = None,
+    ):
+        self.corp_id = corp_id
+        self.used_app_detail_list = used_app_detail_list
+        self.user_id = user_id
+
+    def validate(self):
+        if self.used_app_detail_list:
+            for k in self.used_app_detail_list:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.corp_id is not None:
+            result['corpId'] = self.corp_id
+        result['usedAppDetailList'] = []
+        if self.used_app_detail_list is not None:
+            for k in self.used_app_detail_list:
+                result['usedAppDetailList'].append(k.to_map() if k else None)
+        if self.user_id is not None:
+            result['userId'] = self.user_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('corpId') is not None:
+            self.corp_id = m.get('corpId')
+        self.used_app_detail_list = []
+        if m.get('usedAppDetailList') is not None:
+            for k in m.get('usedAppDetailList'):
+                temp_model = AddRecentUserAppListRequestUsedAppDetailList()
+                self.used_app_detail_list.append(temp_model.from_map(k))
+        if m.get('userId') is not None:
+            self.user_id = m.get('userId')
+        return self
+
+
+class AddRecentUserAppListResponseBody(TeaModel):
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
+class AddRecentUserAppListResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: AddRecentUserAppListResponseBody = None,
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
+            temp_model = AddRecentUserAppListResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class GetDingPortalDetailHeaders(TeaModel):
     def __init__(
         self,
         common_headers: Dict[str, str] = None,
         x_acs_dingtalk_access_token: str = None,
     ):
         self.common_headers = common_headers
```

### Comparing `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/workflow_1_0/client.py` & `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/workflow_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/workflow_1_0/models.py` & `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/workflow_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/workrecord_1_0/client.py` & `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/workrecord_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/workrecord_1_0/models.py` & `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/yun_shu_1_0/models.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*-
 # This file is auto-generated, don't edit it. Thanks.
 from Tea.model import TeaModel
 from typing import Dict
 
 
-class CountWorkRecordHeaders(TeaModel):
+class SaveOpenExternalLogHeaders(TeaModel):
     def __init__(
         self,
         common_headers: Dict[str, str] = None,
         x_acs_dingtalk_access_token: str = None,
     ):
         self.common_headers = common_headers
         self.x_acs_dingtalk_access_token = x_acs_dingtalk_access_token
@@ -33,74 +33,92 @@
         if m.get('commonHeaders') is not None:
             self.common_headers = m.get('commonHeaders')
         if m.get('x-acs-dingtalk-access-token') is not None:
             self.x_acs_dingtalk_access_token = m.get('x-acs-dingtalk-access-token')
         return self
 
 
-class CountWorkRecordRequest(TeaModel):
+class SaveOpenExternalLogRequest(TeaModel):
     def __init__(
         self,
-        user_id: str = None,
+        corp_id: str = None,
+        log_source: str = None,
+        log_type: str = None,
+        open_ext: str = None,
     ):
-        self.user_id = user_id
+        self.corp_id = corp_id
+        self.log_source = log_source
+        self.log_type = log_type
+        self.open_ext = open_ext
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.user_id is not None:
-            result['userId'] = self.user_id
+        if self.corp_id is not None:
+            result['corpId'] = self.corp_id
+        if self.log_source is not None:
+            result['logSource'] = self.log_source
+        if self.log_type is not None:
+            result['logType'] = self.log_type
+        if self.open_ext is not None:
+            result['openExt'] = self.open_ext
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('userId') is not None:
-            self.user_id = m.get('userId')
+        if m.get('corpId') is not None:
+            self.corp_id = m.get('corpId')
+        if m.get('logSource') is not None:
+            self.log_source = m.get('logSource')
+        if m.get('logType') is not None:
+            self.log_type = m.get('logType')
+        if m.get('openExt') is not None:
+            self.open_ext = m.get('openExt')
         return self
 
 
-class CountWorkRecordResponseBody(TeaModel):
+class SaveOpenExternalLogResponseBody(TeaModel):
     def __init__(
         self,
-        undo_count: int = None,
+        success: bool = None,
     ):
-        self.undo_count = undo_count
+        self.success = success
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.undo_count is not None:
-            result['undoCount'] = self.undo_count
+        if self.success is not None:
+            result['success'] = self.success
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('undoCount') is not None:
-            self.undo_count = m.get('undoCount')
+        if m.get('success') is not None:
+            self.success = m.get('success')
         return self
 
 
-class CountWorkRecordResponse(TeaModel):
+class SaveOpenExternalLogResponse(TeaModel):
     def __init__(
         self,
         headers: Dict[str, str] = None,
         status_code: int = None,
-        body: CountWorkRecordResponseBody = None,
+        body: SaveOpenExternalLogResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
@@ -126,12 +144,12 @@
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('headers') is not None:
             self.headers = m.get('headers')
         if m.get('statusCode') is not None:
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
-            temp_model = CountWorkRecordResponseBody()
+            temp_model = SaveOpenExternalLogResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
```

### Comparing `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/yida_1_0/client.py` & `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/yida_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/yida_1_0/models.py` & `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk/yida_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk.egg-info/PKG-INFO` & `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-dingtalk
-Version: 2.0.21
+Version: 2.0.22
 Summary: Alibaba Cloud Dingtalk SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk.egg-info/SOURCES.txt` & `alibabacloud_dingtalk-2.0.22/alibabacloud_dingtalk.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -163,14 +163,17 @@
 alibabacloud_dingtalk/jzcrm_1_0/models.py
 alibabacloud_dingtalk/link_1_0/__init__.py
 alibabacloud_dingtalk/link_1_0/client.py
 alibabacloud_dingtalk/link_1_0/models.py
 alibabacloud_dingtalk/live_1_0/__init__.py
 alibabacloud_dingtalk/live_1_0/client.py
 alibabacloud_dingtalk/live_1_0/models.py
+alibabacloud_dingtalk/live_activities_1_0/__init__.py
+alibabacloud_dingtalk/live_activities_1_0/client.py
+alibabacloud_dingtalk/live_activities_1_0/models.py
 alibabacloud_dingtalk/manufacturing_1_0/__init__.py
 alibabacloud_dingtalk/manufacturing_1_0/client.py
 alibabacloud_dingtalk/manufacturing_1_0/models.py
 alibabacloud_dingtalk/micro_app_1_0/__init__.py
 alibabacloud_dingtalk/micro_app_1_0/client.py
 alibabacloud_dingtalk/micro_app_1_0/models.py
 alibabacloud_dingtalk/miniapp_1_0/__init__.py
```

### Comparing `alibabacloud_dingtalk-2.0.21/setup.py` & `alibabacloud_dingtalk-2.0.22/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,29 +20,29 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_dingtalk.
 
-Created on 16/06/2023
+Created on 05/07/2023
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_dingtalk"
 NAME = "alibabacloud_dingtalk" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud Dingtalk SDK Library for Python"
 AUTHOR = "Alibaba Cloud SDK"
 AUTHOR_EMAIL = "sdk-team@alibabacloud.com"
 URL = "https://github.com/aliyun/alibabacloud-sdk"
 VERSION = __import__(PACKAGE).__version__
 REQUIRES = [
     "alibabacloud_tea_openapi>=0.3.6, <1.0.0",
-    "alibabacloud_tea_util>=0.3.8, <1.0.0",
+    "alibabacloud_tea_util>=0.3.9, <1.0.0",
     "alibabacloud_openapi_util>=0.2.1, <1.0.0",
     "alibabacloud_endpoint_util>=0.0.3, <1.0.0",
     "alibabacloud_gateway_spi>=0.0.1, <1.0.0",
     "alibabacloud_gateway_dingtalk>=1.0.2, <2.0.0"
 ]
 
 LONG_DESCRIPTION = ''
```

