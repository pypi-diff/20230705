# Comparing `tmp/google-cloud-iam-2.8.2.tar.gz` & `tmp/google-cloud-iam-2.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-cloud-iam-2.8.2.tar", last modified: Tue Aug 16 16:29:09 2022, max compression
+gzip compressed data, was "google-cloud-iam-2.9.0.tar", last modified: Mon Oct 24 19:24:54 2022, max compression
```

## Comparing `google-cloud-iam-2.8.2.tar` & `google-cloud-iam-2.9.0.tar`

### file list

```diff
@@ -1,73 +1,96 @@
-drwxr-sr-x   0 root         (0)     1003        0 2022-08-16 16:29:09.254753 google-cloud-iam-2.8.2/
--rw-rw-r--   0 root         (0)     1003    11358 2022-08-16 16:26:25.000000 google-cloud-iam-2.8.2/LICENSE
--rw-rw-r--   0 root         (0)     1003      860 2022-08-16 16:26:25.000000 google-cloud-iam-2.8.2/MANIFEST.in
--rw-r--r--   0 root         (0)     1003     4803 2022-08-16 16:29:09.258754 google-cloud-iam-2.8.2/PKG-INFO
--rw-rw-r--   0 root         (0)     1003     3913 2022-08-16 16:26:25.000000 google-cloud-iam-2.8.2/README.rst
-drwxr-sr-x   0 root         (0)     1003        0 2022-08-16 16:29:09.246752 google-cloud-iam-2.8.2/google/
-drwxr-sr-x   0 root         (0)     1003        0 2022-08-16 16:29:09.246752 google-cloud-iam-2.8.2/google/cloud/
-drwxr-sr-x   0 root         (0)     1003        0 2022-08-16 16:29:09.246752 google-cloud-iam-2.8.2/google/cloud/iam_credentials/
--rw-rw-r--   0 root         (0)     1003     1389 2022-08-16 16:26:25.000000 google-cloud-iam-2.8.2/google/cloud/iam_credentials/__init__.py
--rw-rw-r--   0 root         (0)     1003       77 2022-08-16 16:26:25.000000 google-cloud-iam-2.8.2/google/cloud/iam_credentials/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2022-08-16 16:29:09.250753 google-cloud-iam-2.8.2/google/cloud/iam_credentials_v1/
--rw-rw-r--   0 root         (0)     1003     1221 2022-08-16 16:26:25.000000 google-cloud-iam-2.8.2/google/cloud/iam_credentials_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003     1523 2022-08-16 16:26:25.000000 google-cloud-iam-2.8.2/google/cloud/iam_credentials_v1/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003       77 2022-08-16 16:26:25.000000 google-cloud-iam-2.8.2/google/cloud/iam_credentials_v1/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2022-08-16 16:29:09.250753 google-cloud-iam-2.8.2/google/cloud/iam_credentials_v1/services/
--rw-rw-r--   0 root         (0)     1003      600 2022-08-16 16:26:25.000000 google-cloud-iam-2.8.2/google/cloud/iam_credentials_v1/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-08-16 16:29:09.250753 google-cloud-iam-2.8.2/google/cloud/iam_credentials_v1/services/iam_credentials/
--rw-rw-r--   0 root         (0)     1003      769 2022-08-16 16:26:25.000000 google-cloud-iam-2.8.2/google/cloud/iam_credentials_v1/services/iam_credentials/__init__.py
--rw-rw-r--   0 root         (0)     1003    33469 2022-08-16 16:26:25.000000 google-cloud-iam-2.8.2/google/cloud/iam_credentials_v1/services/iam_credentials/async_client.py
--rw-rw-r--   0 root         (0)     1003    41351 2022-08-16 16:26:25.000000 google-cloud-iam-2.8.2/google/cloud/iam_credentials_v1/services/iam_credentials/client.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-08-16 16:29:09.250753 google-cloud-iam-2.8.2/google/cloud/iam_credentials_v1/services/iam_credentials/transports/
--rw-rw-r--   0 root         (0)     1003     1193 2022-08-16 16:26:25.000000 google-cloud-iam-2.8.2/google/cloud/iam_credentials_v1/services/iam_credentials/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     9076 2022-08-16 16:26:25.000000 google-cloud-iam-2.8.2/google/cloud/iam_credentials_v1/services/iam_credentials/transports/base.py
--rw-rw-r--   0 root         (0)     1003    15526 2022-08-16 16:26:25.000000 google-cloud-iam-2.8.2/google/cloud/iam_credentials_v1/services/iam_credentials/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    15863 2022-08-16 16:26:25.000000 google-cloud-iam-2.8.2/google/cloud/iam_credentials_v1/services/iam_credentials/transports/grpc_asyncio.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-08-16 16:29:09.250753 google-cloud-iam-2.8.2/google/cloud/iam_credentials_v1/types/
--rw-rw-r--   0 root         (0)     1003     1067 2022-08-16 16:26:25.000000 google-cloud-iam-2.8.2/google/cloud/iam_credentials_v1/types/__init__.py
--rw-rw-r--   0 root         (0)     1003     9482 2022-08-16 16:26:25.000000 google-cloud-iam-2.8.2/google/cloud/iam_credentials_v1/types/common.py
--rw-rw-r--   0 root         (0)     1003      740 2022-08-16 16:26:25.000000 google-cloud-iam-2.8.2/google/cloud/iam_credentials_v1/types/iamcredentials.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-08-16 16:29:09.250753 google-cloud-iam-2.8.2/google/cloud/iam_v2beta/
--rw-rw-r--   0 root         (0)     1003     1239 2022-08-16 16:26:25.000000 google-cloud-iam-2.8.2/google/cloud/iam_v2beta/__init__.py
--rw-rw-r--   0 root         (0)     1003     1709 2022-08-16 16:26:25.000000 google-cloud-iam-2.8.2/google/cloud/iam_v2beta/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003       77 2022-08-16 16:26:25.000000 google-cloud-iam-2.8.2/google/cloud/iam_v2beta/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2022-08-16 16:29:09.250753 google-cloud-iam-2.8.2/google/cloud/iam_v2beta/services/
--rw-rw-r--   0 root         (0)     1003      600 2022-08-16 16:26:25.000000 google-cloud-iam-2.8.2/google/cloud/iam_v2beta/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-08-16 16:29:09.250753 google-cloud-iam-2.8.2/google/cloud/iam_v2beta/services/policies/
--rw-rw-r--   0 root         (0)     1003      745 2022-08-16 16:26:25.000000 google-cloud-iam-2.8.2/google/cloud/iam_v2beta/services/policies/__init__.py
--rw-rw-r--   0 root         (0)     1003    32807 2022-08-16 16:26:25.000000 google-cloud-iam-2.8.2/google/cloud/iam_v2beta/services/policies/async_client.py
--rw-rw-r--   0 root         (0)     1003    40546 2022-08-16 16:26:25.000000 google-cloud-iam-2.8.2/google/cloud/iam_v2beta/services/policies/client.py
--rw-rw-r--   0 root         (0)     1003     5655 2022-08-16 16:26:25.000000 google-cloud-iam-2.8.2/google/cloud/iam_v2beta/services/policies/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-08-16 16:29:09.254753 google-cloud-iam-2.8.2/google/cloud/iam_v2beta/services/policies/transports/
--rw-rw-r--   0 root         (0)     1003     1139 2022-08-16 16:26:25.000000 google-cloud-iam-2.8.2/google/cloud/iam_v2beta/services/policies/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     9743 2022-08-16 16:26:25.000000 google-cloud-iam-2.8.2/google/cloud/iam_v2beta/services/policies/transports/base.py
--rw-rw-r--   0 root         (0)     1003    17082 2022-08-16 16:26:25.000000 google-cloud-iam-2.8.2/google/cloud/iam_v2beta/services/policies/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    17442 2022-08-16 16:26:25.000000 google-cloud-iam-2.8.2/google/cloud/iam_v2beta/services/policies/transports/grpc_asyncio.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-08-16 16:29:09.254753 google-cloud-iam-2.8.2/google/cloud/iam_v2beta/types/
--rw-rw-r--   0 root         (0)     1003     1110 2022-08-16 16:26:25.000000 google-cloud-iam-2.8.2/google/cloud/iam_v2beta/types/__init__.py
--rw-rw-r--   0 root         (0)     1003     6162 2022-08-16 16:26:25.000000 google-cloud-iam-2.8.2/google/cloud/iam_v2beta/types/deny.py
--rw-rw-r--   0 root         (0)     1003    11926 2022-08-16 16:26:25.000000 google-cloud-iam-2.8.2/google/cloud/iam_v2beta/types/policy.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-08-16 16:29:09.254753 google-cloud-iam-2.8.2/google_cloud_iam.egg-info/
--rw-r--r--   0 root         (0)     1003     4803 2022-08-16 16:29:09.000000 google-cloud-iam-2.8.2/google_cloud_iam.egg-info/PKG-INFO
--rw-r--r--   0 root         (0)     1003     2342 2022-08-16 16:29:09.000000 google-cloud-iam-2.8.2/google_cloud_iam.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0)     1003        1 2022-08-16 16:29:09.000000 google-cloud-iam-2.8.2/google_cloud_iam.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0)     1003       20 2022-08-16 16:29:09.000000 google-cloud-iam-2.8.2/google_cloud_iam.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0)     1003        1 2022-08-16 16:29:09.000000 google-cloud-iam-2.8.2/google_cloud_iam.egg-info/not-zip-safe
--rw-r--r--   0 root         (0)     1003      183 2022-08-16 16:29:09.000000 google-cloud-iam-2.8.2/google_cloud_iam.egg-info/requires.txt
--rw-r--r--   0 root         (0)     1003        7 2022-08-16 16:29:09.000000 google-cloud-iam-2.8.2/google_cloud_iam.egg-info/top_level.txt
-drwxr-sr-x   0 root         (0)     1003        0 2022-08-16 16:29:09.254753 google-cloud-iam-2.8.2/scripts/
--rw-rw-r--   0 root         (0)     1003     6200 2022-08-16 16:26:25.000000 google-cloud-iam-2.8.2/scripts/fixup_iam_credentials_v1_keywords.py
--rw-rw-r--   0 root         (0)     1003       67 2022-08-16 16:29:09.258754 google-cloud-iam-2.8.2/setup.cfg
--rw-rw-r--   0 root         (0)     1003     2705 2022-08-16 16:26:25.000000 google-cloud-iam-2.8.2/setup.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-08-16 16:29:09.254753 google-cloud-iam-2.8.2/tests/
--rw-rw-r--   0 root         (0)     1003      600 2022-08-16 16:26:25.000000 google-cloud-iam-2.8.2/tests/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-08-16 16:29:09.254753 google-cloud-iam-2.8.2/tests/unit/
--rw-rw-r--   0 root         (0)     1003      600 2022-08-16 16:26:25.000000 google-cloud-iam-2.8.2/tests/unit/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-08-16 16:29:09.254753 google-cloud-iam-2.8.2/tests/unit/gapic/
--rw-rw-r--   0 root         (0)     1003      600 2022-08-16 16:26:25.000000 google-cloud-iam-2.8.2/tests/unit/gapic/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-08-16 16:29:09.254753 google-cloud-iam-2.8.2/tests/unit/gapic/iam_credentials_v1/
--rw-rw-r--   0 root         (0)     1003      600 2022-08-16 16:26:25.000000 google-cloud-iam-2.8.2/tests/unit/gapic/iam_credentials_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003    87289 2022-08-16 16:26:25.000000 google-cloud-iam-2.8.2/tests/unit/gapic/iam_credentials_v1/test_iam_credentials.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-08-16 16:29:09.254753 google-cloud-iam-2.8.2/tests/unit/gapic/iam_v2beta/
--rw-rw-r--   0 root         (0)     1003      600 2022-08-16 16:26:25.000000 google-cloud-iam-2.8.2/tests/unit/gapic/iam_v2beta/__init__.py
--rw-rw-r--   0 root         (0)     1003    94740 2022-08-16 16:26:25.000000 google-cloud-iam-2.8.2/tests/unit/gapic/iam_v2beta/test_policies.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-10-24 19:24:54.259108 google-cloud-iam-2.9.0/
+-rw-rw-r--   0 root         (0)     1003    11358 2022-10-24 19:21:29.000000 google-cloud-iam-2.9.0/LICENSE
+-rw-rw-r--   0 root         (0)     1003      860 2022-10-24 19:21:29.000000 google-cloud-iam-2.9.0/MANIFEST.in
+-rw-r--r--   0 root         (0)     1003     4803 2022-10-24 19:24:54.259108 google-cloud-iam-2.9.0/PKG-INFO
+-rw-rw-r--   0 root         (0)     1003     3913 2022-10-24 19:21:29.000000 google-cloud-iam-2.9.0/README.rst
+drwxr-sr-x   0 root         (0)     1003        0 2022-10-24 19:24:54.243109 google-cloud-iam-2.9.0/google/
+drwxr-sr-x   0 root         (0)     1003        0 2022-10-24 19:24:54.243109 google-cloud-iam-2.9.0/google/cloud/
+drwxr-sr-x   0 root         (0)     1003        0 2022-10-24 19:24:54.247109 google-cloud-iam-2.9.0/google/cloud/iam_credentials/
+-rw-rw-r--   0 root         (0)     1003     1389 2022-10-24 19:21:29.000000 google-cloud-iam-2.9.0/google/cloud/iam_credentials/__init__.py
+-rw-rw-r--   0 root         (0)     1003       77 2022-10-24 19:21:29.000000 google-cloud-iam-2.9.0/google/cloud/iam_credentials/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2022-10-24 19:24:54.247109 google-cloud-iam-2.9.0/google/cloud/iam_credentials_v1/
+-rw-rw-r--   0 root         (0)     1003     1221 2022-10-24 19:21:29.000000 google-cloud-iam-2.9.0/google/cloud/iam_credentials_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003     1523 2022-10-24 19:21:29.000000 google-cloud-iam-2.9.0/google/cloud/iam_credentials_v1/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003       77 2022-10-24 19:21:29.000000 google-cloud-iam-2.9.0/google/cloud/iam_credentials_v1/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2022-10-24 19:24:54.247109 google-cloud-iam-2.9.0/google/cloud/iam_credentials_v1/services/
+-rw-rw-r--   0 root         (0)     1003      600 2022-10-24 19:21:29.000000 google-cloud-iam-2.9.0/google/cloud/iam_credentials_v1/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-10-24 19:24:54.251109 google-cloud-iam-2.9.0/google/cloud/iam_credentials_v1/services/iam_credentials/
+-rw-rw-r--   0 root         (0)     1003      769 2022-10-24 19:21:29.000000 google-cloud-iam-2.9.0/google/cloud/iam_credentials_v1/services/iam_credentials/__init__.py
+-rw-rw-r--   0 root         (0)     1003    35347 2022-10-24 19:21:29.000000 google-cloud-iam-2.9.0/google/cloud/iam_credentials_v1/services/iam_credentials/async_client.py
+-rw-rw-r--   0 root         (0)     1003    43229 2022-10-24 19:21:29.000000 google-cloud-iam-2.9.0/google/cloud/iam_credentials_v1/services/iam_credentials/client.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-10-24 19:24:54.251109 google-cloud-iam-2.9.0/google/cloud/iam_credentials_v1/services/iam_credentials/transports/
+-rw-rw-r--   0 root         (0)     1003     1193 2022-10-24 19:21:29.000000 google-cloud-iam-2.9.0/google/cloud/iam_credentials_v1/services/iam_credentials/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     9076 2022-10-24 19:21:29.000000 google-cloud-iam-2.9.0/google/cloud/iam_credentials_v1/services/iam_credentials/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    15526 2022-10-24 19:21:29.000000 google-cloud-iam-2.9.0/google/cloud/iam_credentials_v1/services/iam_credentials/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    15863 2022-10-24 19:21:29.000000 google-cloud-iam-2.9.0/google/cloud/iam_credentials_v1/services/iam_credentials/transports/grpc_asyncio.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-10-24 19:24:54.251109 google-cloud-iam-2.9.0/google/cloud/iam_credentials_v1/types/
+-rw-rw-r--   0 root         (0)     1003     1067 2022-10-24 19:21:29.000000 google-cloud-iam-2.9.0/google/cloud/iam_credentials_v1/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003     9482 2022-10-24 19:21:29.000000 google-cloud-iam-2.9.0/google/cloud/iam_credentials_v1/types/common.py
+-rw-rw-r--   0 root         (0)     1003      740 2022-10-24 19:21:29.000000 google-cloud-iam-2.9.0/google/cloud/iam_credentials_v1/types/iamcredentials.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-10-24 19:24:54.251109 google-cloud-iam-2.9.0/google/cloud/iam_v2/
+-rw-rw-r--   0 root         (0)     1003     1239 2022-10-24 19:21:29.000000 google-cloud-iam-2.9.0/google/cloud/iam_v2/__init__.py
+-rw-rw-r--   0 root         (0)     1003     1701 2022-10-24 19:21:29.000000 google-cloud-iam-2.9.0/google/cloud/iam_v2/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003       77 2022-10-24 19:21:29.000000 google-cloud-iam-2.9.0/google/cloud/iam_v2/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2022-10-24 19:24:54.251109 google-cloud-iam-2.9.0/google/cloud/iam_v2/services/
+-rw-rw-r--   0 root         (0)     1003      600 2022-10-24 19:21:29.000000 google-cloud-iam-2.9.0/google/cloud/iam_v2/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-10-24 19:24:54.251109 google-cloud-iam-2.9.0/google/cloud/iam_v2/services/policies/
+-rw-rw-r--   0 root         (0)     1003      745 2022-10-24 19:21:29.000000 google-cloud-iam-2.9.0/google/cloud/iam_v2/services/policies/__init__.py
+-rw-rw-r--   0 root         (0)     1003    36941 2022-10-24 19:21:29.000000 google-cloud-iam-2.9.0/google/cloud/iam_v2/services/policies/async_client.py
+-rw-rw-r--   0 root         (0)     1003    44341 2022-10-24 19:21:29.000000 google-cloud-iam-2.9.0/google/cloud/iam_v2/services/policies/client.py
+-rw-rw-r--   0 root         (0)     1003     5619 2022-10-24 19:21:29.000000 google-cloud-iam-2.9.0/google/cloud/iam_v2/services/policies/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-10-24 19:24:54.251109 google-cloud-iam-2.9.0/google/cloud/iam_v2/services/policies/transports/
+-rw-rw-r--   0 root         (0)     1003     1139 2022-10-24 19:21:29.000000 google-cloud-iam-2.9.0/google/cloud/iam_v2/services/policies/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     9973 2022-10-24 19:21:29.000000 google-cloud-iam-2.9.0/google/cloud/iam_v2/services/policies/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    17879 2022-10-24 19:21:29.000000 google-cloud-iam-2.9.0/google/cloud/iam_v2/services/policies/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    18239 2022-10-24 19:21:29.000000 google-cloud-iam-2.9.0/google/cloud/iam_v2/services/policies/transports/grpc_asyncio.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-10-24 19:24:54.251109 google-cloud-iam-2.9.0/google/cloud/iam_v2/types/
+-rw-rw-r--   0 root         (0)     1003     1110 2022-10-24 19:21:29.000000 google-cloud-iam-2.9.0/google/cloud/iam_v2/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003     6179 2022-10-24 19:21:29.000000 google-cloud-iam-2.9.0/google/cloud/iam_v2/types/deny.py
+-rw-rw-r--   0 root         (0)     1003    12175 2022-10-24 19:21:29.000000 google-cloud-iam-2.9.0/google/cloud/iam_v2/types/policy.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-10-24 19:24:54.251109 google-cloud-iam-2.9.0/google/cloud/iam_v2beta/
+-rw-rw-r--   0 root         (0)     1003     1239 2022-10-24 19:21:29.000000 google-cloud-iam-2.9.0/google/cloud/iam_v2beta/__init__.py
+-rw-rw-r--   0 root         (0)     1003     1709 2022-10-24 19:21:29.000000 google-cloud-iam-2.9.0/google/cloud/iam_v2beta/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003       77 2022-10-24 19:21:29.000000 google-cloud-iam-2.9.0/google/cloud/iam_v2beta/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2022-10-24 19:24:54.251109 google-cloud-iam-2.9.0/google/cloud/iam_v2beta/services/
+-rw-rw-r--   0 root         (0)     1003      600 2022-10-24 19:21:29.000000 google-cloud-iam-2.9.0/google/cloud/iam_v2beta/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-10-24 19:24:54.251109 google-cloud-iam-2.9.0/google/cloud/iam_v2beta/services/policies/
+-rw-rw-r--   0 root         (0)     1003      745 2022-10-24 19:21:29.000000 google-cloud-iam-2.9.0/google/cloud/iam_v2beta/services/policies/__init__.py
+-rw-rw-r--   0 root         (0)     1003    37061 2022-10-24 19:21:29.000000 google-cloud-iam-2.9.0/google/cloud/iam_v2beta/services/policies/async_client.py
+-rw-rw-r--   0 root         (0)     1003    44461 2022-10-24 19:21:29.000000 google-cloud-iam-2.9.0/google/cloud/iam_v2beta/services/policies/client.py
+-rw-rw-r--   0 root         (0)     1003     5655 2022-10-24 19:21:29.000000 google-cloud-iam-2.9.0/google/cloud/iam_v2beta/services/policies/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-10-24 19:24:54.255109 google-cloud-iam-2.9.0/google/cloud/iam_v2beta/services/policies/transports/
+-rw-rw-r--   0 root         (0)     1003     1139 2022-10-24 19:21:29.000000 google-cloud-iam-2.9.0/google/cloud/iam_v2beta/services/policies/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     9981 2022-10-24 19:21:29.000000 google-cloud-iam-2.9.0/google/cloud/iam_v2beta/services/policies/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    17911 2022-10-24 19:21:29.000000 google-cloud-iam-2.9.0/google/cloud/iam_v2beta/services/policies/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    18271 2022-10-24 19:21:29.000000 google-cloud-iam-2.9.0/google/cloud/iam_v2beta/services/policies/transports/grpc_asyncio.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-10-24 19:24:54.255109 google-cloud-iam-2.9.0/google/cloud/iam_v2beta/types/
+-rw-rw-r--   0 root         (0)     1003     1110 2022-10-24 19:21:29.000000 google-cloud-iam-2.9.0/google/cloud/iam_v2beta/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003     6183 2022-10-24 19:21:29.000000 google-cloud-iam-2.9.0/google/cloud/iam_v2beta/types/deny.py
+-rw-rw-r--   0 root         (0)     1003    11926 2022-10-24 19:21:29.000000 google-cloud-iam-2.9.0/google/cloud/iam_v2beta/types/policy.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-10-24 19:24:54.255109 google-cloud-iam-2.9.0/google_cloud_iam.egg-info/
+-rw-r--r--   0 root         (0)     1003     4803 2022-10-24 19:24:54.000000 google-cloud-iam-2.9.0/google_cloud_iam.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0)     1003     3109 2022-10-24 19:24:54.000000 google-cloud-iam-2.9.0/google_cloud_iam.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0)     1003        1 2022-10-24 19:24:54.000000 google-cloud-iam-2.9.0/google_cloud_iam.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0)     1003       20 2022-10-24 19:24:54.000000 google-cloud-iam-2.9.0/google_cloud_iam.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0)     1003        1 2022-10-24 19:24:54.000000 google-cloud-iam-2.9.0/google_cloud_iam.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0)     1003      255 2022-10-24 19:24:54.000000 google-cloud-iam-2.9.0/google_cloud_iam.egg-info/requires.txt
+-rw-r--r--   0 root         (0)     1003        7 2022-10-24 19:24:54.000000 google-cloud-iam-2.9.0/google_cloud_iam.egg-info/top_level.txt
+drwxr-sr-x   0 root         (0)     1003        0 2022-10-24 19:24:54.255109 google-cloud-iam-2.9.0/scripts/
+-rw-rw-r--   0 root         (0)     1003     6200 2022-10-24 19:21:29.000000 google-cloud-iam-2.9.0/scripts/fixup_iam_credentials_v1_keywords.py
+-rw-rw-r--   0 root         (0)     1003       67 2022-10-24 19:24:54.259108 google-cloud-iam-2.9.0/setup.cfg
+-rw-rw-r--   0 root         (0)     1003     2774 2022-10-24 19:21:29.000000 google-cloud-iam-2.9.0/setup.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-10-24 19:24:54.255109 google-cloud-iam-2.9.0/tests/
+-rw-rw-r--   0 root         (0)     1003      600 2022-10-24 19:21:29.000000 google-cloud-iam-2.9.0/tests/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-10-24 19:24:54.255109 google-cloud-iam-2.9.0/tests/unit/
+-rw-rw-r--   0 root         (0)     1003      600 2022-10-24 19:21:29.000000 google-cloud-iam-2.9.0/tests/unit/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-10-24 19:24:54.255109 google-cloud-iam-2.9.0/tests/unit/gapic/
+-rw-rw-r--   0 root         (0)     1003      600 2022-10-24 19:21:29.000000 google-cloud-iam-2.9.0/tests/unit/gapic/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-10-24 19:24:54.259108 google-cloud-iam-2.9.0/tests/unit/gapic/iam_credentials_v1/
+-rw-rw-r--   0 root         (0)     1003      600 2022-10-24 19:21:29.000000 google-cloud-iam-2.9.0/tests/unit/gapic/iam_credentials_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003    87370 2022-10-24 19:21:29.000000 google-cloud-iam-2.9.0/tests/unit/gapic/iam_credentials_v1/test_iam_credentials.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-10-24 19:24:54.259108 google-cloud-iam-2.9.0/tests/unit/gapic/iam_v2/
+-rw-rw-r--   0 root         (0)     1003      600 2022-10-24 19:21:29.000000 google-cloud-iam-2.9.0/tests/unit/gapic/iam_v2/__init__.py
+-rw-rw-r--   0 root         (0)     1003    99964 2022-10-24 19:21:29.000000 google-cloud-iam-2.9.0/tests/unit/gapic/iam_v2/test_policies.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-10-24 19:24:54.259108 google-cloud-iam-2.9.0/tests/unit/gapic/iam_v2beta/
+-rw-rw-r--   0 root         (0)     1003      600 2022-10-24 19:21:29.000000 google-cloud-iam-2.9.0/tests/unit/gapic/iam_v2beta/__init__.py
+-rw-rw-r--   0 root         (0)     1003    99736 2022-10-24 19:21:29.000000 google-cloud-iam-2.9.0/tests/unit/gapic/iam_v2beta/test_policies.py
```

### Comparing `google-cloud-iam-2.8.2/LICENSE` & `google-cloud-iam-2.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `google-cloud-iam-2.8.2/MANIFEST.in` & `google-cloud-iam-2.9.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `google-cloud-iam-2.8.2/PKG-INFO` & `google-cloud-iam-2.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-iam
-Version: 2.8.2
+Version: 2.9.0
 Summary: IAM Service Account Credentials API client library
 Home-page: https://github.com/googleapis/python-iam
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `google-cloud-iam-2.8.2/README.rst` & `google-cloud-iam-2.9.0/README.rst`

 * *Files identical despite different names*

