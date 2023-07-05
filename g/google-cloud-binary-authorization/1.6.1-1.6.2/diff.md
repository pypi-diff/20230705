# Comparing `tmp/google-cloud-binary-authorization-1.6.1.tar.gz` & `tmp/google-cloud-binary-authorization-1.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-cloud-binary-authorization-1.6.1.tar", last modified: Mon Mar 27 14:59:48 2023, max compression
+gzip compressed data, was "google-cloud-binary-authorization-1.6.2.tar", last modified: Wed Jul  5 15:14:52 2023, max compression
```

## Comparing `google-cloud-binary-authorization-1.6.1.tar` & `google-cloud-binary-authorization-1.6.2.tar`

### file list

```diff
@@ -1,111 +1,111 @@
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:59:47.997533 google-cloud-binary-authorization-1.6.1/
--rw-rw-r--   0 root         (0)     1003    11358 2023-03-27 14:57:47.000000 google-cloud-binary-authorization-1.6.1/LICENSE
--rw-rw-r--   0 root         (0)     1003      860 2023-03-27 14:57:47.000000 google-cloud-binary-authorization-1.6.1/MANIFEST.in
--rw-r--r--   0 root         (0)     1003     4870 2023-03-27 14:59:47.997533 google-cloud-binary-authorization-1.6.1/PKG-INFO
--rw-rw-r--   0 root         (0)     1003     3916 2023-03-27 14:57:47.000000 google-cloud-binary-authorization-1.6.1/README.rst
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:59:47.981529 google-cloud-binary-authorization-1.6.1/google/
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:59:47.981529 google-cloud-binary-authorization-1.6.1/google/cloud/
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:59:47.985530 google-cloud-binary-authorization-1.6.1/google/cloud/binaryauthorization/
--rw-rw-r--   0 root         (0)     1003     2818 2023-03-27 14:57:47.000000 google-cloud-binary-authorization-1.6.1/google/cloud/binaryauthorization/__init__.py
--rw-rw-r--   0 root         (0)     1003      652 2023-03-27 14:57:47.000000 google-cloud-binary-authorization-1.6.1/google/cloud/binaryauthorization/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       94 2023-03-27 14:57:47.000000 google-cloud-binary-authorization-1.6.1/google/cloud/binaryauthorization/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:59:47.985530 google-cloud-binary-authorization-1.6.1/google/cloud/binaryauthorization_v1/
--rw-rw-r--   0 root         (0)     1003     2321 2023-03-27 14:57:47.000000 google-cloud-binary-authorization-1.6.1/google/cloud/binaryauthorization_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003     4934 2023-03-27 14:57:47.000000 google-cloud-binary-authorization-1.6.1/google/cloud/binaryauthorization_v1/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003      652 2023-03-27 14:57:47.000000 google-cloud-binary-authorization-1.6.1/google/cloud/binaryauthorization_v1/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       94 2023-03-27 14:57:47.000000 google-cloud-binary-authorization-1.6.1/google/cloud/binaryauthorization_v1/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:59:47.985530 google-cloud-binary-authorization-1.6.1/google/cloud/binaryauthorization_v1/services/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 14:57:47.000000 google-cloud-binary-authorization-1.6.1/google/cloud/binaryauthorization_v1/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:59:47.985530 google-cloud-binary-authorization-1.6.1/google/cloud/binaryauthorization_v1/services/binauthz_management_service_v1/
--rw-rw-r--   0 root         (0)     1003      821 2023-03-27 14:57:47.000000 google-cloud-binary-authorization-1.6.1/google/cloud/binaryauthorization_v1/services/binauthz_management_service_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003    46378 2023-03-27 14:57:47.000000 google-cloud-binary-authorization-1.6.1/google/cloud/binaryauthorization_v1/services/binauthz_management_service_v1/async_client.py
--rw-rw-r--   0 root         (0)     1003    54229 2023-03-27 14:57:47.000000 google-cloud-binary-authorization-1.6.1/google/cloud/binaryauthorization_v1/services/binauthz_management_service_v1/client.py
--rw-rw-r--   0 root         (0)     1003     5825 2023-03-27 14:57:47.000000 google-cloud-binary-authorization-1.6.1/google/cloud/binaryauthorization_v1/services/binauthz_management_service_v1/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:59:47.985530 google-cloud-binary-authorization-1.6.1/google/cloud/binaryauthorization_v1/services/binauthz_management_service_v1/transports/
--rw-rw-r--   0 root         (0)     1003     1603 2023-03-27 14:57:47.000000 google-cloud-binary-authorization-1.6.1/google/cloud/binaryauthorization_v1/services/binauthz_management_service_v1/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003    11002 2023-03-27 14:57:47.000000 google-cloud-binary-authorization-1.6.1/google/cloud/binaryauthorization_v1/services/binauthz_management_service_v1/transports/base.py
--rw-rw-r--   0 root         (0)     1003    20560 2023-03-27 14:57:47.000000 google-cloud-binary-authorization-1.6.1/google/cloud/binaryauthorization_v1/services/binauthz_management_service_v1/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    20945 2023-03-27 14:57:47.000000 google-cloud-binary-authorization-1.6.1/google/cloud/binaryauthorization_v1/services/binauthz_management_service_v1/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    42437 2023-03-27 14:57:47.000000 google-cloud-binary-authorization-1.6.1/google/cloud/binaryauthorization_v1/services/binauthz_management_service_v1/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:59:47.985530 google-cloud-binary-authorization-1.6.1/google/cloud/binaryauthorization_v1/services/system_policy_v1/
--rw-rw-r--   0 root         (0)     1003      769 2023-03-27 14:57:47.000000 google-cloud-binary-authorization-1.6.1/google/cloud/binaryauthorization_v1/services/system_policy_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003    13561 2023-03-27 14:57:47.000000 google-cloud-binary-authorization-1.6.1/google/cloud/binaryauthorization_v1/services/system_policy_v1/async_client.py
--rw-rw-r--   0 root         (0)     1003    22480 2023-03-27 14:57:47.000000 google-cloud-binary-authorization-1.6.1/google/cloud/binaryauthorization_v1/services/system_policy_v1/client.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:59:47.989531 google-cloud-binary-authorization-1.6.1/google/cloud/binaryauthorization_v1/services/system_policy_v1/transports/
--rw-rw-r--   0 root         (0)     1003     1400 2023-03-27 14:57:47.000000 google-cloud-binary-authorization-1.6.1/google/cloud/binaryauthorization_v1/services/system_policy_v1/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     6036 2023-03-27 14:57:47.000000 google-cloud-binary-authorization-1.6.1/google/cloud/binaryauthorization_v1/services/system_policy_v1/transports/base.py
--rw-rw-r--   0 root         (0)     1003    11769 2023-03-27 14:57:47.000000 google-cloud-binary-authorization-1.6.1/google/cloud/binaryauthorization_v1/services/system_policy_v1/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    11974 2023-03-27 14:57:47.000000 google-cloud-binary-authorization-1.6.1/google/cloud/binaryauthorization_v1/services/system_policy_v1/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    11980 2023-03-27 14:57:47.000000 google-cloud-binary-authorization-1.6.1/google/cloud/binaryauthorization_v1/services/system_policy_v1/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:59:47.989531 google-cloud-binary-authorization-1.6.1/google/cloud/binaryauthorization_v1/services/validation_helper_v1/
--rw-rw-r--   0 root         (0)     1003      785 2023-03-27 14:57:47.000000 google-cloud-binary-authorization-1.6.1/google/cloud/binaryauthorization_v1/services/validation_helper_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003    13060 2023-03-27 14:57:47.000000 google-cloud-binary-authorization-1.6.1/google/cloud/binaryauthorization_v1/services/validation_helper_v1/async_client.py
--rw-rw-r--   0 root         (0)     1003    21652 2023-03-27 14:57:47.000000 google-cloud-binary-authorization-1.6.1/google/cloud/binaryauthorization_v1/services/validation_helper_v1/client.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:59:47.989531 google-cloud-binary-authorization-1.6.1/google/cloud/binaryauthorization_v1/services/validation_helper_v1/transports/
--rw-rw-r--   0 root         (0)     1003     1464 2023-03-27 14:57:47.000000 google-cloud-binary-authorization-1.6.1/google/cloud/binaryauthorization_v1/services/validation_helper_v1/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     6186 2023-03-27 14:57:47.000000 google-cloud-binary-authorization-1.6.1/google/cloud/binaryauthorization_v1/services/validation_helper_v1/transports/base.py
--rw-rw-r--   0 root         (0)     1003    12086 2023-03-27 14:57:47.000000 google-cloud-binary-authorization-1.6.1/google/cloud/binaryauthorization_v1/services/validation_helper_v1/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    12295 2023-03-27 14:57:47.000000 google-cloud-binary-authorization-1.6.1/google/cloud/binaryauthorization_v1/services/validation_helper_v1/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    13129 2023-03-27 14:57:47.000000 google-cloud-binary-authorization-1.6.1/google/cloud/binaryauthorization_v1/services/validation_helper_v1/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:59:47.989531 google-cloud-binary-authorization-1.6.1/google/cloud/binaryauthorization_v1/types/
--rw-rw-r--   0 root         (0)     1003     1627 2023-03-27 14:57:47.000000 google-cloud-binary-authorization-1.6.1/google/cloud/binaryauthorization_v1/types/__init__.py
--rw-rw-r--   0 root         (0)     1003    21089 2023-03-27 14:57:47.000000 google-cloud-binary-authorization-1.6.1/google/cloud/binaryauthorization_v1/types/resources.py
--rw-rw-r--   0 root         (0)     1003    10579 2023-03-27 14:57:47.000000 google-cloud-binary-authorization-1.6.1/google/cloud/binaryauthorization_v1/types/service.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:59:47.989531 google-cloud-binary-authorization-1.6.1/google/cloud/binaryauthorization_v1beta1/
--rw-rw-r--   0 root         (0)     1003     2144 2023-03-27 14:57:47.000000 google-cloud-binary-authorization-1.6.1/google/cloud/binaryauthorization_v1beta1/__init__.py
--rw-rw-r--   0 root         (0)     1003     4102 2023-03-27 14:57:47.000000 google-cloud-binary-authorization-1.6.1/google/cloud/binaryauthorization_v1beta1/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003      652 2023-03-27 14:57:47.000000 google-cloud-binary-authorization-1.6.1/google/cloud/binaryauthorization_v1beta1/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       94 2023-03-27 14:57:47.000000 google-cloud-binary-authorization-1.6.1/google/cloud/binaryauthorization_v1beta1/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:59:47.989531 google-cloud-binary-authorization-1.6.1/google/cloud/binaryauthorization_v1beta1/services/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 14:57:47.000000 google-cloud-binary-authorization-1.6.1/google/cloud/binaryauthorization_v1beta1/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:59:47.989531 google-cloud-binary-authorization-1.6.1/google/cloud/binaryauthorization_v1beta1/services/binauthz_management_service_v1_beta1/
--rw-rw-r--   0 root         (0)     1003      841 2023-03-27 14:57:47.000000 google-cloud-binary-authorization-1.6.1/google/cloud/binaryauthorization_v1beta1/services/binauthz_management_service_v1_beta1/__init__.py
--rw-rw-r--   0 root         (0)     1003    47077 2023-03-27 14:57:47.000000 google-cloud-binary-authorization-1.6.1/google/cloud/binaryauthorization_v1beta1/services/binauthz_management_service_v1_beta1/async_client.py
--rw-rw-r--   0 root         (0)     1003    54863 2023-03-27 14:57:47.000000 google-cloud-binary-authorization-1.6.1/google/cloud/binaryauthorization_v1beta1/services/binauthz_management_service_v1_beta1/client.py
--rw-rw-r--   0 root         (0)     1003     5870 2023-03-27 14:57:47.000000 google-cloud-binary-authorization-1.6.1/google/cloud/binaryauthorization_v1beta1/services/binauthz_management_service_v1_beta1/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:59:47.993532 google-cloud-binary-authorization-1.6.1/google/cloud/binaryauthorization_v1beta1/services/binauthz_management_service_v1_beta1/transports/
--rw-rw-r--   0 root         (0)     1003     1679 2023-03-27 14:57:47.000000 google-cloud-binary-authorization-1.6.1/google/cloud/binaryauthorization_v1beta1/services/binauthz_management_service_v1_beta1/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003    11027 2023-03-27 14:57:47.000000 google-cloud-binary-authorization-1.6.1/google/cloud/binaryauthorization_v1beta1/services/binauthz_management_service_v1_beta1/transports/base.py
--rw-rw-r--   0 root         (0)     1003    20788 2023-03-27 14:57:47.000000 google-cloud-binary-authorization-1.6.1/google/cloud/binaryauthorization_v1beta1/services/binauthz_management_service_v1_beta1/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    21172 2023-03-27 14:57:47.000000 google-cloud-binary-authorization-1.6.1/google/cloud/binaryauthorization_v1beta1/services/binauthz_management_service_v1_beta1/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    42727 2023-03-27 14:57:47.000000 google-cloud-binary-authorization-1.6.1/google/cloud/binaryauthorization_v1beta1/services/binauthz_management_service_v1_beta1/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:59:47.993532 google-cloud-binary-authorization-1.6.1/google/cloud/binaryauthorization_v1beta1/services/system_policy_v1_beta1/
--rw-rw-r--   0 root         (0)     1003      789 2023-03-27 14:57:47.000000 google-cloud-binary-authorization-1.6.1/google/cloud/binaryauthorization_v1beta1/services/system_policy_v1_beta1/__init__.py
--rw-rw-r--   0 root         (0)     1003    13791 2023-03-27 14:57:47.000000 google-cloud-binary-authorization-1.6.1/google/cloud/binaryauthorization_v1beta1/services/system_policy_v1_beta1/async_client.py
--rw-rw-r--   0 root         (0)     1003    22646 2023-03-27 14:57:47.000000 google-cloud-binary-authorization-1.6.1/google/cloud/binaryauthorization_v1beta1/services/system_policy_v1_beta1/client.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:59:47.993532 google-cloud-binary-authorization-1.6.1/google/cloud/binaryauthorization_v1beta1/services/system_policy_v1_beta1/transports/
--rw-rw-r--   0 root         (0)     1003     1478 2023-03-27 14:57:47.000000 google-cloud-binary-authorization-1.6.1/google/cloud/binaryauthorization_v1beta1/services/system_policy_v1_beta1/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     6061 2023-03-27 14:57:47.000000 google-cloud-binary-authorization-1.6.1/google/cloud/binaryauthorization_v1beta1/services/system_policy_v1_beta1/transports/base.py
--rw-rw-r--   0 root         (0)     1003    11809 2023-03-27 14:57:47.000000 google-cloud-binary-authorization-1.6.1/google/cloud/binaryauthorization_v1beta1/services/system_policy_v1_beta1/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    12019 2023-03-27 14:57:47.000000 google-cloud-binary-authorization-1.6.1/google/cloud/binaryauthorization_v1beta1/services/system_policy_v1_beta1/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    12095 2023-03-27 14:57:47.000000 google-cloud-binary-authorization-1.6.1/google/cloud/binaryauthorization_v1beta1/services/system_policy_v1_beta1/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:59:47.993532 google-cloud-binary-authorization-1.6.1/google/cloud/binaryauthorization_v1beta1/types/
--rw-rw-r--   0 root         (0)     1003     1555 2023-03-27 14:57:47.000000 google-cloud-binary-authorization-1.6.1/google/cloud/binaryauthorization_v1beta1/types/__init__.py
--rw-rw-r--   0 root         (0)     1003     6623 2023-03-27 14:57:47.000000 google-cloud-binary-authorization-1.6.1/google/cloud/binaryauthorization_v1beta1/types/continuous_validation_logging.py
--rw-rw-r--   0 root         (0)     1003    21395 2023-03-27 14:57:47.000000 google-cloud-binary-authorization-1.6.1/google/cloud/binaryauthorization_v1beta1/types/resources.py
--rw-rw-r--   0 root         (0)     1003     7569 2023-03-27 14:57:47.000000 google-cloud-binary-authorization-1.6.1/google/cloud/binaryauthorization_v1beta1/types/service.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:59:47.997533 google-cloud-binary-authorization-1.6.1/google_cloud_binary_authorization.egg-info/
--rw-r--r--   0 root         (0)     1003     4870 2023-03-27 14:59:47.000000 google-cloud-binary-authorization-1.6.1/google_cloud_binary_authorization.egg-info/PKG-INFO
--rw-r--r--   0 root         (0)     1003     5932 2023-03-27 14:59:47.000000 google-cloud-binary-authorization-1.6.1/google_cloud_binary_authorization.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0)     1003        1 2023-03-27 14:59:47.000000 google-cloud-binary-authorization-1.6.1/google_cloud_binary_authorization.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0)     1003       20 2023-03-27 14:59:47.000000 google-cloud-binary-authorization-1.6.1/google_cloud_binary_authorization.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0)     1003        1 2023-03-27 14:59:47.000000 google-cloud-binary-authorization-1.6.1/google_cloud_binary_authorization.egg-info/not-zip-safe
--rw-r--r--   0 root         (0)     1003      338 2023-03-27 14:59:47.000000 google-cloud-binary-authorization-1.6.1/google_cloud_binary_authorization.egg-info/requires.txt
--rw-r--r--   0 root         (0)     1003        7 2023-03-27 14:59:47.000000 google-cloud-binary-authorization-1.6.1/google_cloud_binary_authorization.egg-info/top_level.txt
--rw-rw-r--   0 root         (0)     1003       67 2023-03-27 14:59:47.997533 google-cloud-binary-authorization-1.6.1/setup.cfg
--rw-rw-r--   0 root         (0)     1003     3063 2023-03-27 14:57:47.000000 google-cloud-binary-authorization-1.6.1/setup.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:59:47.997533 google-cloud-binary-authorization-1.6.1/tests/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 14:57:47.000000 google-cloud-binary-authorization-1.6.1/tests/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:59:47.997533 google-cloud-binary-authorization-1.6.1/tests/unit/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 14:57:47.000000 google-cloud-binary-authorization-1.6.1/tests/unit/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:59:47.997533 google-cloud-binary-authorization-1.6.1/tests/unit/gapic/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 14:57:47.000000 google-cloud-binary-authorization-1.6.1/tests/unit/gapic/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:59:47.997533 google-cloud-binary-authorization-1.6.1/tests/unit/gapic/binaryauthorization_v1/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 14:57:47.000000 google-cloud-binary-authorization-1.6.1/tests/unit/gapic/binaryauthorization_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003   198994 2023-03-27 14:57:47.000000 google-cloud-binary-authorization-1.6.1/tests/unit/gapic/binaryauthorization_v1/test_binauthz_management_service_v1.py
--rw-rw-r--   0 root         (0)     1003    71636 2023-03-27 14:57:47.000000 google-cloud-binary-authorization-1.6.1/tests/unit/gapic/binaryauthorization_v1/test_system_policy_v1.py
--rw-rw-r--   0 root         (0)     1003    69359 2023-03-27 14:57:47.000000 google-cloud-binary-authorization-1.6.1/tests/unit/gapic/binaryauthorization_v1/test_validation_helper_v1.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:59:47.997533 google-cloud-binary-authorization-1.6.1/tests/unit/gapic/binaryauthorization_v1beta1/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 14:57:47.000000 google-cloud-binary-authorization-1.6.1/tests/unit/gapic/binaryauthorization_v1beta1/__init__.py
--rw-rw-r--   0 root         (0)     1003   201074 2023-03-27 14:57:47.000000 google-cloud-binary-authorization-1.6.1/tests/unit/gapic/binaryauthorization_v1beta1/test_binauthz_management_service_v1_beta1.py
--rw-rw-r--   0 root         (0)     1003    73262 2023-03-27 14:57:47.000000 google-cloud-binary-authorization-1.6.1/tests/unit/gapic/binaryauthorization_v1beta1/test_system_policy_v1_beta1.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:14:52.715777 google-cloud-binary-authorization-1.6.2/
+-rw-rw-r--   0 root         (0)     1003    11358 2023-07-05 15:13:01.000000 google-cloud-binary-authorization-1.6.2/LICENSE
+-rw-rw-r--   0 root         (0)     1003      860 2023-07-05 15:13:01.000000 google-cloud-binary-authorization-1.6.2/MANIFEST.in
+-rw-r--r--   0 root         (0)     1003     4870 2023-07-05 15:14:52.719776 google-cloud-binary-authorization-1.6.2/PKG-INFO
+-rw-rw-r--   0 root         (0)     1003     3916 2023-07-05 15:13:01.000000 google-cloud-binary-authorization-1.6.2/README.rst
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:14:52.695784 google-cloud-binary-authorization-1.6.2/google/
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:14:52.695784 google-cloud-binary-authorization-1.6.2/google/cloud/
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:14:52.699782 google-cloud-binary-authorization-1.6.2/google/cloud/binaryauthorization/
+-rw-rw-r--   0 root         (0)     1003     2818 2023-07-05 15:13:01.000000 google-cloud-binary-authorization-1.6.2/google/cloud/binaryauthorization/__init__.py
+-rw-rw-r--   0 root         (0)     1003      652 2023-07-05 15:13:01.000000 google-cloud-binary-authorization-1.6.2/google/cloud/binaryauthorization/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       94 2023-07-05 15:13:01.000000 google-cloud-binary-authorization-1.6.2/google/cloud/binaryauthorization/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:14:52.699782 google-cloud-binary-authorization-1.6.2/google/cloud/binaryauthorization_v1/
+-rw-rw-r--   0 root         (0)     1003     2321 2023-07-05 15:13:01.000000 google-cloud-binary-authorization-1.6.2/google/cloud/binaryauthorization_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003     4934 2023-07-05 15:13:01.000000 google-cloud-binary-authorization-1.6.2/google/cloud/binaryauthorization_v1/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      652 2023-07-05 15:13:01.000000 google-cloud-binary-authorization-1.6.2/google/cloud/binaryauthorization_v1/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       94 2023-07-05 15:13:01.000000 google-cloud-binary-authorization-1.6.2/google/cloud/binaryauthorization_v1/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:14:52.699782 google-cloud-binary-authorization-1.6.2/google/cloud/binaryauthorization_v1/services/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:13:01.000000 google-cloud-binary-authorization-1.6.2/google/cloud/binaryauthorization_v1/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:14:52.699782 google-cloud-binary-authorization-1.6.2/google/cloud/binaryauthorization_v1/services/binauthz_management_service_v1/
+-rw-rw-r--   0 root         (0)     1003      821 2023-07-05 15:13:01.000000 google-cloud-binary-authorization-1.6.2/google/cloud/binaryauthorization_v1/services/binauthz_management_service_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003    46422 2023-07-05 15:13:01.000000 google-cloud-binary-authorization-1.6.2/google/cloud/binaryauthorization_v1/services/binauthz_management_service_v1/async_client.py
+-rw-rw-r--   0 root         (0)     1003    54229 2023-07-05 15:13:01.000000 google-cloud-binary-authorization-1.6.2/google/cloud/binaryauthorization_v1/services/binauthz_management_service_v1/client.py
+-rw-rw-r--   0 root         (0)     1003     5825 2023-07-05 15:13:01.000000 google-cloud-binary-authorization-1.6.2/google/cloud/binaryauthorization_v1/services/binauthz_management_service_v1/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:14:52.703781 google-cloud-binary-authorization-1.6.2/google/cloud/binaryauthorization_v1/services/binauthz_management_service_v1/transports/
+-rw-rw-r--   0 root         (0)     1003     1603 2023-07-05 15:13:01.000000 google-cloud-binary-authorization-1.6.2/google/cloud/binaryauthorization_v1/services/binauthz_management_service_v1/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003    11002 2023-07-05 15:13:01.000000 google-cloud-binary-authorization-1.6.2/google/cloud/binaryauthorization_v1/services/binauthz_management_service_v1/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    20560 2023-07-05 15:13:01.000000 google-cloud-binary-authorization-1.6.2/google/cloud/binaryauthorization_v1/services/binauthz_management_service_v1/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    20945 2023-07-05 15:13:01.000000 google-cloud-binary-authorization-1.6.2/google/cloud/binaryauthorization_v1/services/binauthz_management_service_v1/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    42437 2023-07-05 15:13:01.000000 google-cloud-binary-authorization-1.6.2/google/cloud/binaryauthorization_v1/services/binauthz_management_service_v1/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:14:52.703781 google-cloud-binary-authorization-1.6.2/google/cloud/binaryauthorization_v1/services/system_policy_v1/
+-rw-rw-r--   0 root         (0)     1003      769 2023-07-05 15:13:01.000000 google-cloud-binary-authorization-1.6.2/google/cloud/binaryauthorization_v1/services/system_policy_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003    13592 2023-07-05 15:13:01.000000 google-cloud-binary-authorization-1.6.2/google/cloud/binaryauthorization_v1/services/system_policy_v1/async_client.py
+-rw-rw-r--   0 root         (0)     1003    22480 2023-07-05 15:13:01.000000 google-cloud-binary-authorization-1.6.2/google/cloud/binaryauthorization_v1/services/system_policy_v1/client.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:14:52.703781 google-cloud-binary-authorization-1.6.2/google/cloud/binaryauthorization_v1/services/system_policy_v1/transports/
+-rw-rw-r--   0 root         (0)     1003     1400 2023-07-05 15:13:01.000000 google-cloud-binary-authorization-1.6.2/google/cloud/binaryauthorization_v1/services/system_policy_v1/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     6036 2023-07-05 15:13:01.000000 google-cloud-binary-authorization-1.6.2/google/cloud/binaryauthorization_v1/services/system_policy_v1/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    11769 2023-07-05 15:13:01.000000 google-cloud-binary-authorization-1.6.2/google/cloud/binaryauthorization_v1/services/system_policy_v1/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    11974 2023-07-05 15:13:01.000000 google-cloud-binary-authorization-1.6.2/google/cloud/binaryauthorization_v1/services/system_policy_v1/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    11980 2023-07-05 15:13:01.000000 google-cloud-binary-authorization-1.6.2/google/cloud/binaryauthorization_v1/services/system_policy_v1/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:14:52.703781 google-cloud-binary-authorization-1.6.2/google/cloud/binaryauthorization_v1/services/validation_helper_v1/
+-rw-rw-r--   0 root         (0)     1003      785 2023-07-05 15:13:01.000000 google-cloud-binary-authorization-1.6.2/google/cloud/binaryauthorization_v1/services/validation_helper_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003    13095 2023-07-05 15:13:01.000000 google-cloud-binary-authorization-1.6.2/google/cloud/binaryauthorization_v1/services/validation_helper_v1/async_client.py
+-rw-rw-r--   0 root         (0)     1003    21652 2023-07-05 15:13:01.000000 google-cloud-binary-authorization-1.6.2/google/cloud/binaryauthorization_v1/services/validation_helper_v1/client.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:14:52.703781 google-cloud-binary-authorization-1.6.2/google/cloud/binaryauthorization_v1/services/validation_helper_v1/transports/
+-rw-rw-r--   0 root         (0)     1003     1464 2023-07-05 15:13:01.000000 google-cloud-binary-authorization-1.6.2/google/cloud/binaryauthorization_v1/services/validation_helper_v1/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     6186 2023-07-05 15:13:01.000000 google-cloud-binary-authorization-1.6.2/google/cloud/binaryauthorization_v1/services/validation_helper_v1/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    12086 2023-07-05 15:13:01.000000 google-cloud-binary-authorization-1.6.2/google/cloud/binaryauthorization_v1/services/validation_helper_v1/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    12295 2023-07-05 15:13:01.000000 google-cloud-binary-authorization-1.6.2/google/cloud/binaryauthorization_v1/services/validation_helper_v1/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    13129 2023-07-05 15:13:01.000000 google-cloud-binary-authorization-1.6.2/google/cloud/binaryauthorization_v1/services/validation_helper_v1/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:14:52.707780 google-cloud-binary-authorization-1.6.2/google/cloud/binaryauthorization_v1/types/
+-rw-rw-r--   0 root         (0)     1003     1627 2023-07-05 15:13:01.000000 google-cloud-binary-authorization-1.6.2/google/cloud/binaryauthorization_v1/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003    21089 2023-07-05 15:13:01.000000 google-cloud-binary-authorization-1.6.2/google/cloud/binaryauthorization_v1/types/resources.py
+-rw-rw-r--   0 root         (0)     1003    10579 2023-07-05 15:13:01.000000 google-cloud-binary-authorization-1.6.2/google/cloud/binaryauthorization_v1/types/service.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:14:52.707780 google-cloud-binary-authorization-1.6.2/google/cloud/binaryauthorization_v1beta1/
+-rw-rw-r--   0 root         (0)     1003     2144 2023-07-05 15:13:01.000000 google-cloud-binary-authorization-1.6.2/google/cloud/binaryauthorization_v1beta1/__init__.py
+-rw-rw-r--   0 root         (0)     1003     4102 2023-07-05 15:13:01.000000 google-cloud-binary-authorization-1.6.2/google/cloud/binaryauthorization_v1beta1/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      652 2023-07-05 15:13:01.000000 google-cloud-binary-authorization-1.6.2/google/cloud/binaryauthorization_v1beta1/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       94 2023-07-05 15:13:01.000000 google-cloud-binary-authorization-1.6.2/google/cloud/binaryauthorization_v1beta1/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:14:52.707780 google-cloud-binary-authorization-1.6.2/google/cloud/binaryauthorization_v1beta1/services/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:13:01.000000 google-cloud-binary-authorization-1.6.2/google/cloud/binaryauthorization_v1beta1/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:14:52.707780 google-cloud-binary-authorization-1.6.2/google/cloud/binaryauthorization_v1beta1/services/binauthz_management_service_v1_beta1/
+-rw-rw-r--   0 root         (0)     1003      841 2023-07-05 15:13:01.000000 google-cloud-binary-authorization-1.6.2/google/cloud/binaryauthorization_v1beta1/services/binauthz_management_service_v1_beta1/__init__.py
+-rw-rw-r--   0 root         (0)     1003    47126 2023-07-05 15:13:01.000000 google-cloud-binary-authorization-1.6.2/google/cloud/binaryauthorization_v1beta1/services/binauthz_management_service_v1_beta1/async_client.py
+-rw-rw-r--   0 root         (0)     1003    54863 2023-07-05 15:13:01.000000 google-cloud-binary-authorization-1.6.2/google/cloud/binaryauthorization_v1beta1/services/binauthz_management_service_v1_beta1/client.py
+-rw-rw-r--   0 root         (0)     1003     5870 2023-07-05 15:13:01.000000 google-cloud-binary-authorization-1.6.2/google/cloud/binaryauthorization_v1beta1/services/binauthz_management_service_v1_beta1/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:14:52.711778 google-cloud-binary-authorization-1.6.2/google/cloud/binaryauthorization_v1beta1/services/binauthz_management_service_v1_beta1/transports/
+-rw-rw-r--   0 root         (0)     1003     1679 2023-07-05 15:13:01.000000 google-cloud-binary-authorization-1.6.2/google/cloud/binaryauthorization_v1beta1/services/binauthz_management_service_v1_beta1/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003    11027 2023-07-05 15:13:01.000000 google-cloud-binary-authorization-1.6.2/google/cloud/binaryauthorization_v1beta1/services/binauthz_management_service_v1_beta1/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    20788 2023-07-05 15:13:01.000000 google-cloud-binary-authorization-1.6.2/google/cloud/binaryauthorization_v1beta1/services/binauthz_management_service_v1_beta1/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    21172 2023-07-05 15:13:01.000000 google-cloud-binary-authorization-1.6.2/google/cloud/binaryauthorization_v1beta1/services/binauthz_management_service_v1_beta1/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    42727 2023-07-05 15:13:01.000000 google-cloud-binary-authorization-1.6.2/google/cloud/binaryauthorization_v1beta1/services/binauthz_management_service_v1_beta1/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:14:52.711778 google-cloud-binary-authorization-1.6.2/google/cloud/binaryauthorization_v1beta1/services/system_policy_v1_beta1/
+-rw-rw-r--   0 root         (0)     1003      789 2023-07-05 15:13:01.000000 google-cloud-binary-authorization-1.6.2/google/cloud/binaryauthorization_v1beta1/services/system_policy_v1_beta1/__init__.py
+-rw-rw-r--   0 root         (0)     1003    13827 2023-07-05 15:13:01.000000 google-cloud-binary-authorization-1.6.2/google/cloud/binaryauthorization_v1beta1/services/system_policy_v1_beta1/async_client.py
+-rw-rw-r--   0 root         (0)     1003    22646 2023-07-05 15:13:01.000000 google-cloud-binary-authorization-1.6.2/google/cloud/binaryauthorization_v1beta1/services/system_policy_v1_beta1/client.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:14:52.711778 google-cloud-binary-authorization-1.6.2/google/cloud/binaryauthorization_v1beta1/services/system_policy_v1_beta1/transports/
+-rw-rw-r--   0 root         (0)     1003     1478 2023-07-05 15:13:01.000000 google-cloud-binary-authorization-1.6.2/google/cloud/binaryauthorization_v1beta1/services/system_policy_v1_beta1/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     6061 2023-07-05 15:13:01.000000 google-cloud-binary-authorization-1.6.2/google/cloud/binaryauthorization_v1beta1/services/system_policy_v1_beta1/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    11809 2023-07-05 15:13:01.000000 google-cloud-binary-authorization-1.6.2/google/cloud/binaryauthorization_v1beta1/services/system_policy_v1_beta1/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    12019 2023-07-05 15:13:01.000000 google-cloud-binary-authorization-1.6.2/google/cloud/binaryauthorization_v1beta1/services/system_policy_v1_beta1/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    12095 2023-07-05 15:13:01.000000 google-cloud-binary-authorization-1.6.2/google/cloud/binaryauthorization_v1beta1/services/system_policy_v1_beta1/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:14:52.711778 google-cloud-binary-authorization-1.6.2/google/cloud/binaryauthorization_v1beta1/types/
+-rw-rw-r--   0 root         (0)     1003     1555 2023-07-05 15:13:01.000000 google-cloud-binary-authorization-1.6.2/google/cloud/binaryauthorization_v1beta1/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003     6623 2023-07-05 15:13:01.000000 google-cloud-binary-authorization-1.6.2/google/cloud/binaryauthorization_v1beta1/types/continuous_validation_logging.py
+-rw-rw-r--   0 root         (0)     1003    21395 2023-07-05 15:13:01.000000 google-cloud-binary-authorization-1.6.2/google/cloud/binaryauthorization_v1beta1/types/resources.py
+-rw-rw-r--   0 root         (0)     1003     7569 2023-07-05 15:13:01.000000 google-cloud-binary-authorization-1.6.2/google/cloud/binaryauthorization_v1beta1/types/service.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:14:52.715777 google-cloud-binary-authorization-1.6.2/google_cloud_binary_authorization.egg-info/
+-rw-r--r--   0 root         (0)     1003     4870 2023-07-05 15:14:52.000000 google-cloud-binary-authorization-1.6.2/google_cloud_binary_authorization.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0)     1003     5932 2023-07-05 15:14:52.000000 google-cloud-binary-authorization-1.6.2/google_cloud_binary_authorization.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-07-05 15:14:52.000000 google-cloud-binary-authorization-1.6.2/google_cloud_binary_authorization.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0)     1003       20 2023-07-05 15:14:52.000000 google-cloud-binary-authorization-1.6.2/google_cloud_binary_authorization.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-07-05 15:14:52.000000 google-cloud-binary-authorization-1.6.2/google_cloud_binary_authorization.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0)     1003      338 2023-07-05 15:14:52.000000 google-cloud-binary-authorization-1.6.2/google_cloud_binary_authorization.egg-info/requires.txt
+-rw-r--r--   0 root         (0)     1003        7 2023-07-05 15:14:52.000000 google-cloud-binary-authorization-1.6.2/google_cloud_binary_authorization.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0)     1003       67 2023-07-05 15:14:52.719776 google-cloud-binary-authorization-1.6.2/setup.cfg
+-rw-rw-r--   0 root         (0)     1003     3063 2023-07-05 15:13:01.000000 google-cloud-binary-authorization-1.6.2/setup.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:14:52.715777 google-cloud-binary-authorization-1.6.2/tests/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:13:01.000000 google-cloud-binary-authorization-1.6.2/tests/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:14:52.715777 google-cloud-binary-authorization-1.6.2/tests/unit/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:13:01.000000 google-cloud-binary-authorization-1.6.2/tests/unit/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:14:52.715777 google-cloud-binary-authorization-1.6.2/tests/unit/gapic/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:13:01.000000 google-cloud-binary-authorization-1.6.2/tests/unit/gapic/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:14:52.715777 google-cloud-binary-authorization-1.6.2/tests/unit/gapic/binaryauthorization_v1/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:13:01.000000 google-cloud-binary-authorization-1.6.2/tests/unit/gapic/binaryauthorization_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003   198371 2023-07-05 15:13:01.000000 google-cloud-binary-authorization-1.6.2/tests/unit/gapic/binaryauthorization_v1/test_binauthz_management_service_v1.py
+-rw-rw-r--   0 root         (0)     1003    71636 2023-07-05 15:13:01.000000 google-cloud-binary-authorization-1.6.2/tests/unit/gapic/binaryauthorization_v1/test_system_policy_v1.py
+-rw-rw-r--   0 root         (0)     1003    69359 2023-07-05 15:13:01.000000 google-cloud-binary-authorization-1.6.2/tests/unit/gapic/binaryauthorization_v1/test_validation_helper_v1.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:14:52.715777 google-cloud-binary-authorization-1.6.2/tests/unit/gapic/binaryauthorization_v1beta1/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:13:01.000000 google-cloud-binary-authorization-1.6.2/tests/unit/gapic/binaryauthorization_v1beta1/__init__.py
+-rw-rw-r--   0 root         (0)     1003   200451 2023-07-05 15:13:01.000000 google-cloud-binary-authorization-1.6.2/tests/unit/gapic/binaryauthorization_v1beta1/test_binauthz_management_service_v1_beta1.py
+-rw-rw-r--   0 root         (0)     1003    73262 2023-07-05 15:13:01.000000 google-cloud-binary-authorization-1.6.2/tests/unit/gapic/binaryauthorization_v1beta1/test_system_policy_v1_beta1.py
```

### Comparing `google-cloud-binary-authorization-1.6.1/LICENSE` & `google-cloud-binary-authorization-1.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `google-cloud-binary-authorization-1.6.1/MANIFEST.in` & `google-cloud-binary-authorization-1.6.2/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `google-cloud-binary-authorization-1.6.1/PKG-INFO` & `google-cloud-binary-authorization-1.6.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-binary-authorization
-Version: 1.6.1
+Version: 1.6.2
 Summary: Google Cloud Binaryauthorization API client library
 Home-page: https://github.com/googleapis/python-binary-authorization
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `google-cloud-binary-authorization-1.6.1/README.rst` & `google-cloud-binary-authorization-1.6.2/README.rst`

 * *Files identical despite different names*

