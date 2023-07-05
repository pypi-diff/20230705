# Comparing `tmp/google-cloud-beyondcorp-clientconnectorservices-0.4.2.tar.gz` & `tmp/google-cloud-beyondcorp-clientconnectorservices-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-cloud-beyondcorp-clientconnectorservices-0.4.2.tar", last modified: Mon Mar 27 14:54:00 2023, max compression
+gzip compressed data, was "google-cloud-beyondcorp-clientconnectorservices-0.4.3.tar", last modified: Wed Jul  5 15:50:46 2023, max compression
```

## Comparing `google-cloud-beyondcorp-clientconnectorservices-0.4.2.tar` & `google-cloud-beyondcorp-clientconnectorservices-0.4.3.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:54:00.735986 google-cloud-beyondcorp-clientconnectorservices-0.4.2/
--rw-rw-r--   0 root         (0)     1003    11358 2023-03-27 14:52:02.000000 google-cloud-beyondcorp-clientconnectorservices-0.4.2/LICENSE
--rw-rw-r--   0 root         (0)     1003      860 2023-03-27 14:52:02.000000 google-cloud-beyondcorp-clientconnectorservices-0.4.2/MANIFEST.in
--rw-r--r--   0 root         (0)     1003     5198 2023-03-27 14:54:00.735986 google-cloud-beyondcorp-clientconnectorservices-0.4.2/PKG-INFO
--rw-rw-r--   0 root         (0)     1003     4214 2023-03-27 14:52:02.000000 google-cloud-beyondcorp-clientconnectorservices-0.4.2/README.rst
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:54:00.727984 google-cloud-beyondcorp-clientconnectorservices-0.4.2/google/
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:54:00.727984 google-cloud-beyondcorp-clientconnectorservices-0.4.2/google/cloud/
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:54:00.731985 google-cloud-beyondcorp-clientconnectorservices-0.4.2/google/cloud/beyondcorp_clientconnectorservices/
--rw-rw-r--   0 root         (0)     1003     1937 2023-03-27 14:52:02.000000 google-cloud-beyondcorp-clientconnectorservices-0.4.2/google/cloud/beyondcorp_clientconnectorservices/__init__.py
--rw-rw-r--   0 root         (0)     1003      652 2023-03-27 14:52:02.000000 google-cloud-beyondcorp-clientconnectorservices-0.4.2/google/cloud/beyondcorp_clientconnectorservices/gapic_version.py
--rw-rw-r--   0 root         (0)     1003      108 2023-03-27 14:52:02.000000 google-cloud-beyondcorp-clientconnectorservices-0.4.2/google/cloud/beyondcorp_clientconnectorservices/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:54:00.731985 google-cloud-beyondcorp-clientconnectorservices-0.4.2/google/cloud/beyondcorp_clientconnectorservices_v1/
--rw-rw-r--   0 root         (0)     1003     1710 2023-03-27 14:52:02.000000 google-cloud-beyondcorp-clientconnectorservices-0.4.2/google/cloud/beyondcorp_clientconnectorservices_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003     3060 2023-03-27 14:52:02.000000 google-cloud-beyondcorp-clientconnectorservices-0.4.2/google/cloud/beyondcorp_clientconnectorservices_v1/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003      652 2023-03-27 14:52:02.000000 google-cloud-beyondcorp-clientconnectorservices-0.4.2/google/cloud/beyondcorp_clientconnectorservices_v1/gapic_version.py
--rw-rw-r--   0 root         (0)     1003      108 2023-03-27 14:52:02.000000 google-cloud-beyondcorp-clientconnectorservices-0.4.2/google/cloud/beyondcorp_clientconnectorservices_v1/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:54:00.731985 google-cloud-beyondcorp-clientconnectorservices-0.4.2/google/cloud/beyondcorp_clientconnectorservices_v1/services/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 14:52:02.000000 google-cloud-beyondcorp-clientconnectorservices-0.4.2/google/cloud/beyondcorp_clientconnectorservices_v1/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:54:00.731985 google-cloud-beyondcorp-clientconnectorservices-0.4.2/google/cloud/beyondcorp_clientconnectorservices_v1/services/client_connector_services_service/
--rw-rw-r--   0 root         (0)     1003      833 2023-03-27 14:52:02.000000 google-cloud-beyondcorp-clientconnectorservices-0.4.2/google/cloud/beyondcorp_clientconnectorservices_v1/services/client_connector_services_service/__init__.py
--rw-rw-r--   0 root         (0)     1003    64380 2023-03-27 14:52:02.000000 google-cloud-beyondcorp-clientconnectorservices-0.4.2/google/cloud/beyondcorp_clientconnectorservices_v1/services/client_connector_services_service/async_client.py
--rw-rw-r--   0 root         (0)     1003    74619 2023-03-27 14:52:02.000000 google-cloud-beyondcorp-clientconnectorservices-0.4.2/google/cloud/beyondcorp_clientconnectorservices_v1/services/client_connector_services_service/client.py
--rw-rw-r--   0 root         (0)     1003     7039 2023-03-27 14:52:02.000000 google-cloud-beyondcorp-clientconnectorservices-0.4.2/google/cloud/beyondcorp_clientconnectorservices_v1/services/client_connector_services_service/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:54:00.731985 google-cloud-beyondcorp-clientconnectorservices-0.4.2/google/cloud/beyondcorp_clientconnectorservices_v1/services/client_connector_services_service/transports/
--rw-rw-r--   0 root         (0)     1003     1645 2023-03-27 14:52:02.000000 google-cloud-beyondcorp-clientconnectorservices-0.4.2/google/cloud/beyondcorp_clientconnectorservices_v1/services/client_connector_services_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003    11111 2023-03-27 14:52:02.000000 google-cloud-beyondcorp-clientconnectorservices-0.4.2/google/cloud/beyondcorp_clientconnectorservices_v1/services/client_connector_services_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    27813 2023-03-27 14:52:02.000000 google-cloud-beyondcorp-clientconnectorservices-0.4.2/google/cloud/beyondcorp_clientconnectorservices_v1/services/client_connector_services_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    28189 2023-03-27 14:52:02.000000 google-cloud-beyondcorp-clientconnectorservices-0.4.2/google/cloud/beyondcorp_clientconnectorservices_v1/services/client_connector_services_service/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    73921 2023-03-27 14:52:02.000000 google-cloud-beyondcorp-clientconnectorservices-0.4.2/google/cloud/beyondcorp_clientconnectorservices_v1/services/client_connector_services_service/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:54:00.731985 google-cloud-beyondcorp-clientconnectorservices-0.4.2/google/cloud/beyondcorp_clientconnectorservices_v1/types/
--rw-rw-r--   0 root         (0)     1003     1312 2023-03-27 14:52:02.000000 google-cloud-beyondcorp-clientconnectorservices-0.4.2/google/cloud/beyondcorp_clientconnectorservices_v1/types/__init__.py
--rw-rw-r--   0 root         (0)     1003    20030 2023-03-27 14:52:02.000000 google-cloud-beyondcorp-clientconnectorservices-0.4.2/google/cloud/beyondcorp_clientconnectorservices_v1/types/client_connector_services_service.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:54:00.735986 google-cloud-beyondcorp-clientconnectorservices-0.4.2/google_cloud_beyondcorp_clientconnectorservices.egg-info/
--rw-r--r--   0 root         (0)     1003     5198 2023-03-27 14:54:00.000000 google-cloud-beyondcorp-clientconnectorservices-0.4.2/google_cloud_beyondcorp_clientconnectorservices.egg-info/PKG-INFO
--rw-r--r--   0 root         (0)     1003     2467 2023-03-27 14:54:00.000000 google-cloud-beyondcorp-clientconnectorservices-0.4.2/google_cloud_beyondcorp_clientconnectorservices.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0)     1003        1 2023-03-27 14:54:00.000000 google-cloud-beyondcorp-clientconnectorservices-0.4.2/google_cloud_beyondcorp_clientconnectorservices.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0)     1003       20 2023-03-27 14:54:00.000000 google-cloud-beyondcorp-clientconnectorservices-0.4.2/google_cloud_beyondcorp_clientconnectorservices.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0)     1003        1 2023-03-27 14:54:00.000000 google-cloud-beyondcorp-clientconnectorservices-0.4.2/google_cloud_beyondcorp_clientconnectorservices.egg-info/not-zip-safe
--rw-r--r--   0 root         (0)     1003      352 2023-03-27 14:54:00.000000 google-cloud-beyondcorp-clientconnectorservices-0.4.2/google_cloud_beyondcorp_clientconnectorservices.egg-info/requires.txt
--rw-r--r--   0 root         (0)     1003        7 2023-03-27 14:54:00.000000 google-cloud-beyondcorp-clientconnectorservices-0.4.2/google_cloud_beyondcorp_clientconnectorservices.egg-info/top_level.txt
--rw-rw-r--   0 root         (0)     1003       67 2023-03-27 14:54:00.735986 google-cloud-beyondcorp-clientconnectorservices-0.4.2/setup.cfg
--rw-rw-r--   0 root         (0)     1003     3096 2023-03-27 14:52:02.000000 google-cloud-beyondcorp-clientconnectorservices-0.4.2/setup.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:54:00.735986 google-cloud-beyondcorp-clientconnectorservices-0.4.2/tests/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 14:52:02.000000 google-cloud-beyondcorp-clientconnectorservices-0.4.2/tests/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:54:00.735986 google-cloud-beyondcorp-clientconnectorservices-0.4.2/tests/unit/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 14:52:02.000000 google-cloud-beyondcorp-clientconnectorservices-0.4.2/tests/unit/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:54:00.735986 google-cloud-beyondcorp-clientconnectorservices-0.4.2/tests/unit/gapic/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 14:52:02.000000 google-cloud-beyondcorp-clientconnectorservices-0.4.2/tests/unit/gapic/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:54:00.735986 google-cloud-beyondcorp-clientconnectorservices-0.4.2/tests/unit/gapic/beyondcorp_clientconnectorservices_v1/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 14:52:02.000000 google-cloud-beyondcorp-clientconnectorservices-0.4.2/tests/unit/gapic/beyondcorp_clientconnectorservices_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003   250363 2023-03-27 14:52:02.000000 google-cloud-beyondcorp-clientconnectorservices-0.4.2/tests/unit/gapic/beyondcorp_clientconnectorservices_v1/test_client_connector_services_service.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:50:46.025867 google-cloud-beyondcorp-clientconnectorservices-0.4.3/
+-rw-rw-r--   0 root         (0)     1003    11358 2023-07-05 15:46:58.000000 google-cloud-beyondcorp-clientconnectorservices-0.4.3/LICENSE
+-rw-rw-r--   0 root         (0)     1003      860 2023-07-05 15:46:58.000000 google-cloud-beyondcorp-clientconnectorservices-0.4.3/MANIFEST.in
+-rw-r--r--   0 root         (0)     1003     5140 2023-07-05 15:50:46.025867 google-cloud-beyondcorp-clientconnectorservices-0.4.3/PKG-INFO
+-rw-rw-r--   0 root         (0)     1003     4178 2023-07-05 15:46:58.000000 google-cloud-beyondcorp-clientconnectorservices-0.4.3/README.rst
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:50:46.017866 google-cloud-beyondcorp-clientconnectorservices-0.4.3/google/
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:50:46.017866 google-cloud-beyondcorp-clientconnectorservices-0.4.3/google/cloud/
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:50:46.017866 google-cloud-beyondcorp-clientconnectorservices-0.4.3/google/cloud/beyondcorp_clientconnectorservices/
+-rw-rw-r--   0 root         (0)     1003     1937 2023-07-05 15:46:58.000000 google-cloud-beyondcorp-clientconnectorservices-0.4.3/google/cloud/beyondcorp_clientconnectorservices/__init__.py
+-rw-rw-r--   0 root         (0)     1003      652 2023-07-05 15:46:58.000000 google-cloud-beyondcorp-clientconnectorservices-0.4.3/google/cloud/beyondcorp_clientconnectorservices/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003      108 2023-07-05 15:46:58.000000 google-cloud-beyondcorp-clientconnectorservices-0.4.3/google/cloud/beyondcorp_clientconnectorservices/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:50:46.021867 google-cloud-beyondcorp-clientconnectorservices-0.4.3/google/cloud/beyondcorp_clientconnectorservices_v1/
+-rw-rw-r--   0 root         (0)     1003     1710 2023-07-05 15:46:58.000000 google-cloud-beyondcorp-clientconnectorservices-0.4.3/google/cloud/beyondcorp_clientconnectorservices_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003     3060 2023-07-05 15:46:58.000000 google-cloud-beyondcorp-clientconnectorservices-0.4.3/google/cloud/beyondcorp_clientconnectorservices_v1/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      652 2023-07-05 15:46:58.000000 google-cloud-beyondcorp-clientconnectorservices-0.4.3/google/cloud/beyondcorp_clientconnectorservices_v1/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003      108 2023-07-05 15:46:58.000000 google-cloud-beyondcorp-clientconnectorservices-0.4.3/google/cloud/beyondcorp_clientconnectorservices_v1/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:50:46.021867 google-cloud-beyondcorp-clientconnectorservices-0.4.3/google/cloud/beyondcorp_clientconnectorservices_v1/services/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:58.000000 google-cloud-beyondcorp-clientconnectorservices-0.4.3/google/cloud/beyondcorp_clientconnectorservices_v1/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:50:46.021867 google-cloud-beyondcorp-clientconnectorservices-0.4.3/google/cloud/beyondcorp_clientconnectorservices_v1/services/client_connector_services_service/
+-rw-rw-r--   0 root         (0)     1003      833 2023-07-05 15:46:58.000000 google-cloud-beyondcorp-clientconnectorservices-0.4.3/google/cloud/beyondcorp_clientconnectorservices_v1/services/client_connector_services_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003    64427 2023-07-05 15:46:58.000000 google-cloud-beyondcorp-clientconnectorservices-0.4.3/google/cloud/beyondcorp_clientconnectorservices_v1/services/client_connector_services_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003    74619 2023-07-05 15:46:58.000000 google-cloud-beyondcorp-clientconnectorservices-0.4.3/google/cloud/beyondcorp_clientconnectorservices_v1/services/client_connector_services_service/client.py
+-rw-rw-r--   0 root         (0)     1003     7039 2023-07-05 15:46:58.000000 google-cloud-beyondcorp-clientconnectorservices-0.4.3/google/cloud/beyondcorp_clientconnectorservices_v1/services/client_connector_services_service/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:50:46.021867 google-cloud-beyondcorp-clientconnectorservices-0.4.3/google/cloud/beyondcorp_clientconnectorservices_v1/services/client_connector_services_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1645 2023-07-05 15:46:58.000000 google-cloud-beyondcorp-clientconnectorservices-0.4.3/google/cloud/beyondcorp_clientconnectorservices_v1/services/client_connector_services_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003    11111 2023-07-05 15:46:58.000000 google-cloud-beyondcorp-clientconnectorservices-0.4.3/google/cloud/beyondcorp_clientconnectorservices_v1/services/client_connector_services_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    27813 2023-07-05 15:46:58.000000 google-cloud-beyondcorp-clientconnectorservices-0.4.3/google/cloud/beyondcorp_clientconnectorservices_v1/services/client_connector_services_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    28189 2023-07-05 15:46:58.000000 google-cloud-beyondcorp-clientconnectorservices-0.4.3/google/cloud/beyondcorp_clientconnectorservices_v1/services/client_connector_services_service/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    73885 2023-07-05 15:46:58.000000 google-cloud-beyondcorp-clientconnectorservices-0.4.3/google/cloud/beyondcorp_clientconnectorservices_v1/services/client_connector_services_service/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:50:46.021867 google-cloud-beyondcorp-clientconnectorservices-0.4.3/google/cloud/beyondcorp_clientconnectorservices_v1/types/
+-rw-rw-r--   0 root         (0)     1003     1312 2023-07-05 15:46:58.000000 google-cloud-beyondcorp-clientconnectorservices-0.4.3/google/cloud/beyondcorp_clientconnectorservices_v1/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003    20030 2023-07-05 15:46:58.000000 google-cloud-beyondcorp-clientconnectorservices-0.4.3/google/cloud/beyondcorp_clientconnectorservices_v1/types/client_connector_services_service.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:50:46.025867 google-cloud-beyondcorp-clientconnectorservices-0.4.3/google_cloud_beyondcorp_clientconnectorservices.egg-info/
+-rw-r--r--   0 root         (0)     1003     5140 2023-07-05 15:50:45.000000 google-cloud-beyondcorp-clientconnectorservices-0.4.3/google_cloud_beyondcorp_clientconnectorservices.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0)     1003     2467 2023-07-05 15:50:45.000000 google-cloud-beyondcorp-clientconnectorservices-0.4.3/google_cloud_beyondcorp_clientconnectorservices.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-07-05 15:50:45.000000 google-cloud-beyondcorp-clientconnectorservices-0.4.3/google_cloud_beyondcorp_clientconnectorservices.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0)     1003       20 2023-07-05 15:50:45.000000 google-cloud-beyondcorp-clientconnectorservices-0.4.3/google_cloud_beyondcorp_clientconnectorservices.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-07-05 15:50:45.000000 google-cloud-beyondcorp-clientconnectorservices-0.4.3/google_cloud_beyondcorp_clientconnectorservices.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0)     1003      352 2023-07-05 15:50:45.000000 google-cloud-beyondcorp-clientconnectorservices-0.4.3/google_cloud_beyondcorp_clientconnectorservices.egg-info/requires.txt
+-rw-r--r--   0 root         (0)     1003        7 2023-07-05 15:50:45.000000 google-cloud-beyondcorp-clientconnectorservices-0.4.3/google_cloud_beyondcorp_clientconnectorservices.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0)     1003       67 2023-07-05 15:50:46.025867 google-cloud-beyondcorp-clientconnectorservices-0.4.3/setup.cfg
+-rw-rw-r--   0 root         (0)     1003     3074 2023-07-05 15:46:58.000000 google-cloud-beyondcorp-clientconnectorservices-0.4.3/setup.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:50:46.025867 google-cloud-beyondcorp-clientconnectorservices-0.4.3/tests/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:58.000000 google-cloud-beyondcorp-clientconnectorservices-0.4.3/tests/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:50:46.025867 google-cloud-beyondcorp-clientconnectorservices-0.4.3/tests/unit/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:58.000000 google-cloud-beyondcorp-clientconnectorservices-0.4.3/tests/unit/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:50:46.025867 google-cloud-beyondcorp-clientconnectorservices-0.4.3/tests/unit/gapic/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:58.000000 google-cloud-beyondcorp-clientconnectorservices-0.4.3/tests/unit/gapic/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:50:46.025867 google-cloud-beyondcorp-clientconnectorservices-0.4.3/tests/unit/gapic/beyondcorp_clientconnectorservices_v1/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:58.000000 google-cloud-beyondcorp-clientconnectorservices-0.4.3/tests/unit/gapic/beyondcorp_clientconnectorservices_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003   250562 2023-07-05 15:46:58.000000 google-cloud-beyondcorp-clientconnectorservices-0.4.3/tests/unit/gapic/beyondcorp_clientconnectorservices_v1/test_client_connector_services_service.py
```

### Comparing `google-cloud-beyondcorp-clientconnectorservices-0.4.2/LICENSE` & `google-cloud-beyondcorp-clientconnectorservices-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `google-cloud-beyondcorp-clientconnectorservices-0.4.2/MANIFEST.in` & `google-cloud-beyondcorp-clientconnectorservices-0.4.3/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `google-cloud-beyondcorp-clientconnectorservices-0.4.2/PKG-INFO` & `google-cloud-beyondcorp-clientconnectorservices-0.4.3/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: google-cloud-beyondcorp-clientconnectorservices
-Version: 0.4.2
+Version: 0.4.3
 Summary: Google Cloud Beyondcorp Clientconnectorservices API client library