### Comparing `google-cloud-iam-2.8.2/google/cloud/iam_credentials/__init__.py` & `google-cloud-iam-2.9.0/google/cloud/iam_credentials/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-iam-2.8.2/google/cloud/iam_credentials_v1/__init__.py` & `google-cloud-iam-2.9.0/google/cloud/iam_credentials_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-iam-2.8.2/google/cloud/iam_credentials_v1/gapic_metadata.json` & `google-cloud-iam-2.9.0/google/cloud/iam_credentials_v1/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-cloud-iam-2.8.2/google/cloud/iam_credentials_v1/services/__init__.py` & `google-cloud-iam-2.9.0/google/cloud/iam_credentials_v1/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-iam-2.8.2/google/cloud/iam_credentials_v1/services/iam_credentials/__init__.py` & `google-cloud-iam-2.9.0/google/cloud/iam_credentials_v1/services/iam_credentials/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-iam-2.8.2/google/cloud/iam_credentials_v1/services/iam_credentials/async_client.py` & `google-cloud-iam-2.9.0/google/cloud/iam_credentials_v1/services/iam_credentials/async_client.py`

 * *Files 4% similar despite different names*

```diff
@@ -230,24 +230,31 @@
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> common.GenerateAccessTokenResponse:
         r"""Generates an OAuth 2.0 access token for a service
         account.
 
         .. code-block:: python
 
+            # This snippet has been automatically generated and should be regarded as a
+            # code template only.
+            # It will require modifications to work:
+            # - It may require correct/in-range values for request initialization.
+            # - It may require specifying regional endpoints when creating the service
+            #   client as shown in:
+            #   https://googleapis.dev/python/google-api-core/latest/client_options.html
             from google.cloud import iam_credentials_v1
 
             async def sample_generate_access_token():
                 # Create a client
                 client = iam_credentials_v1.IAMCredentialsAsyncClient()
 
                 # Initialize request argument(s)
                 request = iam_credentials_v1.GenerateAccessTokenRequest(
                     name="name_value",
-                    scope=['scope_value_1', 'scope_value_2'],
+                    scope=['scope_value1', 'scope_value2'],
                 )
 
                 # Make the request
                 response = await client.generate_access_token(request=request)
 
                 # Handle the response
                 print(response)
@@ -387,14 +394,21 @@
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> common.GenerateIdTokenResponse:
         r"""Generates an OpenID Connect ID token for a service
         account.
 
         .. code-block:: python
 
+            # This snippet has been automatically generated and should be regarded as a
+            # code template only.
+            # It will require modifications to work:
+            # - It may require correct/in-range values for request initialization.
+            # - It may require specifying regional endpoints when creating the service
+            #   client as shown in:
+            #   https://googleapis.dev/python/google-api-core/latest/client_options.html
             from google.cloud import iam_credentials_v1
 
             async def sample_generate_id_token():
                 # Create a client
                 client = iam_credentials_v1.IAMCredentialsAsyncClient()
 
                 # Initialize request argument(s)
@@ -537,14 +551,21 @@
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> common.SignBlobResponse:
         r"""Signs a blob using a service account's system-managed
         private key.
 
         .. code-block:: python
 
+            # This snippet has been automatically generated and should be regarded as a
+            # code template only.
+            # It will require modifications to work:
+            # - It may require correct/in-range values for request initialization.
+            # - It may require specifying regional endpoints when creating the service
+            #   client as shown in:
+            #   https://googleapis.dev/python/google-api-core/latest/client_options.html
             from google.cloud import iam_credentials_v1
 
             async def sample_sign_blob():
                 # Create a client
                 client = iam_credentials_v1.IAMCredentialsAsyncClient()
 
                 # Initialize request argument(s)
@@ -674,14 +695,21 @@
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> common.SignJwtResponse:
         r"""Signs a JWT using a service account's system-managed
         private key.
 
         .. code-block:: python
 
+            # This snippet has been automatically generated and should be regarded as a
+            # code template only.
+            # It will require modifications to work:
+            # - It may require correct/in-range values for request initialization.
+            # - It may require specifying regional endpoints when creating the service
+            #   client as shown in:
+            #   https://googleapis.dev/python/google-api-core/latest/client_options.html
             from google.cloud import iam_credentials_v1
 
             async def sample_sign_jwt():
                 # Create a client
                 client = iam_credentials_v1.IAMCredentialsAsyncClient()
 
                 # Initialize request argument(s)
```