### Comparing `google-cloud-binary-authorization-1.6.1/google/cloud/binaryauthorization/__init__.py` & `google-cloud-binary-authorization-1.6.2/google/cloud/binaryauthorization/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-binary-authorization-1.6.1/google/cloud/binaryauthorization/gapic_version.py` & `google-cloud-binary-authorization-1.6.2/google/cloud/binaryauthorization/gapic_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "1.6.1"  # {x-release-please-version}
+__version__ = "1.6.2"  # {x-release-please-version}
```

### Comparing `google-cloud-binary-authorization-1.6.1/google/cloud/binaryauthorization_v1/__init__.py` & `google-cloud-binary-authorization-1.6.2/google/cloud/binaryauthorization_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-binary-authorization-1.6.1/google/cloud/binaryauthorization_v1/gapic_metadata.json` & `google-cloud-binary-authorization-1.6.2/google/cloud/binaryauthorization_v1/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-cloud-binary-authorization-1.6.1/google/cloud/binaryauthorization_v1/gapic_version.py` & `google-cloud-binary-authorization-1.6.2/google/cloud/binaryauthorization_v1/gapic_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "1.6.1"  # {x-release-please-version}
+__version__ = "1.6.2"  # {x-release-please-version}
```

### Comparing `google-cloud-binary-authorization-1.6.1/google/cloud/binaryauthorization_v1/services/__init__.py` & `google-cloud-binary-authorization-1.6.2/google/cloud/binaryauthorization_v1/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-binary-authorization-1.6.1/google/cloud/binaryauthorization_v1/services/binauthz_management_service_v1/__init__.py` & `google-cloud-binary-authorization-1.6.2/google/cloud/binaryauthorization_v1/services/binauthz_management_service_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-binary-authorization-1.6.1/google/cloud/binaryauthorization_v1/services/binauthz_management_service_v1/async_client.py` & `google-cloud-binary-authorization-1.6.2/google/cloud/binaryauthorization_v1/services/binauthz_management_service_v1/async_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1105,15 +1105,15 @@
         await rpc(
             request,
             retry=retry,
             timeout=timeout,
             metadata=metadata,
         )
 
