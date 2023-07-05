# Comparing `tmp/wedeliver_core_plus-0.0.7.tar.gz` & `tmp/wedeliver_core_plus-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/platformLibraries/platformLibraries/wedeliver_core_plus/dist/.tmp-ux8tjy38/wedeliver_core_plus-0.0.7.tar", last modified: Wed Jun 21 11:06:12 2023, max compression
+gzip compressed data, was "/home/runner/work/platformLibraries/platformLibraries/wedeliver_core_plus/dist/.tmp-z837u9w0/wedeliver_core_plus-0.0.8.tar", last modified: Wed Jul  5 12:02:46 2023, max compression
```

## Comparing `wedeliver_core_plus-0.0.7.tar` & `wedeliver_core_plus-0.0.8.tar`

### file list

```diff
@@ -1,68 +1,68 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-21 11:06:12.000000 wedeliver_core_plus-0.0.7/
--rw-r--r--   0 runner    (1001) docker     (122)      773 2023-06-21 11:06:12.000000 wedeliver_core_plus-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-21 11:06:12.000000 wedeliver_core_plus-0.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1368 2023-06-21 11:05:56.000000 wedeliver_core_plus-0.0.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-21 11:06:12.000000 wedeliver_core_plus-0.0.7/wedeliver_core_plus/
--rw-r--r--   0 runner    (1001) docker     (122)      893 2023-06-21 11:05:56.000000 wedeliver_core_plus-0.0.7/wedeliver_core_plus/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-21 11:06:12.000000 wedeliver_core_plus-0.0.7/wedeliver_core_plus/app_decorators/
--rw-r--r--   0 runner    (1001) docker     (122)      247 2023-06-21 11:05:56.000000 wedeliver_core_plus-0.0.7/wedeliver_core_plus/app_decorators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1012 2023-06-21 11:05:56.000000 wedeliver_core_plus-0.0.7/wedeliver_core_plus/app_decorators/app_entry.py
--rw-r--r--   0 runner    (1001) docker     (122)     2272 2023-06-21 11:05:56.000000 wedeliver_core_plus-0.0.7/wedeliver_core_plus/app_decorators/handle_auth.py
--rw-r--r--   0 runner    (1001) docker     (122)     2374 2023-06-21 11:05:56.000000 wedeliver_core_plus-0.0.7/wedeliver_core_plus/app_decorators/handle_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (122)      786 2023-06-21 11:05:56.000000 wedeliver_core_plus-0.0.7/wedeliver_core_plus/app_decorators/handle_response.py
--rw-r--r--   0 runner    (1001) docker     (122)     4721 2023-06-21 11:05:56.000000 wedeliver_core_plus-0.0.7/wedeliver_core_plus/app_decorators/serializer.py
--rw-r--r--   0 runner    (1001) docker     (122)     2404 2023-06-21 11:05:56.000000 wedeliver_core_plus-0.0.7/wedeliver_core_plus/base.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-21 11:06:12.000000 wedeliver_core_plus-0.0.7/wedeliver_core_plus/helpers/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-21 11:05:56.000000 wedeliver_core_plus-0.0.7/wedeliver_core_plus/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      855 2023-06-21 11:05:56.000000 wedeliver_core_plus-0.0.7/wedeliver_core_plus/helpers/acl_enum.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-21 11:06:12.000000 wedeliver_core_plus-0.0.7/wedeliver_core_plus/helpers/amazon/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-21 11:05:56.000000 wedeliver_core_plus-0.0.7/wedeliver_core_plus/helpers/amazon/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      593 2023-06-21 11:05:56.000000 wedeliver_core_plus-0.0.7/wedeliver_core_plus/helpers/amazon/append_plain_urls_to_list_dict.py
--rw-r--r--   0 runner    (1001) docker     (122)     1365 2023-06-21 11:05:56.000000 wedeliver_core_plus-0.0.7/wedeliver_core_plus/helpers/amazon/get_file_url.py
--rw-r--r--   0 runner    (1001) docker     (122)      318 2023-06-21 11:05:56.000000 wedeliver_core_plus-0.0.7/wedeliver_core_plus/helpers/amazon/get_plain_url.py
--rw-r--r--   0 runner    (1001) docker     (122)     1607 2023-06-21 11:05:56.000000 wedeliver_core_plus-0.0.7/wedeliver_core_plus/helpers/amazon/get_s3_client.py
--rw-r--r--   0 runner    (1001) docker     (122)      590 2023-06-21 11:05:56.000000 wedeliver_core_plus-0.0.7/wedeliver_core_plus/helpers/amazon/upload_file.py
--rw-r--r--   0 runner    (1001) docker     (122)      852 2023-06-21 11:05:56.000000 wedeliver_core_plus-0.0.7/wedeliver_core_plus/helpers/atomic_transactions.py
--rw-r--r--   0 runner    (1001) docker     (122)      940 2023-06-21 11:05:56.000000 wedeliver_core_plus-0.0.7/wedeliver_core_plus/helpers/atomic_transactions_v2.py
--rw-r--r--   0 runner    (1001) docker     (122)     1844 2023-06-21 11:05:56.000000 wedeliver_core_plus-0.0.7/wedeliver_core_plus/helpers/auth.py
--rw-r--r--   0 runner    (1001) docker     (122)     1316 2023-06-21 11:05:56.000000 wedeliver_core_plus-0.0.7/wedeliver_core_plus/helpers/config.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-21 11:06:12.000000 wedeliver_core_plus-0.0.7/wedeliver_core_plus/helpers/database/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-21 11:05:56.000000 wedeliver_core_plus-0.0.7/wedeliver_core_plus/helpers/database/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      703 2023-06-21 11:05:56.000000 wedeliver_core_plus-0.0.7/wedeliver_core_plus/helpers/database/base_model.py
--rw-r--r--   0 runner    (1001) docker     (122)     4418 2023-06-21 11:05:56.000000 wedeliver_core_plus-0.0.7/wedeliver_core_plus/helpers/database/log_model.py
--rw-r--r--   0 runner    (1001) docker     (122)     2251 2023-06-21 11:05:56.000000 wedeliver_core_plus-0.0.7/wedeliver_core_plus/helpers/enums.py
--rw-r--r--   0 runner    (1001) docker     (122)     1092 2023-06-21 11:05:56.000000 wedeliver_core_plus-0.0.7/wedeliver_core_plus/helpers/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (122)     3719 2023-06-21 11:05:56.000000 wedeliver_core_plus-0.0.7/wedeliver_core_plus/helpers/fetch_relational_data.py
--rw-r--r--   0 runner    (1001) docker     (122)     4730 2023-06-21 11:05:56.000000 wedeliver_core_plus-0.0.7/wedeliver_core_plus/helpers/filters.py
--rw-r--r--   0 runner    (1001) docker     (122)     2202 2023-06-21 11:05:56.000000 wedeliver_core_plus-0.0.7/wedeliver_core_plus/helpers/format_exception.py
--rw-r--r--   0 runner    (1001) docker     (122)      385 2023-06-21 11:05:56.000000 wedeliver_core_plus-0.0.7/wedeliver_core_plus/helpers/get_callback.py
--rw-r--r--   0 runner    (1001) docker     (122)      223 2023-06-21 11:05:56.000000 wedeliver_core_plus-0.0.7/wedeliver_core_plus/helpers/get_country_code.py
--rw-r--r--   0 runner    (1001) docker     (122)      629 2023-06-21 11:05:56.000000 wedeliver_core_plus-0.0.7/wedeliver_core_plus/helpers/get_embedded_function.py
--rw-r--r--   0 runner    (1001) docker     (122)      424 2023-06-21 11:05:56.000000 wedeliver_core_plus-0.0.7/wedeliver_core_plus/helpers/get_obj_value.py
--rw-r--r--   0 runner    (1001) docker     (122)      342 2023-06-21 11:05:56.000000 wedeliver_core_plus-0.0.7/wedeliver_core_plus/helpers/get_prefix.py
--rw-r--r--   0 runner    (1001) docker     (122)     2768 2023-06-21 11:05:56.000000 wedeliver_core_plus-0.0.7/wedeliver_core_plus/helpers/kafka_listener.py
--rw-r--r--   0 runner    (1001) docker     (122)     3056 2023-06-21 11:05:56.000000 wedeliver_core_plus-0.0.7/wedeliver_core_plus/helpers/kafka_producer.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-21 11:06:12.000000 wedeliver_core_plus-0.0.7/wedeliver_core_plus/helpers/kafka_producers/
--rw-r--r--   0 runner    (1001) docker     (122)      378 2023-06-21 11:05:56.000000 wedeliver_core_plus-0.0.7/wedeliver_core_plus/helpers/kafka_producers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      451 2023-06-21 11:05:56.000000 wedeliver_core_plus-0.0.7/wedeliver_core_plus/helpers/kafka_producers/log_model_changes.py
--rw-r--r--   0 runner    (1001) docker     (122)     2098 2023-06-21 11:05:56.000000 wedeliver_core_plus-0.0.7/wedeliver_core_plus/helpers/kafka_producers/notification_center.py
--rw-r--r--   0 runner    (1001) docker     (122)      292 2023-06-21 11:05:56.000000 wedeliver_core_plus-0.0.7/wedeliver_core_plus/helpers/kafka_producers/send_sms.py
--rw-r--r--   0 runner    (1001) docker     (122)      322 2023-06-21 11:05:56.000000 wedeliver_core_plus-0.0.7/wedeliver_core_plus/helpers/kafka_producers/send_topic.py
--rw-r--r--   0 runner    (1001) docker     (122)     2007 2023-06-21 11:05:56.000000 wedeliver_core_plus-0.0.7/wedeliver_core_plus/helpers/log_config.py
--rw-r--r--   0 runner    (1001) docker     (122)    12487 2023-06-21 11:05:56.000000 wedeliver_core_plus-0.0.7/wedeliver_core_plus/helpers/micro_fetcher.py
--rw-r--r--   0 runner    (1001) docker     (122)      128 2023-06-21 11:05:56.000000 wedeliver_core_plus-0.0.7/wedeliver_core_plus/helpers/numbers.py
--rw-r--r--   0 runner    (1001) docker     (122)     4284 2023-06-21 11:05:56.000000 wedeliver_core_plus-0.0.7/wedeliver_core_plus/helpers/search_function.py
--rw-r--r--   0 runner    (1001) docker     (122)     2021 2023-06-21 11:05:56.000000 wedeliver_core_plus-0.0.7/wedeliver_core_plus/helpers/security.py
--rw-r--r--   0 runner    (1001) docker     (122)      663 2023-06-21 11:05:56.000000 wedeliver_core_plus-0.0.7/wedeliver_core_plus/helpers/service_config.py
--rw-r--r--   0 runner    (1001) docker     (122)      850 2023-06-21 11:05:56.000000 wedeliver_core_plus-0.0.7/wedeliver_core_plus/helpers/sql.py
--rw-r--r--   0 runner    (1001) docker     (122)      139 2023-06-21 11:05:56.000000 wedeliver_core_plus-0.0.7/wedeliver_core_plus/helpers/system_roles.py
--rw-r--r--   0 runner    (1001) docker     (122)     7639 2023-06-21 11:05:56.000000 wedeliver_core_plus-0.0.7/wedeliver_core_plus/helpers/time.py
--rw-r--r--   0 runner    (1001) docker     (122)      629 2023-06-21 11:05:56.000000 wedeliver_core_plus-0.0.7/wedeliver_core_plus/helpers/topics.py
--rw-r--r--   0 runner    (1001) docker     (122)     1205 2023-06-21 11:05:56.000000 wedeliver_core_plus-0.0.7/wedeliver_core_plus/helpers/validate_mobile_number.py
--rw-r--r--   0 runner    (1001) docker     (122)     1002 2023-06-21 11:05:56.000000 wedeliver_core_plus-0.0.7/wedeliver_core_plus/helpers/validate_parameters.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-21 11:06:12.000000 wedeliver_core_plus-0.0.7/wedeliver_core_plus.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)      773 2023-06-21 11:06:12.000000 wedeliver_core_plus-0.0.7/wedeliver_core_plus.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     2678 2023-06-21 11:06:12.000000 wedeliver_core_plus-0.0.7/wedeliver_core_plus.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-21 11:06:12.000000 wedeliver_core_plus-0.0.7/wedeliver_core_plus.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       85 2023-06-21 11:06:12.000000 wedeliver_core_plus-0.0.7/wedeliver_core_plus.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       20 2023-06-21 11:06:12.000000 wedeliver_core_plus-0.0.7/wedeliver_core_plus.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 12:02:46.000000 wedeliver_core_plus-0.0.8/
+-rw-r--r--   0 runner    (1001) docker     (122)      773 2023-07-05 12:02:46.000000 wedeliver_core_plus-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-05 12:02:46.000000 wedeliver_core_plus-0.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1368 2023-07-05 12:02:37.000000 wedeliver_core_plus-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 12:02:46.000000 wedeliver_core_plus-0.0.8/wedeliver_core_plus/
+-rw-r--r--   0 runner    (1001) docker     (122)      893 2023-07-05 12:02:37.000000 wedeliver_core_plus-0.0.8/wedeliver_core_plus/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 12:02:46.000000 wedeliver_core_plus-0.0.8/wedeliver_core_plus/app_decorators/
+-rw-r--r--   0 runner    (1001) docker     (122)      247 2023-07-05 12:02:37.000000 wedeliver_core_plus-0.0.8/wedeliver_core_plus/app_decorators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1012 2023-07-05 12:02:37.000000 wedeliver_core_plus-0.0.8/wedeliver_core_plus/app_decorators/app_entry.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2272 2023-07-05 12:02:37.000000 wedeliver_core_plus-0.0.8/wedeliver_core_plus/app_decorators/handle_auth.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2374 2023-07-05 12:02:37.000000 wedeliver_core_plus-0.0.8/wedeliver_core_plus/app_decorators/handle_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)      786 2023-07-05 12:02:37.000000 wedeliver_core_plus-0.0.8/wedeliver_core_plus/app_decorators/handle_response.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4721 2023-07-05 12:02:37.000000 wedeliver_core_plus-0.0.8/wedeliver_core_plus/app_decorators/serializer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2404 2023-07-05 12:02:37.000000 wedeliver_core_plus-0.0.8/wedeliver_core_plus/base.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 12:02:46.000000 wedeliver_core_plus-0.0.8/wedeliver_core_plus/helpers/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-05 12:02:37.000000 wedeliver_core_plus-0.0.8/wedeliver_core_plus/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      855 2023-07-05 12:02:37.000000 wedeliver_core_plus-0.0.8/wedeliver_core_plus/helpers/acl_enum.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 12:02:46.000000 wedeliver_core_plus-0.0.8/wedeliver_core_plus/helpers/amazon/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-05 12:02:37.000000 wedeliver_core_plus-0.0.8/wedeliver_core_plus/helpers/amazon/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      593 2023-07-05 12:02:37.000000 wedeliver_core_plus-0.0.8/wedeliver_core_plus/helpers/amazon/append_plain_urls_to_list_dict.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1855 2023-07-05 12:02:37.000000 wedeliver_core_plus-0.0.8/wedeliver_core_plus/helpers/amazon/get_file_url.py
+-rw-r--r--   0 runner    (1001) docker     (122)      318 2023-07-05 12:02:37.000000 wedeliver_core_plus-0.0.8/wedeliver_core_plus/helpers/amazon/get_plain_url.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1607 2023-07-05 12:02:37.000000 wedeliver_core_plus-0.0.8/wedeliver_core_plus/helpers/amazon/get_s3_client.py
+-rw-r--r--   0 runner    (1001) docker     (122)      590 2023-07-05 12:02:37.000000 wedeliver_core_plus-0.0.8/wedeliver_core_plus/helpers/amazon/upload_file.py
+-rw-r--r--   0 runner    (1001) docker     (122)      852 2023-07-05 12:02:37.000000 wedeliver_core_plus-0.0.8/wedeliver_core_plus/helpers/atomic_transactions.py
+-rw-r--r--   0 runner    (1001) docker     (122)      940 2023-07-05 12:02:37.000000 wedeliver_core_plus-0.0.8/wedeliver_core_plus/helpers/atomic_transactions_v2.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1844 2023-07-05 12:02:37.000000 wedeliver_core_plus-0.0.8/wedeliver_core_plus/helpers/auth.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1316 2023-07-05 12:02:37.000000 wedeliver_core_plus-0.0.8/wedeliver_core_plus/helpers/config.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 12:02:46.000000 wedeliver_core_plus-0.0.8/wedeliver_core_plus/helpers/database/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-05 12:02:37.000000 wedeliver_core_plus-0.0.8/wedeliver_core_plus/helpers/database/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      703 2023-07-05 12:02:37.000000 wedeliver_core_plus-0.0.8/wedeliver_core_plus/helpers/database/base_model.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4418 2023-07-05 12:02:37.000000 wedeliver_core_plus-0.0.8/wedeliver_core_plus/helpers/database/log_model.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2251 2023-07-05 12:02:37.000000 wedeliver_core_plus-0.0.8/wedeliver_core_plus/helpers/enums.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1092 2023-07-05 12:02:37.000000 wedeliver_core_plus-0.0.8/wedeliver_core_plus/helpers/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3719 2023-07-05 12:02:37.000000 wedeliver_core_plus-0.0.8/wedeliver_core_plus/helpers/fetch_relational_data.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4730 2023-07-05 12:02:37.000000 wedeliver_core_plus-0.0.8/wedeliver_core_plus/helpers/filters.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2202 2023-07-05 12:02:37.000000 wedeliver_core_plus-0.0.8/wedeliver_core_plus/helpers/format_exception.py
+-rw-r--r--   0 runner    (1001) docker     (122)      385 2023-07-05 12:02:37.000000 wedeliver_core_plus-0.0.8/wedeliver_core_plus/helpers/get_callback.py
+-rw-r--r--   0 runner    (1001) docker     (122)      223 2023-07-05 12:02:37.000000 wedeliver_core_plus-0.0.8/wedeliver_core_plus/helpers/get_country_code.py
+-rw-r--r--   0 runner    (1001) docker     (122)      629 2023-07-05 12:02:37.000000 wedeliver_core_plus-0.0.8/wedeliver_core_plus/helpers/get_embedded_function.py
+-rw-r--r--   0 runner    (1001) docker     (122)      424 2023-07-05 12:02:37.000000 wedeliver_core_plus-0.0.8/wedeliver_core_plus/helpers/get_obj_value.py
+-rw-r--r--   0 runner    (1001) docker     (122)      342 2023-07-05 12:02:37.000000 wedeliver_core_plus-0.0.8/wedeliver_core_plus/helpers/get_prefix.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2768 2023-07-05 12:02:37.000000 wedeliver_core_plus-0.0.8/wedeliver_core_plus/helpers/kafka_listener.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3056 2023-07-05 12:02:37.000000 wedeliver_core_plus-0.0.8/wedeliver_core_plus/helpers/kafka_producer.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 12:02:46.000000 wedeliver_core_plus-0.0.8/wedeliver_core_plus/helpers/kafka_producers/
+-rw-r--r--   0 runner    (1001) docker     (122)      378 2023-07-05 12:02:37.000000 wedeliver_core_plus-0.0.8/wedeliver_core_plus/helpers/kafka_producers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      451 2023-07-05 12:02:37.000000 wedeliver_core_plus-0.0.8/wedeliver_core_plus/helpers/kafka_producers/log_model_changes.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2098 2023-07-05 12:02:37.000000 wedeliver_core_plus-0.0.8/wedeliver_core_plus/helpers/kafka_producers/notification_center.py
+-rw-r--r--   0 runner    (1001) docker     (122)      292 2023-07-05 12:02:37.000000 wedeliver_core_plus-0.0.8/wedeliver_core_plus/helpers/kafka_producers/send_sms.py
+-rw-r--r--   0 runner    (1001) docker     (122)      322 2023-07-05 12:02:37.000000 wedeliver_core_plus-0.0.8/wedeliver_core_plus/helpers/kafka_producers/send_topic.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2007 2023-07-05 12:02:37.000000 wedeliver_core_plus-0.0.8/wedeliver_core_plus/helpers/log_config.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12487 2023-07-05 12:02:37.000000 wedeliver_core_plus-0.0.8/wedeliver_core_plus/helpers/micro_fetcher.py
+-rw-r--r--   0 runner    (1001) docker     (122)      128 2023-07-05 12:02:37.000000 wedeliver_core_plus-0.0.8/wedeliver_core_plus/helpers/numbers.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4284 2023-07-05 12:02:37.000000 wedeliver_core_plus-0.0.8/wedeliver_core_plus/helpers/search_function.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2021 2023-07-05 12:02:37.000000 wedeliver_core_plus-0.0.8/wedeliver_core_plus/helpers/security.py
+-rw-r--r--   0 runner    (1001) docker     (122)      663 2023-07-05 12:02:37.000000 wedeliver_core_plus-0.0.8/wedeliver_core_plus/helpers/service_config.py
+-rw-r--r--   0 runner    (1001) docker     (122)      850 2023-07-05 12:02:37.000000 wedeliver_core_plus-0.0.8/wedeliver_core_plus/helpers/sql.py
+-rw-r--r--   0 runner    (1001) docker     (122)      139 2023-07-05 12:02:37.000000 wedeliver_core_plus-0.0.8/wedeliver_core_plus/helpers/system_roles.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7639 2023-07-05 12:02:37.000000 wedeliver_core_plus-0.0.8/wedeliver_core_plus/helpers/time.py
+-rw-r--r--   0 runner    (1001) docker     (122)      629 2023-07-05 12:02:37.000000 wedeliver_core_plus-0.0.8/wedeliver_core_plus/helpers/topics.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1205 2023-07-05 12:02:37.000000 wedeliver_core_plus-0.0.8/wedeliver_core_plus/helpers/validate_mobile_number.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1002 2023-07-05 12:02:37.000000 wedeliver_core_plus-0.0.8/wedeliver_core_plus/helpers/validate_parameters.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 12:02:46.000000 wedeliver_core_plus-0.0.8/wedeliver_core_plus.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)      773 2023-07-05 12:02:46.000000 wedeliver_core_plus-0.0.8/wedeliver_core_plus.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     2678 2023-07-05 12:02:46.000000 wedeliver_core_plus-0.0.8/wedeliver_core_plus.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-05 12:02:46.000000 wedeliver_core_plus-0.0.8/wedeliver_core_plus.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       85 2023-07-05 12:02:46.000000 wedeliver_core_plus-0.0.8/wedeliver_core_plus.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       20 2023-07-05 12:02:46.000000 wedeliver_core_plus-0.0.8/wedeliver_core_plus.egg-info/top_level.txt
```

### Comparing `wedeliver_core_plus-0.0.7/PKG-INFO` & `wedeliver_core_plus-0.0.8/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wedeliver_core_plus
-Version: 0.0.7
+Version: 0.0.8
 Summary: wedeliver_core_plus package
 Home-page: https://www.wedeliverapp.com/
 Author: Eyad Farra
 Author-email: info@wedeliverapp.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `wedeliver_core_plus-0.0.7/setup.py` & `wedeliver_core_plus-0.0.8/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     "Programming Language :: Python :: 3.4",
     "Programming Language :: Python :: 3.5",
     "Programming Language :: Python :: 3.6",
 ]
 
 setup(
     name="wedeliver_core_plus",
-    version="0.0.7",
+    version="0.0.8",
     description="wedeliver_core_plus package",
     long_description="""# Markdown supported!\n\n* wedeliver core plus\n* List of features\n""",
     long_description_content_type="text/markdown",
     url="https://www.wedeliverapp.com/",
     author="Eyad Farra",
     author_email="info@wedeliverapp.com",
     license="MIT",
```