### Comparing `google-cloud-iam-2.8.2/google/cloud/iam_credentials_v1/services/iam_credentials/client.py` & `google-cloud-iam-2.9.0/google/cloud/iam_credentials_v1/services/iam_credentials/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -451,24 +451,31 @@
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> common.GenerateAccessTokenResponse:
         r"""Generates an OAuth 2.0 access token for a service
         account.
 
         .. code-block:: python
 
+            # This snippet has been automatically generated and should be regarded as a
+            # code template only.
+            # It will require modifications to work:
+            # - It may require correct/in-range values for request initialization.
+            # - It may require specifying regional endpoints when creating the service
+            #   client as shown in:
+            #   https://googleapis.dev/python/google-api-core/latest/client_options.html
             from google.cloud import iam_credentials_v1
 
             def sample_generate_access_token():
                 # Create a client
                 client = iam_credentials_v1.IAMCredentialsClient()
 
                 # Initialize request argument(s)
                 request = iam_credentials_v1.GenerateAccessTokenRequest(
                     name="name_value",
-                    scope=['scope_value_1', 'scope_value_2'],
+                    scope=['scope_value1', 'scope_value2'],
                 )
 
                 # Make the request
                 response = client.generate_access_token(request=request)
 
                 # Handle the response
                 print(response)
@@ -598,14 +605,21 @@
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> common.GenerateIdTokenResponse:
         r"""Generates an OpenID Connect ID token for a service
         account.
 
         .. code-block:: python
 