-    async def __aenter__(self):
+    async def __aenter__(self) -> "BinauthzManagementServiceV1AsyncClient":
         return self
 
     async def __aexit__(self, exc_type, exc, tb):
         await self.transport.close()
 
 
 DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
```

### Comparing `google-cloud-binary-authorization-1.6.1/google/cloud/binaryauthorization_v1/services/binauthz_management_service_v1/client.py` & `google-cloud-binary-authorization-1.6.2/google/cloud/binaryauthorization_v1/services/binauthz_management_service_v1/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-binary-authorization-1.6.1/google/cloud/binaryauthorization_v1/services/binauthz_management_service_v1/pagers.py` & `google-cloud-binary-authorization-1.6.2/google/cloud/binaryauthorization_v1/services/binauthz_management_service_v1/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-binary-authorization-1.6.1/google/cloud/binaryauthorization_v1/services/binauthz_management_service_v1/transports/__init__.py` & `google-cloud-binary-authorization-1.6.2/google/cloud/binaryauthorization_v1/services/binauthz_management_service_v1/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-binary-authorization-1.6.1/google/cloud/binaryauthorization_v1/services/binauthz_management_service_v1/transports/base.py` & `google-cloud-binary-authorization-1.6.2/google/cloud/binaryauthorization_v1/services/binauthz_management_service_v1/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-binary-authorization-1.6.1/google/cloud/binaryauthorization_v1/services/binauthz_management_service_v1/transports/grpc.py` & `google-cloud-binary-authorization-1.6.2/google/cloud/binaryauthorization_v1/services/binauthz_management_service_v1/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-binary-authorization-1.6.1/google/cloud/binaryauthorization_v1/services/binauthz_management_service_v1/transports/grpc_asyncio.py` & `google-cloud-binary-authorization-1.6.2/google/cloud/binaryauthorization_v1/services/binauthz_management_service_v1/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-binary-authorization-1.6.1/google/cloud/binaryauthorization_v1/services/binauthz_management_service_v1/transports/rest.py` & `google-cloud-binary-authorization-1.6.2/google/cloud/binaryauthorization_v1/services/binauthz_management_service_v1/transports/rest.py`

 * *Files identical despite different names*

### Comparing `google-cloud-binary-authorization-1.6.1/google/cloud/binaryauthorization_v1/services/system_policy_v1/__init__.py` & `google-cloud-binary-authorization-1.6.2/google/cloud/binaryauthorization_v1/services/system_policy_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-binary-authorization-1.6.1/google/cloud/binaryauthorization_v1/services/system_policy_v1/async_client.py` & `google-cloud-binary-authorization-1.6.2/google/cloud/binaryauthorization_v1/services/system_policy_v1/async_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -315,15 +315,15 @@
             timeout=timeout,
             metadata=metadata,
         )
 
         # Done; return the response.
         return response
 