### Comparing `wedeliver_core_plus-0.0.7/wedeliver_core_plus/__init__.py` & `wedeliver_core_plus-0.0.8/wedeliver_core_plus/__init__.py`

 * *Files identical despite different names*

### Comparing `wedeliver_core_plus-0.0.7/wedeliver_core_plus/app_decorators/app_entry.py` & `wedeliver_core_plus-0.0.8/wedeliver_core_plus/app_decorators/app_entry.py`

 * *Files identical despite different names*

### Comparing `wedeliver_core_plus-0.0.7/wedeliver_core_plus/app_decorators/handle_auth.py` & `wedeliver_core_plus-0.0.8/wedeliver_core_plus/app_decorators/handle_auth.py`

 * *Files identical despite different names*

### Comparing `wedeliver_core_plus-0.0.7/wedeliver_core_plus/app_decorators/handle_exceptions.py` & `wedeliver_core_plus-0.0.8/wedeliver_core_plus/app_decorators/handle_exceptions.py`

 * *Files identical despite different names*

### Comparing `wedeliver_core_plus-0.0.7/wedeliver_core_plus/app_decorators/handle_response.py` & `wedeliver_core_plus-0.0.8/wedeliver_core_plus/app_decorators/handle_response.py`

 * *Files identical despite different names*

