# Comparing `tmp/google-cloud-service-directory-1.8.1.tar.gz` & `tmp/google-cloud-service-directory-1.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-cloud-service-directory-1.8.1.tar", last modified: Mon Mar 27 16:03:27 2023, max compression
+gzip compressed data, was "google-cloud-service-directory-1.8.2.tar", last modified: Wed Jul  5 15:55:45 2023, max compression
```

## Comparing `google-cloud-service-directory-1.8.1.tar` & `google-cloud-service-directory-1.8.2.tar`

### file list

```diff
@@ -1,105 +1,105 @@
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 16:03:27.241364 google-cloud-service-directory-1.8.1/
--rw-rw-r--   0 root         (0)     1003    11358 2023-03-27 16:00:53.000000 google-cloud-service-directory-1.8.1/LICENSE
--rw-rw-r--   0 root         (0)     1003      860 2023-03-27 16:00:53.000000 google-cloud-service-directory-1.8.1/MANIFEST.in
--rw-r--r--   0 root         (0)     1003     4677 2023-03-27 16:03:27.241364 google-cloud-service-directory-1.8.1/PKG-INFO
--rw-rw-r--   0 root         (0)     1003     3731 2023-03-27 16:00:53.000000 google-cloud-service-directory-1.8.1/README.rst
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 16:03:27.221361 google-cloud-service-directory-1.8.1/google/
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 16:03:27.221361 google-cloud-service-directory-1.8.1/google/cloud/
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 16:03:27.225362 google-cloud-service-directory-1.8.1/google/cloud/servicedirectory/
--rw-rw-r--   0 root         (0)     1003     2830 2023-03-27 16:00:53.000000 google-cloud-service-directory-1.8.1/google/cloud/servicedirectory/__init__.py
--rw-rw-r--   0 root         (0)     1003      652 2023-03-27 16:00:53.000000 google-cloud-service-directory-1.8.1/google/cloud/servicedirectory/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       91 2023-03-27 16:00:53.000000 google-cloud-service-directory-1.8.1/google/cloud/servicedirectory/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 16:03:27.225362 google-cloud-service-directory-1.8.1/google/cloud/servicedirectory_v1/
--rw-rw-r--   0 root         (0)     1003     2391 2023-03-27 16:00:53.000000 google-cloud-service-directory-1.8.1/google/cloud/servicedirectory_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003     8096 2023-03-27 16:00:53.000000 google-cloud-service-directory-1.8.1/google/cloud/servicedirectory_v1/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003      652 2023-03-27 16:00:53.000000 google-cloud-service-directory-1.8.1/google/cloud/servicedirectory_v1/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       91 2023-03-27 16:00:53.000000 google-cloud-service-directory-1.8.1/google/cloud/servicedirectory_v1/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 16:03:27.225362 google-cloud-service-directory-1.8.1/google/cloud/servicedirectory_v1/services/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 16:00:53.000000 google-cloud-service-directory-1.8.1/google/cloud/servicedirectory_v1/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 16:03:27.225362 google-cloud-service-directory-1.8.1/google/cloud/servicedirectory_v1/services/lookup_service/
--rw-rw-r--   0 root         (0)     1003      765 2023-03-27 16:00:53.000000 google-cloud-service-directory-1.8.1/google/cloud/servicedirectory_v1/services/lookup_service/__init__.py
--rw-rw-r--   0 root         (0)     1003    12985 2023-03-27 16:00:53.000000 google-cloud-service-directory-1.8.1/google/cloud/servicedirectory_v1/services/lookup_service/async_client.py
--rw-rw-r--   0 root         (0)     1003    22993 2023-03-27 16:00:53.000000 google-cloud-service-directory-1.8.1/google/cloud/servicedirectory_v1/services/lookup_service/client.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 16:03:27.225362 google-cloud-service-directory-1.8.1/google/cloud/servicedirectory_v1/services/lookup_service/transports/
--rw-rw-r--   0 root         (0)     1003     1386 2023-03-27 16:00:53.000000 google-cloud-service-directory-1.8.1/google/cloud/servicedirectory_v1/services/lookup_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     6097 2023-03-27 16:00:53.000000 google-cloud-service-directory-1.8.1/google/cloud/servicedirectory_v1/services/lookup_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    11949 2023-03-27 16:00:53.000000 google-cloud-service-directory-1.8.1/google/cloud/servicedirectory_v1/services/lookup_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    12162 2023-03-27 16:00:53.000000 google-cloud-service-directory-1.8.1/google/cloud/servicedirectory_v1/services/lookup_service/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    12672 2023-03-27 16:00:53.000000 google-cloud-service-directory-1.8.1/google/cloud/servicedirectory_v1/services/lookup_service/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 16:03:27.229362 google-cloud-service-directory-1.8.1/google/cloud/servicedirectory_v1/services/registration_service/
--rw-rw-r--   0 root         (0)     1003      789 2023-03-27 16:00:53.000000 google-cloud-service-directory-1.8.1/google/cloud/servicedirectory_v1/services/registration_service/__init__.py
--rw-rw-r--   0 root         (0)     1003    97008 2023-03-27 16:00:53.000000 google-cloud-service-directory-1.8.1/google/cloud/servicedirectory_v1/services/registration_service/async_client.py
--rw-rw-r--   0 root         (0)     1003   110000 2023-03-27 16:00:53.000000 google-cloud-service-directory-1.8.1/google/cloud/servicedirectory_v1/services/registration_service/client.py
--rw-rw-r--   0 root         (0)     1003    16223 2023-03-27 16:00:53.000000 google-cloud-service-directory-1.8.1/google/cloud/servicedirectory_v1/services/registration_service/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 16:03:27.229362 google-cloud-service-directory-1.8.1/google/cloud/servicedirectory_v1/services/registration_service/transports/
--rw-rw-r--   0 root         (0)     1003     1478 2023-03-27 16:00:53.000000 google-cloud-service-directory-1.8.1/google/cloud/servicedirectory_v1/services/registration_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003    14234 2023-03-27 16:00:53.000000 google-cloud-service-directory-1.8.1/google/cloud/servicedirectory_v1/services/registration_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    32351 2023-03-27 16:00:53.000000 google-cloud-service-directory-1.8.1/google/cloud/servicedirectory_v1/services/registration_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    33079 2023-03-27 16:00:53.000000 google-cloud-service-directory-1.8.1/google/cloud/servicedirectory_v1/services/registration_service/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003   109437 2023-03-27 16:00:53.000000 google-cloud-service-directory-1.8.1/google/cloud/servicedirectory_v1/services/registration_service/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 16:03:27.229362 google-cloud-service-directory-1.8.1/google/cloud/servicedirectory_v1/types/
--rw-rw-r--   0 root         (0)     1003     1911 2023-03-27 16:00:53.000000 google-cloud-service-directory-1.8.1/google/cloud/servicedirectory_v1/types/__init__.py
--rw-rw-r--   0 root         (0)     1003     3578 2023-03-27 16:00:53.000000 google-cloud-service-directory-1.8.1/google/cloud/servicedirectory_v1/types/endpoint.py
--rw-rw-r--   0 root         (0)     1003     3222 2023-03-27 16:00:53.000000 google-cloud-service-directory-1.8.1/google/cloud/servicedirectory_v1/types/lookup_service.py
--rw-rw-r--   0 root         (0)     1003     1773 2023-03-27 16:00:53.000000 google-cloud-service-directory-1.8.1/google/cloud/servicedirectory_v1/types/namespace.py
--rw-rw-r--   0 root         (0)     1003    20397 2023-03-27 16:00:53.000000 google-cloud-service-directory-1.8.1/google/cloud/servicedirectory_v1/types/registration_service.py
--rw-rw-r--   0 root         (0)     1003     3593 2023-03-27 16:00:53.000000 google-cloud-service-directory-1.8.1/google/cloud/servicedirectory_v1/types/service.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 16:03:27.233363 google-cloud-service-directory-1.8.1/google/cloud/servicedirectory_v1beta1/
--rw-rw-r--   0 root         (0)     1003     2396 2023-03-27 16:00:53.000000 google-cloud-service-directory-1.8.1/google/cloud/servicedirectory_v1beta1/__init__.py
--rw-rw-r--   0 root         (0)     1003     8106 2023-03-27 16:00:53.000000 google-cloud-service-directory-1.8.1/google/cloud/servicedirectory_v1beta1/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003      652 2023-03-27 16:00:53.000000 google-cloud-service-directory-1.8.1/google/cloud/servicedirectory_v1beta1/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       91 2023-03-27 16:00:53.000000 google-cloud-service-directory-1.8.1/google/cloud/servicedirectory_v1beta1/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 16:03:27.233363 google-cloud-service-directory-1.8.1/google/cloud/servicedirectory_v1beta1/services/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 16:00:53.000000 google-cloud-service-directory-1.8.1/google/cloud/servicedirectory_v1beta1/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 16:03:27.233363 google-cloud-service-directory-1.8.1/google/cloud/servicedirectory_v1beta1/services/lookup_service/
--rw-rw-r--   0 root         (0)     1003      765 2023-03-27 16:00:53.000000 google-cloud-service-directory-1.8.1/google/cloud/servicedirectory_v1beta1/services/lookup_service/__init__.py
--rw-rw-r--   0 root         (0)     1003    13184 2023-03-27 16:00:53.000000 google-cloud-service-directory-1.8.1/google/cloud/servicedirectory_v1beta1/services/lookup_service/async_client.py
--rw-rw-r--   0 root         (0)     1003    23671 2023-03-27 16:00:53.000000 google-cloud-service-directory-1.8.1/google/cloud/servicedirectory_v1beta1/services/lookup_service/client.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 16:03:27.233363 google-cloud-service-directory-1.8.1/google/cloud/servicedirectory_v1beta1/services/lookup_service/transports/
--rw-rw-r--   0 root         (0)     1003     1386 2023-03-27 16:00:53.000000 google-cloud-service-directory-1.8.1/google/cloud/servicedirectory_v1beta1/services/lookup_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     6107 2023-03-27 16:00:53.000000 google-cloud-service-directory-1.8.1/google/cloud/servicedirectory_v1beta1/services/lookup_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    11972 2023-03-27 16:00:53.000000 google-cloud-service-directory-1.8.1/google/cloud/servicedirectory_v1beta1/services/lookup_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    12185 2023-03-27 16:00:53.000000 google-cloud-service-directory-1.8.1/google/cloud/servicedirectory_v1beta1/services/lookup_service/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    12692 2023-03-27 16:00:53.000000 google-cloud-service-directory-1.8.1/google/cloud/servicedirectory_v1beta1/services/lookup_service/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 16:03:27.233363 google-cloud-service-directory-1.8.1/google/cloud/servicedirectory_v1beta1/services/registration_service/
--rw-rw-r--   0 root         (0)     1003      789 2023-03-27 16:00:53.000000 google-cloud-service-directory-1.8.1/google/cloud/servicedirectory_v1beta1/services/registration_service/__init__.py
--rw-rw-r--   0 root         (0)     1003    97838 2023-03-27 16:00:53.000000 google-cloud-service-directory-1.8.1/google/cloud/servicedirectory_v1beta1/services/registration_service/async_client.py
--rw-rw-r--   0 root         (0)     1003   111297 2023-03-27 16:00:53.000000 google-cloud-service-directory-1.8.1/google/cloud/servicedirectory_v1beta1/services/registration_service/client.py
--rw-rw-r--   0 root         (0)     1003    16348 2023-03-27 16:00:53.000000 google-cloud-service-directory-1.8.1/google/cloud/servicedirectory_v1beta1/services/registration_service/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 16:03:27.233363 google-cloud-service-directory-1.8.1/google/cloud/servicedirectory_v1beta1/services/registration_service/transports/
--rw-rw-r--   0 root         (0)     1003     1478 2023-03-27 16:00:53.000000 google-cloud-service-directory-1.8.1/google/cloud/servicedirectory_v1beta1/services/registration_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003    14274 2023-03-27 16:00:53.000000 google-cloud-service-directory-1.8.1/google/cloud/servicedirectory_v1beta1/services/registration_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    32502 2023-03-27 16:00:53.000000 google-cloud-service-directory-1.8.1/google/cloud/servicedirectory_v1beta1/services/registration_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    33230 2023-03-27 16:00:53.000000 google-cloud-service-directory-1.8.1/google/cloud/servicedirectory_v1beta1/services/registration_service/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003   109730 2023-03-27 16:00:53.000000 google-cloud-service-directory-1.8.1/google/cloud/servicedirectory_v1beta1/services/registration_service/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 16:03:27.237363 google-cloud-service-directory-1.8.1/google/cloud/servicedirectory_v1beta1/types/
--rw-rw-r--   0 root         (0)     1003     1911 2023-03-27 16:00:53.000000 google-cloud-service-directory-1.8.1/google/cloud/servicedirectory_v1beta1/types/__init__.py
--rw-rw-r--   0 root         (0)     1003     4827 2023-03-27 16:00:53.000000 google-cloud-service-directory-1.8.1/google/cloud/servicedirectory_v1beta1/types/endpoint.py
--rw-rw-r--   0 root         (0)     1003     4396 2023-03-27 16:00:53.000000 google-cloud-service-directory-1.8.1/google/cloud/servicedirectory_v1beta1/types/lookup_service.py
--rw-rw-r--   0 root         (0)     1003     2425 2023-03-27 16:00:53.000000 google-cloud-service-directory-1.8.1/google/cloud/servicedirectory_v1beta1/types/namespace.py
--rw-rw-r--   0 root         (0)     1003    22661 2023-03-27 16:00:53.000000 google-cloud-service-directory-1.8.1/google/cloud/servicedirectory_v1beta1/types/registration_service.py
--rw-rw-r--   0 root         (0)     1003     4552 2023-03-27 16:00:53.000000 google-cloud-service-directory-1.8.1/google/cloud/servicedirectory_v1beta1/types/service.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 16:03:27.237363 google-cloud-service-directory-1.8.1/google_cloud_service_directory.egg-info/
--rw-r--r--   0 root         (0)     1003     4677 2023-03-27 16:03:27.000000 google-cloud-service-directory-1.8.1/google_cloud_service_directory.egg-info/PKG-INFO
--rw-r--r--   0 root         (0)     1003     4919 2023-03-27 16:03:27.000000 google-cloud-service-directory-1.8.1/google_cloud_service_directory.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0)     1003        1 2023-03-27 16:03:27.000000 google-cloud-service-directory-1.8.1/google_cloud_service_directory.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0)     1003       20 2023-03-27 16:03:27.000000 google-cloud-service-directory-1.8.1/google_cloud_service_directory.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0)     1003        1 2023-03-27 16:03:27.000000 google-cloud-service-directory-1.8.1/google_cloud_service_directory.egg-info/not-zip-safe
--rw-r--r--   0 root         (0)     1003      352 2023-03-27 16:03:27.000000 google-cloud-service-directory-1.8.1/google_cloud_service_directory.egg-info/requires.txt
--rw-r--r--   0 root         (0)     1003        7 2023-03-27 16:03:27.000000 google-cloud-service-directory-1.8.1/google_cloud_service_directory.egg-info/top_level.txt
--rw-rw-r--   0 root         (0)     1003       67 2023-03-27 16:03:27.241364 google-cloud-service-directory-1.8.1/setup.cfg
--rw-rw-r--   0 root         (0)     1003     3013 2023-03-27 16:00:53.000000 google-cloud-service-directory-1.8.1/setup.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 16:03:27.237363 google-cloud-service-directory-1.8.1/tests/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 16:00:53.000000 google-cloud-service-directory-1.8.1/tests/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 16:03:27.237363 google-cloud-service-directory-1.8.1/tests/unit/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 16:00:53.000000 google-cloud-service-directory-1.8.1/tests/unit/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 16:03:27.237363 google-cloud-service-directory-1.8.1/tests/unit/gapic/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 16:00:53.000000 google-cloud-service-directory-1.8.1/tests/unit/gapic/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 16:03:27.237363 google-cloud-service-directory-1.8.1/tests/unit/gapic/servicedirectory_v1/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 16:00:53.000000 google-cloud-service-directory-1.8.1/tests/unit/gapic/servicedirectory_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003    67100 2023-03-27 16:00:53.000000 google-cloud-service-directory-1.8.1/tests/unit/gapic/servicedirectory_v1/test_lookup_service.py
--rw-rw-r--   0 root         (0)     1003   408490 2023-03-27 16:00:53.000000 google-cloud-service-directory-1.8.1/tests/unit/gapic/servicedirectory_v1/test_registration_service.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 16:03:27.241364 google-cloud-service-directory-1.8.1/tests/unit/gapic/servicedirectory_v1beta1/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 16:00:53.000000 google-cloud-service-directory-1.8.1/tests/unit/gapic/servicedirectory_v1beta1/__init__.py
--rw-rw-r--   0 root         (0)     1003    67752 2023-03-27 16:00:53.000000 google-cloud-service-directory-1.8.1/tests/unit/gapic/servicedirectory_v1beta1/test_lookup_service.py
--rw-rw-r--   0 root         (0)     1003   411724 2023-03-27 16:00:53.000000 google-cloud-service-directory-1.8.1/tests/unit/gapic/servicedirectory_v1beta1/test_registration_service.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:55:45.209954 google-cloud-service-directory-1.8.2/
+-rw-rw-r--   0 root         (0)     1003    11358 2023-07-05 15:46:59.000000 google-cloud-service-directory-1.8.2/LICENSE
+-rw-rw-r--   0 root         (0)     1003      860 2023-07-05 15:46:59.000000 google-cloud-service-directory-1.8.2/MANIFEST.in
+-rw-r--r--   0 root         (0)     1003     4636 2023-07-05 15:55:45.209954 google-cloud-service-directory-1.8.2/PKG-INFO
+-rw-rw-r--   0 root         (0)     1003     3695 2023-07-05 15:46:59.000000 google-cloud-service-directory-1.8.2/README.rst
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:55:45.193955 google-cloud-service-directory-1.8.2/google/
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:55:45.193955 google-cloud-service-directory-1.8.2/google/cloud/
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:55:45.197955 google-cloud-service-directory-1.8.2/google/cloud/servicedirectory/
+-rw-rw-r--   0 root         (0)     1003     2830 2023-07-05 15:46:59.000000 google-cloud-service-directory-1.8.2/google/cloud/servicedirectory/__init__.py
+-rw-rw-r--   0 root         (0)     1003      652 2023-07-05 15:46:59.000000 google-cloud-service-directory-1.8.2/google/cloud/servicedirectory/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       91 2023-07-05 15:46:59.000000 google-cloud-service-directory-1.8.2/google/cloud/servicedirectory/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:55:45.197955 google-cloud-service-directory-1.8.2/google/cloud/servicedirectory_v1/
+-rw-rw-r--   0 root         (0)     1003     2391 2023-07-05 15:46:59.000000 google-cloud-service-directory-1.8.2/google/cloud/servicedirectory_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003     8096 2023-07-05 15:46:59.000000 google-cloud-service-directory-1.8.2/google/cloud/servicedirectory_v1/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      652 2023-07-05 15:46:59.000000 google-cloud-service-directory-1.8.2/google/cloud/servicedirectory_v1/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       91 2023-07-05 15:46:59.000000 google-cloud-service-directory-1.8.2/google/cloud/servicedirectory_v1/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:55:45.197955 google-cloud-service-directory-1.8.2/google/cloud/servicedirectory_v1/services/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:59.000000 google-cloud-service-directory-1.8.2/google/cloud/servicedirectory_v1/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:55:45.197955 google-cloud-service-directory-1.8.2/google/cloud/servicedirectory_v1/services/lookup_service/
+-rw-rw-r--   0 root         (0)     1003      765 2023-07-05 15:46:59.000000 google-cloud-service-directory-1.8.2/google/cloud/servicedirectory_v1/services/lookup_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003    13015 2023-07-05 15:46:59.000000 google-cloud-service-directory-1.8.2/google/cloud/servicedirectory_v1/services/lookup_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003    22993 2023-07-05 15:46:59.000000 google-cloud-service-directory-1.8.2/google/cloud/servicedirectory_v1/services/lookup_service/client.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:55:45.197955 google-cloud-service-directory-1.8.2/google/cloud/servicedirectory_v1/services/lookup_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1386 2023-07-05 15:46:59.000000 google-cloud-service-directory-1.8.2/google/cloud/servicedirectory_v1/services/lookup_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     6097 2023-07-05 15:46:59.000000 google-cloud-service-directory-1.8.2/google/cloud/servicedirectory_v1/services/lookup_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    11949 2023-07-05 15:46:59.000000 google-cloud-service-directory-1.8.2/google/cloud/servicedirectory_v1/services/lookup_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    12162 2023-07-05 15:46:59.000000 google-cloud-service-directory-1.8.2/google/cloud/servicedirectory_v1/services/lookup_service/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    12672 2023-07-05 15:46:59.000000 google-cloud-service-directory-1.8.2/google/cloud/servicedirectory_v1/services/lookup_service/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:55:45.201954 google-cloud-service-directory-1.8.2/google/cloud/servicedirectory_v1/services/registration_service/
+-rw-rw-r--   0 root         (0)     1003      789 2023-07-05 15:46:59.000000 google-cloud-service-directory-1.8.2/google/cloud/servicedirectory_v1/services/registration_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003    97044 2023-07-05 15:46:59.000000 google-cloud-service-directory-1.8.2/google/cloud/servicedirectory_v1/services/registration_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003   110000 2023-07-05 15:46:59.000000 google-cloud-service-directory-1.8.2/google/cloud/servicedirectory_v1/services/registration_service/client.py
+-rw-rw-r--   0 root         (0)     1003    16223 2023-07-05 15:46:59.000000 google-cloud-service-directory-1.8.2/google/cloud/servicedirectory_v1/services/registration_service/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:55:45.201954 google-cloud-service-directory-1.8.2/google/cloud/servicedirectory_v1/services/registration_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1478 2023-07-05 15:46:59.000000 google-cloud-service-directory-1.8.2/google/cloud/servicedirectory_v1/services/registration_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003    14234 2023-07-05 15:46:59.000000 google-cloud-service-directory-1.8.2/google/cloud/servicedirectory_v1/services/registration_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    32351 2023-07-05 15:46:59.000000 google-cloud-service-directory-1.8.2/google/cloud/servicedirectory_v1/services/registration_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    33079 2023-07-05 15:46:59.000000 google-cloud-service-directory-1.8.2/google/cloud/servicedirectory_v1/services/registration_service/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003   109437 2023-07-05 15:46:59.000000 google-cloud-service-directory-1.8.2/google/cloud/servicedirectory_v1/services/registration_service/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:55:45.201954 google-cloud-service-directory-1.8.2/google/cloud/servicedirectory_v1/types/
+-rw-rw-r--   0 root         (0)     1003     1911 2023-07-05 15:46:59.000000 google-cloud-service-directory-1.8.2/google/cloud/servicedirectory_v1/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003     3578 2023-07-05 15:46:59.000000 google-cloud-service-directory-1.8.2/google/cloud/servicedirectory_v1/types/endpoint.py
+-rw-rw-r--   0 root         (0)     1003     3222 2023-07-05 15:46:59.000000 google-cloud-service-directory-1.8.2/google/cloud/servicedirectory_v1/types/lookup_service.py
+-rw-rw-r--   0 root         (0)     1003     1773 2023-07-05 15:46:59.000000 google-cloud-service-directory-1.8.2/google/cloud/servicedirectory_v1/types/namespace.py
+-rw-rw-r--   0 root         (0)     1003    20397 2023-07-05 15:46:59.000000 google-cloud-service-directory-1.8.2/google/cloud/servicedirectory_v1/types/registration_service.py
+-rw-rw-r--   0 root         (0)     1003     3593 2023-07-05 15:46:59.000000 google-cloud-service-directory-1.8.2/google/cloud/servicedirectory_v1/types/service.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:55:45.201954 google-cloud-service-directory-1.8.2/google/cloud/servicedirectory_v1beta1/
+-rw-rw-r--   0 root         (0)     1003     2396 2023-07-05 15:46:59.000000 google-cloud-service-directory-1.8.2/google/cloud/servicedirectory_v1beta1/__init__.py
+-rw-rw-r--   0 root         (0)     1003     8106 2023-07-05 15:46:59.000000 google-cloud-service-directory-1.8.2/google/cloud/servicedirectory_v1beta1/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      652 2023-07-05 15:46:59.000000 google-cloud-service-directory-1.8.2/google/cloud/servicedirectory_v1beta1/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       91 2023-07-05 15:46:59.000000 google-cloud-service-directory-1.8.2/google/cloud/servicedirectory_v1beta1/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:55:45.201954 google-cloud-service-directory-1.8.2/google/cloud/servicedirectory_v1beta1/services/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:59.000000 google-cloud-service-directory-1.8.2/google/cloud/servicedirectory_v1beta1/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:55:45.201954 google-cloud-service-directory-1.8.2/google/cloud/servicedirectory_v1beta1/services/lookup_service/
+-rw-rw-r--   0 root         (0)     1003      765 2023-07-05 15:46:59.000000 google-cloud-service-directory-1.8.2/google/cloud/servicedirectory_v1beta1/services/lookup_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003    13214 2023-07-05 15:46:59.000000 google-cloud-service-directory-1.8.2/google/cloud/servicedirectory_v1beta1/services/lookup_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003    23671 2023-07-05 15:46:59.000000 google-cloud-service-directory-1.8.2/google/cloud/servicedirectory_v1beta1/services/lookup_service/client.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:55:45.205954 google-cloud-service-directory-1.8.2/google/cloud/servicedirectory_v1beta1/services/lookup_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1386 2023-07-05 15:46:59.000000 google-cloud-service-directory-1.8.2/google/cloud/servicedirectory_v1beta1/services/lookup_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     6107 2023-07-05 15:46:59.000000 google-cloud-service-directory-1.8.2/google/cloud/servicedirectory_v1beta1/services/lookup_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    11972 2023-07-05 15:46:59.000000 google-cloud-service-directory-1.8.2/google/cloud/servicedirectory_v1beta1/services/lookup_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    12185 2023-07-05 15:46:59.000000 google-cloud-service-directory-1.8.2/google/cloud/servicedirectory_v1beta1/services/lookup_service/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    12692 2023-07-05 15:46:59.000000 google-cloud-service-directory-1.8.2/google/cloud/servicedirectory_v1beta1/services/lookup_service/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:55:45.205954 google-cloud-service-directory-1.8.2/google/cloud/servicedirectory_v1beta1/services/registration_service/
+-rw-rw-r--   0 root         (0)     1003      789 2023-07-05 15:46:59.000000 google-cloud-service-directory-1.8.2/google/cloud/servicedirectory_v1beta1/services/registration_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003    97874 2023-07-05 15:46:59.000000 google-cloud-service-directory-1.8.2/google/cloud/servicedirectory_v1beta1/services/registration_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003   111297 2023-07-05 15:46:59.000000 google-cloud-service-directory-1.8.2/google/cloud/servicedirectory_v1beta1/services/registration_service/client.py
+-rw-rw-r--   0 root         (0)     1003    16348 2023-07-05 15:46:59.000000 google-cloud-service-directory-1.8.2/google/cloud/servicedirectory_v1beta1/services/registration_service/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:55:45.205954 google-cloud-service-directory-1.8.2/google/cloud/servicedirectory_v1beta1/services/registration_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1478 2023-07-05 15:46:59.000000 google-cloud-service-directory-1.8.2/google/cloud/servicedirectory_v1beta1/services/registration_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003    14274 2023-07-05 15:46:59.000000 google-cloud-service-directory-1.8.2/google/cloud/servicedirectory_v1beta1/services/registration_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    32502 2023-07-05 15:46:59.000000 google-cloud-service-directory-1.8.2/google/cloud/servicedirectory_v1beta1/services/registration_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    33230 2023-07-05 15:46:59.000000 google-cloud-service-directory-1.8.2/google/cloud/servicedirectory_v1beta1/services/registration_service/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003   109730 2023-07-05 15:46:59.000000 google-cloud-service-directory-1.8.2/google/cloud/servicedirectory_v1beta1/services/registration_service/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:55:45.205954 google-cloud-service-directory-1.8.2/google/cloud/servicedirectory_v1beta1/types/
+-rw-rw-r--   0 root         (0)     1003     1911 2023-07-05 15:46:59.000000 google-cloud-service-directory-1.8.2/google/cloud/servicedirectory_v1beta1/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003     4827 2023-07-05 15:46:59.000000 google-cloud-service-directory-1.8.2/google/cloud/servicedirectory_v1beta1/types/endpoint.py
+-rw-rw-r--   0 root         (0)     1003     4396 2023-07-05 15:46:59.000000 google-cloud-service-directory-1.8.2/google/cloud/servicedirectory_v1beta1/types/lookup_service.py
+-rw-rw-r--   0 root         (0)     1003     2425 2023-07-05 15:46:59.000000 google-cloud-service-directory-1.8.2/google/cloud/servicedirectory_v1beta1/types/namespace.py
+-rw-rw-r--   0 root         (0)     1003    22661 2023-07-05 15:46:59.000000 google-cloud-service-directory-1.8.2/google/cloud/servicedirectory_v1beta1/types/registration_service.py
+-rw-rw-r--   0 root         (0)     1003     4552 2023-07-05 15:46:59.000000 google-cloud-service-directory-1.8.2/google/cloud/servicedirectory_v1beta1/types/service.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:55:45.209954 google-cloud-service-directory-1.8.2/google_cloud_service_directory.egg-info/
+-rw-r--r--   0 root         (0)     1003     4636 2023-07-05 15:55:45.000000 google-cloud-service-directory-1.8.2/google_cloud_service_directory.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0)     1003     4919 2023-07-05 15:55:45.000000 google-cloud-service-directory-1.8.2/google_cloud_service_directory.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-07-05 15:55:45.000000 google-cloud-service-directory-1.8.2/google_cloud_service_directory.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0)     1003       20 2023-07-05 15:55:45.000000 google-cloud-service-directory-1.8.2/google_cloud_service_directory.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-07-05 15:55:45.000000 google-cloud-service-directory-1.8.2/google_cloud_service_directory.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0)     1003      352 2023-07-05 15:55:45.000000 google-cloud-service-directory-1.8.2/google_cloud_service_directory.egg-info/requires.txt
+-rw-r--r--   0 root         (0)     1003        7 2023-07-05 15:55:45.000000 google-cloud-service-directory-1.8.2/google_cloud_service_directory.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0)     1003       67 2023-07-05 15:55:45.209954 google-cloud-service-directory-1.8.2/setup.cfg
+-rw-rw-r--   0 root         (0)     1003     3008 2023-07-05 15:46:59.000000 google-cloud-service-directory-1.8.2/setup.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:55:45.209954 google-cloud-service-directory-1.8.2/tests/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:59.000000 google-cloud-service-directory-1.8.2/tests/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:55:45.209954 google-cloud-service-directory-1.8.2/tests/unit/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:59.000000 google-cloud-service-directory-1.8.2/tests/unit/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:55:45.209954 google-cloud-service-directory-1.8.2/tests/unit/gapic/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:59.000000 google-cloud-service-directory-1.8.2/tests/unit/gapic/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:55:45.209954 google-cloud-service-directory-1.8.2/tests/unit/gapic/servicedirectory_v1/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:59.000000 google-cloud-service-directory-1.8.2/tests/unit/gapic/servicedirectory_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003    67100 2023-07-05 15:46:59.000000 google-cloud-service-directory-1.8.2/tests/unit/gapic/servicedirectory_v1/test_lookup_service.py
+-rw-rw-r--   0 root         (0)     1003   409087 2023-07-05 15:46:59.000000 google-cloud-service-directory-1.8.2/tests/unit/gapic/servicedirectory_v1/test_registration_service.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:55:45.209954 google-cloud-service-directory-1.8.2/tests/unit/gapic/servicedirectory_v1beta1/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:59.000000 google-cloud-service-directory-1.8.2/tests/unit/gapic/servicedirectory_v1beta1/__init__.py
+-rw-rw-r--   0 root         (0)     1003    67752 2023-07-05 15:46:59.000000 google-cloud-service-directory-1.8.2/tests/unit/gapic/servicedirectory_v1beta1/test_lookup_service.py
+-rw-rw-r--   0 root         (0)     1003   412321 2023-07-05 15:46:59.000000 google-cloud-service-directory-1.8.2/tests/unit/gapic/servicedirectory_v1beta1/test_registration_service.py
```

### Comparing `google-cloud-service-directory-1.8.1/LICENSE` & `google-cloud-service-directory-1.8.2/LICENSE`

 * *Files identical despite different names*

### Comparing `google-cloud-service-directory-1.8.1/MANIFEST.in` & `google-cloud-service-directory-1.8.2/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `google-cloud-service-directory-1.8.1/PKG-INFO` & `google-cloud-service-directory-1.8.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: google-cloud-service-directory
-Version: 1.8.1
+Version: 1.8.2
 Summary: Google Cloud Service Directory API client library
-Home-page: https://github.com/googleapis/python-service-directory
+Home-page: https://github.com/googleapis/google-cloud-python
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
@@ -18,47 +18,47 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Internet
 Requires-Python: >=3.7
 License-File: LICENSE
 
-Python Client for Service Directory API
-=======================================
+Python Client for Service Directory
+===================================
 
 |stable| |pypi| |versions|
 
-`Service Directory API`_: Allows the registration and lookup of services.
+`Service Directory`_: Allows the registration and lookup of services.
 
 - `Client Library Documentation`_
 - `Product Documentation`_
 
 .. |stable| image:: https://img.shields.io/badge/support-stable-gold.svg
    :target: https://github.com/googleapis/google-cloud-python/blob/main/README.rst#stability-levels
 .. |pypi| image:: https://img.shields.io/pypi/v/google-cloud-service-directory.svg
    :target: https://pypi.org/project/google-cloud-service-directory/
 .. |versions| image:: https://img.shields.io/pypi/pyversions/google-cloud-service-directory.svg
    :target: https://pypi.org/project/google-cloud-service-directory/
-.. _Service Directory API: https://cloud.google.com/service-directory/
+.. _Service Directory: https://cloud.google.com/service-directory/
 .. _Client Library Documentation: https://cloud.google.com/python/docs/reference/servicedirectory/latest
 .. _Product Documentation:  https://cloud.google.com/service-directory/
 
 Quick Start
 -----------
 
 In order to use this library, you first need to go through the following steps:
 
 1. `Select or create a Cloud Platform project.`_
 2. `Enable billing for your project.`_
-3. `Enable the Service Directory API.`_
+3. `Enable the Service Directory.`_
 4. `Setup Authentication.`_
 
 .. _Select or create a Cloud Platform project.: https://console.cloud.google.com/project
 .. _Enable billing for your project.: https://cloud.google.com/billing/docs/how-to/modify-project#enable_billing_for_a_project
-.. _Enable the Service Directory API.:  https://cloud.google.com/service-directory/
+.. _Enable the Service Directory.:  https://cloud.google.com/service-directory/
 .. _Setup Authentication.: https://googleapis.dev/python/google-api-core/latest/auth.html
 
 Installation
 ~~~~~~~~~~~~
 
 Install this library in a `virtualenv`_ using pip. `virtualenv`_ is a tool to
 create isolated Python environments. The basic problem it addresses is one of
@@ -116,16 +116,16 @@
     virtualenv <your-env>
     <your-env>\Scripts\activate
     <your-env>\Scripts\pip.exe install google-cloud-service-directory
 
 Next Steps
 ~~~~~~~~~~
 
--  Read the `Client Library Documentation`_ for Service Directory API
+-  Read the `Client Library Documentation`_ for Service Directory
    to see other available methods on the client.
--  Read the `Service Directory API Product documentation`_ to learn
+-  Read the `Service Directory Product documentation`_ to learn
    more about the product and see How-to Guides.
 -  View this `README`_ to see the full list of Cloud
    APIs that we cover.
 
-.. _Service Directory API Product documentation:  https://cloud.google.com/service-directory/
+.. _Service Directory Product documentation:  https://cloud.google.com/service-directory/
 .. _README: https://github.com/googleapis/google-cloud-python/blob/main/README.rst
```