-    async def __aenter__(self):
+    async def __aenter__(self) -> "SystemPolicyV1AsyncClient":
         return self
 
     async def __aexit__(self, exc_type, exc, tb):
         await self.transport.close()
 
 
 DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
```

### Comparing `google-cloud-binary-authorization-1.6.1/google/cloud/binaryauthorization_v1/services/system_policy_v1/client.py` & `google-cloud-binary-authorization-1.6.2/google/cloud/binaryauthorization_v1/services/system_policy_v1/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-binary-authorization-1.6.1/google/cloud/binaryauthorization_v1/services/system_policy_v1/transports/__init__.py` & `google-cloud-binary-authorization-1.6.2/google/cloud/binaryauthorization_v1/services/system_policy_v1/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-binary-authorization-1.6.1/google/cloud/binaryauthorization_v1/services/system_policy_v1/transports/base.py` & `google-cloud-binary-authorization-1.6.2/google/cloud/binaryauthorization_v1/services/system_policy_v1/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-binary-authorization-1.6.1/google/cloud/binaryauthorization_v1/services/system_policy_v1/transports/grpc.py` & `google-cloud-binary-authorization-1.6.2/google/cloud/binaryauthorization_v1/services/system_policy_v1/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-binary-authorization-1.6.1/google/cloud/binaryauthorization_v1/services/system_policy_v1/transports/grpc_asyncio.py` & `google-cloud-binary-authorization-1.6.2/google/cloud/binaryauthorization_v1/services/system_policy_v1/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-binary-authorization-1.6.1/google/cloud/binaryauthorization_v1/services/system_policy_v1/transports/rest.py` & `google-cloud-binary-authorization-1.6.2/google/cloud/binaryauthorization_v1/services/system_policy_v1/transports/rest.py`

 * *Files identical despite different names*

### Comparing `google-cloud-binary-authorization-1.6.1/google/cloud/binaryauthorization_v1/services/validation_helper_v1/__init__.py` & `google-cloud-binary-authorization-1.6.2/google/cloud/binaryauthorization_v1/services/validation_helper_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-binary-authorization-1.6.1/google/cloud/binaryauthorization_v1/services/validation_helper_v1/async_client.py` & `google-cloud-binary-authorization-1.6.2/google/cloud/binaryauthorization_v1/services/validation_helper_v1/async_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -293,15 +293,15 @@
             timeout=timeout,
             metadata=metadata,
         )
 
         # Done; return the response.
         return response
 