### Comparing `wedeliver_core_plus-0.0.7/wedeliver_core_plus/app_decorators/serializer.py` & `wedeliver_core_plus-0.0.8/wedeliver_core_plus/app_decorators/serializer.py`

 * *Files identical despite different names*

### Comparing `wedeliver_core_plus-0.0.7/wedeliver_core_plus/base.py` & `wedeliver_core_plus-0.0.8/wedeliver_core_plus/base.py`

 * *Files identical despite different names*

### Comparing `wedeliver_core_plus-0.0.7/wedeliver_core_plus/helpers/acl_enum.py` & `wedeliver_core_plus-0.0.8/wedeliver_core_plus/helpers/acl_enum.py`

 * *Files identical despite different names*

### Comparing `wedeliver_core_plus-0.0.7/wedeliver_core_plus/helpers/amazon/append_plain_urls_to_list_dict.py` & `wedeliver_core_plus-0.0.8/wedeliver_core_plus/helpers/amazon/append_plain_urls_to_list_dict.py`

 * *Files identical despite different names*

### Comparing `wedeliver_core_plus-0.0.7/wedeliver_core_plus/helpers/amazon/get_file_url.py` & `wedeliver_core_plus-0.0.8/wedeliver_core_plus/helpers/amazon/get_file_url.py`

 * *Files 20% similar despite different names*