### Comparing `google-cloud-service-directory-1.8.1/README.rst` & `google-cloud-service-directory-1.8.2/README.rst`

 * *Files 5% similar despite different names*

```diff
@@ -1,40 +1,40 @@
-Python Client for Service Directory API
-=======================================
+Python Client for Service Directory
+===================================
 
 |stable| |pypi| |versions|
 
-`Service Directory API`_: Allows the registration and lookup of services.
+`Service Directory`_: Allows the registration and lookup of services.
 
 - `Client Library Documentation`_
 - `Product Documentation`_
 
 .. |stable| image:: https://img.shields.io/badge/support-stable-gold.svg
    :target: https://github.com/googleapis/google-cloud-python/blob/main/README.rst#stability-levels
 .. |pypi| image:: https://img.shields.io/pypi/v/google-cloud-service-directory.svg
    :target: https://pypi.org/project/google-cloud-service-directory/
 .. |versions| image:: https://img.shields.io/pypi/pyversions/google-cloud-service-directory.svg
    :target: https://pypi.org/project/google-cloud-service-directory/
-.. _Service Directory API: https://cloud.google.com/service-directory/
+.. _Service Directory: https://cloud.google.com/service-directory/
 .. _Client Library Documentation: https://cloud.google.com/python/docs/reference/servicedirectory/latest
 .. _Product Documentation:  https://cloud.google.com/service-directory/
 
 Quick Start
 -----------
 
 In order to use this library, you first need to go through the following steps:
 
 1. `Select or create a Cloud Platform project.`_
 2. `Enable billing for your project.`_
-3. `Enable the Service Directory API.`_
+3. `Enable the Service Directory.`_
 4. `Setup Authentication.`_
 
 .. _Select or create a Cloud Platform project.: https://console.cloud.google.com/project
 .. _Enable billing for your project.: https://cloud.google.com/billing/docs/how-to/modify-project#enable_billing_for_a_project
-.. _Enable the Service Directory API.:  https://cloud.google.com/service-directory/
+.. _Enable the Service Directory.:  https://cloud.google.com/service-directory/
 .. _Setup Authentication.: https://googleapis.dev/python/google-api-core/latest/auth.html
 
 Installation
 ~~~~~~~~~~~~
 
 Install this library in a `virtualenv`_ using pip. `virtualenv`_ is a tool to
 create isolated Python environments. The basic problem it addresses is one of
@@ -92,16 +92,16 @@
     virtualenv <your-env>
     <your-env>\Scripts\activate
     <your-env>\Scripts\pip.exe install google-cloud-service-directory
 
 Next Steps
 ~~~~~~~~~~
 
--  Read the `Client Library Documentation`_ for Service Directory API
+-  Read the `Client Library Documentation`_ for Service Directory
    to see other available methods on the client.
--  Read the `Service Directory API Product documentation`_ to learn
+-  Read the `Service Directory Product documentation`_ to learn
    more about the product and see How-to Guides.
 -  View this `README`_ to see the full list of Cloud
    APIs that we cover.
 
-.. _Service Directory API Product documentation:  https://cloud.google.com/service-directory/
+.. _Service Directory Product documentation:  https://cloud.google.com/service-directory/
 .. _README: https://github.com/googleapis/google-cloud-python/blob/main/README.rst
```