+            # This snippet has been automatically generated and should be regarded as a
+            # code template only.
+            # It will require modifications to work:
+            # - It may require correct/in-range values for request initialization.
+            # - It may require specifying regional endpoints when creating the service
+            #   client as shown in:
+            #   https://googleapis.dev/python/google-api-core/latest/client_options.html
             from google.cloud import iam_credentials_v1
 
             def sample_generate_id_token():
                 # Create a client
                 client = iam_credentials_v1.IAMCredentialsClient()
 
                 # Initialize request argument(s)
@@ -738,14 +752,21 @@
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> common.SignBlobResponse:
         r"""Signs a blob using a service account's system-managed
         private key.
 
         .. code-block:: python
 
+            # This snippet has been automatically generated and should be regarded as a
+            # code template only.
+            # It will require modifications to work:
+            # - It may require correct/in-range values for request initialization.
+            # - It may require specifying regional endpoints when creating the service
+            #   client as shown in:
+            #   https://googleapis.dev/python/google-api-core/latest/client_options.html
             from google.cloud import iam_credentials_v1
 
             def sample_sign_blob():
                 # Create a client
                 client = iam_credentials_v1.IAMCredentialsClient()
 
                 # Initialize request argument(s)
@@ -865,14 +886,21 @@
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> common.SignJwtResponse:
         r"""Signs a JWT using a service account's system-managed
         private key.
 
         .. code-block:: python
 
+            # This snippet has been automatically generated and should be regarded as a
+            # code template only.
+            # It will require modifications to work:
+            # - It may require correct/in-range values for request initialization.
+            # - It may require specifying regional endpoints when creating the service
+            #   client as shown in:
+            #   https://googleapis.dev/python/google-api-core/latest/client_options.html
             from google.cloud import iam_credentials_v1
 
             def sample_sign_jwt():
                 # Create a client
                 client = iam_credentials_v1.IAMCredentialsClient()
 
                 # Initialize request argument(s)
```

### Comparing `google-cloud-iam-2.8.2/google/cloud/iam_credentials_v1/services/iam_credentials/transports/__init__.py` & `google-cloud-iam-2.9.0/google/cloud/iam_credentials_v1/services/iam_credentials/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-iam-2.8.2/google/cloud/iam_credentials_v1/services/iam_credentials/transports/base.py` & `google-cloud-iam-2.9.0/google/cloud/iam_credentials_v1/services/iam_credentials/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-iam-2.8.2/google/cloud/iam_credentials_v1/services/iam_credentials/transports/grpc.py` & `google-cloud-iam-2.9.0/google/cloud/iam_credentials_v1/services/iam_credentials/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-iam-2.8.2/google/cloud/iam_credentials_v1/services/iam_credentials/transports/grpc_asyncio.py` & `google-cloud-iam-2.9.0/google/cloud/iam_credentials_v1/services/iam_credentials/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-iam-2.8.2/google/cloud/iam_credentials_v1/types/__init__.py` & `google-cloud-iam-2.9.0/google/cloud/iam_credentials_v1/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-iam-2.8.2/google/cloud/iam_credentials_v1/types/common.py` & `google-cloud-iam-2.9.0/google/cloud/iam_credentials_v1/types/common.py`

 * *Files identical despite different names*

### Comparing `google-cloud-iam-2.8.2/google/cloud/iam_credentials_v1/types/iamcredentials.py` & `google-cloud-iam-2.9.0/google/cloud/iam_credentials_v1/types/iamcredentials.py`

 * *Files identical despite different names*

### Comparing `google-cloud-iam-2.8.2/google/cloud/iam_v2beta/__init__.py` & `google-cloud-iam-2.9.0/google/cloud/iam_v2/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-iam-2.8.2/google/cloud/iam_v2beta/gapic_metadata.json` & `google-cloud-iam-2.9.0/google/cloud/iam_v2beta/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-cloud-iam-2.8.2/google/cloud/iam_v2beta/services/__init__.py` & `google-cloud-iam-2.9.0/google/cloud/iam_v2/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-iam-2.8.2/google/cloud/iam_v2beta/services/policies/__init__.py` & `google-cloud-iam-2.9.0/google/cloud/iam_v2/services/policies/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-iam-2.8.2/google/cloud/iam_v2beta/services/policies/async_client.py` & `google-cloud-iam-2.9.0/google/cloud/iam_v2beta/services/policies/async_client.py`

 * *Files 5% similar despite different names*

```diff
@@ -29,14 +29,15 @@
 try:
     OptionalRetry = Union[retries.Retry, gapic_v1.method._MethodDefault]
 except AttributeError:  # pragma: NO COVER
     OptionalRetry = Union[retries.Retry, object]  # type: ignore
 
 from google.api_core import operation  # type: ignore
 from google.api_core import operation_async  # type: ignore
+from google.longrunning import operations_pb2
 from google.protobuf import timestamp_pb2  # type: ignore
 
 from google.cloud.iam_v2beta.services.policies import pagers
 from google.cloud.iam_v2beta.types import policy
 from google.cloud.iam_v2beta.types import policy as gi_policy
 
 from .client import PoliciesClient
@@ -50,16 +51,14 @@
     """
 
     _client: PoliciesClient
 
     DEFAULT_ENDPOINT = PoliciesClient.DEFAULT_ENDPOINT
     DEFAULT_MTLS_ENDPOINT = PoliciesClient.DEFAULT_MTLS_ENDPOINT
 
-    policy_path = staticmethod(PoliciesClient.policy_path)
-    parse_policy_path = staticmethod(PoliciesClient.parse_policy_path)
     common_billing_account_path = staticmethod(
         PoliciesClient.common_billing_account_path
     )
     parse_common_billing_account_path = staticmethod(
         PoliciesClient.parse_common_billing_account_path
     )
     common_folder_path = staticmethod(PoliciesClient.common_folder_path)
@@ -215,14 +214,21 @@
         attached to a resource.
 
         The response lists only policy metadata. In particular,
         policy rules are omitted.
 
         .. code-block:: python
 
+            # This snippet has been automatically generated and should be regarded as a
+            # code template only.
+            # It will require modifications to work:
+            # - It may require correct/in-range values for request initialization.
+            # - It may require specifying regional endpoints when creating the service
+            #   client as shown in:
+            #   https://googleapis.dev/python/google-api-core/latest/client_options.html
             from google.cloud import iam_v2beta
 
             async def sample_list_policies():
                 # Create a client
                 client = iam_v2beta.PoliciesAsyncClient()
 
                 # Initialize request argument(s)
@@ -341,14 +347,21 @@
         timeout: float = None,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> policy.Policy:
         r"""Gets a policy.
 
         .. code-block:: python
 