-Home-page: https://github.com/googleapis/python-beyondcorp-clientconnectorservices
+Home-page: https://github.com/googleapis/google-cloud-python
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
@@ -18,47 +18,47 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Internet
 Requires-Python: >=3.7
 License-File: LICENSE
 
-Python Client for BeyondCorp ClientConnectorServices API
-========================================================
+Python Client for BeyondCorp ClientConnectorServices
+====================================================
 
 |preview| |pypi| |versions|
 
-`BeyondCorp ClientConnectorServices API`_: Beyondcorp Enterprise provides identity and context aware access controls for enterprise resources and enables zero-trust access. Using the Beyondcorp Enterprise APIs, enterprises can set up multi-cloud and on-prem connectivity using the App Connector hybrid connectivity solution.
+`BeyondCorp ClientConnectorServices`_: Beyondcorp Enterprise provides identity and context aware access controls for enterprise resources and enables zero-trust access. Using the Beyondcorp Enterprise APIs, enterprises can set up multi-cloud and on-prem connectivity using the App Connector hybrid connectivity solution.
 
 - `Client Library Documentation`_
 - `Product Documentation`_
 
 .. |preview| image:: https://img.shields.io/badge/support-preview-orange.svg
    :target: https://github.com/googleapis/google-cloud-python/blob/main/README.rst#stability-levels
 .. |pypi| image:: https://img.shields.io/pypi/v/google-cloud-beyondcorp-clientconnectorservices.svg
    :target: https://pypi.org/project/google-cloud-beyondcorp-clientconnectorservices/
 .. |versions| image:: https://img.shields.io/pypi/pyversions/google-cloud-beyondcorp-clientconnectorservices.svg
    :target: https://pypi.org/project/google-cloud-beyondcorp-clientconnectorservices/