-    async def __aenter__(self):
+    async def __aenter__(self) -> "ValidationHelperV1AsyncClient":
         return self
 
     async def __aexit__(self, exc_type, exc, tb):
         await self.transport.close()
 
 
 DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
```

### Comparing `google-cloud-binary-authorization-1.6.1/google/cloud/binaryauthorization_v1/services/validation_helper_v1/client.py` & `google-cloud-binary-authorization-1.6.2/google/cloud/binaryauthorization_v1/services/validation_helper_v1/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-binary-authorization-1.6.1/google/cloud/binaryauthorization_v1/services/validation_helper_v1/transports/__init__.py` & `google-cloud-binary-authorization-1.6.2/google/cloud/binaryauthorization_v1/services/validation_helper_v1/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-binary-authorization-1.6.1/google/cloud/binaryauthorization_v1/services/validation_helper_v1/transports/base.py` & `google-cloud-binary-authorization-1.6.2/google/cloud/binaryauthorization_v1/services/validation_helper_v1/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-binary-authorization-1.6.1/google/cloud/binaryauthorization_v1/services/validation_helper_v1/transports/grpc.py` & `google-cloud-binary-authorization-1.6.2/google/cloud/binaryauthorization_v1/services/validation_helper_v1/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-binary-authorization-1.6.1/google/cloud/binaryauthorization_v1/services/validation_helper_v1/transports/grpc_asyncio.py` & `google-cloud-binary-authorization-1.6.2/google/cloud/binaryauthorization_v1/services/validation_helper_v1/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-binary-authorization-1.6.1/google/cloud/binaryauthorization_v1/services/validation_helper_v1/transports/rest.py` & `google-cloud-binary-authorization-1.6.2/google/cloud/binaryauthorization_v1/services/validation_helper_v1/transports/rest.py`

 * *Files identical despite different names*

### Comparing `google-cloud-binary-authorization-1.6.1/google/cloud/binaryauthorization_v1/types/__init__.py` & `google-cloud-binary-authorization-1.6.2/google/cloud/binaryauthorization_v1/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-binary-authorization-1.6.1/google/cloud/binaryauthorization_v1/types/resources.py` & `google-cloud-binary-authorization-1.6.2/google/cloud/binaryauthorization_v1/types/resources.py`

 * *Files identical despite different names*

### Comparing `google-cloud-binary-authorization-1.6.1/google/cloud/binaryauthorization_v1/types/service.py` & `google-cloud-binary-authorization-1.6.2/google/cloud/binaryauthorization_v1/types/service.py`

 * *Files identical despite different names*

### Comparing `google-cloud-binary-authorization-1.6.1/google/cloud/binaryauthorization_v1beta1/__init__.py` & `google-cloud-binary-authorization-1.6.2/google/cloud/binaryauthorization_v1beta1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-binary-authorization-1.6.1/google/cloud/binaryauthorization_v1beta1/gapic_metadata.json` & `google-cloud-binary-authorization-1.6.2/google/cloud/binaryauthorization_v1beta1/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-cloud-binary-authorization-1.6.1/google/cloud/binaryauthorization_v1beta1/gapic_version.py` & `google-cloud-binary-authorization-1.6.2/google/cloud/binaryauthorization_v1beta1/gapic_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "1.6.1"  # {x-release-please-version}
+__version__ = "1.6.2"  # {x-release-please-version}
```

### Comparing `google-cloud-binary-authorization-1.6.1/google/cloud/binaryauthorization_v1beta1/services/__init__.py` & `google-cloud-binary-authorization-1.6.2/google/cloud/binaryauthorization_v1beta1/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-binary-authorization-1.6.1/google/cloud/binaryauthorization_v1beta1/services/binauthz_management_service_v1_beta1/__init__.py` & `google-cloud-binary-authorization-1.6.2/google/cloud/binaryauthorization_v1beta1/services/binauthz_management_service_v1_beta1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-binary-authorization-1.6.1/google/cloud/binaryauthorization_v1beta1/services/binauthz_management_service_v1_beta1/async_client.py` & `google-cloud-binary-authorization-1.6.2/google/cloud/binaryauthorization_v1beta1/services/binauthz_management_service_v1_beta1/async_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1118,15 +1118,15 @@
         await rpc(
             request,
             retry=retry,
             timeout=timeout,
             metadata=metadata,
         )
 