### Comparing `google-cloud-service-directory-1.8.1/google/cloud/servicedirectory/__init__.py` & `google-cloud-service-directory-1.8.2/google/cloud/servicedirectory/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-service-directory-1.8.1/google/cloud/servicedirectory/gapic_version.py` & `google-cloud-service-directory-1.8.2/google/cloud/servicedirectory/gapic_version.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "1.8.1"  # {x-release-please-version}
+__version__ = "1.8.2"  # {x-release-please-version}
```

### Comparing `google-cloud-service-directory-1.8.1/google/cloud/servicedirectory_v1/__init__.py` & `google-cloud-service-directory-1.8.2/google/cloud/servicedirectory_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-service-directory-1.8.1/google/cloud/servicedirectory_v1/gapic_metadata.json` & `google-cloud-service-directory-1.8.2/google/cloud/servicedirectory_v1/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-cloud-service-directory-1.8.1/google/cloud/servicedirectory_v1/gapic_version.py` & `google-cloud-service-directory-1.8.2/google/cloud/servicedirectory_v1/gapic_version.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "1.8.1"  # {x-release-please-version}
+__version__ = "1.8.2"  # {x-release-please-version}
```

### Comparing `google-cloud-service-directory-1.8.1/google/cloud/servicedirectory_v1/services/__init__.py` & `google-cloud-service-directory-1.8.2/google/cloud/servicedirectory_v1/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-service-directory-1.8.1/google/cloud/servicedirectory_v1/services/lookup_service/__init__.py` & `google-cloud-service-directory-1.8.2/google/cloud/servicedirectory_v1/services/lookup_service/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-service-directory-1.8.1/google/cloud/servicedirectory_v1/services/lookup_service/async_client.py` & `google-cloud-service-directory-1.8.2/google/cloud/servicedirectory_v1/services/lookup_service/async_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -295,15 +295,15 @@
             timeout=timeout,
             metadata=metadata,
         )
 
         # Done; return the response.
         return response
 