-.. _BeyondCorp ClientConnectorServices API: https://cloud.google.com/beyondcorp/
+.. _BeyondCorp ClientConnectorServices: https://cloud.google.com/beyondcorp/
 .. _Client Library Documentation: https://cloud.google.com/python/docs/reference/beyondcorpclientconnectorservices/latest
 .. _Product Documentation:  https://cloud.google.com/beyondcorp/
 
 Quick Start
 -----------
 
 In order to use this library, you first need to go through the following steps:
 
 1. `Select or create a Cloud Platform project.`_
 2. `Enable billing for your project.`_
-3. `Enable the BeyondCorp ClientConnectorServices API.`_
+3. `Enable the BeyondCorp ClientConnectorServices.`_
 4. `Setup Authentication.`_
 
 .. _Select or create a Cloud Platform project.: https://console.cloud.google.com/project
 .. _Enable billing for your project.: https://cloud.google.com/billing/docs/how-to/modify-project#enable_billing_for_a_project
-.. _Enable the BeyondCorp ClientConnectorServices API.:  https://cloud.google.com/beyondcorp/
+.. _Enable the BeyondCorp ClientConnectorServices.:  https://cloud.google.com/beyondcorp/
 .. _Setup Authentication.: https://googleapis.dev/python/google-api-core/latest/auth.html
 
 Installation
 ~~~~~~~~~~~~
 
 Install this library in a `virtualenv`_ using pip. `virtualenv`_ is a tool to
 create isolated Python environments. The basic problem it addresses is one of