+            # This snippet has been automatically generated and should be regarded as a
+            # code template only.
+            # It will require modifications to work:
+            # - It may require correct/in-range values for request initialization.
+            # - It may require specifying regional endpoints when creating the service
+            #   client as shown in:
+            #   https://googleapis.dev/python/google-api-core/latest/client_options.html
             from google.cloud import iam_v2beta
 
             async def sample_get_policy():
                 # Create a client
                 client = iam_v2beta.PoliciesAsyncClient()
 
                 # Initialize request argument(s)
@@ -454,14 +467,21 @@
         timeout: float = None,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> operation_async.AsyncOperation:
         r"""Creates a policy.
 
         .. code-block:: python
 
+            # This snippet has been automatically generated and should be regarded as a
+            # code template only.
+            # It will require modifications to work:
+            # - It may require correct/in-range values for request initialization.
+            # - It may require specifying regional endpoints when creating the service
+            #   client as shown in:
+            #   https://googleapis.dev/python/google-api-core/latest/client_options.html
             from google.cloud import iam_v2beta
 
             async def sample_create_policy():
                 # Create a client
                 client = iam_v2beta.PoliciesAsyncClient()
 
                 # Initialize request argument(s)
@@ -614,14 +634,21 @@
         2. Modify the policy as needed.
         3. Use ``UpdatePolicy`` to write the updated policy.
 
         This pattern helps prevent conflicts between concurrent updates.
 
         .. code-block:: python
 
+            # This snippet has been automatically generated and should be regarded as a
+            # code template only.
+            # It will require modifications to work:
+            # - It may require correct/in-range values for request initialization.
+            # - It may require specifying regional endpoints when creating the service
+            #   client as shown in:
+            #   https://googleapis.dev/python/google-api-core/latest/client_options.html
             from google.cloud import iam_v2beta
 
             async def sample_update_policy():
                 # Create a client
                 client = iam_v2beta.PoliciesAsyncClient()
 
                 # Initialize request argument(s)
@@ -712,14 +739,21 @@
         timeout: float = None,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> operation_async.AsyncOperation:
         r"""Deletes a policy. This action is permanent.
 
         .. code-block:: python
 
+            # This snippet has been automatically generated and should be regarded as a
+            # code template only.
+            # It will require modifications to work:
+            # - It may require correct/in-range values for request initialization.
+            # - It may require specifying regional endpoints when creating the service
+            #   client as shown in:
+            #   https://googleapis.dev/python/google-api-core/latest/client_options.html
             from google.cloud import iam_v2beta
 
             async def sample_delete_policy():
                 # Create a client
                 client = iam_v2beta.PoliciesAsyncClient()
 
                 # Initialize request argument(s)
@@ -827,14 +861,68 @@
             policy.Policy,
             metadata_type=policy.PolicyOperationMetadata,
         )
 
         # Done; return the response.
         return response
 
+    async def get_operation(
+        self,
+        request: operations_pb2.GetOperationRequest = None,
+        *,
+        retry: OptionalRetry = gapic_v1.method.DEFAULT,
+        timeout: float = None,
+        metadata: Sequence[Tuple[str, str]] = (),
+    ) -> operations_pb2.Operation:
+        r"""Gets the latest state of a long-running operation.
+
+        Args:
+            request (:class:`~.operations_pb2.GetOperationRequest`):
+                The request object. Request message for
+                `GetOperation` method.
+            retry (google.api_core.retry.Retry): Designation of what errors,
+                    if any, should be retried.
+            timeout (float): The timeout for this request.
+            metadata (Sequence[Tuple[str, str]]): Strings which should be
+                sent along with the request as metadata.
+        Returns:
+            ~.operations_pb2.Operation:
+                An ``Operation`` object.
+        """
+        # Create or coerce a protobuf request object.
+        # The request isn't a proto-plus wrapped type,
+        # so it must be constructed via keyword expansion.
+        if isinstance(request, dict):
+            request = operations_pb2.GetOperationRequest(**request)
+
+        # Wrap the RPC method; this adds retry and timeout information,
+        # and friendly error handling.
+        rpc = gapic_v1.method.wrap_method(
+            self._client._transport.get_operation,
+            default_timeout=None,
+            client_info=DEFAULT_CLIENT_INFO,
+        )
+
+        # Certain fields should be provided within the metadata header;
+        # add these here.
+        metadata = tuple(metadata) + (
+            gapic_v1.routing_header.to_grpc_metadata((("name", request.name),)),
+        )
+
+        # Send the request.
+        response = await rpc(
+            request,
+            retry=retry,
+            timeout=timeout,
+            metadata=metadata,
+        )
+
+        # Done; return the response.
+        return response
+
     async def __aenter__(self):
         return self
 
     async def __aexit__(self, exc_type, exc, tb):
         await self.transport.close()
```

### Comparing `google-cloud-iam-2.8.2/google/cloud/iam_v2beta/services/policies/client.py` & `google-cloud-iam-2.9.0/google/cloud/iam_v2beta/services/policies/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,14 +32,15 @@
 try:
     OptionalRetry = Union[retries.Retry, gapic_v1.method._MethodDefault]
 except AttributeError:  # pragma: NO COVER
     OptionalRetry = Union[retries.Retry, object]  # type: ignore
 
 from google.api_core import operation  # type: ignore
 from google.api_core import operation_async  # type: ignore
+from google.longrunning import operations_pb2
 from google.protobuf import timestamp_pb2  # type: ignore
 
 from google.cloud.iam_v2beta.services.policies import pagers
 from google.cloud.iam_v2beta.types import policy
 from google.cloud.iam_v2beta.types import policy as gi_policy
 
 from .transports.base import DEFAULT_CLIENT_INFO, PoliciesTransport
@@ -165,29 +166,14 @@
         Returns:
             PoliciesTransport: The transport used by the client
                 instance.
         """
         return self._transport
 
     @staticmethod
-    def policy_path(
-        policy: str,
-    ) -> str:
-        """Returns a fully-qualified policy string."""
-        return "policies/{policy}".format(
-            policy=policy,
-        )
-
-    @staticmethod
-    def parse_policy_path(path: str) -> Dict[str, str]:
-        """Parses a policy path into its component segments."""
-        m = re.match(r"^policies/(?P<policy>.+?)$", path)
-        return m.groupdict() if m else {}
-
-    @staticmethod
     def common_billing_account_path(
         billing_account: str,
     ) -> str:
         """Returns a fully-qualified billing_account string."""
         return "billingAccounts/{billing_account}".format(
             billing_account=billing_account,
         )
@@ -439,14 +425,21 @@
         attached to a resource.
 
         The response lists only policy metadata. In particular,
         policy rules are omitted.
 
         .. code-block:: python
 
+            # This snippet has been automatically generated and should be regarded as a
+            # code template only.
+            # It will require modifications to work:
+            # - It may require correct/in-range values for request initialization.
+            # - It may require specifying regional endpoints when creating the service
+            #   client as shown in:
+            #   https://googleapis.dev/python/google-api-core/latest/client_options.html
             from google.cloud import iam_v2beta
 
             def sample_list_policies():
                 # Create a client
                 client = iam_v2beta.PoliciesClient()
 
                 # Initialize request argument(s)
@@ -556,14 +549,21 @@
         timeout: float = None,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> policy.Policy:
         r"""Gets a policy.
 
         .. code-block:: python
 
+            # This snippet has been automatically generated and should be regarded as a
+            # code template only.
+            # It will require modifications to work:
+            # - It may require correct/in-range values for request initialization.
+            # - It may require specifying regional endpoints when creating the service
+            #   client as shown in:
+            #   https://googleapis.dev/python/google-api-core/latest/client_options.html
             from google.cloud import iam_v2beta
 
             def sample_get_policy():
                 # Create a client
                 client = iam_v2beta.PoliciesClient()
 
                 # Initialize request argument(s)
@@ -660,14 +660,21 @@
         timeout: float = None,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> operation.Operation:
         r"""Creates a policy.
 
         .. code-block:: python
 
+            # This snippet has been automatically generated and should be regarded as a
+            # code template only.
+            # It will require modifications to work:
+            # - It may require correct/in-range values for request initialization.
+            # - It may require specifying regional endpoints when creating the service
+            #   client as shown in:
+            #   https://googleapis.dev/python/google-api-core/latest/client_options.html
             from google.cloud import iam_v2beta
 
             def sample_create_policy():
                 # Create a client
                 client = iam_v2beta.PoliciesClient()
 
                 # Initialize request argument(s)
@@ -811,14 +818,21 @@
         2. Modify the policy as needed.
         3. Use ``UpdatePolicy`` to write the updated policy.
 
         This pattern helps prevent conflicts between concurrent updates.
 
         .. code-block:: python
 
+            # This snippet has been automatically generated and should be regarded as a
+            # code template only.
+            # It will require modifications to work:
+            # - It may require correct/in-range values for request initialization.
+            # - It may require specifying regional endpoints when creating the service
+            #   client as shown in:
+            #   https://googleapis.dev/python/google-api-core/latest/client_options.html
             from google.cloud import iam_v2beta
 
             def sample_update_policy():
                 # Create a client
                 client = iam_v2beta.PoliciesClient()
 
                 # Initialize request argument(s)
@@ -901,14 +915,21 @@
         timeout: float = None,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> operation.Operation:
         r"""Deletes a policy. This action is permanent.
 
         .. code-block:: python
 