```diff
@@ -17,15 +17,15 @@
         s3_path = "https://{}/{}".format(app.config.get("S3_BUCKET"), s3_path)
 
     path_parts = s3_path.replace("https://", "").split("/")
     bucket = path_parts.pop(0).split(".").pop(0)
     key = "/".join(path_parts)
 
     response = None
-    s3_client = None
+    # s3_client = None
     try:
         s3_client = s3_client or get_s3_client()
         response = s3_client.generate_presigned_url(
             "get_object",
             Params={"Bucket": bucket, "Key": key},
             ExpiresIn=int(timedelta(minutes=expiration_minutes).total_seconds()),
         )
@@ -33,13 +33,26 @@
         app.logger.error(str(e))
 
     # The response contains the presigned URL
     app.logger.debug(response)
     return response
 
 
+def get_file_url_bulk(list_dict, key_name, s3_client=None):
+    """
+    This function will append plain url to list of dictionaries
+    :param list_dict: list of dictionaries
+    :param key_name: key name to append plain url to
+    :param s3_client: s3 client
+    :return: list of dictionaries
+    """
+    s3_client = s3_client or get_s3_client()
+    for item in list_dict:
+        item[key_name] = get_file_url(item.get(key_name), s3_client=s3_client)
+    return list_dict
+
 if __name__ == "__main__":
     url = get_file_url(
         s3_path="owner_national_attachment/1660823074_ihbxlpymqxxjuzrqom.jpe"
         # s3_path="https://dev-wedeliver-slips.s3.eu-west-1.amazonaws.com/development/PS/images/cad3b9038e021648.jpg"
     )
     test = url
```