@@ -116,16 +116,16 @@
     virtualenv <your-env>
     <your-env>\Scripts\activate
     <your-env>\Scripts\pip.exe install google-cloud-beyondcorp-clientconnectorservices
 
 Next Steps
 ~~~~~~~~~~
 
--  Read the `Client Library Documentation`_ for BeyondCorp ClientConnectorServices API
+-  Read the `Client Library Documentation`_ for BeyondCorp ClientConnectorServices
    to see other available methods on the client.
--  Read the `BeyondCorp ClientConnectorServices API Product documentation`_ to learn
+-  Read the `BeyondCorp ClientConnectorServices Product documentation`_ to learn
    more about the product and see How-to Guides.
 -  View this `README`_ to see the full list of Cloud
    APIs that we cover.
 
-.. _BeyondCorp ClientConnectorServices API Product documentation:  https://cloud.google.com/beyondcorp/
+.. _BeyondCorp ClientConnectorServices Product documentation:  https://cloud.google.com/beyondcorp/
 .. _README: https://github.com/googleapis/google-cloud-python/blob/main/README.rst
```

### Comparing `google-cloud-beyondcorp-clientconnectorservices-0.4.2/README.rst` & `google-cloud-beyondcorp-clientconnectorservices-0.4.3/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,40 +1,40 @@
-Python Client for BeyondCorp ClientConnectorServices API
-========================================================
+Python Client for BeyondCorp ClientConnectorServices
+====================================================
 
 |preview| |pypi| |versions|
 