-    async def __aenter__(self):
+    async def __aenter__(self) -> "BinauthzManagementServiceV1Beta1AsyncClient":
         return self
 
     async def __aexit__(self, exc_type, exc, tb):
         await self.transport.close()
 
 
 DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
```

### Comparing `google-cloud-binary-authorization-1.6.1/google/cloud/binaryauthorization_v1beta1/services/binauthz_management_service_v1_beta1/client.py` & `google-cloud-binary-authorization-1.6.2/google/cloud/binaryauthorization_v1beta1/services/binauthz_management_service_v1_beta1/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-binary-authorization-1.6.1/google/cloud/binaryauthorization_v1beta1/services/binauthz_management_service_v1_beta1/pagers.py` & `google-cloud-binary-authorization-1.6.2/google/cloud/binaryauthorization_v1beta1/services/binauthz_management_service_v1_beta1/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-binary-authorization-1.6.1/google/cloud/binaryauthorization_v1beta1/services/binauthz_management_service_v1_beta1/transports/__init__.py` & `google-cloud-binary-authorization-1.6.2/google/cloud/binaryauthorization_v1beta1/services/binauthz_management_service_v1_beta1/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-binary-authorization-1.6.1/google/cloud/binaryauthorization_v1beta1/services/binauthz_management_service_v1_beta1/transports/base.py` & `google-cloud-binary-authorization-1.6.2/google/cloud/binaryauthorization_v1beta1/services/binauthz_management_service_v1_beta1/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-binary-authorization-1.6.1/google/cloud/binaryauthorization_v1beta1/services/binauthz_management_service_v1_beta1/transports/grpc.py` & `google-cloud-binary-authorization-1.6.2/google/cloud/binaryauthorization_v1beta1/services/binauthz_management_service_v1_beta1/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-binary-authorization-1.6.1/google/cloud/binaryauthorization_v1beta1/services/binauthz_management_service_v1_beta1/transports/grpc_asyncio.py` & `google-cloud-binary-authorization-1.6.2/google/cloud/binaryauthorization_v1beta1/services/binauthz_management_service_v1_beta1/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-binary-authorization-1.6.1/google/cloud/binaryauthorization_v1beta1/services/binauthz_management_service_v1_beta1/transports/rest.py` & `google-cloud-binary-authorization-1.6.2/google/cloud/binaryauthorization_v1beta1/services/binauthz_management_service_v1_beta1/transports/rest.py`

 * *Files identical despite different names*

### Comparing `google-cloud-binary-authorization-1.6.1/google/cloud/binaryauthorization_v1beta1/services/system_policy_v1_beta1/__init__.py` & `google-cloud-binary-authorization-1.6.2/google/cloud/binaryauthorization_v1beta1/services/system_policy_v1_beta1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-binary-authorization-1.6.1/google/cloud/binaryauthorization_v1beta1/services/system_policy_v1_beta1/async_client.py` & `google-cloud-binary-authorization-1.6.2/google/cloud/binaryauthorization_v1beta1/services/system_policy_v1_beta1/async_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -317,15 +317,15 @@
             timeout=timeout,
             metadata=metadata,
         )
 
         # Done; return the response.
         return response
 