-    async def __aenter__(self):
+    async def __aenter__(self) -> "LookupServiceAsyncClient":
         return self
 
     async def __aexit__(self, exc_type, exc, tb):
         await self.transport.close()
 
 
 DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
```

### Comparing `google-cloud-service-directory-1.8.1/google/cloud/servicedirectory_v1/services/lookup_service/client.py` & `google-cloud-service-directory-1.8.2/google/cloud/servicedirectory_v1/services/lookup_service/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-service-directory-1.8.1/google/cloud/servicedirectory_v1/services/lookup_service/transports/__init__.py` & `google-cloud-service-directory-1.8.2/google/cloud/servicedirectory_v1/services/lookup_service/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-service-directory-1.8.1/google/cloud/servicedirectory_v1/services/lookup_service/transports/base.py` & `google-cloud-service-directory-1.8.2/google/cloud/servicedirectory_v1/services/lookup_service/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-service-directory-1.8.1/google/cloud/servicedirectory_v1/services/lookup_service/transports/grpc.py` & `google-cloud-service-directory-1.8.2/google/cloud/servicedirectory_v1/services/lookup_service/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-service-directory-1.8.1/google/cloud/servicedirectory_v1/services/lookup_service/transports/grpc_asyncio.py` & `google-cloud-service-directory-1.8.2/google/cloud/servicedirectory_v1/services/lookup_service/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-service-directory-1.8.1/google/cloud/servicedirectory_v1/services/lookup_service/transports/rest.py` & `google-cloud-service-directory-1.8.2/google/cloud/servicedirectory_v1/services/lookup_service/transports/rest.py`

 * *Files identical despite different names*

### Comparing `google-cloud-service-directory-1.8.1/google/cloud/servicedirectory_v1/services/registration_service/__init__.py` & `google-cloud-service-directory-1.8.2/google/cloud/servicedirectory_v1/services/registration_service/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-service-directory-1.8.1/google/cloud/servicedirectory_v1/services/registration_service/async_client.py` & `google-cloud-service-directory-1.8.2/google/cloud/servicedirectory_v1/services/registration_service/async_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -2298,15 +2298,15 @@
             timeout=timeout,
             metadata=metadata,
         )
 
         # Done; return the response.
         return response
 