-`BeyondCorp ClientConnectorServices API`_: Beyondcorp Enterprise provides identity and context aware access controls for enterprise resources and enables zero-trust access. Using the Beyondcorp Enterprise APIs, enterprises can set up multi-cloud and on-prem connectivity using the App Connector hybrid connectivity solution.
+`BeyondCorp ClientConnectorServices`_: Beyondcorp Enterprise provides identity and context aware access controls for enterprise resources and enables zero-trust access. Using the Beyondcorp Enterprise APIs, enterprises can set up multi-cloud and on-prem connectivity using the App Connector hybrid connectivity solution.
 
 - `Client Library Documentation`_
 - `Product Documentation`_
 
 .. |preview| image:: https://img.shields.io/badge/support-preview-orange.svg
    :target: https://github.com/googleapis/google-cloud-python/blob/main/README.rst#stability-levels
 .. |pypi| image:: https://img.shields.io/pypi/v/google-cloud-beyondcorp-clientconnectorservices.svg
    :target: https://pypi.org/project/google-cloud-beyondcorp-clientconnectorservices/
 .. |versions| image:: https://img.shields.io/pypi/pyversions/google-cloud-beyondcorp-clientconnectorservices.svg
    :target: https://pypi.org/project/google-cloud-beyondcorp-clientconnectorservices/
-.. _BeyondCorp ClientConnectorServices API: https://cloud.google.com/beyondcorp/
+.. _BeyondCorp ClientConnectorServices: https://cloud.google.com/beyondcorp/
 .. _Client Library Documentation: https://cloud.google.com/python/docs/reference/beyondcorpclientconnectorservices/latest
 .. _Product Documentation:  https://cloud.google.com/beyondcorp/
 
 Quick Start
 -----------
 
 In order to use this library, you first need to go through the following steps:
 
 1. `Select or create a Cloud Platform project.`_
 2. `Enable billing for your project.`_
-3. `Enable the BeyondCorp ClientConnectorServices API.`_
+3. `Enable the BeyondCorp ClientConnectorServices.`_
 4. `Setup Authentication.`_
 
 .. _Select or create a Cloud Platform project.: https://console.cloud.google.com/project
 .. _Enable billing for your project.: https://cloud.google.com/billing/docs/how-to/modify-project#enable_billing_for_a_project
-.. _Enable the BeyondCorp ClientConnectorServices API.:  https://cloud.google.com/beyondcorp/
+.. _Enable the BeyondCorp ClientConnectorServices.:  https://cloud.google.com/beyondcorp/
 .. _Setup Authentication.: https://googleapis.dev/python/google-api-core/latest/auth.html
 
 Installation
 ~~~~~~~~~~~~
 
 Install this library in a `virtualenv`_ using pip. `virtualenv`_ is a tool to
 create isolated Python environments. The basic problem it addresses is one of
@@ -92,16 +92,16 @@
     virtualenv <your-env>
     <your-env>\Scripts\activate
     <your-env>\Scripts\pip.exe install google-cloud-beyondcorp-clientconnectorservices
 
 Next Steps
 ~~~~~~~~~~
 