### Comparing `wedeliver_core_plus-0.0.7/wedeliver_core_plus/helpers/amazon/get_s3_client.py` & `wedeliver_core_plus-0.0.8/wedeliver_core_plus/helpers/amazon/get_s3_client.py`

 * *Files identical despite different names*

### Comparing `wedeliver_core_plus-0.0.7/wedeliver_core_plus/helpers/amazon/upload_file.py` & `wedeliver_core_plus-0.0.8/wedeliver_core_plus/helpers/amazon/upload_file.py`

 * *Files identical despite different names*

### Comparing `wedeliver_core_plus-0.0.7/wedeliver_core_plus/helpers/atomic_transactions.py` & `wedeliver_core_plus-0.0.8/wedeliver_core_plus/helpers/atomic_transactions.py`

 * *Files identical despite different names*

### Comparing `wedeliver_core_plus-0.0.7/wedeliver_core_plus/helpers/atomic_transactions_v2.py` & `wedeliver_core_plus-0.0.8/wedeliver_core_plus/helpers/atomic_transactions_v2.py`

 * *Files identical despite different names*

### Comparing `wedeliver_core_plus-0.0.7/wedeliver_core_plus/helpers/auth.py` & `wedeliver_core_plus-0.0.8/wedeliver_core_plus/helpers/auth.py`

 * *Files identical despite different names*