-    async def __aenter__(self):
+    async def __aenter__(self) -> "RegistrationServiceAsyncClient":
         return self
 
     async def __aexit__(self, exc_type, exc, tb):
         await self.transport.close()
 
 
 DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
```

### Comparing `google-cloud-service-directory-1.8.1/google/cloud/servicedirectory_v1/services/registration_service/client.py` & `google-cloud-service-directory-1.8.2/google/cloud/servicedirectory_v1/services/registration_service/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-service-directory-1.8.1/google/cloud/servicedirectory_v1/services/registration_service/pagers.py` & `google-cloud-service-directory-1.8.2/google/cloud/servicedirectory_v1/services/registration_service/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-service-directory-1.8.1/google/cloud/servicedirectory_v1/services/registration_service/transports/__init__.py` & `google-cloud-service-directory-1.8.2/google/cloud/servicedirectory_v1/services/registration_service/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-service-directory-1.8.1/google/cloud/servicedirectory_v1/services/registration_service/transports/base.py` & `google-cloud-service-directory-1.8.2/google/cloud/servicedirectory_v1/services/registration_service/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-service-directory-1.8.1/google/cloud/servicedirectory_v1/services/registration_service/transports/grpc.py` & `google-cloud-service-directory-1.8.2/google/cloud/servicedirectory_v1/services/registration_service/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-service-directory-1.8.1/google/cloud/servicedirectory_v1/services/registration_service/transports/grpc_asyncio.py` & `google-cloud-service-directory-1.8.2/google/cloud/servicedirectory_v1/services/registration_service/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-service-directory-1.8.1/google/cloud/servicedirectory_v1/services/registration_service/transports/rest.py` & `google-cloud-service-directory-1.8.2/google/cloud/servicedirectory_v1/services/registration_service/transports/rest.py`

 * *Files identical despite different names*

### Comparing `google-cloud-service-directory-1.8.1/google/cloud/servicedirectory_v1/types/__init__.py` & `google-cloud-service-directory-1.8.2/google/cloud/servicedirectory_v1/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-service-directory-1.8.1/google/cloud/servicedirectory_v1/types/endpoint.py` & `google-cloud-service-directory-1.8.2/google/cloud/servicedirectory_v1/types/endpoint.py`

 * *Files identical despite different names*

### Comparing `google-cloud-service-directory-1.8.1/google/cloud/servicedirectory_v1/types/lookup_service.py` & `google-cloud-service-directory-1.8.2/google/cloud/servicedirectory_v1/types/lookup_service.py`

 * *Files identical despite different names*

### Comparing `google-cloud-service-directory-1.8.1/google/cloud/servicedirectory_v1/types/namespace.py` & `google-cloud-service-directory-1.8.2/google/cloud/servicedirectory_v1/types/namespace.py`

 * *Files identical despite different names*

### Comparing `google-cloud-service-directory-1.8.1/google/cloud/servicedirectory_v1/types/registration_service.py` & `google-cloud-service-directory-1.8.2/google/cloud/servicedirectory_v1/types/registration_service.py`

 * *Files identical despite different names*

### Comparing `google-cloud-service-directory-1.8.1/google/cloud/servicedirectory_v1/types/service.py` & `google-cloud-service-directory-1.8.2/google/cloud/servicedirectory_v1/types/service.py`

 * *Files identical despite different names*

### Comparing `google-cloud-service-directory-1.8.1/google/cloud/servicedirectory_v1beta1/__init__.py` & `google-cloud-service-directory-1.8.2/google/cloud/servicedirectory_v1beta1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-service-directory-1.8.1/google/cloud/servicedirectory_v1beta1/gapic_metadata.json` & `google-cloud-service-directory-1.8.2/google/cloud/servicedirectory_v1beta1/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-cloud-service-directory-1.8.1/google/cloud/servicedirectory_v1beta1/gapic_version.py` & `google-cloud-service-directory-1.8.2/google/cloud/servicedirectory_v1beta1/gapic_version.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "1.8.1"  # {x-release-please-version}
+__version__ = "1.8.2"  # {x-release-please-version}
```

### Comparing `google-cloud-service-directory-1.8.1/google/cloud/servicedirectory_v1beta1/services/__init__.py` & `google-cloud-service-directory-1.8.2/google/cloud/servicedirectory_v1beta1/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-service-directory-1.8.1/google/cloud/servicedirectory_v1beta1/services/lookup_service/__init__.py` & `google-cloud-service-directory-1.8.2/google/cloud/servicedirectory_v1beta1/services/lookup_service/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-service-directory-1.8.1/google/cloud/servicedirectory_v1beta1/services/lookup_service/async_client.py` & `google-cloud-service-directory-1.8.2/google/cloud/servicedirectory_v1beta1/services/lookup_service/async_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -298,15 +298,15 @@
             timeout=timeout,
             metadata=metadata,
         )
 
         # Done; return the response.
         return response
 