--  Read the `Client Library Documentation`_ for BeyondCorp ClientConnectorServices API
+-  Read the `Client Library Documentation`_ for BeyondCorp ClientConnectorServices
    to see other available methods on the client.
--  Read the `BeyondCorp ClientConnectorServices API Product documentation`_ to learn
+-  Read the `BeyondCorp ClientConnectorServices Product documentation`_ to learn
    more about the product and see How-to Guides.
 -  View this `README`_ to see the full list of Cloud
    APIs that we cover.
 
-.. _BeyondCorp ClientConnectorServices API Product documentation:  https://cloud.google.com/beyondcorp/
+.. _BeyondCorp ClientConnectorServices Product documentation:  https://cloud.google.com/beyondcorp/
 .. _README: https://github.com/googleapis/google-cloud-python/blob/main/README.rst
```

### Comparing `google-cloud-beyondcorp-clientconnectorservices-0.4.2/google/cloud/beyondcorp_clientconnectorservices/__init__.py` & `google-cloud-beyondcorp-clientconnectorservices-0.4.3/google/cloud/beyondcorp_clientconnectorservices/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-beyondcorp-clientconnectorservices-0.4.2/google/cloud/beyondcorp_clientconnectorservices/gapic_version.py` & `google-cloud-beyondcorp-clientconnectorservices-0.4.3/google/cloud/beyondcorp_clientconnectorservices/gapic_version.py`

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
-__version__ = "0.4.2"  # {x-release-please-version}
+__version__ = "0.4.3"  # {x-release-please-version}
```

### Comparing `google-cloud-beyondcorp-clientconnectorservices-0.4.2/google/cloud/beyondcorp_clientconnectorservices_v1/__init__.py` & `google-cloud-beyondcorp-clientconnectorservices-0.4.3/google/cloud/beyondcorp_clientconnectorservices_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-beyondcorp-clientconnectorservices-0.4.2/google/cloud/beyondcorp_clientconnectorservices_v1/gapic_metadata.json` & `google-cloud-beyondcorp-clientconnectorservices-0.4.3/google/cloud/beyondcorp_clientconnectorservices_v1/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-cloud-beyondcorp-clientconnectorservices-0.4.2/google/cloud/beyondcorp_clientconnectorservices_v1/gapic_version.py` & `google-cloud-beyondcorp-clientconnectorservices-0.4.3/google/cloud/beyondcorp_clientconnectorservices_v1/gapic_version.py`

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
-__version__ = "0.4.2"  # {x-release-please-version}
+__version__ = "0.4.3"  # {x-release-please-version}
```

### Comparing `google-cloud-beyondcorp-clientconnectorservices-0.4.2/google/cloud/beyondcorp_clientconnectorservices_v1/services/__init__.py` & `google-cloud-beyondcorp-clientconnectorservices-0.4.3/google/cloud/beyondcorp_clientconnectorservices_v1/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-beyondcorp-clientconnectorservices-0.4.2/google/cloud/beyondcorp_clientconnectorservices_v1/services/client_connector_services_service/__init__.py` & `google-cloud-beyondcorp-clientconnectorservices-0.4.3/google/cloud/beyondcorp_clientconnectorservices_v1/services/client_connector_services_service/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-beyondcorp-clientconnectorservices-0.4.2/google/cloud/beyondcorp_clientconnectorservices_v1/services/client_connector_services_service/async_client.py` & `google-cloud-beyondcorp-clientconnectorservices-0.4.3/google/cloud/beyondcorp_clientconnectorservices_v1/services/client_connector_services_service/async_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1551,15 +1551,15 @@
             timeout=timeout,
             metadata=metadata,
         )
 
         # Done; return the response.
         return response
 
-    async def __aenter__(self):
+    async def __aenter__(self) -> "ClientConnectorServicesServiceAsyncClient":
         return self
 
     async def __aexit__(self, exc_type, exc, tb):
         await self.transport.close()
 
 
 DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
```

### Comparing `google-cloud-beyondcorp-clientconnectorservices-0.4.2/google/cloud/beyondcorp_clientconnectorservices_v1/services/client_connector_services_service/client.py` & `google-cloud-beyondcorp-clientconnectorservices-0.4.3/google/cloud/beyondcorp_clientconnectorservices_v1/services/client_connector_services_service/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-beyondcorp-clientconnectorservices-0.4.2/google/cloud/beyondcorp_clientconnectorservices_v1/services/client_connector_services_service/pagers.py` & `google-cloud-beyondcorp-clientconnectorservices-0.4.3/google/cloud/beyondcorp_clientconnectorservices_v1/services/client_connector_services_service/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-beyondcorp-clientconnectorservices-0.4.2/google/cloud/beyondcorp_clientconnectorservices_v1/services/client_connector_services_service/transports/__init__.py` & `google-cloud-beyondcorp-clientconnectorservices-0.4.3/google/cloud/beyondcorp_clientconnectorservices_v1/services/client_connector_services_service/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-beyondcorp-clientconnectorservices-0.4.2/google/cloud/beyondcorp_clientconnectorservices_v1/services/client_connector_services_service/transports/base.py` & `google-cloud-beyondcorp-clientconnectorservices-0.4.3/google/cloud/beyondcorp_clientconnectorservices_v1/services/client_connector_services_service/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-beyondcorp-clientconnectorservices-0.4.2/google/cloud/beyondcorp_clientconnectorservices_v1/services/client_connector_services_service/transports/grpc.py` & `google-cloud-beyondcorp-clientconnectorservices-0.4.3/google/cloud/beyondcorp_clientconnectorservices_v1/services/client_connector_services_service/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-beyondcorp-clientconnectorservices-0.4.2/google/cloud/beyondcorp_clientconnectorservices_v1/services/client_connector_services_service/transports/grpc_asyncio.py` & `google-cloud-beyondcorp-clientconnectorservices-0.4.3/google/cloud/beyondcorp_clientconnectorservices_v1/services/client_connector_services_service/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-beyondcorp-clientconnectorservices-0.4.2/google/cloud/beyondcorp_clientconnectorservices_v1/services/client_connector_services_service/transports/rest.py` & `google-cloud-beyondcorp-clientconnectorservices-0.4.3/google/cloud/beyondcorp_clientconnectorservices_v1/services/client_connector_services_service/transports/rest.py`

 * *Files 0% similar despite different names*

```diff
@@ -1442,15 +1442,15 @@
                 },
             ]
 
             request, metadata = self._interceptor.pre_set_iam_policy(request, metadata)
             request_kwargs = json_format.MessageToDict(request)
             transcoded_request = path_template.transcode(http_options, **request_kwargs)
 