### Comparing `wedeliver_core_plus-0.0.7/wedeliver_core_plus/helpers/config.py` & `wedeliver_core_plus-0.0.8/wedeliver_core_plus/helpers/config.py`

 * *Files identical despite different names*

### Comparing `wedeliver_core_plus-0.0.7/wedeliver_core_plus/helpers/database/base_model.py` & `wedeliver_core_plus-0.0.8/wedeliver_core_plus/helpers/database/base_model.py`

 * *Files identical despite different names*

### Comparing `wedeliver_core_plus-0.0.7/wedeliver_core_plus/helpers/database/log_model.py` & `wedeliver_core_plus-0.0.8/wedeliver_core_plus/helpers/database/log_model.py`

 * *Files identical despite different names*

### Comparing `wedeliver_core_plus-0.0.7/wedeliver_core_plus/helpers/enums.py` & `wedeliver_core_plus-0.0.8/wedeliver_core_plus/helpers/enums.py`

 * *Files identical despite different names*

### Comparing `wedeliver_core_plus-0.0.7/wedeliver_core_plus/helpers/exceptions.py` & `wedeliver_core_plus-0.0.8/wedeliver_core_plus/helpers/exceptions.py`

 * *Files identical despite different names*

### Comparing `wedeliver_core_plus-0.0.7/wedeliver_core_plus/helpers/fetch_relational_data.py` & `wedeliver_core_plus-0.0.8/wedeliver_core_plus/helpers/fetch_relational_data.py`

 * *Files identical despite different names*