-    async def __aenter__(self):
+    async def __aenter__(self) -> "LookupServiceAsyncClient":
         return self
 
     async def __aexit__(self, exc_type, exc, tb):
         await self.transport.close()
 
 
 DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
```

### Comparing `google-cloud-service-directory-1.8.1/google/cloud/servicedirectory_v1beta1/services/lookup_service/client.py` & `google-cloud-service-directory-1.8.2/google/cloud/servicedirectory_v1beta1/services/lookup_service/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-service-directory-1.8.1/google/cloud/servicedirectory_v1beta1/services/lookup_service/transports/__init__.py` & `google-cloud-service-directory-1.8.2/google/cloud/servicedirectory_v1beta1/services/lookup_service/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-service-directory-1.8.1/google/cloud/servicedirectory_v1beta1/services/lookup_service/transports/base.py` & `google-cloud-service-directory-1.8.2/google/cloud/servicedirectory_v1beta1/services/lookup_service/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-service-directory-1.8.1/google/cloud/servicedirectory_v1beta1/services/lookup_service/transports/grpc.py` & `google-cloud-service-directory-1.8.2/google/cloud/servicedirectory_v1beta1/services/lookup_service/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-service-directory-1.8.1/google/cloud/servicedirectory_v1beta1/services/lookup_service/transports/grpc_asyncio.py` & `google-cloud-service-directory-1.8.2/google/cloud/servicedirectory_v1beta1/services/lookup_service/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-service-directory-1.8.1/google/cloud/servicedirectory_v1beta1/services/lookup_service/transports/rest.py` & `google-cloud-service-directory-1.8.2/google/cloud/servicedirectory_v1beta1/services/lookup_service/transports/rest.py`

 * *Files identical despite different names*

### Comparing `google-cloud-service-directory-1.8.1/google/cloud/servicedirectory_v1beta1/services/registration_service/__init__.py` & `google-cloud-service-directory-1.8.2/google/cloud/servicedirectory_v1beta1/services/registration_service/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-service-directory-1.8.1/google/cloud/servicedirectory_v1beta1/services/registration_service/async_client.py` & `google-cloud-service-directory-1.8.2/google/cloud/servicedirectory_v1beta1/services/registration_service/async_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -2302,15 +2302,15 @@
             timeout=timeout,
             metadata=metadata,
         )
 
         # Done; return the response.
         return response
 