-    async def __aenter__(self):
+    async def __aenter__(self) -> "SystemPolicyV1Beta1AsyncClient":
         return self
 
     async def __aexit__(self, exc_type, exc, tb):
         await self.transport.close()
 
 
 DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
```

### Comparing `google-cloud-binary-authorization-1.6.1/google/cloud/binaryauthorization_v1beta1/services/system_policy_v1_beta1/client.py` & `google-cloud-binary-authorization-1.6.2/google/cloud/binaryauthorization_v1beta1/services/system_policy_v1_beta1/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-binary-authorization-1.6.1/google/cloud/binaryauthorization_v1beta1/services/system_policy_v1_beta1/transports/__init__.py` & `google-cloud-binary-authorization-1.6.2/google/cloud/binaryauthorization_v1beta1/services/system_policy_v1_beta1/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-binary-authorization-1.6.1/google/cloud/binaryauthorization_v1beta1/services/system_policy_v1_beta1/transports/base.py` & `google-cloud-binary-authorization-1.6.2/google/cloud/binaryauthorization_v1beta1/services/system_policy_v1_beta1/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-binary-authorization-1.6.1/google/cloud/binaryauthorization_v1beta1/services/system_policy_v1_beta1/transports/grpc.py` & `google-cloud-binary-authorization-1.6.2/google/cloud/binaryauthorization_v1beta1/services/system_policy_v1_beta1/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-binary-authorization-1.6.1/google/cloud/binaryauthorization_v1beta1/services/system_policy_v1_beta1/transports/grpc_asyncio.py` & `google-cloud-binary-authorization-1.6.2/google/cloud/binaryauthorization_v1beta1/services/system_policy_v1_beta1/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-binary-authorization-1.6.1/google/cloud/binaryauthorization_v1beta1/services/system_policy_v1_beta1/transports/rest.py` & `google-cloud-binary-authorization-1.6.2/google/cloud/binaryauthorization_v1beta1/services/system_policy_v1_beta1/transports/rest.py`

 * *Files identical despite different names*

### Comparing `google-cloud-binary-authorization-1.6.1/google/cloud/binaryauthorization_v1beta1/types/__init__.py` & `google-cloud-binary-authorization-1.6.2/google/cloud/binaryauthorization_v1beta1/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-binary-authorization-1.6.1/google/cloud/binaryauthorization_v1beta1/types/continuous_validation_logging.py` & `google-cloud-binary-authorization-1.6.2/google/cloud/binaryauthorization_v1beta1/types/continuous_validation_logging.py`

 * *Files identical despite different names*

### Comparing `google-cloud-binary-authorization-1.6.1/google/cloud/binaryauthorization_v1beta1/types/resources.py` & `google-cloud-binary-authorization-1.6.2/google/cloud/binaryauthorization_v1beta1/types/resources.py`

 * *Files identical despite different names*

### Comparing `google-cloud-binary-authorization-1.6.1/google/cloud/binaryauthorization_v1beta1/types/service.py` & `google-cloud-binary-authorization-1.6.2/google/cloud/binaryauthorization_v1beta1/types/service.py`

 * *Files identical despite different names*

### Comparing `google-cloud-binary-authorization-1.6.1/google_cloud_binary_authorization.egg-info/PKG-INFO` & `google-cloud-binary-authorization-1.6.2/google_cloud_binary_authorization.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-binary-authorization
-Version: 1.6.1
+Version: 1.6.2
 Summary: Google Cloud Binaryauthorization API client library
 Home-page: https://github.com/googleapis/python-binary-authorization
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `google-cloud-binary-authorization-1.6.1/google_cloud_binary_authorization.egg-info/SOURCES.txt` & `google-cloud-binary-authorization-1.6.2/google_cloud_binary_authorization.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `google-cloud-binary-authorization-1.6.1/setup.py` & `google-cloud-binary-authorization-1.6.2/setup.py`

 * *Files identical despite different names*

### Comparing `google-cloud-binary-authorization-1.6.1/tests/__init__.py` & `google-cloud-binary-authorization-1.6.2/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-binary-authorization-1.6.1/tests/unit/__init__.py` & `google-cloud-binary-authorization-1.6.2/tests/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-binary-authorization-1.6.1/tests/unit/gapic/__init__.py` & `google-cloud-binary-authorization-1.6.2/tests/unit/gapic/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-binary-authorization-1.6.1/tests/unit/gapic/binaryauthorization_v1/__init__.py` & `google-cloud-binary-authorization-1.6.2/tests/unit/gapic/binaryauthorization_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-binary-authorization-1.6.1/tests/unit/gapic/binaryauthorization_v1/test_binauthz_management_service_v1.py` & `google-cloud-binary-authorization-1.6.2/tests/unit/gapic/binaryauthorization_v1/test_binauthz_management_service_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1261,17 +1261,14 @@
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(type(client.transport.create_attestor), "__call__") as call:
         # Designate an appropriate return value for the call.
         call.return_value = resources.Attestor(
             name="name_value",
             description="description_value",
-            user_owned_grafeas_note=resources.UserOwnedGrafeasNote(
-                note_reference="note_reference_value"
-            ),
         )
         response = client.create_attestor(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
         assert args[0] == service.CreateAttestorRequest()
@@ -1516,17 +1513,14 @@
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(type(client.transport.get_attestor), "__call__") as call:
         # Designate an appropriate return value for the call.
         call.return_value = resources.Attestor(
             name="name_value",
             description="description_value",
-            user_owned_grafeas_note=resources.UserOwnedGrafeasNote(
-                note_reference="note_reference_value"
-            ),
         )
         response = client.get_attestor(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
         assert args[0] == service.GetAttestorRequest()
@@ -1751,17 +1745,14 @@
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(type(client.transport.update_attestor), "__call__") as call:
         # Designate an appropriate return value for the call.
         call.return_value = resources.Attestor(
             name="name_value",
             description="description_value",
-            user_owned_grafeas_note=resources.UserOwnedGrafeasNote(
-                note_reference="note_reference_value"
-            ),
         )
         response = client.update_attestor(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
         assert args[0] == service.UpdateAttestorRequest()
@@ -2375,17 +2366,19 @@
                     resources.Attestor(),
                     resources.Attestor(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.list_attestors(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
@@ -3214,17 +3207,14 @@
 
     # Mock the http request call within the method and fake a response.
     with mock.patch.object(type(client.transport._session), "request") as req:
         # Designate an appropriate value for the returned response.
         return_value = resources.Attestor(
             name="name_value",
             description="description_value",
-            user_owned_grafeas_note=resources.UserOwnedGrafeasNote(
-                note_reference="note_reference_value"
-            ),
         )
 
         # Wrap the value into a proper Response obj
         response_value = Response()
         response_value.status_code = 200
         pb_return_value = resources.Attestor.pb(return_value)
         json_return_value = json_format.MessageToJson(pb_return_value)
@@ -3530,17 +3520,14 @@
 
     # Mock the http request call within the method and fake a response.
     with mock.patch.object(type(client.transport._session), "request") as req:
         # Designate an appropriate value for the returned response.
         return_value = resources.Attestor(
             name="name_value",
             description="description_value",
-            user_owned_grafeas_note=resources.UserOwnedGrafeasNote(
-                note_reference="note_reference_value"
-            ),
         )
 
         # Wrap the value into a proper Response obj
         response_value = Response()
         response_value.status_code = 200
         pb_return_value = resources.Attestor.pb(return_value)
         json_return_value = json_format.MessageToJson(pb_return_value)
@@ -3815,17 +3802,14 @@
 
     # Mock the http request call within the method and fake a response.
     with mock.patch.object(type(client.transport._session), "request") as req:
         # Designate an appropriate value for the returned response.
         return_value = resources.Attestor(
             name="name_value",
             description="description_value",
-            user_owned_grafeas_note=resources.UserOwnedGrafeasNote(
-                note_reference="note_reference_value"
-            ),
         )
 
         # Wrap the value into a proper Response obj
         response_value = Response()
         response_value.status_code = 200
         pb_return_value = resources.Attestor.pb(return_value)
         json_return_value = json_format.MessageToJson(pb_return_value)
```

### Comparing `google-cloud-binary-authorization-1.6.1/tests/unit/gapic/binaryauthorization_v1/test_system_policy_v1.py` & `google-cloud-binary-authorization-1.6.2/tests/unit/gapic/binaryauthorization_v1/test_system_policy_v1.py`

 * *Files identical despite different names*

### Comparing `google-cloud-binary-authorization-1.6.1/tests/unit/gapic/binaryauthorization_v1/test_validation_helper_v1.py` & `google-cloud-binary-authorization-1.6.2/tests/unit/gapic/binaryauthorization_v1/test_validation_helper_v1.py`

 * *Files identical despite different names*

### Comparing `google-cloud-binary-authorization-1.6.1/tests/unit/gapic/binaryauthorization_v1beta1/__init__.py` & `google-cloud-binary-authorization-1.6.2/tests/unit/gapic/binaryauthorization_v1beta1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-binary-authorization-1.6.1/tests/unit/gapic/binaryauthorization_v1beta1/test_binauthz_management_service_v1_beta1.py` & `google-cloud-binary-authorization-1.6.2/tests/unit/gapic/binaryauthorization_v1beta1/test_binauthz_management_service_v1_beta1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1273,17 +1273,14 @@
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(type(client.transport.create_attestor), "__call__") as call:
         # Designate an appropriate return value for the call.
         call.return_value = resources.Attestor(
             name="name_value",
             description="description_value",
-            user_owned_drydock_note=resources.UserOwnedDrydockNote(
-                note_reference="note_reference_value"
-            ),
         )
         response = client.create_attestor(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
         assert args[0] == service.CreateAttestorRequest()
@@ -1528,17 +1525,14 @@
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(type(client.transport.get_attestor), "__call__") as call:
         # Designate an appropriate return value for the call.
         call.return_value = resources.Attestor(
             name="name_value",
             description="description_value",
-            user_owned_drydock_note=resources.UserOwnedDrydockNote(
-                note_reference="note_reference_value"
-            ),
         )
         response = client.get_attestor(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
         assert args[0] == service.GetAttestorRequest()
@@ -1763,17 +1757,14 @@
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(type(client.transport.update_attestor), "__call__") as call:
         # Designate an appropriate return value for the call.
         call.return_value = resources.Attestor(
             name="name_value",
             description="description_value",
-            user_owned_drydock_note=resources.UserOwnedDrydockNote(
-                note_reference="note_reference_value"
-            ),
         )
         response = client.update_attestor(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
         assert args[0] == service.UpdateAttestorRequest()
@@ -2387,17 +2378,19 @@
                     resources.Attestor(),
                     resources.Attestor(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.list_attestors(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
@@ -3227,17 +3220,14 @@
 
     # Mock the http request call within the method and fake a response.
     with mock.patch.object(type(client.transport._session), "request") as req:
         # Designate an appropriate value for the returned response.
         return_value = resources.Attestor(
             name="name_value",
             description="description_value",
-            user_owned_drydock_note=resources.UserOwnedDrydockNote(
-                note_reference="note_reference_value"
-            ),
         )
 
         # Wrap the value into a proper Response obj
         response_value = Response()
         response_value.status_code = 200
         pb_return_value = resources.Attestor.pb(return_value)
         json_return_value = json_format.MessageToJson(pb_return_value)
@@ -3545,17 +3535,14 @@
 
     # Mock the http request call within the method and fake a response.
     with mock.patch.object(type(client.transport._session), "request") as req:
         # Designate an appropriate value for the returned response.
         return_value = resources.Attestor(
             name="name_value",
             description="description_value",
-            user_owned_drydock_note=resources.UserOwnedDrydockNote(
-                note_reference="note_reference_value"
-            ),
         )
 
         # Wrap the value into a proper Response obj
         response_value = Response()
         response_value.status_code = 200
         pb_return_value = resources.Attestor.pb(return_value)
         json_return_value = json_format.MessageToJson(pb_return_value)
@@ -3830,17 +3817,14 @@
 
     # Mock the http request call within the method and fake a response.
     with mock.patch.object(type(client.transport._session), "request") as req:
         # Designate an appropriate value for the returned response.
         return_value = resources.Attestor(
             name="name_value",
             description="description_value",
-            user_owned_drydock_note=resources.UserOwnedDrydockNote(
-                note_reference="note_reference_value"
-            ),
         )
 
         # Wrap the value into a proper Response obj
         response_value = Response()
         response_value.status_code = 200
         pb_return_value = resources.Attestor.pb(return_value)
         json_return_value = json_format.MessageToJson(pb_return_value)
```

### Comparing `google-cloud-binary-authorization-1.6.1/tests/unit/gapic/binaryauthorization_v1beta1/test_system_policy_v1_beta1.py` & `google-cloud-binary-authorization-1.6.2/tests/unit/gapic/binaryauthorization_v1beta1/test_system_policy_v1_beta1.py`

 * *Files identical despite different names*