-            body = json.loads(json.dumps(transcoded_request["body"]))
+            body = json.dumps(transcoded_request["body"])
             uri = transcoded_request["uri"]
             method = transcoded_request["method"]
 
             # Jsonify the query params
             query_params = json.loads(json.dumps(transcoded_request["query_params"]))
 
             # Send the request
@@ -1534,15 +1534,15 @@
 
             request, metadata = self._interceptor.pre_test_iam_permissions(
                 request, metadata
             )
             request_kwargs = json_format.MessageToDict(request)
             transcoded_request = path_template.transcode(http_options, **request_kwargs)
 
-            body = json.loads(json.dumps(transcoded_request["body"]))
+            body = json.dumps(transcoded_request["body"])
             uri = transcoded_request["uri"]
             method = transcoded_request["method"]
 
             # Jsonify the query params
             query_params = json.loads(json.dumps(transcoded_request["query_params"]))
 
             # Send the request
@@ -1603,15 +1603,15 @@
 
             request, metadata = self._interceptor.pre_cancel_operation(
                 request, metadata
             )
             request_kwargs = json_format.MessageToDict(request)
             transcoded_request = path_template.transcode(http_options, **request_kwargs)
 
-            body = json.loads(json.dumps(transcoded_request["body"]))
+            body = json.dumps(transcoded_request["body"])
             uri = transcoded_request["uri"]
             method = transcoded_request["method"]
 
             # Jsonify the query params
             query_params = json.loads(json.dumps(transcoded_request["query_params"]))
 
             # Send the request
```

### Comparing `google-cloud-beyondcorp-clientconnectorservices-0.4.2/google/cloud/beyondcorp_clientconnectorservices_v1/types/__init__.py` & `google-cloud-beyondcorp-clientconnectorservices-0.4.3/google/cloud/beyondcorp_clientconnectorservices_v1/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-beyondcorp-clientconnectorservices-0.4.2/google/cloud/beyondcorp_clientconnectorservices_v1/types/client_connector_services_service.py` & `google-cloud-beyondcorp-clientconnectorservices-0.4.3/google/cloud/beyondcorp_clientconnectorservices_v1/types/client_connector_services_service.py`

 * *Files identical despite different names*

### Comparing `google-cloud-beyondcorp-clientconnectorservices-0.4.2/google_cloud_beyondcorp_clientconnectorservices.egg-info/PKG-INFO` & `google-cloud-beyondcorp-clientconnectorservices-0.4.3/google_cloud_beyondcorp_clientconnectorservices.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: google-cloud-beyondcorp-clientconnectorservices
-Version: 0.4.2
+Version: 0.4.3
 Summary: Google Cloud Beyondcorp Clientconnectorservices API client library
-Home-page: https://github.com/googleapis/python-beyondcorp-clientconnectorservices
+Home-page: https://github.com/googleapis/google-cloud-python
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
@@ -18,47 +18,47 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Internet
 Requires-Python: >=3.7
 License-File: LICENSE
 
-Python Client for BeyondCorp ClientConnectorServices API
-========================================================
+Python Client for BeyondCorp ClientConnectorServices
+====================================================
 
 |preview| |pypi| |versions|
 
-`BeyondCorp ClientConnectorServices API`_: Beyondcorp Enterprise provides identity and context aware access controls for enterprise resources and enables zero-trust access. Using the Beyondcorp Enterprise APIs, enterprises can set up multi-cloud and on-prem connectivity using the App Connector hybrid connectivity solution.
+`BeyondCorp ClientConnectorServices`_: Beyondcorp Enterprise provides identity and context aware access controls for enterprise resources and enables zero-trust access. Using the Beyondcorp Enterprise APIs, enterprises can set up multi-cloud and on-prem connectivity using the App Connector hybrid connectivity solution.
 
 - `Client Library Documentation`_
 - `Product Documentation`_
 
 .. |preview| image:: https://img.shields.io/badge/support-preview-orange.svg
    :target: https://github.com/googleapis/google-cloud-python/blob/main/README.rst#stability-levels
 .. |pypi| image:: https://img.shields.io/pypi/v/google-cloud-beyondcorp-clientconnectorservices.svg
    :target: https://pypi.org/project/google-cloud-beyondcorp-clientconnectorservices/
 .. |versions| image:: https://img.shields.io/pypi/pyversions/google-cloud-beyondcorp-clientconnectorservices.svg
    :target: https://pypi.org/project/google-cloud-beyondcorp-clientconnectorservices/