-    async def __aenter__(self):
+    async def __aenter__(self) -> "RegistrationServiceAsyncClient":
         return self
 
     async def __aexit__(self, exc_type, exc, tb):
         await self.transport.close()
 
 
 DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
```

### Comparing `google-cloud-service-directory-1.8.1/google/cloud/servicedirectory_v1beta1/services/registration_service/client.py` & `google-cloud-service-directory-1.8.2/google/cloud/servicedirectory_v1beta1/services/registration_service/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-service-directory-1.8.1/google/cloud/servicedirectory_v1beta1/services/registration_service/pagers.py` & `google-cloud-service-directory-1.8.2/google/cloud/servicedirectory_v1beta1/services/registration_service/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-service-directory-1.8.1/google/cloud/servicedirectory_v1beta1/services/registration_service/transports/__init__.py` & `google-cloud-service-directory-1.8.2/google/cloud/servicedirectory_v1beta1/services/registration_service/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-service-directory-1.8.1/google/cloud/servicedirectory_v1beta1/services/registration_service/transports/base.py` & `google-cloud-service-directory-1.8.2/google/cloud/servicedirectory_v1beta1/services/registration_service/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-service-directory-1.8.1/google/cloud/servicedirectory_v1beta1/services/registration_service/transports/grpc.py` & `google-cloud-service-directory-1.8.2/google/cloud/servicedirectory_v1beta1/services/registration_service/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-service-directory-1.8.1/google/cloud/servicedirectory_v1beta1/services/registration_service/transports/grpc_asyncio.py` & `google-cloud-service-directory-1.8.2/google/cloud/servicedirectory_v1beta1/services/registration_service/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-service-directory-1.8.1/google/cloud/servicedirectory_v1beta1/services/registration_service/transports/rest.py` & `google-cloud-service-directory-1.8.2/google/cloud/servicedirectory_v1beta1/services/registration_service/transports/rest.py`

 * *Files identical despite different names*

### Comparing `google-cloud-service-directory-1.8.1/google/cloud/servicedirectory_v1beta1/types/__init__.py` & `google-cloud-service-directory-1.8.2/google/cloud/servicedirectory_v1beta1/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-service-directory-1.8.1/google/cloud/servicedirectory_v1beta1/types/endpoint.py` & `google-cloud-service-directory-1.8.2/google/cloud/servicedirectory_v1beta1/types/endpoint.py`

 * *Files identical despite different names*

### Comparing `google-cloud-service-directory-1.8.1/google/cloud/servicedirectory_v1beta1/types/lookup_service.py` & `google-cloud-service-directory-1.8.2/google/cloud/servicedirectory_v1beta1/types/lookup_service.py`

 * *Files identical despite different names*

### Comparing `google-cloud-service-directory-1.8.1/google/cloud/servicedirectory_v1beta1/types/namespace.py` & `google-cloud-service-directory-1.8.2/google/cloud/servicedirectory_v1beta1/types/namespace.py`

 * *Files identical despite different names*

### Comparing `google-cloud-service-directory-1.8.1/google/cloud/servicedirectory_v1beta1/types/registration_service.py` & `google-cloud-service-directory-1.8.2/google/cloud/servicedirectory_v1beta1/types/registration_service.py`

 * *Files identical despite different names*

### Comparing `google-cloud-service-directory-1.8.1/google/cloud/servicedirectory_v1beta1/types/service.py` & `google-cloud-service-directory-1.8.2/google/cloud/servicedirectory_v1beta1/types/service.py`

 * *Files identical despite different names*

### Comparing `google-cloud-service-directory-1.8.1/google_cloud_service_directory.egg-info/PKG-INFO` & `google-cloud-service-directory-1.8.2/google_cloud_service_directory.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: google-cloud-service-directory
-Version: 1.8.1
+Version: 1.8.2
 Summary: Google Cloud Service Directory API client library