### Comparing `wedeliver_core_plus-0.0.7/wedeliver_core_plus/helpers/filters.py` & `wedeliver_core_plus-0.0.8/wedeliver_core_plus/helpers/filters.py`

 * *Files identical despite different names*

### Comparing `wedeliver_core_plus-0.0.7/wedeliver_core_plus/helpers/format_exception.py` & `wedeliver_core_plus-0.0.8/wedeliver_core_plus/helpers/format_exception.py`

 * *Files identical despite different names*

### Comparing `wedeliver_core_plus-0.0.7/wedeliver_core_plus/helpers/get_embedded_function.py` & `wedeliver_core_plus-0.0.8/wedeliver_core_plus/helpers/get_embedded_function.py`

 * *Files identical despite different names*

### Comparing `wedeliver_core_plus-0.0.7/wedeliver_core_plus/helpers/kafka_listener.py` & `wedeliver_core_plus-0.0.8/wedeliver_core_plus/helpers/kafka_listener.py`

 * *Files identical despite different names*

### Comparing `wedeliver_core_plus-0.0.7/wedeliver_core_plus/helpers/kafka_producer.py` & `wedeliver_core_plus-0.0.8/wedeliver_core_plus/helpers/kafka_producer.py`

 * *Files identical despite different names*

### Comparing `wedeliver_core_plus-0.0.7/wedeliver_core_plus/helpers/kafka_producers/notification_center.py` & `wedeliver_core_plus-0.0.8/wedeliver_core_plus/helpers/kafka_producers/notification_center.py`

 * *Files identical despite different names*