+            # This snippet has been automatically generated and should be regarded as a
+            # code template only.
+            # It will require modifications to work:
+            # - It may require correct/in-range values for request initialization.
+            # - It may require specifying regional endpoints when creating the service
+            #   client as shown in:
+            #   https://googleapis.dev/python/google-api-core/latest/client_options.html
             from google.cloud import iam_v2beta
 
             def sample_delete_policy():
                 # Create a client
                 client = iam_v2beta.PoliciesClient()
 
                 # Initialize request argument(s)
@@ -1020,14 +1041,68 @@
         .. warning::
             ONLY use as a context manager if the transport is NOT shared
             with other clients! Exiting the with block will CLOSE the transport
             and may cause errors in other clients!
         """
         self.transport.close()
 
+    def get_operation(
+        self,
+        request: operations_pb2.GetOperationRequest = None,
+        *,
+        retry: OptionalRetry = gapic_v1.method.DEFAULT,
+        timeout: float = None,
+        metadata: Sequence[Tuple[str, str]] = (),
+    ) -> operations_pb2.Operation:
+        r"""Gets the latest state of a long-running operation.
+
+        Args:
+            request (:class:`~.operations_pb2.GetOperationRequest`):
+                The request object. Request message for
+                `GetOperation` method.
+            retry (google.api_core.retry.Retry): Designation of what errors,
+                    if any, should be retried.
+            timeout (float): The timeout for this request.
+            metadata (Sequence[Tuple[str, str]]): Strings which should be
+                sent along with the request as metadata.
+        Returns:
+            ~.operations_pb2.Operation:
+                An ``Operation`` object.
+        """
+        # Create or coerce a protobuf request object.
+        # The request isn't a proto-plus wrapped type,
+        # so it must be constructed via keyword expansion.
+        if isinstance(request, dict):
+            request = operations_pb2.GetOperationRequest(**request)
+
+        # Wrap the RPC method; this adds retry and timeout information,
+        # and friendly error handling.
+        rpc = gapic_v1.method.wrap_method(
+            self._transport.get_operation,
+            default_timeout=None,
+            client_info=DEFAULT_CLIENT_INFO,
+        )
+
+        # Certain fields should be provided within the metadata header;
+        # add these here.
+        metadata = tuple(metadata) + (
+            gapic_v1.routing_header.to_grpc_metadata((("name", request.name),)),
+        )
+
+        # Send the request.
+        response = rpc(
+            request,
+            retry=retry,
+            timeout=timeout,
+            metadata=metadata,
+        )
+
+        # Done; return the response.
+        return response
+
 
 try:
     DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
         gapic_version=pkg_resources.get_distribution(
             "google-cloud-iam",
         ).version,
     )
```

### Comparing `google-cloud-iam-2.8.2/google/cloud/iam_v2beta/services/policies/pagers.py` & `google-cloud-iam-2.9.0/google/cloud/iam_v2beta/services/policies/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-iam-2.8.2/google/cloud/iam_v2beta/services/policies/transports/__init__.py` & `google-cloud-iam-2.9.0/google/cloud/iam_v2/services/policies/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-iam-2.8.2/google/cloud/iam_v2beta/services/policies/transports/base.py` & `google-cloud-iam-2.9.0/google/cloud/iam_v2/services/policies/transports/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -22,16 +22,16 @@
 from google.api_core import retry as retries
 import google.auth  # type: ignore
 from google.auth import credentials as ga_credentials  # type: ignore
 from google.longrunning import operations_pb2  # type: ignore
 from google.oauth2 import service_account  # type: ignore
 import pkg_resources
 
-from google.cloud.iam_v2beta.types import policy
-from google.cloud.iam_v2beta.types import policy as gi_policy
+from google.cloud.iam_v2.types import policy
+from google.cloud.iam_v2.types import policy as gi_policy
 
 try:
     DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
         gapic_version=pkg_resources.get_distribution(
             "google-cloud-iam",
         ).version,
     )
@@ -256,12 +256,21 @@
     ) -> Callable[
         [policy.DeletePolicyRequest],
         Union[operations_pb2.Operation, Awaitable[operations_pb2.Operation]],
     ]:
         raise NotImplementedError()
 
     @property
+    def get_operation(
+        self,
+    ) -> Callable[
+        [operations_pb2.GetOperationRequest],
+        Union[operations_pb2.Operation, Awaitable[operations_pb2.Operation]],
+    ]:
+        raise NotImplementedError()
+
+    @property
     def kind(self) -> str:
         raise NotImplementedError()
 
 
 __all__ = ("PoliciesTransport",)
```

### Comparing `google-cloud-iam-2.8.2/google/cloud/iam_v2beta/services/policies/transports/grpc.py` & `google-cloud-iam-2.9.0/google/cloud/iam_v2beta/services/policies/transports/grpc.py`

 * *Files 2% similar despite different names*

```diff
@@ -390,12 +390,29 @@
             )
         return self._stubs["delete_policy"]
 
     def close(self):
         self.grpc_channel.close()
 
     @property
+    def get_operation(
+        self,
+    ) -> Callable[[operations_pb2.GetOperationRequest], operations_pb2.Operation]:
+        r"""Return a callable for the get_operation method over gRPC."""
+        # Generate a "stub function" on-the-fly which will actually make
+        # the request.
+        # gRPC handles serialization and deserialization, so we just need
+        # to pass in the functions for each.
+        if "get_operation" not in self._stubs:
+            self._stubs["get_operation"] = self.grpc_channel.unary_unary(
+                "/google.longrunning.Operations/GetOperation",
+                request_serializer=operations_pb2.GetOperationRequest.SerializeToString,
+                response_deserializer=operations_pb2.Operation.FromString,
+            )
+        return self._stubs["get_operation"]
+
+    @property
     def kind(self) -> str:
         return "grpc"
 
 
 __all__ = ("PoliciesGrpcTransport",)
```

### Comparing `google-cloud-iam-2.8.2/google/cloud/iam_v2beta/services/policies/transports/grpc_asyncio.py` & `google-cloud-iam-2.9.0/google/cloud/iam_v2beta/services/policies/transports/grpc_asyncio.py`

 * *Files 2% similar despite different names*

```diff
@@ -396,9 +396,26 @@
                 response_deserializer=operations_pb2.Operation.FromString,
             )
         return self._stubs["delete_policy"]
 
     def close(self):
         return self.grpc_channel.close()
 
+    @property
+    def get_operation(
+        self,
+    ) -> Callable[[operations_pb2.GetOperationRequest], operations_pb2.Operation]:
+        r"""Return a callable for the get_operation method over gRPC."""
+        # Generate a "stub function" on-the-fly which will actually make
+        # the request.
+        # gRPC handles serialization and deserialization, so we just need
+        # to pass in the functions for each.
+        if "get_operation" not in self._stubs:
+            self._stubs["get_operation"] = self.grpc_channel.unary_unary(
+                "/google.longrunning.Operations/GetOperation",
+                request_serializer=operations_pb2.GetOperationRequest.SerializeToString,
+                response_deserializer=operations_pb2.Operation.FromString,
+            )
+        return self._stubs["get_operation"]
+
 
 __all__ = ("PoliciesGrpcAsyncIOTransport",)
```

### Comparing `google-cloud-iam-2.8.2/google/cloud/iam_v2beta/types/__init__.py` & `google-cloud-iam-2.9.0/google/cloud/iam_v2/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-iam-2.8.2/google/cloud/iam_v2beta/types/deny.py` & `google-cloud-iam-2.9.0/google/cloud/iam_v2beta/types/deny.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,16 +30,17 @@
     Attributes:
         denied_principals (Sequence[str]):
             The identities that are prevented from using one or more
             permissions on Google Cloud resources. This field can
             contain the following values:
 
             -  ``principalSet://goog/public:all``: A special identifier
-               that represents any user who is on the internet, even if
-               they do not have a Google Account or are not logged in.
+               that represents any principal that is on the internet,
+               even if they do not have a Google Account or are not
+               logged in.
 
             -  ``principal://goog/subject/{email_id}``: A specific
                Google Account. Includes Gmail, Cloud Identity, and
                Google Workspace user accounts. For example,
                ``principal://goog/subject/alice@example.com``.
 
             -  ``deleted:principal://goog/subject/{email_id}?uid={uid}``:
```

### Comparing `google-cloud-iam-2.8.2/google/cloud/iam_v2beta/types/policy.py` & `google-cloud-iam-2.9.0/google/cloud/iam_v2beta/types/policy.py`

 * *Files identical despite different names*

### Comparing `google-cloud-iam-2.8.2/google_cloud_iam.egg-info/PKG-INFO` & `google-cloud-iam-2.9.0/google_cloud_iam.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-iam
-Version: 2.8.2
+Version: 2.9.0
 Summary: IAM Service Account Credentials API client library
 Home-page: https://github.com/googleapis/python-iam
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `google-cloud-iam-2.8.2/google_cloud_iam.egg-info/SOURCES.txt` & `google-cloud-iam-2.9.0/google_cloud_iam.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -15,14 +15,29 @@
 google/cloud/iam_credentials_v1/services/iam_credentials/transports/__init__.py
 google/cloud/iam_credentials_v1/services/iam_credentials/transports/base.py
 google/cloud/iam_credentials_v1/services/iam_credentials/transports/grpc.py
 google/cloud/iam_credentials_v1/services/iam_credentials/transports/grpc_asyncio.py
 google/cloud/iam_credentials_v1/types/__init__.py
 google/cloud/iam_credentials_v1/types/common.py
 google/cloud/iam_credentials_v1/types/iamcredentials.py
+google/cloud/iam_v2/__init__.py
+google/cloud/iam_v2/gapic_metadata.json
+google/cloud/iam_v2/py.typed
+google/cloud/iam_v2/services/__init__.py
+google/cloud/iam_v2/services/policies/__init__.py
+google/cloud/iam_v2/services/policies/async_client.py
+google/cloud/iam_v2/services/policies/client.py
+google/cloud/iam_v2/services/policies/pagers.py
+google/cloud/iam_v2/services/policies/transports/__init__.py
+google/cloud/iam_v2/services/policies/transports/base.py
+google/cloud/iam_v2/services/policies/transports/grpc.py
+google/cloud/iam_v2/services/policies/transports/grpc_asyncio.py
+google/cloud/iam_v2/types/__init__.py
+google/cloud/iam_v2/types/deny.py
+google/cloud/iam_v2/types/policy.py
 google/cloud/iam_v2beta/__init__.py
 google/cloud/iam_v2beta/gapic_metadata.json
 google/cloud/iam_v2beta/py.typed
 google/cloud/iam_v2beta/services/__init__.py
 google/cloud/iam_v2beta/services/policies/__init__.py
 google/cloud/iam_v2beta/services/policies/async_client.py
 google/cloud/iam_v2beta/services/policies/client.py
@@ -43,9 +58,11 @@
 google_cloud_iam.egg-info/top_level.txt
 scripts/fixup_iam_credentials_v1_keywords.py
 tests/__init__.py
 tests/unit/__init__.py
 tests/unit/gapic/__init__.py
 tests/unit/gapic/iam_credentials_v1/__init__.py
 tests/unit/gapic/iam_credentials_v1/test_iam_credentials.py
+tests/unit/gapic/iam_v2/__init__.py
+tests/unit/gapic/iam_v2/test_policies.py
 tests/unit/gapic/iam_v2beta/__init__.py
 tests/unit/gapic/iam_v2beta/test_policies.py
```

### Comparing `google-cloud-iam-2.8.2/scripts/fixup_iam_credentials_v1_keywords.py` & `google-cloud-iam-2.9.0/scripts/fixup_iam_credentials_v1_keywords.py`

 * *Files identical despite different names*

### Comparing `google-cloud-iam-2.8.2/setup.py` & `google-cloud-iam-2.9.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,24 +17,24 @@
 import io
 import os
 
 import setuptools
 
 name = "google-cloud-iam"
 description = "IAM Service Account Credentials API client library"
-version = "2.8.2"
+version = "2.9.0"
 # Should be one of:
 # 'Development Status :: 3 - Alpha'
 # 'Development Status :: 4 - Beta'
 # 'Development Status :: 5 - Production/Stable'
 release_status = "Development Status :: 5 - Production/Stable"
 dependencies = [
     "google-api-core[grpc] >= 1.32.0, <3.0.0dev,!=2.0.*,!=2.1.*,!=2.2.*,!=2.3.*,!=2.4.*,!=2.5.*,!=2.6.*,!=2.7.*",
     "proto-plus >= 1.22.0, <2.0.0dev",
-    "protobuf >= 3.19.0, <5.0.0dev",
+    "protobuf>=3.19.5,<5.0.0dev,!=3.20.0,!=3.20.1,!=4.21.0,!=4.21.1,!=4.21.2,!=4.21.3,!=4.21.4,!=4.21.5",
 ]
 
 package_root = os.path.abspath(os.path.dirname(__file__))
 
 readme_filename = os.path.join(package_root, "README.rst")
 with io.open(readme_filename, encoding="utf-8") as readme_file:
     readme = readme_file.read()
```

### Comparing `google-cloud-iam-2.8.2/tests/__init__.py` & `google-cloud-iam-2.9.0/google/cloud/iam_v2beta/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-iam-2.8.2/tests/unit/__init__.py` & `google-cloud-iam-2.9.0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-iam-2.8.2/tests/unit/gapic/__init__.py` & `google-cloud-iam-2.9.0/tests/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-iam-2.8.2/tests/unit/gapic/iam_credentials_v1/__init__.py` & `google-cloud-iam-2.9.0/tests/unit/gapic/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-iam-2.8.2/tests/unit/gapic/iam_credentials_v1/test_iam_credentials.py` & `google-cloud-iam-2.9.0/tests/unit/gapic/iam_credentials_v1/test_iam_credentials.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,16 +14,16 @@
 # limitations under the License.
 #
 import os
 
 # try/except added for compatibility with python < 3.8
 try:
     from unittest import mock
-    from unittest.mock import AsyncMock
-except ImportError:
+    from unittest.mock import AsyncMock  # pragma: NO COVER
+except ImportError:  # pragma: NO COVER
     import mock
 
 import math
 
 from google.api_core import gapic_v1, grpc_helpers, grpc_helpers_async, path_template
 from google.api_core import client_options
 from google.api_core import exceptions as core_exceptions
@@ -31,14 +31,15 @@
 from google.auth import credentials as ga_credentials
 from google.auth.exceptions import MutualTLSChannelError
 from google.oauth2 import service_account
 from google.protobuf import duration_pb2  # type: ignore
 from google.protobuf import timestamp_pb2  # type: ignore
 import grpc
 from grpc.experimental import aio
+from proto.marshal.rules import wrappers
 from proto.marshal.rules.dates import DurationRule, TimestampRule
 import pytest
 
 from google.cloud.iam_credentials_v1.services.iam_credentials import (
     IAMCredentialsAsyncClient,
     IAMCredentialsClient,
     transports,
```

### Comparing `google-cloud-iam-2.8.2/tests/unit/gapic/iam_v2beta/__init__.py` & `google-cloud-iam-2.9.0/tests/unit/gapic/iam_credentials_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-iam-2.8.2/tests/unit/gapic/iam_v2beta/test_policies.py` & `google-cloud-iam-2.9.0/tests/unit/gapic/iam_v2/test_policies.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,16 +14,16 @@
 # limitations under the License.
 #
 import os
 
 # try/except added for compatibility with python < 3.8
 try:
     from unittest import mock
-    from unittest.mock import AsyncMock
-except ImportError:
+    from unittest.mock import AsyncMock  # pragma: NO COVER
+except ImportError:  # pragma: NO COVER
     import mock
 
 import math
 
 from google.api_core import (
     future,
     gapic_v1,
@@ -41,26 +41,27 @@
 from google.auth.exceptions import MutualTLSChannelError
 from google.longrunning import operations_pb2
 from google.oauth2 import service_account
 from google.protobuf import timestamp_pb2  # type: ignore
 from google.type import expr_pb2  # type: ignore
 import grpc
 from grpc.experimental import aio
+from proto.marshal.rules import wrappers
 from proto.marshal.rules.dates import DurationRule, TimestampRule
 import pytest
 
-from google.cloud.iam_v2beta.services.policies import (
+from google.cloud.iam_v2.services.policies import (
     PoliciesAsyncClient,
     PoliciesClient,
     pagers,
     transports,
 )
-from google.cloud.iam_v2beta.types import deny
-from google.cloud.iam_v2beta.types import policy
-from google.cloud.iam_v2beta.types import policy as gi_policy
+from google.cloud.iam_v2.types import deny
+from google.cloud.iam_v2.types import policy
+from google.cloud.iam_v2.types import policy as gi_policy
 
 
 def client_cert_source_callback():
     return b"cert bytes", b"key bytes"
 
 
 # If default endpoint is localhost, then default mtls endpoint will be the same.
@@ -575,15 +576,15 @@
             always_use_jwt_access=True,
             api_audience=None,
         )
 
 
 def test_policies_client_client_options_from_dict():
     with mock.patch(
-        "google.cloud.iam_v2beta.services.policies.transports.PoliciesGrpcTransport.__init__"
+        "google.cloud.iam_v2.services.policies.transports.PoliciesGrpcTransport.__init__"
     ) as grpc_transport:
         grpc_transport.return_value = None
         client = PoliciesClient(client_options={"api_endpoint": "squid.clam.whelk"})
         grpc_transport.assert_called_once_with(
             credentials=None,
             credentials_file=None,
             host="squid.clam.whelk",
@@ -1100,14 +1101,15 @@
         # Designate an appropriate return value for the call.
         call.return_value = policy.Policy(
             name="name_value",
             uid="uid_value",
             kind="kind_value",
             display_name="display_name_value",
             etag="etag_value",
+            managing_authority="managing_authority_value",
         )
         response = client.get_policy(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
         assert args[0] == policy.GetPolicyRequest()
@@ -1115,14 +1117,15 @@
     # Establish that the response is the type that we expect.
     assert isinstance(response, policy.Policy)
     assert response.name == "name_value"
     assert response.uid == "uid_value"
     assert response.kind == "kind_value"
     assert response.display_name == "display_name_value"
     assert response.etag == "etag_value"
+    assert response.managing_authority == "managing_authority_value"
 
 
 def test_get_policy_empty_call():
     # This test is a coverage failsafe to make sure that totally empty calls,
     # i.e. request == None and no flattened fields passed, work.
     client = PoliciesClient(
         credentials=ga_credentials.AnonymousCredentials(),
@@ -1156,14 +1159,15 @@
         call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
             policy.Policy(
                 name="name_value",
                 uid="uid_value",
                 kind="kind_value",
                 display_name="display_name_value",
                 etag="etag_value",
+                managing_authority="managing_authority_value",
             )
         )
         response = await client.get_policy(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls)
         _, args, _ = call.mock_calls[0]
@@ -1172,14 +1176,15 @@
     # Establish that the response is the type that we expect.
     assert isinstance(response, policy.Policy)
     assert response.name == "name_value"
     assert response.uid == "uid_value"
     assert response.kind == "kind_value"
     assert response.display_name == "display_name_value"
     assert response.etag == "etag_value"
+    assert response.managing_authority == "managing_authority_value"
 
 
 @pytest.mark.asyncio
 async def test_get_policy_async_from_dict():
     await test_get_policy_async(request_type=dict)
 
 
@@ -2061,29 +2066,30 @@
             credentials_file="credentials.json",
         )
 
 
 def test_policies_base_transport():
     # Instantiate the base transport.
     with mock.patch(
-        "google.cloud.iam_v2beta.services.policies.transports.PoliciesTransport.__init__"
+        "google.cloud.iam_v2.services.policies.transports.PoliciesTransport.__init__"
     ) as Transport:
         Transport.return_value = None
         transport = transports.PoliciesTransport(
             credentials=ga_credentials.AnonymousCredentials(),
         )
 
     # Every method on the transport should just blindly
     # raise NotImplementedError.
     methods = (
         "list_policies",
         "get_policy",
         "create_policy",
         "update_policy",
         "delete_policy",
+        "get_operation",
     )
     for method in methods:
         with pytest.raises(NotImplementedError):
             getattr(transport, method)(request=object())
 
     with pytest.raises(NotImplementedError):
         transport.close()
@@ -2103,15 +2109,15 @@
 
 
 def test_policies_base_transport_with_credentials_file():
     # Instantiate the base transport with a credentials file
     with mock.patch.object(
         google.auth, "load_credentials_from_file", autospec=True
     ) as load_creds, mock.patch(
-        "google.cloud.iam_v2beta.services.policies.transports.PoliciesTransport._prep_wrapped_messages"
+        "google.cloud.iam_v2.services.policies.transports.PoliciesTransport._prep_wrapped_messages"
     ) as Transport:
         Transport.return_value = None
         load_creds.return_value = (ga_credentials.AnonymousCredentials(), None)
         transport = transports.PoliciesTransport(
             credentials_file="credentials.json",
             quota_project_id="octopus",
         )
@@ -2122,15 +2128,15 @@
             quota_project_id="octopus",
         )
 
 
 def test_policies_base_transport_with_adc():
     # Test the default credentials are used if credentials and credentials_file are None.
     with mock.patch.object(google.auth, "default", autospec=True) as adc, mock.patch(
-        "google.cloud.iam_v2beta.services.policies.transports.PoliciesTransport._prep_wrapped_messages"
+        "google.cloud.iam_v2.services.policies.transports.PoliciesTransport._prep_wrapped_messages"
     ) as Transport:
         Transport.return_value = None
         adc.return_value = (ga_credentials.AnonymousCredentials(), None)
         transport = transports.PoliciesTransport()
         adc.assert_called_once()
 
 
@@ -2447,129 +2453,109 @@
         operations_v1.OperationsAsyncClient,
     )
 
     # Ensure that subsequent calls to the property send the exact same object.
     assert transport.operations_client is transport.operations_client
 
 
-def test_policy_path():
-    policy = "squid"
-    expected = "policies/{policy}".format(
-        policy=policy,
-    )
-    actual = PoliciesClient.policy_path(policy)
-    assert expected == actual
-
-
-def test_parse_policy_path():
-    expected = {
-        "policy": "clam",
-    }
-    path = PoliciesClient.policy_path(**expected)
-
-    # Check that the path construction is reversible.
-    actual = PoliciesClient.parse_policy_path(path)
-    assert expected == actual
-
-
 def test_common_billing_account_path():
-    billing_account = "whelk"
+    billing_account = "squid"
     expected = "billingAccounts/{billing_account}".format(
         billing_account=billing_account,
     )
     actual = PoliciesClient.common_billing_account_path(billing_account)
     assert expected == actual
 
 
 def test_parse_common_billing_account_path():
     expected = {
-        "billing_account": "octopus",
+        "billing_account": "clam",
     }
     path = PoliciesClient.common_billing_account_path(**expected)
 
     # Check that the path construction is reversible.
     actual = PoliciesClient.parse_common_billing_account_path(path)
     assert expected == actual
 
 
 def test_common_folder_path():
-    folder = "oyster"
+    folder = "whelk"
     expected = "folders/{folder}".format(
         folder=folder,
     )
     actual = PoliciesClient.common_folder_path(folder)
     assert expected == actual
 
 
 def test_parse_common_folder_path():
     expected = {
-        "folder": "nudibranch",
+        "folder": "octopus",
     }
     path = PoliciesClient.common_folder_path(**expected)
 
     # Check that the path construction is reversible.
     actual = PoliciesClient.parse_common_folder_path(path)
     assert expected == actual
 
 
 def test_common_organization_path():
-    organization = "cuttlefish"
+    organization = "oyster"
     expected = "organizations/{organization}".format(
         organization=organization,
     )
     actual = PoliciesClient.common_organization_path(organization)
     assert expected == actual
 
 
 def test_parse_common_organization_path():
     expected = {
-        "organization": "mussel",
+        "organization": "nudibranch",
     }
     path = PoliciesClient.common_organization_path(**expected)
 
     # Check that the path construction is reversible.
     actual = PoliciesClient.parse_common_organization_path(path)
     assert expected == actual
 
 
 def test_common_project_path():
-    project = "winkle"
+    project = "cuttlefish"
     expected = "projects/{project}".format(
         project=project,
     )
     actual = PoliciesClient.common_project_path(project)
     assert expected == actual
 
 
 def test_parse_common_project_path():
     expected = {
-        "project": "nautilus",
+        "project": "mussel",
     }
     path = PoliciesClient.common_project_path(**expected)
 
     # Check that the path construction is reversible.
     actual = PoliciesClient.parse_common_project_path(path)
     assert expected == actual
 
 
 def test_common_location_path():
-    project = "scallop"
-    location = "abalone"
+    project = "winkle"
+    location = "nautilus"
     expected = "projects/{project}/locations/{location}".format(
         project=project,
         location=location,
     )
     actual = PoliciesClient.common_location_path(project, location)
     assert expected == actual
 
 
 def test_parse_common_location_path():
     expected = {
-        "project": "squid",
-        "location": "clam",
+        "project": "scallop",
+        "location": "abalone",
     }
     path = PoliciesClient.common_location_path(**expected)
 
     # Check that the path construction is reversible.
     actual = PoliciesClient.parse_common_location_path(path)
     assert expected == actual
 
@@ -2607,14 +2593,159 @@
         type(getattr(client.transport, "grpc_channel")), "close"
     ) as close:
         async with client:
             close.assert_not_called()
         close.assert_called_once()
 
 
+def test_get_operation(transport: str = "grpc"):
+    client = PoliciesClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport=transport,
+    )
+
+    # Everything is optional in proto3 as far as the runtime is concerned,
+    # and we are mocking out the actual API, so just send an empty request.
+    request = operations_pb2.GetOperationRequest()
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(type(client.transport.get_operation), "__call__") as call:
+        # Designate an appropriate return value for the call.
+        call.return_value = operations_pb2.Operation()
+        response = client.get_operation(request)
+        # Establish that the underlying gRPC stub method was called.
+        assert len(call.mock_calls) == 1
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == request
+
+    # Establish that the response is the type that we expect.
+    assert isinstance(response, operations_pb2.Operation)
+
+
+@pytest.mark.asyncio
+async def test_get_operation_async(transport: str = "grpc"):
+    client = PoliciesAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport=transport,
+    )
+
+    # Everything is optional in proto3 as far as the runtime is concerned,
+    # and we are mocking out the actual API, so just send an empty request.
+    request = operations_pb2.GetOperationRequest()
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(type(client.transport.get_operation), "__call__") as call:
+        # Designate an appropriate return value for the call.
+        call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
+            operations_pb2.Operation()
+        )
+        response = await client.get_operation(request)
+        # Establish that the underlying gRPC stub method was called.
+        assert len(call.mock_calls) == 1
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == request
+
+    # Establish that the response is the type that we expect.
+    assert isinstance(response, operations_pb2.Operation)
+
+
+def test_get_operation_field_headers():
+    client = PoliciesClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
+
+    # Any value that is part of the HTTP/1.1 URI should be sent as
+    # a field header. Set these to a non-empty value.
+    request = operations_pb2.GetOperationRequest()
+    request.name = "locations"
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(type(client.transport.get_operation), "__call__") as call:
+        call.return_value = operations_pb2.Operation()
+
+        client.get_operation(request)
+        # Establish that the underlying gRPC stub method was called.
+        assert len(call.mock_calls) == 1
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == request
+
+    # Establish that the field header was sent.
+    _, _, kw = call.mock_calls[0]
+    assert (
+        "x-goog-request-params",
+        "name=locations",
+    ) in kw["metadata"]
+
+
+@pytest.mark.asyncio
+async def test_get_operation_field_headers_async():
+    client = PoliciesAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
+
+    # Any value that is part of the HTTP/1.1 URI should be sent as
+    # a field header. Set these to a non-empty value.
+    request = operations_pb2.GetOperationRequest()
+    request.name = "locations"
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(type(client.transport.get_operation), "__call__") as call:
+        call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
+            operations_pb2.Operation()
+        )
+        await client.get_operation(request)
+        # Establish that the underlying gRPC stub method was called.
+        assert len(call.mock_calls) == 1
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == request
+
+    # Establish that the field header was sent.
+    _, _, kw = call.mock_calls[0]
+    assert (
+        "x-goog-request-params",
+        "name=locations",
+    ) in kw["metadata"]
+
+
+def test_get_operation_from_dict():
+    client = PoliciesClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(type(client.transport.get_operation), "__call__") as call:
+        # Designate an appropriate return value for the call.
+        call.return_value = operations_pb2.Operation()
+
+        response = client.get_operation(
+            request={
+                "name": "locations",
+            }
+        )
+        call.assert_called()
+
+
+@pytest.mark.asyncio
+async def test_get_operation_from_dict_async():
+    client = PoliciesAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(type(client.transport.get_operation), "__call__") as call:
+        # Designate an appropriate return value for the call.
+        call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
+            operations_pb2.Operation()
+        )
+        response = await client.get_operation(
+            request={
+                "name": "locations",
+            }
+        )
+        call.assert_called()
+
+
 def test_transport_close():
     transports = {
         "grpc": "_grpc_channel",
     }
 
     for transport, close_name in transports.items():
         client = PoliciesClient(
```