-Home-page: https://github.com/googleapis/python-service-directory
+Home-page: https://github.com/googleapis/google-cloud-python
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
@@ -18,47 +18,47 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Internet
 Requires-Python: >=3.7
 License-File: LICENSE
 
-Python Client for Service Directory API
-=======================================
+Python Client for Service Directory
+===================================
 
 |stable| |pypi| |versions|
 
-`Service Directory API`_: Allows the registration and lookup of services.
+`Service Directory`_: Allows the registration and lookup of services.
 
 - `Client Library Documentation`_
 - `Product Documentation`_
 
 .. |stable| image:: https://img.shields.io/badge/support-stable-gold.svg
    :target: https://github.com/googleapis/google-cloud-python/blob/main/README.rst#stability-levels
 .. |pypi| image:: https://img.shields.io/pypi/v/google-cloud-service-directory.svg
    :target: https://pypi.org/project/google-cloud-service-directory/
 .. |versions| image:: https://img.shields.io/pypi/pyversions/google-cloud-service-directory.svg
    :target: https://pypi.org/project/google-cloud-service-directory/
-.. _Service Directory API: https://cloud.google.com/service-directory/
+.. _Service Directory: https://cloud.google.com/service-directory/
 .. _Client Library Documentation: https://cloud.google.com/python/docs/reference/servicedirectory/latest
 .. _Product Documentation:  https://cloud.google.com/service-directory/
 
 Quick Start
 -----------
 
 In order to use this library, you first need to go through the following steps:
 
 1. `Select or create a Cloud Platform project.`_
 2. `Enable billing for your project.`_
-3. `Enable the Service Directory API.`_
+3. `Enable the Service Directory.`_
 4. `Setup Authentication.`_
 
 .. _Select or create a Cloud Platform project.: https://console.cloud.google.com/project
 .. _Enable billing for your project.: https://cloud.google.com/billing/docs/how-to/modify-project#enable_billing_for_a_project
-.. _Enable the Service Directory API.:  https://cloud.google.com/service-directory/
+.. _Enable the Service Directory.:  https://cloud.google.com/service-directory/
 .. _Setup Authentication.: https://googleapis.dev/python/google-api-core/latest/auth.html
 
 Installation
 ~~~~~~~~~~~~
 
 Install this library in a `virtualenv`_ using pip. `virtualenv`_ is a tool to
 create isolated Python environments. The basic problem it addresses is one of
@@ -116,16 +116,16 @@
     virtualenv <your-env>
     <your-env>\Scripts\activate
     <your-env>\Scripts\pip.exe install google-cloud-service-directory
 
 Next Steps
 ~~~~~~~~~~
 
--  Read the `Client Library Documentation`_ for Service Directory API
+-  Read the `Client Library Documentation`_ for Service Directory
    to see other available methods on the client.
--  Read the `Service Directory API Product documentation`_ to learn
+-  Read the `Service Directory Product documentation`_ to learn
    more about the product and see How-to Guides.
 -  View this `README`_ to see the full list of Cloud
    APIs that we cover.
 
-.. _Service Directory API Product documentation:  https://cloud.google.com/service-directory/
+.. _Service Directory Product documentation:  https://cloud.google.com/service-directory/
 .. _README: https://github.com/googleapis/google-cloud-python/blob/main/README.rst
```

### Comparing `google-cloud-service-directory-1.8.1/google_cloud_service_directory.egg-info/SOURCES.txt` & `google-cloud-service-directory-1.8.2/google_cloud_service_directory.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `google-cloud-service-directory-1.8.1/setup.py` & `google-cloud-service-directory-1.8.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 dependencies = [
     "google-api-core[grpc] >= 1.34.0, <3.0.0dev,!=2.0.*,!=2.1.*,!=2.2.*,!=2.3.*,!=2.4.*,!=2.5.*,!=2.6.*,!=2.7.*,!=2.8.*,!=2.9.*,!=2.10.*",
     "proto-plus >= 1.22.0, <2.0.0dev",
     "proto-plus >= 1.22.2, <2.0.0dev; python_version>='3.11'",
     "protobuf>=3.19.5,<5.0.0dev,!=3.20.0,!=3.20.1,!=4.21.0,!=4.21.1,!=4.21.2,!=4.21.3,!=4.21.4,!=4.21.5",
     "grpc-google-iam-v1 >= 0.12.4, <1.0.0dev",
 ]
-url = "https://github.com/googleapis/python-service-directory"
+url = "https://github.com/googleapis/google-cloud-python"
 
 package_root = os.path.abspath(os.path.dirname(__file__))
 
 readme_filename = os.path.join(package_root, "README.rst")
 with io.open(readme_filename, encoding="utf-8") as readme_file:
     readme = readme_file.read()
```

### Comparing `google-cloud-service-directory-1.8.1/tests/__init__.py` & `google-cloud-service-directory-1.8.2/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-service-directory-1.8.1/tests/unit/__init__.py` & `google-cloud-service-directory-1.8.2/tests/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-service-directory-1.8.1/tests/unit/gapic/__init__.py` & `google-cloud-service-directory-1.8.2/tests/unit/gapic/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-service-directory-1.8.1/tests/unit/gapic/servicedirectory_v1/__init__.py` & `google-cloud-service-directory-1.8.2/tests/unit/gapic/servicedirectory_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-service-directory-1.8.1/tests/unit/gapic/servicedirectory_v1/test_lookup_service.py` & `google-cloud-service-directory-1.8.2/tests/unit/gapic/servicedirectory_v1/test_lookup_service.py`

 * *Files identical despite different names*

### Comparing `google-cloud-service-directory-1.8.1/tests/unit/gapic/servicedirectory_v1/test_registration_service.py` & `google-cloud-service-directory-1.8.2/tests/unit/gapic/servicedirectory_v1/test_registration_service.py`

 * *Files 0% similar despite different names*

```diff
@@ -1421,17 +1421,19 @@
                     namespace.Namespace(),
                     namespace.Namespace(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.list_namespaces(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
@@ -2784,17 +2786,19 @@
                     service.Service(),
                     service.Service(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.list_services(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
@@ -4154,17 +4158,19 @@
                     endpoint.Endpoint(),
                     endpoint.Endpoint(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.list_endpoints(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
```

### Comparing `google-cloud-service-directory-1.8.1/tests/unit/gapic/servicedirectory_v1beta1/__init__.py` & `google-cloud-service-directory-1.8.2/tests/unit/gapic/servicedirectory_v1beta1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-service-directory-1.8.1/tests/unit/gapic/servicedirectory_v1beta1/test_lookup_service.py` & `google-cloud-service-directory-1.8.2/tests/unit/gapic/servicedirectory_v1beta1/test_lookup_service.py`

 * *Files identical despite different names*

### Comparing `google-cloud-service-directory-1.8.1/tests/unit/gapic/servicedirectory_v1beta1/test_registration_service.py` & `google-cloud-service-directory-1.8.2/tests/unit/gapic/servicedirectory_v1beta1/test_registration_service.py`

 * *Files 0% similar despite different names*

```diff
@@ -1422,17 +1422,19 @@
                     namespace.Namespace(),
                     namespace.Namespace(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.list_namespaces(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
@@ -2785,17 +2787,19 @@
                     service.Service(),
                     service.Service(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.list_services(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
@@ -4159,17 +4163,19 @@
                     endpoint.Endpoint(),
                     endpoint.Endpoint(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.list_endpoints(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
```