-.. _BeyondCorp ClientConnectorServices API: https://cloud.google.com/beyondcorp/
+.. _BeyondCorp ClientConnectorServices: https://cloud.google.com/beyondcorp/
 .. _Client Library Documentation: https://cloud.google.com/python/docs/reference/beyondcorpclientconnectorservices/latest
 .. _Product Documentation:  https://cloud.google.com/beyondcorp/
 
 Quick Start
 -----------
 
 In order to use this library, you first need to go through the following steps:
 
 1. `Select or create a Cloud Platform project.`_
 2. `Enable billing for your project.`_
-3. `Enable the BeyondCorp ClientConnectorServices API.`_
+3. `Enable the BeyondCorp ClientConnectorServices.`_
 4. `Setup Authentication.`_
 
 .. _Select or create a Cloud Platform project.: https://console.cloud.google.com/project
 .. _Enable billing for your project.: https://cloud.google.com/billing/docs/how-to/modify-project#enable_billing_for_a_project
-.. _Enable the BeyondCorp ClientConnectorServices API.:  https://cloud.google.com/beyondcorp/
+.. _Enable the BeyondCorp ClientConnectorServices.:  https://cloud.google.com/beyondcorp/
 .. _Setup Authentication.: https://googleapis.dev/python/google-api-core/latest/auth.html
 
 Installation
 ~~~~~~~~~~~~
 
 Install this library in a `virtualenv`_ using pip. `virtualenv`_ is a tool to
 create isolated Python environments. The basic problem it addresses is one of
@@ -116,16 +116,16 @@
     virtualenv <your-env>
     <your-env>\Scripts\activate
     <your-env>\Scripts\pip.exe install google-cloud-beyondcorp-clientconnectorservices
 
 Next Steps
 ~~~~~~~~~~
 
--  Read the `Client Library Documentation`_ for BeyondCorp ClientConnectorServices API
+-  Read the `Client Library Documentation`_ for BeyondCorp ClientConnectorServices
    to see other available methods on the client.
--  Read the `BeyondCorp ClientConnectorServices API Product documentation`_ to learn
+-  Read the `BeyondCorp ClientConnectorServices Product documentation`_ to learn
    more about the product and see How-to Guides.
 -  View this `README`_ to see the full list of Cloud
    APIs that we cover.
 
-.. _BeyondCorp ClientConnectorServices API Product documentation:  https://cloud.google.com/beyondcorp/
+.. _BeyondCorp ClientConnectorServices Product documentation:  https://cloud.google.com/beyondcorp/
 .. _README: https://github.com/googleapis/google-cloud-python/blob/main/README.rst
```

### Comparing `google-cloud-beyondcorp-clientconnectorservices-0.4.2/google_cloud_beyondcorp_clientconnectorservices.egg-info/SOURCES.txt` & `google-cloud-beyondcorp-clientconnectorservices-0.4.3/google_cloud_beyondcorp_clientconnectorservices.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `google-cloud-beyondcorp-clientconnectorservices-0.4.2/setup.py` & `google-cloud-beyondcorp-clientconnectorservices-0.4.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,15 +42,15 @@
 dependencies = [
     "google-api-core[grpc] >= 1.34.0, <3.0.0dev,!=2.0.*,!=2.1.*,!=2.2.*,!=2.3.*,!=2.4.*,!=2.5.*,!=2.6.*,!=2.7.*,!=2.8.*,!=2.9.*,!=2.10.*",
     "proto-plus >= 1.22.0, <2.0.0dev",
     "proto-plus >= 1.22.2, <2.0.0dev; python_version>='3.11'",
     "protobuf>=3.19.5,<5.0.0dev,!=3.20.0,!=3.20.1,!=4.21.0,!=4.21.1,!=4.21.2,!=4.21.3,!=4.21.4,!=4.21.5",
     "grpc-google-iam-v1 >= 0.12.4, <1.0.0dev",
 ]
-url = "https://github.com/googleapis/python-beyondcorp-clientconnectorservices"
+url = "https://github.com/googleapis/google-cloud-python"
 
 package_root = os.path.abspath(os.path.dirname(__file__))
 
 readme_filename = os.path.join(package_root, "README.rst")
 with io.open(readme_filename, encoding="utf-8") as readme_file:
     readme = readme_file.read()
```

### Comparing `google-cloud-beyondcorp-clientconnectorservices-0.4.2/tests/__init__.py` & `google-cloud-beyondcorp-clientconnectorservices-0.4.3/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-beyondcorp-clientconnectorservices-0.4.2/tests/unit/__init__.py` & `google-cloud-beyondcorp-clientconnectorservices-0.4.3/tests/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-beyondcorp-clientconnectorservices-0.4.2/tests/unit/gapic/__init__.py` & `google-cloud-beyondcorp-clientconnectorservices-0.4.3/tests/unit/gapic/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-beyondcorp-clientconnectorservices-0.4.2/tests/unit/gapic/beyondcorp_clientconnectorservices_v1/__init__.py` & `google-cloud-beyondcorp-clientconnectorservices-0.4.3/tests/unit/gapic/beyondcorp_clientconnectorservices_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-beyondcorp-clientconnectorservices-0.4.2/tests/unit/gapic/beyondcorp_clientconnectorservices_v1/test_client_connector_services_service.py` & `google-cloud-beyondcorp-clientconnectorservices-0.4.3/tests/unit/gapic/beyondcorp_clientconnectorservices_v1/test_client_connector_services_service.py`

 * *Files 0% similar despite different names*

```diff
@@ -1238,17 +1238,19 @@
                     client_connector_services_service.ClientConnectorService(),
                     client_connector_services_service.ClientConnectorService(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.list_client_connector_services(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
```