### Comparing `wedeliver_core_plus-0.0.7/wedeliver_core_plus/helpers/log_config.py` & `wedeliver_core_plus-0.0.8/wedeliver_core_plus/helpers/log_config.py`

 * *Files identical despite different names*

### Comparing `wedeliver_core_plus-0.0.7/wedeliver_core_plus/helpers/micro_fetcher.py` & `wedeliver_core_plus-0.0.8/wedeliver_core_plus/helpers/micro_fetcher.py`

 * *Files identical despite different names*

### Comparing `wedeliver_core_plus-0.0.7/wedeliver_core_plus/helpers/search_function.py` & `wedeliver_core_plus-0.0.8/wedeliver_core_plus/helpers/search_function.py`

 * *Files identical despite different names*

### Comparing `wedeliver_core_plus-0.0.7/wedeliver_core_plus/helpers/security.py` & `wedeliver_core_plus-0.0.8/wedeliver_core_plus/helpers/security.py`

 * *Files identical despite different names*

### Comparing `wedeliver_core_plus-0.0.7/wedeliver_core_plus/helpers/service_config.py` & `wedeliver_core_plus-0.0.8/wedeliver_core_plus/helpers/service_config.py`

 * *Files identical despite different names*

### Comparing `wedeliver_core_plus-0.0.7/wedeliver_core_plus/helpers/sql.py` & `wedeliver_core_plus-0.0.8/wedeliver_core_plus/helpers/sql.py`

 * *Files identical despite different names*

### Comparing `wedeliver_core_plus-0.0.7/wedeliver_core_plus/helpers/time.py` & `wedeliver_core_plus-0.0.8/wedeliver_core_plus/helpers/time.py`

 * *Files identical despite different names*

### Comparing `wedeliver_core_plus-0.0.7/wedeliver_core_plus/helpers/topics.py` & `wedeliver_core_plus-0.0.8/wedeliver_core_plus/helpers/topics.py`

 * *Files identical despite different names*

### Comparing `wedeliver_core_plus-0.0.7/wedeliver_core_plus/helpers/validate_mobile_number.py` & `wedeliver_core_plus-0.0.8/wedeliver_core_plus/helpers/validate_mobile_number.py`

 * *Files identical despite different names*

### Comparing `wedeliver_core_plus-0.0.7/wedeliver_core_plus/helpers/validate_parameters.py` & `wedeliver_core_plus-0.0.8/wedeliver_core_plus/helpers/validate_parameters.py`

 * *Files identical despite different names*

### Comparing `wedeliver_core_plus-0.0.7/wedeliver_core_plus.egg-info/PKG-INFO` & `wedeliver_core_plus-0.0.8/wedeliver_core_plus.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wedeliver-core-plus
-Version: 0.0.7
+Version: 0.0.8
 Summary: wedeliver_core_plus package
 Home-page: https://www.wedeliverapp.com/
 Author: Eyad Farra
 Author-email: info@wedeliverapp.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `wedeliver_core_plus-0.0.7/wedeliver_core_plus.egg-info/SOURCES.txt` & `wedeliver_core_plus-0.0.8/wedeliver_core_plus.egg-info/SOURCES.txt`

 * *Files identical despite different names*

