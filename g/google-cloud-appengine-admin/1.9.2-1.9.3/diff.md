# Comparing `tmp/google-cloud-appengine-admin-1.9.2.tar.gz` & `tmp/google-cloud-appengine-admin-1.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-cloud-appengine-admin-1.9.2.tar", last modified: Mon Apr  3 13:59:00 2023, max compression
+gzip compressed data, was "google-cloud-appengine-admin-1.9.3.tar", last modified: Wed Jul  5 15:14:57 2023, max compression
```

## Comparing `google-cloud-appengine-admin-1.9.2.tar` & `google-cloud-appengine-admin-1.9.3.tar`

### file list

```diff
@@ -1,149 +1,149 @@
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-03 13:59:00.571553 google-cloud-appengine-admin-1.9.2/
--rw-rw-r--   0 root         (0)     1003    11358 2023-04-03 13:56:12.000000 google-cloud-appengine-admin-1.9.2/LICENSE
--rw-rw-r--   0 root         (0)     1003      860 2023-04-03 13:56:12.000000 google-cloud-appengine-admin-1.9.2/MANIFEST.in
--rw-r--r--   0 root         (0)     1003     4674 2023-04-03 13:59:00.571553 google-cloud-appengine-admin-1.9.2/PKG-INFO
--rw-rw-r--   0 root         (0)     1003     3734 2023-04-03 13:56:12.000000 google-cloud-appengine-admin-1.9.2/README.rst
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-03 13:59:00.543552 google-cloud-appengine-admin-1.9.2/google/
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-03 13:59:00.543552 google-cloud-appengine-admin-1.9.2/google/cloud/
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-03 13:59:00.547552 google-cloud-appengine-admin-1.9.2/google/cloud/appengine_admin/
--rw-rw-r--   0 root         (0)     1003     8893 2023-04-03 13:56:12.000000 google-cloud-appengine-admin-1.9.2/google/cloud/appengine_admin/__init__.py
--rw-rw-r--   0 root         (0)     1003      652 2023-04-03 13:56:12.000000 google-cloud-appengine-admin-1.9.2/google/cloud/appengine_admin/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       89 2023-04-03 13:56:12.000000 google-cloud-appengine-admin-1.9.2/google/cloud/appengine_admin/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-03 13:59:00.547552 google-cloud-appengine-admin-1.9.2/google/cloud/appengine_admin_v1/
--rw-rw-r--   0 root         (0)     1003     7356 2023-04-03 13:56:12.000000 google-cloud-appengine-admin-1.9.2/google/cloud/appengine_admin_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003    16689 2023-04-03 13:56:12.000000 google-cloud-appengine-admin-1.9.2/google/cloud/appengine_admin_v1/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003      652 2023-04-03 13:56:12.000000 google-cloud-appengine-admin-1.9.2/google/cloud/appengine_admin_v1/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       89 2023-04-03 13:56:12.000000 google-cloud-appengine-admin-1.9.2/google/cloud/appengine_admin_v1/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-03 13:59:00.547552 google-cloud-appengine-admin-1.9.2/google/cloud/appengine_admin_v1/services/
--rw-rw-r--   0 root         (0)     1003      600 2023-04-03 13:56:12.000000 google-cloud-appengine-admin-1.9.2/google/cloud/appengine_admin_v1/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-03 13:59:00.547552 google-cloud-appengine-admin-1.9.2/google/cloud/appengine_admin_v1/services/applications/
--rw-rw-r--   0 root         (0)     1003      761 2023-04-03 13:56:12.000000 google-cloud-appengine-admin-1.9.2/google/cloud/appengine_admin_v1/services/applications/__init__.py
--rw-rw-r--   0 root         (0)     1003    25655 2023-04-03 13:56:12.000000 google-cloud-appengine-admin-1.9.2/google/cloud/appengine_admin_v1/services/applications/async_client.py
--rw-rw-r--   0 root         (0)     1003    34672 2023-04-03 13:56:12.000000 google-cloud-appengine-admin-1.9.2/google/cloud/appengine_admin_v1/services/applications/client.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-03 13:59:00.551552 google-cloud-appengine-admin-1.9.2/google/cloud/appengine_admin_v1/services/applications/transports/
--rw-rw-r--   0 root         (0)     1003     1372 2023-04-03 13:56:12.000000 google-cloud-appengine-admin-1.9.2/google/cloud/appengine_admin_v1/services/applications/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     7736 2023-04-03 13:56:12.000000 google-cloud-appengine-admin-1.9.2/google/cloud/appengine_admin_v1/services/applications/transports/base.py
--rw-rw-r--   0 root         (0)     1003    17364 2023-04-03 13:56:12.000000 google-cloud-appengine-admin-1.9.2/google/cloud/appengine_admin_v1/services/applications/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    17734 2023-04-03 13:56:12.000000 google-cloud-appengine-admin-1.9.2/google/cloud/appengine_admin_v1/services/applications/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    27977 2023-04-03 13:56:12.000000 google-cloud-appengine-admin-1.9.2/google/cloud/appengine_admin_v1/services/applications/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-03 13:59:00.551552 google-cloud-appengine-admin-1.9.2/google/cloud/appengine_admin_v1/services/authorized_certificates/
--rw-rw-r--   0 root         (0)     1003      801 2023-04-03 13:56:12.000000 google-cloud-appengine-admin-1.9.2/google/cloud/appengine_admin_v1/services/authorized_certificates/__init__.py
--rw-rw-r--   0 root         (0)     1003    26771 2023-04-03 13:56:12.000000 google-cloud-appengine-admin-1.9.2/google/cloud/appengine_admin_v1/services/authorized_certificates/async_client.py
--rw-rw-r--   0 root         (0)     1003    36103 2023-04-03 13:56:12.000000 google-cloud-appengine-admin-1.9.2/google/cloud/appengine_admin_v1/services/authorized_certificates/client.py
--rw-rw-r--   0 root         (0)     1003     6190 2023-04-03 13:56:12.000000 google-cloud-appengine-admin-1.9.2/google/cloud/appengine_admin_v1/services/authorized_certificates/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-03 13:59:00.551552 google-cloud-appengine-admin-1.9.2/google/cloud/appengine_admin_v1/services/authorized_certificates/transports/
--rw-rw-r--   0 root         (0)     1003     1533 2023-04-03 13:56:12.000000 google-cloud-appengine-admin-1.9.2/google/cloud/appengine_admin_v1/services/authorized_certificates/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     8455 2023-04-03 13:56:12.000000 google-cloud-appengine-admin-1.9.2/google/cloud/appengine_admin_v1/services/authorized_certificates/transports/base.py
--rw-rw-r--   0 root         (0)     1003    17555 2023-04-03 13:56:12.000000 google-cloud-appengine-admin-1.9.2/google/cloud/appengine_admin_v1/services/authorized_certificates/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    17879 2023-04-03 13:56:12.000000 google-cloud-appengine-admin-1.9.2/google/cloud/appengine_admin_v1/services/authorized_certificates/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    32569 2023-04-03 13:56:12.000000 google-cloud-appengine-admin-1.9.2/google/cloud/appengine_admin_v1/services/authorized_certificates/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-03 13:59:00.551552 google-cloud-appengine-admin-1.9.2/google/cloud/appengine_admin_v1/services/authorized_domains/
--rw-rw-r--   0 root         (0)     1003      781 2023-04-03 13:56:12.000000 google-cloud-appengine-admin-1.9.2/google/cloud/appengine_admin_v1/services/authorized_domains/__init__.py
--rw-rw-r--   0 root         (0)     1003    13234 2023-04-03 13:56:12.000000 google-cloud-appengine-admin-1.9.2/google/cloud/appengine_admin_v1/services/authorized_domains/async_client.py
--rw-rw-r--   0 root         (0)     1003    21784 2023-04-03 13:56:12.000000 google-cloud-appengine-admin-1.9.2/google/cloud/appengine_admin_v1/services/authorized_domains/client.py
--rw-rw-r--   0 root         (0)     1003     6000 2023-04-03 13:56:12.000000 google-cloud-appengine-admin-1.9.2/google/cloud/appengine_admin_v1/services/authorized_domains/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-03 13:59:00.551552 google-cloud-appengine-admin-1.9.2/google/cloud/appengine_admin_v1/services/authorized_domains/transports/
--rw-rw-r--   0 root         (0)     1003     1442 2023-04-03 13:56:12.000000 google-cloud-appengine-admin-1.9.2/google/cloud/appengine_admin_v1/services/authorized_domains/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     6266 2023-04-03 13:56:12.000000 google-cloud-appengine-admin-1.9.2/google/cloud/appengine_admin_v1/services/authorized_domains/transports/base.py
--rw-rw-r--   0 root         (0)     1003    12034 2023-04-03 13:56:12.000000 google-cloud-appengine-admin-1.9.2/google/cloud/appengine_admin_v1/services/authorized_domains/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    12242 2023-04-03 13:56:12.000000 google-cloud-appengine-admin-1.9.2/google/cloud/appengine_admin_v1/services/authorized_domains/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    12095 2023-04-03 13:56:12.000000 google-cloud-appengine-admin-1.9.2/google/cloud/appengine_admin_v1/services/authorized_domains/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-03 13:59:00.555552 google-cloud-appengine-admin-1.9.2/google/cloud/appengine_admin_v1/services/domain_mappings/
--rw-rw-r--   0 root         (0)     1003      769 2023-04-03 13:56:12.000000 google-cloud-appengine-admin-1.9.2/google/cloud/appengine_admin_v1/services/domain_mappings/__init__.py
--rw-rw-r--   0 root         (0)     1003    28070 2023-04-03 13:56:12.000000 google-cloud-appengine-admin-1.9.2/google/cloud/appengine_admin_v1/services/domain_mappings/async_client.py
--rw-rw-r--   0 root         (0)     1003    37217 2023-04-03 13:56:12.000000 google-cloud-appengine-admin-1.9.2/google/cloud/appengine_admin_v1/services/domain_mappings/client.py
--rw-rw-r--   0 root         (0)     1003     5994 2023-04-03 13:56:12.000000 google-cloud-appengine-admin-1.9.2/google/cloud/appengine_admin_v1/services/domain_mappings/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-03 13:59:00.555552 google-cloud-appengine-admin-1.9.2/google/cloud/appengine_admin_v1/services/domain_mappings/transports/
--rw-rw-r--   0 root         (0)     1003     1400 2023-04-03 13:56:12.000000 google-cloud-appengine-admin-1.9.2/google/cloud/appengine_admin_v1/services/domain_mappings/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     8309 2023-04-03 13:56:12.000000 google-cloud-appengine-admin-1.9.2/google/cloud/appengine_admin_v1/services/domain_mappings/transports/base.py
--rw-rw-r--   0 root         (0)     1003    17690 2023-04-03 13:56:12.000000 google-cloud-appengine-admin-1.9.2/google/cloud/appengine_admin_v1/services/domain_mappings/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    18093 2023-04-03 13:56:12.000000 google-cloud-appengine-admin-1.9.2/google/cloud/appengine_admin_v1/services/domain_mappings/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    32856 2023-04-03 13:56:12.000000 google-cloud-appengine-admin-1.9.2/google/cloud/appengine_admin_v1/services/domain_mappings/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-03 13:59:00.555552 google-cloud-appengine-admin-1.9.2/google/cloud/appengine_admin_v1/services/firewall/
--rw-rw-r--   0 root         (0)     1003      745 2023-04-03 13:56:12.000000 google-cloud-appengine-admin-1.9.2/google/cloud/appengine_admin_v1/services/firewall/__init__.py
--rw-rw-r--   0 root         (0)     1003    28630 2023-04-03 13:56:12.000000 google-cloud-appengine-admin-1.9.2/google/cloud/appengine_admin_v1/services/firewall/async_client.py
--rw-rw-r--   0 root         (0)     1003    38139 2023-04-03 13:56:12.000000 google-cloud-appengine-admin-1.9.2/google/cloud/appengine_admin_v1/services/firewall/client.py
--rw-rw-r--   0 root         (0)     1003     5914 2023-04-03 13:56:12.000000 google-cloud-appengine-admin-1.9.2/google/cloud/appengine_admin_v1/services/firewall/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-03 13:59:00.559552 google-cloud-appengine-admin-1.9.2/google/cloud/appengine_admin_v1/services/firewall/transports/
--rw-rw-r--   0 root         (0)     1003     1316 2023-04-03 13:56:12.000000 google-cloud-appengine-admin-1.9.2/google/cloud/appengine_admin_v1/services/firewall/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     8556 2023-04-03 13:56:12.000000 google-cloud-appengine-admin-1.9.2/google/cloud/appengine_admin_v1/services/firewall/transports/base.py
--rw-rw-r--   0 root         (0)     1003    18412 2023-04-03 13:56:12.000000 google-cloud-appengine-admin-1.9.2/google/cloud/appengine_admin_v1/services/firewall/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    18758 2023-04-03 13:56:12.000000 google-cloud-appengine-admin-1.9.2/google/cloud/appengine_admin_v1/services/firewall/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    35843 2023-04-03 13:56:12.000000 google-cloud-appengine-admin-1.9.2/google/cloud/appengine_admin_v1/services/firewall/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-03 13:59:00.559552 google-cloud-appengine-admin-1.9.2/google/cloud/appengine_admin_v1/services/instances/
--rw-rw-r--   0 root         (0)     1003      749 2023-04-03 13:56:12.000000 google-cloud-appengine-admin-1.9.2/google/cloud/appengine_admin_v1/services/instances/__init__.py
--rw-rw-r--   0 root         (0)     1003    24971 2023-04-03 13:56:12.000000 google-cloud-appengine-admin-1.9.2/google/cloud/appengine_admin_v1/services/instances/async_client.py
--rw-rw-r--   0 root         (0)     1003    34633 2023-04-03 13:56:12.000000 google-cloud-appengine-admin-1.9.2/google/cloud/appengine_admin_v1/services/instances/client.py
--rw-rw-r--   0 root         (0)     1003     5808 2023-04-03 13:56:12.000000 google-cloud-appengine-admin-1.9.2/google/cloud/appengine_admin_v1/services/instances/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-03 13:59:00.559552 google-cloud-appengine-admin-1.9.2/google/cloud/appengine_admin_v1/services/instances/transports/
--rw-rw-r--   0 root         (0)     1003     1330 2023-04-03 13:56:12.000000 google-cloud-appengine-admin-1.9.2/google/cloud/appengine_admin_v1/services/instances/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     7692 2023-04-03 13:56:12.000000 google-cloud-appengine-admin-1.9.2/google/cloud/appengine_admin_v1/services/instances/transports/base.py
--rw-rw-r--   0 root         (0)     1003    17044 2023-04-03 13:56:12.000000 google-cloud-appengine-admin-1.9.2/google/cloud/appengine_admin_v1/services/instances/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    17397 2023-04-03 13:56:12.000000 google-cloud-appengine-admin-1.9.2/google/cloud/appengine_admin_v1/services/instances/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    26981 2023-04-03 13:56:12.000000 google-cloud-appengine-admin-1.9.2/google/cloud/appengine_admin_v1/services/instances/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-03 13:59:00.559552 google-cloud-appengine-admin-1.9.2/google/cloud/appengine_admin_v1/services/services/
--rw-rw-r--   0 root         (0)     1003      745 2023-04-03 13:56:12.000000 google-cloud-appengine-admin-1.9.2/google/cloud/appengine_admin_v1/services/services/__init__.py
--rw-rw-r--   0 root         (0)     1003    24350 2023-04-03 13:56:12.000000 google-cloud-appengine-admin-1.9.2/google/cloud/appengine_admin_v1/services/services/async_client.py
--rw-rw-r--   0 root         (0)     1003    33405 2023-04-03 13:56:12.000000 google-cloud-appengine-admin-1.9.2/google/cloud/appengine_admin_v1/services/services/client.py
--rw-rw-r--   0 root         (0)     1003     5773 2023-04-03 13:56:12.000000 google-cloud-appengine-admin-1.9.2/google/cloud/appengine_admin_v1/services/services/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-03 13:59:00.563552 google-cloud-appengine-admin-1.9.2/google/cloud/appengine_admin_v1/services/services/transports/
--rw-rw-r--   0 root         (0)     1003     1316 2023-04-03 13:56:12.000000 google-cloud-appengine-admin-1.9.2/google/cloud/appengine_admin_v1/services/services/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     7670 2023-04-03 13:56:12.000000 google-cloud-appengine-admin-1.9.2/google/cloud/appengine_admin_v1/services/services/transports/base.py
--rw-rw-r--   0 root         (0)     1003    15635 2023-04-03 13:56:12.000000 google-cloud-appengine-admin-1.9.2/google/cloud/appengine_admin_v1/services/services/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    16002 2023-04-03 13:56:12.000000 google-cloud-appengine-admin-1.9.2/google/cloud/appengine_admin_v1/services/services/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    27245 2023-04-03 13:56:12.000000 google-cloud-appengine-admin-1.9.2/google/cloud/appengine_admin_v1/services/services/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-03 13:59:00.563552 google-cloud-appengine-admin-1.9.2/google/cloud/appengine_admin_v1/services/versions/
--rw-rw-r--   0 root         (0)     1003      745 2023-04-03 13:56:12.000000 google-cloud-appengine-admin-1.9.2/google/cloud/appengine_admin_v1/services/versions/__init__.py
--rw-rw-r--   0 root         (0)     1003    30354 2023-04-03 13:56:12.000000 google-cloud-appengine-admin-1.9.2/google/cloud/appengine_admin_v1/services/versions/async_client.py
--rw-rw-r--   0 root         (0)     1003    39535 2023-04-03 13:56:12.000000 google-cloud-appengine-admin-1.9.2/google/cloud/appengine_admin_v1/services/versions/client.py
--rw-rw-r--   0 root         (0)     1003     5773 2023-04-03 13:56:12.000000 google-cloud-appengine-admin-1.9.2/google/cloud/appengine_admin_v1/services/versions/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-03 13:59:00.563552 google-cloud-appengine-admin-1.9.2/google/cloud/appengine_admin_v1/services/versions/transports/
--rw-rw-r--   0 root         (0)     1003     1316 2023-04-03 13:56:12.000000 google-cloud-appengine-admin-1.9.2/google/cloud/appengine_admin_v1/services/versions/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     8098 2023-04-03 13:56:12.000000 google-cloud-appengine-admin-1.9.2/google/cloud/appengine_admin_v1/services/versions/transports/base.py
--rw-rw-r--   0 root         (0)     1003    19936 2023-04-03 13:56:12.000000 google-cloud-appengine-admin-1.9.2/google/cloud/appengine_admin_v1/services/versions/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    20339 2023-04-03 13:56:12.000000 google-cloud-appengine-admin-1.9.2/google/cloud/appengine_admin_v1/services/versions/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    31625 2023-04-03 13:56:12.000000 google-cloud-appengine-admin-1.9.2/google/cloud/appengine_admin_v1/services/versions/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-03 13:59:00.567553 google-cloud-appengine-admin-1.9.2/google/cloud/appengine_admin_v1/types/
--rw-rw-r--   0 root         (0)     1003     5992 2023-04-03 13:56:12.000000 google-cloud-appengine-admin-1.9.2/google/cloud/appengine_admin_v1/types/__init__.py
--rw-rw-r--   0 root         (0)     1003    20745 2023-04-03 13:56:12.000000 google-cloud-appengine-admin-1.9.2/google/cloud/appengine_admin_v1/types/app_yaml.py
--rw-rw-r--   0 root         (0)     1003    34093 2023-04-03 13:56:12.000000 google-cloud-appengine-admin-1.9.2/google/cloud/appengine_admin_v1/types/appengine.py
--rw-rw-r--   0 root         (0)     1003    10495 2023-04-03 13:56:12.000000 google-cloud-appengine-admin-1.9.2/google/cloud/appengine_admin_v1/types/application.py
--rw-rw-r--   0 root         (0)     1003     2986 2023-04-03 13:56:12.000000 google-cloud-appengine-admin-1.9.2/google/cloud/appengine_admin_v1/types/audit_data.py
--rw-rw-r--   0 root         (0)     1003     9546 2023-04-03 13:56:12.000000 google-cloud-appengine-admin-1.9.2/google/cloud/appengine_admin_v1/types/certificate.py
--rw-rw-r--   0 root         (0)     1003     6119 2023-04-03 13:56:12.000000 google-cloud-appengine-admin-1.9.2/google/cloud/appengine_admin_v1/types/deploy.py
--rw-rw-r--   0 root         (0)     1003      762 2023-04-03 13:56:12.000000 google-cloud-appengine-admin-1.9.2/google/cloud/appengine_admin_v1/types/deployed_files.py
--rw-rw-r--   0 root         (0)     1003     1605 2023-04-03 13:56:12.000000 google-cloud-appengine-admin-1.9.2/google/cloud/appengine_admin_v1/types/domain.py
--rw-rw-r--   0 root         (0)     1003     6607 2023-04-03 13:56:12.000000 google-cloud-appengine-admin-1.9.2/google/cloud/appengine_admin_v1/types/domain_mapping.py
--rw-rw-r--   0 root         (0)     1003     3257 2023-04-03 13:56:12.000000 google-cloud-appengine-admin-1.9.2/google/cloud/appengine_admin_v1/types/firewall.py
--rw-rw-r--   0 root         (0)     1003     7401 2023-04-03 13:56:12.000000 google-cloud-appengine-admin-1.9.2/google/cloud/appengine_admin_v1/types/instance.py
--rw-rw-r--   0 root         (0)     1003     1869 2023-04-03 13:56:12.000000 google-cloud-appengine-admin-1.9.2/google/cloud/appengine_admin_v1/types/location.py
--rw-rw-r--   0 root         (0)     1003     2206 2023-04-03 13:56:12.000000 google-cloud-appengine-admin-1.9.2/google/cloud/appengine_admin_v1/types/network_settings.py
--rw-rw-r--   0 root         (0)     1003     3784 2023-04-03 13:56:12.000000 google-cloud-appengine-admin-1.9.2/google/cloud/appengine_admin_v1/types/operation.py
--rw-rw-r--   0 root         (0)     1003     6022 2023-04-03 13:56:12.000000 google-cloud-appengine-admin-1.9.2/google/cloud/appengine_admin_v1/types/service.py
--rw-rw-r--   0 root         (0)     1003    36976 2023-04-03 13:56:12.000000 google-cloud-appengine-admin-1.9.2/google/cloud/appengine_admin_v1/types/version.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-03 13:59:00.567553 google-cloud-appengine-admin-1.9.2/google_cloud_appengine_admin.egg-info/
--rw-r--r--   0 root         (0)     1003     4674 2023-04-03 13:59:00.000000 google-cloud-appengine-admin-1.9.2/google_cloud_appengine_admin.egg-info/PKG-INFO
--rw-r--r--   0 root         (0)     1003     7346 2023-04-03 13:59:00.000000 google-cloud-appengine-admin-1.9.2/google_cloud_appengine_admin.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0)     1003        1 2023-04-03 13:59:00.000000 google-cloud-appengine-admin-1.9.2/google_cloud_appengine_admin.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0)     1003       20 2023-04-03 13:59:00.000000 google-cloud-appengine-admin-1.9.2/google_cloud_appengine_admin.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0)     1003        1 2023-04-03 13:59:00.000000 google-cloud-appengine-admin-1.9.2/google_cloud_appengine_admin.egg-info/not-zip-safe
--rw-r--r--   0 root         (0)     1003      315 2023-04-03 13:59:00.000000 google-cloud-appengine-admin-1.9.2/google_cloud_appengine_admin.egg-info/requires.txt
--rw-r--r--   0 root         (0)     1003        7 2023-04-03 13:59:00.000000 google-cloud-appengine-admin-1.9.2/google_cloud_appengine_admin.egg-info/top_level.txt
--rw-rw-r--   0 root         (0)     1003       67 2023-04-03 13:59:00.571553 google-cloud-appengine-admin-1.9.2/setup.cfg
--rw-rw-r--   0 root         (0)     1003     2959 2023-04-03 13:56:12.000000 google-cloud-appengine-admin-1.9.2/setup.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-03 13:59:00.567553 google-cloud-appengine-admin-1.9.2/tests/
--rw-rw-r--   0 root         (0)     1003      600 2023-04-03 13:56:12.000000 google-cloud-appengine-admin-1.9.2/tests/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-03 13:59:00.567553 google-cloud-appengine-admin-1.9.2/tests/unit/
--rw-rw-r--   0 root         (0)     1003      600 2023-04-03 13:56:12.000000 google-cloud-appengine-admin-1.9.2/tests/unit/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-03 13:59:00.567553 google-cloud-appengine-admin-1.9.2/tests/unit/gapic/
--rw-rw-r--   0 root         (0)     1003      600 2023-04-03 13:56:12.000000 google-cloud-appengine-admin-1.9.2/tests/unit/gapic/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-03 13:59:00.571553 google-cloud-appengine-admin-1.9.2/tests/unit/gapic/appengine_admin_v1/
--rw-rw-r--   0 root         (0)     1003      600 2023-04-03 13:56:12.000000 google-cloud-appengine-admin-1.9.2/tests/unit/gapic/appengine_admin_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003   103785 2023-04-03 13:56:12.000000 google-cloud-appengine-admin-1.9.2/tests/unit/gapic/appengine_admin_v1/test_applications.py
--rw-rw-r--   0 root         (0)     1003   124281 2023-04-03 13:56:12.000000 google-cloud-appengine-admin-1.9.2/tests/unit/gapic/appengine_admin_v1/test_authorized_certificates.py
--rw-rw-r--   0 root         (0)     1003    73383 2023-04-03 13:56:12.000000 google-cloud-appengine-admin-1.9.2/tests/unit/gapic/appengine_admin_v1/test_authorized_domains.py
--rw-rw-r--   0 root         (0)     1003   116137 2023-04-03 13:56:12.000000 google-cloud-appengine-admin-1.9.2/tests/unit/gapic/appengine_admin_v1/test_domain_mappings.py
--rw-rw-r--   0 root         (0)     1003   122379 2023-04-03 13:56:12.000000 google-cloud-appengine-admin-1.9.2/tests/unit/gapic/appengine_admin_v1/test_firewall.py
--rw-rw-r--   0 root         (0)     1003   105746 2023-04-03 13:56:12.000000 google-cloud-appengine-admin-1.9.2/tests/unit/gapic/appengine_admin_v1/test_instances.py
--rw-rw-r--   0 root         (0)     1003   100489 2023-04-03 13:56:12.000000 google-cloud-appengine-admin-1.9.2/tests/unit/gapic/appengine_admin_v1/test_services.py
--rw-rw-r--   0 root         (0)     1003   139870 2023-04-03 13:56:12.000000 google-cloud-appengine-admin-1.9.2/tests/unit/gapic/appengine_admin_v1/test_versions.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:14:57.376995 google-cloud-appengine-admin-1.9.3/
+-rw-rw-r--   0 root         (0)     1003    11358 2023-07-05 15:12:27.000000 google-cloud-appengine-admin-1.9.3/LICENSE
+-rw-rw-r--   0 root         (0)     1003      860 2023-07-05 15:12:27.000000 google-cloud-appengine-admin-1.9.3/MANIFEST.in
+-rw-r--r--   0 root         (0)     1003     4674 2023-07-05 15:14:57.376995 google-cloud-appengine-admin-1.9.3/PKG-INFO
+-rw-rw-r--   0 root         (0)     1003     3734 2023-07-05 15:12:27.000000 google-cloud-appengine-admin-1.9.3/README.rst
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:14:57.348993 google-cloud-appengine-admin-1.9.3/google/
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:14:57.348993 google-cloud-appengine-admin-1.9.3/google/cloud/
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:14:57.352993 google-cloud-appengine-admin-1.9.3/google/cloud/appengine_admin/
+-rw-rw-r--   0 root         (0)     1003     8893 2023-07-05 15:12:27.000000 google-cloud-appengine-admin-1.9.3/google/cloud/appengine_admin/__init__.py
+-rw-rw-r--   0 root         (0)     1003      652 2023-07-05 15:12:27.000000 google-cloud-appengine-admin-1.9.3/google/cloud/appengine_admin/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       89 2023-07-05 15:12:27.000000 google-cloud-appengine-admin-1.9.3/google/cloud/appengine_admin/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:14:57.356994 google-cloud-appengine-admin-1.9.3/google/cloud/appengine_admin_v1/
+-rw-rw-r--   0 root         (0)     1003     7356 2023-07-05 15:12:27.000000 google-cloud-appengine-admin-1.9.3/google/cloud/appengine_admin_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003    16689 2023-07-05 15:12:27.000000 google-cloud-appengine-admin-1.9.3/google/cloud/appengine_admin_v1/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      652 2023-07-05 15:12:27.000000 google-cloud-appengine-admin-1.9.3/google/cloud/appengine_admin_v1/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       89 2023-07-05 15:12:27.000000 google-cloud-appengine-admin-1.9.3/google/cloud/appengine_admin_v1/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:14:57.356994 google-cloud-appengine-admin-1.9.3/google/cloud/appengine_admin_v1/services/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:12:27.000000 google-cloud-appengine-admin-1.9.3/google/cloud/appengine_admin_v1/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:14:57.356994 google-cloud-appengine-admin-1.9.3/google/cloud/appengine_admin_v1/services/applications/
+-rw-rw-r--   0 root         (0)     1003      761 2023-07-05 15:12:27.000000 google-cloud-appengine-admin-1.9.3/google/cloud/appengine_admin_v1/services/applications/__init__.py
+-rw-rw-r--   0 root         (0)     1003    25684 2023-07-05 15:12:27.000000 google-cloud-appengine-admin-1.9.3/google/cloud/appengine_admin_v1/services/applications/async_client.py
+-rw-rw-r--   0 root         (0)     1003    34672 2023-07-05 15:12:27.000000 google-cloud-appengine-admin-1.9.3/google/cloud/appengine_admin_v1/services/applications/client.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:14:57.356994 google-cloud-appengine-admin-1.9.3/google/cloud/appengine_admin_v1/services/applications/transports/
+-rw-rw-r--   0 root         (0)     1003     1372 2023-07-05 15:12:27.000000 google-cloud-appengine-admin-1.9.3/google/cloud/appengine_admin_v1/services/applications/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     7736 2023-07-05 15:12:27.000000 google-cloud-appengine-admin-1.9.3/google/cloud/appengine_admin_v1/services/applications/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    17364 2023-07-05 15:12:27.000000 google-cloud-appengine-admin-1.9.3/google/cloud/appengine_admin_v1/services/applications/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    17734 2023-07-05 15:12:27.000000 google-cloud-appengine-admin-1.9.3/google/cloud/appengine_admin_v1/services/applications/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    27977 2023-07-05 15:12:27.000000 google-cloud-appengine-admin-1.9.3/google/cloud/appengine_admin_v1/services/applications/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:14:57.356994 google-cloud-appengine-admin-1.9.3/google/cloud/appengine_admin_v1/services/authorized_certificates/
+-rw-rw-r--   0 root         (0)     1003      801 2023-07-05 15:12:27.000000 google-cloud-appengine-admin-1.9.3/google/cloud/appengine_admin_v1/services/authorized_certificates/__init__.py
+-rw-rw-r--   0 root         (0)     1003    26810 2023-07-05 15:12:27.000000 google-cloud-appengine-admin-1.9.3/google/cloud/appengine_admin_v1/services/authorized_certificates/async_client.py
+-rw-rw-r--   0 root         (0)     1003    36103 2023-07-05 15:12:27.000000 google-cloud-appengine-admin-1.9.3/google/cloud/appengine_admin_v1/services/authorized_certificates/client.py
+-rw-rw-r--   0 root         (0)     1003     6190 2023-07-05 15:12:27.000000 google-cloud-appengine-admin-1.9.3/google/cloud/appengine_admin_v1/services/authorized_certificates/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:14:57.356994 google-cloud-appengine-admin-1.9.3/google/cloud/appengine_admin_v1/services/authorized_certificates/transports/
+-rw-rw-r--   0 root         (0)     1003     1533 2023-07-05 15:12:27.000000 google-cloud-appengine-admin-1.9.3/google/cloud/appengine_admin_v1/services/authorized_certificates/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     8455 2023-07-05 15:12:27.000000 google-cloud-appengine-admin-1.9.3/google/cloud/appengine_admin_v1/services/authorized_certificates/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    17555 2023-07-05 15:12:27.000000 google-cloud-appengine-admin-1.9.3/google/cloud/appengine_admin_v1/services/authorized_certificates/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    17879 2023-07-05 15:12:27.000000 google-cloud-appengine-admin-1.9.3/google/cloud/appengine_admin_v1/services/authorized_certificates/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    32569 2023-07-05 15:12:27.000000 google-cloud-appengine-admin-1.9.3/google/cloud/appengine_admin_v1/services/authorized_certificates/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:14:57.360994 google-cloud-appengine-admin-1.9.3/google/cloud/appengine_admin_v1/services/authorized_domains/
+-rw-rw-r--   0 root         (0)     1003      781 2023-07-05 15:12:27.000000 google-cloud-appengine-admin-1.9.3/google/cloud/appengine_admin_v1/services/authorized_domains/__init__.py
+-rw-rw-r--   0 root         (0)     1003    13268 2023-07-05 15:12:27.000000 google-cloud-appengine-admin-1.9.3/google/cloud/appengine_admin_v1/services/authorized_domains/async_client.py
+-rw-rw-r--   0 root         (0)     1003    21784 2023-07-05 15:12:27.000000 google-cloud-appengine-admin-1.9.3/google/cloud/appengine_admin_v1/services/authorized_domains/client.py
+-rw-rw-r--   0 root         (0)     1003     6000 2023-07-05 15:12:27.000000 google-cloud-appengine-admin-1.9.3/google/cloud/appengine_admin_v1/services/authorized_domains/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:14:57.360994 google-cloud-appengine-admin-1.9.3/google/cloud/appengine_admin_v1/services/authorized_domains/transports/
+-rw-rw-r--   0 root         (0)     1003     1442 2023-07-05 15:12:27.000000 google-cloud-appengine-admin-1.9.3/google/cloud/appengine_admin_v1/services/authorized_domains/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     6266 2023-07-05 15:12:27.000000 google-cloud-appengine-admin-1.9.3/google/cloud/appengine_admin_v1/services/authorized_domains/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    12034 2023-07-05 15:12:27.000000 google-cloud-appengine-admin-1.9.3/google/cloud/appengine_admin_v1/services/authorized_domains/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    12242 2023-07-05 15:12:27.000000 google-cloud-appengine-admin-1.9.3/google/cloud/appengine_admin_v1/services/authorized_domains/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    12095 2023-07-05 15:12:27.000000 google-cloud-appengine-admin-1.9.3/google/cloud/appengine_admin_v1/services/authorized_domains/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:14:57.360994 google-cloud-appengine-admin-1.9.3/google/cloud/appengine_admin_v1/services/domain_mappings/
+-rw-rw-r--   0 root         (0)     1003      769 2023-07-05 15:12:27.000000 google-cloud-appengine-admin-1.9.3/google/cloud/appengine_admin_v1/services/domain_mappings/__init__.py
+-rw-rw-r--   0 root         (0)     1003    28101 2023-07-05 15:12:27.000000 google-cloud-appengine-admin-1.9.3/google/cloud/appengine_admin_v1/services/domain_mappings/async_client.py
+-rw-rw-r--   0 root         (0)     1003    37217 2023-07-05 15:12:27.000000 google-cloud-appengine-admin-1.9.3/google/cloud/appengine_admin_v1/services/domain_mappings/client.py
+-rw-rw-r--   0 root         (0)     1003     5994 2023-07-05 15:12:27.000000 google-cloud-appengine-admin-1.9.3/google/cloud/appengine_admin_v1/services/domain_mappings/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:14:57.360994 google-cloud-appengine-admin-1.9.3/google/cloud/appengine_admin_v1/services/domain_mappings/transports/
+-rw-rw-r--   0 root         (0)     1003     1400 2023-07-05 15:12:27.000000 google-cloud-appengine-admin-1.9.3/google/cloud/appengine_admin_v1/services/domain_mappings/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     8309 2023-07-05 15:12:27.000000 google-cloud-appengine-admin-1.9.3/google/cloud/appengine_admin_v1/services/domain_mappings/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    17690 2023-07-05 15:12:27.000000 google-cloud-appengine-admin-1.9.3/google/cloud/appengine_admin_v1/services/domain_mappings/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    18093 2023-07-05 15:12:27.000000 google-cloud-appengine-admin-1.9.3/google/cloud/appengine_admin_v1/services/domain_mappings/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    32856 2023-07-05 15:12:27.000000 google-cloud-appengine-admin-1.9.3/google/cloud/appengine_admin_v1/services/domain_mappings/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:14:57.364994 google-cloud-appengine-admin-1.9.3/google/cloud/appengine_admin_v1/services/firewall/
+-rw-rw-r--   0 root         (0)     1003      745 2023-07-05 15:12:27.000000 google-cloud-appengine-admin-1.9.3/google/cloud/appengine_admin_v1/services/firewall/__init__.py
+-rw-rw-r--   0 root         (0)     1003    28655 2023-07-05 15:12:27.000000 google-cloud-appengine-admin-1.9.3/google/cloud/appengine_admin_v1/services/firewall/async_client.py
+-rw-rw-r--   0 root         (0)     1003    38139 2023-07-05 15:12:27.000000 google-cloud-appengine-admin-1.9.3/google/cloud/appengine_admin_v1/services/firewall/client.py
+-rw-rw-r--   0 root         (0)     1003     5914 2023-07-05 15:12:27.000000 google-cloud-appengine-admin-1.9.3/google/cloud/appengine_admin_v1/services/firewall/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:14:57.364994 google-cloud-appengine-admin-1.9.3/google/cloud/appengine_admin_v1/services/firewall/transports/
+-rw-rw-r--   0 root         (0)     1003     1316 2023-07-05 15:12:27.000000 google-cloud-appengine-admin-1.9.3/google/cloud/appengine_admin_v1/services/firewall/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     8556 2023-07-05 15:12:27.000000 google-cloud-appengine-admin-1.9.3/google/cloud/appengine_admin_v1/services/firewall/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    18412 2023-07-05 15:12:27.000000 google-cloud-appengine-admin-1.9.3/google/cloud/appengine_admin_v1/services/firewall/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    18758 2023-07-05 15:12:27.000000 google-cloud-appengine-admin-1.9.3/google/cloud/appengine_admin_v1/services/firewall/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    35843 2023-07-05 15:12:27.000000 google-cloud-appengine-admin-1.9.3/google/cloud/appengine_admin_v1/services/firewall/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:14:57.364994 google-cloud-appengine-admin-1.9.3/google/cloud/appengine_admin_v1/services/instances/
+-rw-rw-r--   0 root         (0)     1003      749 2023-07-05 15:12:27.000000 google-cloud-appengine-admin-1.9.3/google/cloud/appengine_admin_v1/services/instances/__init__.py
+-rw-rw-r--   0 root         (0)     1003    24997 2023-07-05 15:12:27.000000 google-cloud-appengine-admin-1.9.3/google/cloud/appengine_admin_v1/services/instances/async_client.py
+-rw-rw-r--   0 root         (0)     1003    34633 2023-07-05 15:12:27.000000 google-cloud-appengine-admin-1.9.3/google/cloud/appengine_admin_v1/services/instances/client.py
+-rw-rw-r--   0 root         (0)     1003     5808 2023-07-05 15:12:27.000000 google-cloud-appengine-admin-1.9.3/google/cloud/appengine_admin_v1/services/instances/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:14:57.364994 google-cloud-appengine-admin-1.9.3/google/cloud/appengine_admin_v1/services/instances/transports/
+-rw-rw-r--   0 root         (0)     1003     1330 2023-07-05 15:12:27.000000 google-cloud-appengine-admin-1.9.3/google/cloud/appengine_admin_v1/services/instances/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     7692 2023-07-05 15:12:27.000000 google-cloud-appengine-admin-1.9.3/google/cloud/appengine_admin_v1/services/instances/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    17044 2023-07-05 15:12:27.000000 google-cloud-appengine-admin-1.9.3/google/cloud/appengine_admin_v1/services/instances/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    17397 2023-07-05 15:12:27.000000 google-cloud-appengine-admin-1.9.3/google/cloud/appengine_admin_v1/services/instances/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    26981 2023-07-05 15:12:27.000000 google-cloud-appengine-admin-1.9.3/google/cloud/appengine_admin_v1/services/instances/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:14:57.364994 google-cloud-appengine-admin-1.9.3/google/cloud/appengine_admin_v1/services/services/
+-rw-rw-r--   0 root         (0)     1003      745 2023-07-05 15:12:27.000000 google-cloud-appengine-admin-1.9.3/google/cloud/appengine_admin_v1/services/services/__init__.py
+-rw-rw-r--   0 root         (0)     1003    24375 2023-07-05 15:12:27.000000 google-cloud-appengine-admin-1.9.3/google/cloud/appengine_admin_v1/services/services/async_client.py
+-rw-rw-r--   0 root         (0)     1003    33405 2023-07-05 15:12:27.000000 google-cloud-appengine-admin-1.9.3/google/cloud/appengine_admin_v1/services/services/client.py
+-rw-rw-r--   0 root         (0)     1003     5773 2023-07-05 15:12:27.000000 google-cloud-appengine-admin-1.9.3/google/cloud/appengine_admin_v1/services/services/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:14:57.368995 google-cloud-appengine-admin-1.9.3/google/cloud/appengine_admin_v1/services/services/transports/
+-rw-rw-r--   0 root         (0)     1003     1316 2023-07-05 15:12:27.000000 google-cloud-appengine-admin-1.9.3/google/cloud/appengine_admin_v1/services/services/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     7670 2023-07-05 15:12:27.000000 google-cloud-appengine-admin-1.9.3/google/cloud/appengine_admin_v1/services/services/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    15635 2023-07-05 15:12:27.000000 google-cloud-appengine-admin-1.9.3/google/cloud/appengine_admin_v1/services/services/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    16002 2023-07-05 15:12:27.000000 google-cloud-appengine-admin-1.9.3/google/cloud/appengine_admin_v1/services/services/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    27245 2023-07-05 15:12:27.000000 google-cloud-appengine-admin-1.9.3/google/cloud/appengine_admin_v1/services/services/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:14:57.368995 google-cloud-appengine-admin-1.9.3/google/cloud/appengine_admin_v1/services/versions/
+-rw-rw-r--   0 root         (0)     1003      745 2023-07-05 15:12:27.000000 google-cloud-appengine-admin-1.9.3/google/cloud/appengine_admin_v1/services/versions/__init__.py
+-rw-rw-r--   0 root         (0)     1003    30379 2023-07-05 15:12:27.000000 google-cloud-appengine-admin-1.9.3/google/cloud/appengine_admin_v1/services/versions/async_client.py
+-rw-rw-r--   0 root         (0)     1003    39535 2023-07-05 15:12:27.000000 google-cloud-appengine-admin-1.9.3/google/cloud/appengine_admin_v1/services/versions/client.py
+-rw-rw-r--   0 root         (0)     1003     5773 2023-07-05 15:12:27.000000 google-cloud-appengine-admin-1.9.3/google/cloud/appengine_admin_v1/services/versions/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:14:57.368995 google-cloud-appengine-admin-1.9.3/google/cloud/appengine_admin_v1/services/versions/transports/
+-rw-rw-r--   0 root         (0)     1003     1316 2023-07-05 15:12:27.000000 google-cloud-appengine-admin-1.9.3/google/cloud/appengine_admin_v1/services/versions/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     8098 2023-07-05 15:12:27.000000 google-cloud-appengine-admin-1.9.3/google/cloud/appengine_admin_v1/services/versions/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    19936 2023-07-05 15:12:27.000000 google-cloud-appengine-admin-1.9.3/google/cloud/appengine_admin_v1/services/versions/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    20339 2023-07-05 15:12:27.000000 google-cloud-appengine-admin-1.9.3/google/cloud/appengine_admin_v1/services/versions/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    31625 2023-07-05 15:12:27.000000 google-cloud-appengine-admin-1.9.3/google/cloud/appengine_admin_v1/services/versions/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:14:57.372995 google-cloud-appengine-admin-1.9.3/google/cloud/appengine_admin_v1/types/
+-rw-rw-r--   0 root         (0)     1003     5992 2023-07-05 15:12:27.000000 google-cloud-appengine-admin-1.9.3/google/cloud/appengine_admin_v1/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003    20745 2023-07-05 15:12:27.000000 google-cloud-appengine-admin-1.9.3/google/cloud/appengine_admin_v1/types/app_yaml.py
+-rw-rw-r--   0 root         (0)     1003    34093 2023-07-05 15:12:27.000000 google-cloud-appengine-admin-1.9.3/google/cloud/appengine_admin_v1/types/appengine.py
+-rw-rw-r--   0 root         (0)     1003    10495 2023-07-05 15:12:27.000000 google-cloud-appengine-admin-1.9.3/google/cloud/appengine_admin_v1/types/application.py
+-rw-rw-r--   0 root         (0)     1003     2986 2023-07-05 15:12:27.000000 google-cloud-appengine-admin-1.9.3/google/cloud/appengine_admin_v1/types/audit_data.py
+-rw-rw-r--   0 root         (0)     1003     9546 2023-07-05 15:12:27.000000 google-cloud-appengine-admin-1.9.3/google/cloud/appengine_admin_v1/types/certificate.py
+-rw-rw-r--   0 root         (0)     1003     6119 2023-07-05 15:12:27.000000 google-cloud-appengine-admin-1.9.3/google/cloud/appengine_admin_v1/types/deploy.py
+-rw-rw-r--   0 root         (0)     1003      762 2023-07-05 15:12:27.000000 google-cloud-appengine-admin-1.9.3/google/cloud/appengine_admin_v1/types/deployed_files.py
+-rw-rw-r--   0 root         (0)     1003     1605 2023-07-05 15:12:27.000000 google-cloud-appengine-admin-1.9.3/google/cloud/appengine_admin_v1/types/domain.py
+-rw-rw-r--   0 root         (0)     1003     6607 2023-07-05 15:12:27.000000 google-cloud-appengine-admin-1.9.3/google/cloud/appengine_admin_v1/types/domain_mapping.py
+-rw-rw-r--   0 root         (0)     1003     3257 2023-07-05 15:12:27.000000 google-cloud-appengine-admin-1.9.3/google/cloud/appengine_admin_v1/types/firewall.py
+-rw-rw-r--   0 root         (0)     1003     7401 2023-07-05 15:12:27.000000 google-cloud-appengine-admin-1.9.3/google/cloud/appengine_admin_v1/types/instance.py
+-rw-rw-r--   0 root         (0)     1003     1869 2023-07-05 15:12:27.000000 google-cloud-appengine-admin-1.9.3/google/cloud/appengine_admin_v1/types/location.py
+-rw-rw-r--   0 root         (0)     1003     2206 2023-07-05 15:12:27.000000 google-cloud-appengine-admin-1.9.3/google/cloud/appengine_admin_v1/types/network_settings.py
+-rw-rw-r--   0 root         (0)     1003     3784 2023-07-05 15:12:27.000000 google-cloud-appengine-admin-1.9.3/google/cloud/appengine_admin_v1/types/operation.py
+-rw-rw-r--   0 root         (0)     1003     6022 2023-07-05 15:12:27.000000 google-cloud-appengine-admin-1.9.3/google/cloud/appengine_admin_v1/types/service.py
+-rw-rw-r--   0 root         (0)     1003    36976 2023-07-05 15:12:27.000000 google-cloud-appengine-admin-1.9.3/google/cloud/appengine_admin_v1/types/version.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:14:57.372995 google-cloud-appengine-admin-1.9.3/google_cloud_appengine_admin.egg-info/
+-rw-r--r--   0 root         (0)     1003     4674 2023-07-05 15:14:57.000000 google-cloud-appengine-admin-1.9.3/google_cloud_appengine_admin.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0)     1003     7346 2023-07-05 15:14:57.000000 google-cloud-appengine-admin-1.9.3/google_cloud_appengine_admin.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-07-05 15:14:57.000000 google-cloud-appengine-admin-1.9.3/google_cloud_appengine_admin.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0)     1003       20 2023-07-05 15:14:57.000000 google-cloud-appengine-admin-1.9.3/google_cloud_appengine_admin.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-07-05 15:14:57.000000 google-cloud-appengine-admin-1.9.3/google_cloud_appengine_admin.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0)     1003      315 2023-07-05 15:14:57.000000 google-cloud-appengine-admin-1.9.3/google_cloud_appengine_admin.egg-info/requires.txt
+-rw-r--r--   0 root         (0)     1003        7 2023-07-05 15:14:57.000000 google-cloud-appengine-admin-1.9.3/google_cloud_appengine_admin.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0)     1003       67 2023-07-05 15:14:57.376995 google-cloud-appengine-admin-1.9.3/setup.cfg
+-rw-rw-r--   0 root         (0)     1003     2959 2023-07-05 15:12:27.000000 google-cloud-appengine-admin-1.9.3/setup.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:14:57.372995 google-cloud-appengine-admin-1.9.3/tests/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:12:27.000000 google-cloud-appengine-admin-1.9.3/tests/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:14:57.372995 google-cloud-appengine-admin-1.9.3/tests/unit/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:12:27.000000 google-cloud-appengine-admin-1.9.3/tests/unit/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:14:57.372995 google-cloud-appengine-admin-1.9.3/tests/unit/gapic/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:12:27.000000 google-cloud-appengine-admin-1.9.3/tests/unit/gapic/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:14:57.376995 google-cloud-appengine-admin-1.9.3/tests/unit/gapic/appengine_admin_v1/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:12:27.000000 google-cloud-appengine-admin-1.9.3/tests/unit/gapic/appengine_admin_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003   103785 2023-07-05 15:12:27.000000 google-cloud-appengine-admin-1.9.3/tests/unit/gapic/appengine_admin_v1/test_applications.py
+-rw-rw-r--   0 root         (0)     1003   124480 2023-07-05 15:12:27.000000 google-cloud-appengine-admin-1.9.3/tests/unit/gapic/appengine_admin_v1/test_authorized_certificates.py
+-rw-rw-r--   0 root         (0)     1003    73582 2023-07-05 15:12:27.000000 google-cloud-appengine-admin-1.9.3/tests/unit/gapic/appengine_admin_v1/test_authorized_domains.py
+-rw-rw-r--   0 root         (0)     1003   116336 2023-07-05 15:12:27.000000 google-cloud-appengine-admin-1.9.3/tests/unit/gapic/appengine_admin_v1/test_domain_mappings.py
+-rw-rw-r--   0 root         (0)     1003   122578 2023-07-05 15:12:27.000000 google-cloud-appengine-admin-1.9.3/tests/unit/gapic/appengine_admin_v1/test_firewall.py
+-rw-rw-r--   0 root         (0)     1003   105945 2023-07-05 15:12:27.000000 google-cloud-appengine-admin-1.9.3/tests/unit/gapic/appengine_admin_v1/test_instances.py
+-rw-rw-r--   0 root         (0)     1003   100688 2023-07-05 15:12:27.000000 google-cloud-appengine-admin-1.9.3/tests/unit/gapic/appengine_admin_v1/test_services.py
+-rw-rw-r--   0 root         (0)     1003   139791 2023-07-05 15:12:27.000000 google-cloud-appengine-admin-1.9.3/tests/unit/gapic/appengine_admin_v1/test_versions.py
```

### Comparing `google-cloud-appengine-admin-1.9.2/LICENSE` & `google-cloud-appengine-admin-1.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `google-cloud-appengine-admin-1.9.2/MANIFEST.in` & `google-cloud-appengine-admin-1.9.3/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `google-cloud-appengine-admin-1.9.2/PKG-INFO` & `google-cloud-appengine-admin-1.9.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-appengine-admin
-Version: 1.9.2
+Version: 1.9.3
 Summary: Google Cloud Appengine Admin API client library
 Home-page: https://github.com/googleapis/python-appengine-admin
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `google-cloud-appengine-admin-1.9.2/README.rst` & `google-cloud-appengine-admin-1.9.3/README.rst`

 * *Files identical despite different names*

### Comparing `google-cloud-appengine-admin-1.9.2/google/cloud/appengine_admin/__init__.py` & `google-cloud-appengine-admin-1.9.3/google/cloud/appengine_admin/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-appengine-admin-1.9.2/google/cloud/appengine_admin/gapic_version.py` & `google-cloud-appengine-admin-1.9.3/google/cloud/appengine_admin/gapic_version.py`

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
-__version__ = "1.9.2"  # {x-release-please-version}
+__version__ = "1.9.3"  # {x-release-please-version}
```

### Comparing `google-cloud-appengine-admin-1.9.2/google/cloud/appengine_admin_v1/__init__.py` & `google-cloud-appengine-admin-1.9.3/google/cloud/appengine_admin_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-appengine-admin-1.9.2/google/cloud/appengine_admin_v1/gapic_metadata.json` & `google-cloud-appengine-admin-1.9.3/google/cloud/appengine_admin_v1/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-cloud-appengine-admin-1.9.2/google/cloud/appengine_admin_v1/gapic_version.py` & `google-cloud-appengine-admin-1.9.3/google/cloud/appengine_admin_v1/gapic_version.py`

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
-__version__ = "1.9.2"  # {x-release-please-version}
+__version__ = "1.9.3"  # {x-release-please-version}
```

### Comparing `google-cloud-appengine-admin-1.9.2/google/cloud/appengine_admin_v1/services/__init__.py` & `google-cloud-appengine-admin-1.9.3/google/cloud/appengine_admin_v1/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-appengine-admin-1.9.2/google/cloud/appengine_admin_v1/services/applications/__init__.py` & `google-cloud-appengine-admin-1.9.3/google/cloud/appengine_admin_v1/services/applications/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-appengine-admin-1.9.2/google/cloud/appengine_admin_v1/services/applications/async_client.py` & `google-cloud-appengine-admin-1.9.3/google/cloud/appengine_admin_v1/services/applications/async_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -608,15 +608,15 @@
             application.Application,
             metadata_type=ga_operation.OperationMetadataV1,
         )
 
         # Done; return the response.
         return response
 
-    async def __aenter__(self):
+    async def __aenter__(self) -> "ApplicationsAsyncClient":
         return self
 
     async def __aexit__(self, exc_type, exc, tb):
         await self.transport.close()
 
 
 DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
```

### Comparing `google-cloud-appengine-admin-1.9.2/google/cloud/appengine_admin_v1/services/applications/client.py` & `google-cloud-appengine-admin-1.9.3/google/cloud/appengine_admin_v1/services/applications/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-appengine-admin-1.9.2/google/cloud/appengine_admin_v1/services/applications/transports/__init__.py` & `google-cloud-appengine-admin-1.9.3/google/cloud/appengine_admin_v1/services/applications/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-appengine-admin-1.9.2/google/cloud/appengine_admin_v1/services/applications/transports/base.py` & `google-cloud-appengine-admin-1.9.3/google/cloud/appengine_admin_v1/services/applications/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-appengine-admin-1.9.2/google/cloud/appengine_admin_v1/services/applications/transports/grpc.py` & `google-cloud-appengine-admin-1.9.3/google/cloud/appengine_admin_v1/services/applications/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-appengine-admin-1.9.2/google/cloud/appengine_admin_v1/services/applications/transports/grpc_asyncio.py` & `google-cloud-appengine-admin-1.9.3/google/cloud/appengine_admin_v1/services/applications/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-appengine-admin-1.9.2/google/cloud/appengine_admin_v1/services/applications/transports/rest.py` & `google-cloud-appengine-admin-1.9.3/google/cloud/appengine_admin_v1/services/applications/transports/rest.py`

 * *Files identical despite different names*

### Comparing `google-cloud-appengine-admin-1.9.2/google/cloud/appengine_admin_v1/services/authorized_certificates/__init__.py` & `google-cloud-appengine-admin-1.9.3/google/cloud/appengine_admin_v1/services/authorized_certificates/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-appengine-admin-1.9.2/google/cloud/appengine_admin_v1/services/authorized_certificates/async_client.py` & `google-cloud-appengine-admin-1.9.3/google/cloud/appengine_admin_v1/services/authorized_certificates/async_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -637,15 +637,15 @@
         await rpc(
             request,
             retry=retry,
             timeout=timeout,
             metadata=metadata,
         )
 
-    async def __aenter__(self):
+    async def __aenter__(self) -> "AuthorizedCertificatesAsyncClient":
         return self
 
     async def __aexit__(self, exc_type, exc, tb):
         await self.transport.close()
 
 
 DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
```

### Comparing `google-cloud-appengine-admin-1.9.2/google/cloud/appengine_admin_v1/services/authorized_certificates/client.py` & `google-cloud-appengine-admin-1.9.3/google/cloud/appengine_admin_v1/services/authorized_certificates/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-appengine-admin-1.9.2/google/cloud/appengine_admin_v1/services/authorized_certificates/pagers.py` & `google-cloud-appengine-admin-1.9.3/google/cloud/appengine_admin_v1/services/authorized_certificates/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-appengine-admin-1.9.2/google/cloud/appengine_admin_v1/services/authorized_certificates/transports/__init__.py` & `google-cloud-appengine-admin-1.9.3/google/cloud/appengine_admin_v1/services/authorized_certificates/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-appengine-admin-1.9.2/google/cloud/appengine_admin_v1/services/authorized_certificates/transports/base.py` & `google-cloud-appengine-admin-1.9.3/google/cloud/appengine_admin_v1/services/authorized_certificates/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-appengine-admin-1.9.2/google/cloud/appengine_admin_v1/services/authorized_certificates/transports/grpc.py` & `google-cloud-appengine-admin-1.9.3/google/cloud/appengine_admin_v1/services/authorized_certificates/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-appengine-admin-1.9.2/google/cloud/appengine_admin_v1/services/authorized_certificates/transports/grpc_asyncio.py` & `google-cloud-appengine-admin-1.9.3/google/cloud/appengine_admin_v1/services/authorized_certificates/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-appengine-admin-1.9.2/google/cloud/appengine_admin_v1/services/authorized_certificates/transports/rest.py` & `google-cloud-appengine-admin-1.9.3/google/cloud/appengine_admin_v1/services/authorized_certificates/transports/rest.py`

 * *Files identical despite different names*

### Comparing `google-cloud-appengine-admin-1.9.2/google/cloud/appengine_admin_v1/services/authorized_domains/__init__.py` & `google-cloud-appengine-admin-1.9.3/google/cloud/appengine_admin_v1/services/authorized_domains/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-appengine-admin-1.9.2/google/cloud/appengine_admin_v1/services/authorized_domains/async_client.py` & `google-cloud-appengine-admin-1.9.3/google/cloud/appengine_admin_v1/services/authorized_domains/async_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -304,15 +304,15 @@
             response=response,
             metadata=metadata,
         )
 
         # Done; return the response.
         return response
 
-    async def __aenter__(self):
+    async def __aenter__(self) -> "AuthorizedDomainsAsyncClient":
         return self
 
     async def __aexit__(self, exc_type, exc, tb):
         await self.transport.close()
 
 
 DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
```

### Comparing `google-cloud-appengine-admin-1.9.2/google/cloud/appengine_admin_v1/services/authorized_domains/client.py` & `google-cloud-appengine-admin-1.9.3/google/cloud/appengine_admin_v1/services/authorized_domains/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-appengine-admin-1.9.2/google/cloud/appengine_admin_v1/services/authorized_domains/pagers.py` & `google-cloud-appengine-admin-1.9.3/google/cloud/appengine_admin_v1/services/authorized_domains/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-appengine-admin-1.9.2/google/cloud/appengine_admin_v1/services/authorized_domains/transports/__init__.py` & `google-cloud-appengine-admin-1.9.3/google/cloud/appengine_admin_v1/services/authorized_domains/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-appengine-admin-1.9.2/google/cloud/appengine_admin_v1/services/authorized_domains/transports/base.py` & `google-cloud-appengine-admin-1.9.3/google/cloud/appengine_admin_v1/services/authorized_domains/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-appengine-admin-1.9.2/google/cloud/appengine_admin_v1/services/authorized_domains/transports/grpc.py` & `google-cloud-appengine-admin-1.9.3/google/cloud/appengine_admin_v1/services/authorized_domains/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-appengine-admin-1.9.2/google/cloud/appengine_admin_v1/services/authorized_domains/transports/grpc_asyncio.py` & `google-cloud-appengine-admin-1.9.3/google/cloud/appengine_admin_v1/services/authorized_domains/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-appengine-admin-1.9.2/google/cloud/appengine_admin_v1/services/authorized_domains/transports/rest.py` & `google-cloud-appengine-admin-1.9.3/google/cloud/appengine_admin_v1/services/authorized_domains/transports/rest.py`

 * *Files identical despite different names*

### Comparing `google-cloud-appengine-admin-1.9.2/google/cloud/appengine_admin_v1/services/domain_mappings/__init__.py` & `google-cloud-appengine-admin-1.9.3/google/cloud/appengine_admin_v1/services/domain_mappings/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-appengine-admin-1.9.2/google/cloud/appengine_admin_v1/services/domain_mappings/async_client.py` & `google-cloud-appengine-admin-1.9.3/google/cloud/appengine_admin_v1/services/domain_mappings/async_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -680,15 +680,15 @@
             empty_pb2.Empty,
             metadata_type=ga_operation.OperationMetadataV1,
         )
 
         # Done; return the response.
         return response
 
-    async def __aenter__(self):
+    async def __aenter__(self) -> "DomainMappingsAsyncClient":
         return self
 
     async def __aexit__(self, exc_type, exc, tb):
         await self.transport.close()
 
 
 DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
```

### Comparing `google-cloud-appengine-admin-1.9.2/google/cloud/appengine_admin_v1/services/domain_mappings/client.py` & `google-cloud-appengine-admin-1.9.3/google/cloud/appengine_admin_v1/services/domain_mappings/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-appengine-admin-1.9.2/google/cloud/appengine_admin_v1/services/domain_mappings/pagers.py` & `google-cloud-appengine-admin-1.9.3/google/cloud/appengine_admin_v1/services/domain_mappings/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-appengine-admin-1.9.2/google/cloud/appengine_admin_v1/services/domain_mappings/transports/__init__.py` & `google-cloud-appengine-admin-1.9.3/google/cloud/appengine_admin_v1/services/domain_mappings/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-appengine-admin-1.9.2/google/cloud/appengine_admin_v1/services/domain_mappings/transports/base.py` & `google-cloud-appengine-admin-1.9.3/google/cloud/appengine_admin_v1/services/domain_mappings/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-appengine-admin-1.9.2/google/cloud/appengine_admin_v1/services/domain_mappings/transports/grpc.py` & `google-cloud-appengine-admin-1.9.3/google/cloud/appengine_admin_v1/services/domain_mappings/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-appengine-admin-1.9.2/google/cloud/appengine_admin_v1/services/domain_mappings/transports/grpc_asyncio.py` & `google-cloud-appengine-admin-1.9.3/google/cloud/appengine_admin_v1/services/domain_mappings/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-appengine-admin-1.9.2/google/cloud/appengine_admin_v1/services/domain_mappings/transports/rest.py` & `google-cloud-appengine-admin-1.9.3/google/cloud/appengine_admin_v1/services/domain_mappings/transports/rest.py`

 * *Files identical despite different names*

### Comparing `google-cloud-appengine-admin-1.9.2/google/cloud/appengine_admin_v1/services/firewall/__init__.py` & `google-cloud-appengine-admin-1.9.3/google/cloud/appengine_admin_v1/services/firewall/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-appengine-admin-1.9.2/google/cloud/appengine_admin_v1/services/firewall/async_client.py` & `google-cloud-appengine-admin-1.9.3/google/cloud/appengine_admin_v1/services/firewall/async_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -690,15 +690,15 @@
         await rpc(
             request,
             retry=retry,
             timeout=timeout,
             metadata=metadata,
         )
 
-    async def __aenter__(self):
+    async def __aenter__(self) -> "FirewallAsyncClient":
         return self
 
     async def __aexit__(self, exc_type, exc, tb):
         await self.transport.close()
 
 
 DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
```

### Comparing `google-cloud-appengine-admin-1.9.2/google/cloud/appengine_admin_v1/services/firewall/client.py` & `google-cloud-appengine-admin-1.9.3/google/cloud/appengine_admin_v1/services/firewall/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-appengine-admin-1.9.2/google/cloud/appengine_admin_v1/services/firewall/pagers.py` & `google-cloud-appengine-admin-1.9.3/google/cloud/appengine_admin_v1/services/firewall/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-appengine-admin-1.9.2/google/cloud/appengine_admin_v1/services/firewall/transports/__init__.py` & `google-cloud-appengine-admin-1.9.3/google/cloud/appengine_admin_v1/services/firewall/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-appengine-admin-1.9.2/google/cloud/appengine_admin_v1/services/firewall/transports/base.py` & `google-cloud-appengine-admin-1.9.3/google/cloud/appengine_admin_v1/services/firewall/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-appengine-admin-1.9.2/google/cloud/appengine_admin_v1/services/firewall/transports/grpc.py` & `google-cloud-appengine-admin-1.9.3/google/cloud/appengine_admin_v1/services/firewall/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-appengine-admin-1.9.2/google/cloud/appengine_admin_v1/services/firewall/transports/grpc_asyncio.py` & `google-cloud-appengine-admin-1.9.3/google/cloud/appengine_admin_v1/services/firewall/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-appengine-admin-1.9.2/google/cloud/appengine_admin_v1/services/firewall/transports/rest.py` & `google-cloud-appengine-admin-1.9.3/google/cloud/appengine_admin_v1/services/firewall/transports/rest.py`

 * *Files identical despite different names*

### Comparing `google-cloud-appengine-admin-1.9.2/google/cloud/appengine_admin_v1/services/instances/__init__.py` & `google-cloud-appengine-admin-1.9.3/google/cloud/appengine_admin_v1/services/instances/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-appengine-admin-1.9.2/google/cloud/appengine_admin_v1/services/instances/async_client.py` & `google-cloud-appengine-admin-1.9.3/google/cloud/appengine_admin_v1/services/instances/async_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -598,15 +598,15 @@
             instance.Instance,
             metadata_type=ga_operation.OperationMetadataV1,
         )
 
         # Done; return the response.
         return response
 
-    async def __aenter__(self):
+    async def __aenter__(self) -> "InstancesAsyncClient":
         return self
 
     async def __aexit__(self, exc_type, exc, tb):
         await self.transport.close()
 
 
 DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
```

### Comparing `google-cloud-appengine-admin-1.9.2/google/cloud/appengine_admin_v1/services/instances/client.py` & `google-cloud-appengine-admin-1.9.3/google/cloud/appengine_admin_v1/services/instances/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-appengine-admin-1.9.2/google/cloud/appengine_admin_v1/services/instances/pagers.py` & `google-cloud-appengine-admin-1.9.3/google/cloud/appengine_admin_v1/services/instances/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-appengine-admin-1.9.2/google/cloud/appengine_admin_v1/services/instances/transports/__init__.py` & `google-cloud-appengine-admin-1.9.3/google/cloud/appengine_admin_v1/services/instances/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-appengine-admin-1.9.2/google/cloud/appengine_admin_v1/services/instances/transports/base.py` & `google-cloud-appengine-admin-1.9.3/google/cloud/appengine_admin_v1/services/instances/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-appengine-admin-1.9.2/google/cloud/appengine_admin_v1/services/instances/transports/grpc.py` & `google-cloud-appengine-admin-1.9.3/google/cloud/appengine_admin_v1/services/instances/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-appengine-admin-1.9.2/google/cloud/appengine_admin_v1/services/instances/transports/grpc_asyncio.py` & `google-cloud-appengine-admin-1.9.3/google/cloud/appengine_admin_v1/services/instances/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-appengine-admin-1.9.2/google/cloud/appengine_admin_v1/services/instances/transports/rest.py` & `google-cloud-appengine-admin-1.9.3/google/cloud/appengine_admin_v1/services/instances/transports/rest.py`

 * *Files identical despite different names*

### Comparing `google-cloud-appengine-admin-1.9.2/google/cloud/appengine_admin_v1/services/services/__init__.py` & `google-cloud-appengine-admin-1.9.3/google/cloud/appengine_admin_v1/services/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-appengine-admin-1.9.2/google/cloud/appengine_admin_v1/services/services/async_client.py` & `google-cloud-appengine-admin-1.9.3/google/cloud/appengine_admin_v1/services/services/async_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -585,15 +585,15 @@
             empty_pb2.Empty,
             metadata_type=ga_operation.OperationMetadataV1,
         )
 
         # Done; return the response.
         return response
 
-    async def __aenter__(self):
+    async def __aenter__(self) -> "ServicesAsyncClient":
         return self
 
     async def __aexit__(self, exc_type, exc, tb):
         await self.transport.close()
 
 
 DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
```

### Comparing `google-cloud-appengine-admin-1.9.2/google/cloud/appengine_admin_v1/services/services/client.py` & `google-cloud-appengine-admin-1.9.3/google/cloud/appengine_admin_v1/services/services/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-appengine-admin-1.9.2/google/cloud/appengine_admin_v1/services/services/pagers.py` & `google-cloud-appengine-admin-1.9.3/google/cloud/appengine_admin_v1/services/services/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-appengine-admin-1.9.2/google/cloud/appengine_admin_v1/services/services/transports/__init__.py` & `google-cloud-appengine-admin-1.9.3/google/cloud/appengine_admin_v1/services/services/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-appengine-admin-1.9.2/google/cloud/appengine_admin_v1/services/services/transports/base.py` & `google-cloud-appengine-admin-1.9.3/google/cloud/appengine_admin_v1/services/services/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-appengine-admin-1.9.2/google/cloud/appengine_admin_v1/services/services/transports/grpc.py` & `google-cloud-appengine-admin-1.9.3/google/cloud/appengine_admin_v1/services/services/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-appengine-admin-1.9.2/google/cloud/appengine_admin_v1/services/services/transports/grpc_asyncio.py` & `google-cloud-appengine-admin-1.9.3/google/cloud/appengine_admin_v1/services/services/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-appengine-admin-1.9.2/google/cloud/appengine_admin_v1/services/services/transports/rest.py` & `google-cloud-appengine-admin-1.9.3/google/cloud/appengine_admin_v1/services/services/transports/rest.py`

 * *Files identical despite different names*

### Comparing `google-cloud-appengine-admin-1.9.2/google/cloud/appengine_admin_v1/services/versions/__init__.py` & `google-cloud-appengine-admin-1.9.3/google/cloud/appengine_admin_v1/services/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-appengine-admin-1.9.2/google/cloud/appengine_admin_v1/services/versions/async_client.py` & `google-cloud-appengine-admin-1.9.3/google/cloud/appengine_admin_v1/services/versions/async_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -698,15 +698,15 @@
             empty_pb2.Empty,
             metadata_type=ga_operation.OperationMetadataV1,
         )
 
         # Done; return the response.
         return response
 
-    async def __aenter__(self):
+    async def __aenter__(self) -> "VersionsAsyncClient":
         return self
 
     async def __aexit__(self, exc_type, exc, tb):
         await self.transport.close()
 
 
 DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
```

### Comparing `google-cloud-appengine-admin-1.9.2/google/cloud/appengine_admin_v1/services/versions/client.py` & `google-cloud-appengine-admin-1.9.3/google/cloud/appengine_admin_v1/services/versions/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-appengine-admin-1.9.2/google/cloud/appengine_admin_v1/services/versions/pagers.py` & `google-cloud-appengine-admin-1.9.3/google/cloud/appengine_admin_v1/services/versions/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-appengine-admin-1.9.2/google/cloud/appengine_admin_v1/services/versions/transports/__init__.py` & `google-cloud-appengine-admin-1.9.3/google/cloud/appengine_admin_v1/services/versions/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-appengine-admin-1.9.2/google/cloud/appengine_admin_v1/services/versions/transports/base.py` & `google-cloud-appengine-admin-1.9.3/google/cloud/appengine_admin_v1/services/versions/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-appengine-admin-1.9.2/google/cloud/appengine_admin_v1/services/versions/transports/grpc.py` & `google-cloud-appengine-admin-1.9.3/google/cloud/appengine_admin_v1/services/versions/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-appengine-admin-1.9.2/google/cloud/appengine_admin_v1/services/versions/transports/grpc_asyncio.py` & `google-cloud-appengine-admin-1.9.3/google/cloud/appengine_admin_v1/services/versions/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-appengine-admin-1.9.2/google/cloud/appengine_admin_v1/services/versions/transports/rest.py` & `google-cloud-appengine-admin-1.9.3/google/cloud/appengine_admin_v1/services/versions/transports/rest.py`

 * *Files identical despite different names*

### Comparing `google-cloud-appengine-admin-1.9.2/google/cloud/appengine_admin_v1/types/__init__.py` & `google-cloud-appengine-admin-1.9.3/google/cloud/appengine_admin_v1/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-appengine-admin-1.9.2/google/cloud/appengine_admin_v1/types/app_yaml.py` & `google-cloud-appengine-admin-1.9.3/google/cloud/appengine_admin_v1/types/app_yaml.py`

 * *Files identical despite different names*

### Comparing `google-cloud-appengine-admin-1.9.2/google/cloud/appengine_admin_v1/types/appengine.py` & `google-cloud-appengine-admin-1.9.3/google/cloud/appengine_admin_v1/types/appengine.py`

 * *Files identical despite different names*

### Comparing `google-cloud-appengine-admin-1.9.2/google/cloud/appengine_admin_v1/types/application.py` & `google-cloud-appengine-admin-1.9.3/google/cloud/appengine_admin_v1/types/application.py`

 * *Files identical despite different names*

### Comparing `google-cloud-appengine-admin-1.9.2/google/cloud/appengine_admin_v1/types/audit_data.py` & `google-cloud-appengine-admin-1.9.3/google/cloud/appengine_admin_v1/types/audit_data.py`

 * *Files identical despite different names*

### Comparing `google-cloud-appengine-admin-1.9.2/google/cloud/appengine_admin_v1/types/certificate.py` & `google-cloud-appengine-admin-1.9.3/google/cloud/appengine_admin_v1/types/certificate.py`

 * *Files identical despite different names*

### Comparing `google-cloud-appengine-admin-1.9.2/google/cloud/appengine_admin_v1/types/deploy.py` & `google-cloud-appengine-admin-1.9.3/google/cloud/appengine_admin_v1/types/deploy.py`

 * *Files identical despite different names*

### Comparing `google-cloud-appengine-admin-1.9.2/google/cloud/appengine_admin_v1/types/deployed_files.py` & `google-cloud-appengine-admin-1.9.3/google/cloud/appengine_admin_v1/types/deployed_files.py`

 * *Files identical despite different names*

### Comparing `google-cloud-appengine-admin-1.9.2/google/cloud/appengine_admin_v1/types/domain.py` & `google-cloud-appengine-admin-1.9.3/google/cloud/appengine_admin_v1/types/domain.py`

 * *Files identical despite different names*

### Comparing `google-cloud-appengine-admin-1.9.2/google/cloud/appengine_admin_v1/types/domain_mapping.py` & `google-cloud-appengine-admin-1.9.3/google/cloud/appengine_admin_v1/types/domain_mapping.py`

 * *Files identical despite different names*

### Comparing `google-cloud-appengine-admin-1.9.2/google/cloud/appengine_admin_v1/types/firewall.py` & `google-cloud-appengine-admin-1.9.3/google/cloud/appengine_admin_v1/types/firewall.py`

 * *Files identical despite different names*

### Comparing `google-cloud-appengine-admin-1.9.2/google/cloud/appengine_admin_v1/types/instance.py` & `google-cloud-appengine-admin-1.9.3/google/cloud/appengine_admin_v1/types/instance.py`

 * *Files identical despite different names*

### Comparing `google-cloud-appengine-admin-1.9.2/google/cloud/appengine_admin_v1/types/location.py` & `google-cloud-appengine-admin-1.9.3/google/cloud/appengine_admin_v1/types/location.py`

 * *Files identical despite different names*

### Comparing `google-cloud-appengine-admin-1.9.2/google/cloud/appengine_admin_v1/types/network_settings.py` & `google-cloud-appengine-admin-1.9.3/google/cloud/appengine_admin_v1/types/network_settings.py`

 * *Files identical despite different names*

### Comparing `google-cloud-appengine-admin-1.9.2/google/cloud/appengine_admin_v1/types/operation.py` & `google-cloud-appengine-admin-1.9.3/google/cloud/appengine_admin_v1/types/operation.py`

 * *Files identical despite different names*

### Comparing `google-cloud-appengine-admin-1.9.2/google/cloud/appengine_admin_v1/types/service.py` & `google-cloud-appengine-admin-1.9.3/google/cloud/appengine_admin_v1/types/service.py`

 * *Files identical despite different names*

### Comparing `google-cloud-appengine-admin-1.9.2/google/cloud/appengine_admin_v1/types/version.py` & `google-cloud-appengine-admin-1.9.3/google/cloud/appengine_admin_v1/types/version.py`

 * *Files identical despite different names*

### Comparing `google-cloud-appengine-admin-1.9.2/google_cloud_appengine_admin.egg-info/PKG-INFO` & `google-cloud-appengine-admin-1.9.3/google_cloud_appengine_admin.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-appengine-admin
-Version: 1.9.2
+Version: 1.9.3
 Summary: Google Cloud Appengine Admin API client library
 Home-page: https://github.com/googleapis/python-appengine-admin
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `google-cloud-appengine-admin-1.9.2/google_cloud_appengine_admin.egg-info/SOURCES.txt` & `google-cloud-appengine-admin-1.9.3/google_cloud_appengine_admin.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `google-cloud-appengine-admin-1.9.2/setup.py` & `google-cloud-appengine-admin-1.9.3/setup.py`

 * *Files identical despite different names*

### Comparing `google-cloud-appengine-admin-1.9.2/tests/__init__.py` & `google-cloud-appengine-admin-1.9.3/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-appengine-admin-1.9.2/tests/unit/__init__.py` & `google-cloud-appengine-admin-1.9.3/tests/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-appengine-admin-1.9.2/tests/unit/gapic/__init__.py` & `google-cloud-appengine-admin-1.9.3/tests/unit/gapic/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-appengine-admin-1.9.2/tests/unit/gapic/appengine_admin_v1/__init__.py` & `google-cloud-appengine-admin-1.9.3/tests/unit/gapic/appengine_admin_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-appengine-admin-1.9.2/tests/unit/gapic/appengine_admin_v1/test_applications.py` & `google-cloud-appengine-admin-1.9.3/tests/unit/gapic/appengine_admin_v1/test_applications.py`

 * *Files identical despite different names*

### Comparing `google-cloud-appengine-admin-1.9.2/tests/unit/gapic/appengine_admin_v1/test_authorized_certificates.py` & `google-cloud-appengine-admin-1.9.3/tests/unit/gapic/appengine_admin_v1/test_authorized_certificates.py`

 * *Files 0% similar despite different names*

```diff
@@ -1099,17 +1099,19 @@
                     certificate.AuthorizedCertificate(),
                     certificate.AuthorizedCertificate(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.list_authorized_certificates(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
```

### Comparing `google-cloud-appengine-admin-1.9.2/tests/unit/gapic/appengine_admin_v1/test_authorized_domains.py` & `google-cloud-appengine-admin-1.9.3/tests/unit/gapic/appengine_admin_v1/test_authorized_domains.py`

 * *Files 0% similar despite different names*

```diff
@@ -1080,17 +1080,19 @@
                     domain.AuthorizedDomain(),
                     domain.AuthorizedDomain(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.list_authorized_domains(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
```

### Comparing `google-cloud-appengine-admin-1.9.2/tests/unit/gapic/appengine_admin_v1/test_domain_mappings.py` & `google-cloud-appengine-admin-1.9.3/tests/unit/gapic/appengine_admin_v1/test_domain_mappings.py`

 * *Files 0% similar despite different names*

```diff
@@ -1063,17 +1063,19 @@
                     domain_mapping.DomainMapping(),
                     domain_mapping.DomainMapping(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.list_domain_mappings(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
```

### Comparing `google-cloud-appengine-admin-1.9.2/tests/unit/gapic/appengine_admin_v1/test_firewall.py` & `google-cloud-appengine-admin-1.9.3/tests/unit/gapic/appengine_admin_v1/test_firewall.py`

 * *Files 0% similar despite different names*

```diff
@@ -1016,17 +1016,19 @@
                     firewall.FirewallRule(),
                     firewall.FirewallRule(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.list_ingress_rules(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
```

### Comparing `google-cloud-appengine-admin-1.9.2/tests/unit/gapic/appengine_admin_v1/test_instances.py` & `google-cloud-appengine-admin-1.9.3/tests/unit/gapic/appengine_admin_v1/test_instances.py`

 * *Files 0% similar despite different names*

```diff
@@ -1018,17 +1018,19 @@
                     instance.Instance(),
                     instance.Instance(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.list_instances(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
```

### Comparing `google-cloud-appengine-admin-1.9.2/tests/unit/gapic/appengine_admin_v1/test_services.py` & `google-cloud-appengine-admin-1.9.3/tests/unit/gapic/appengine_admin_v1/test_services.py`

 * *Files 0% similar despite different names*

```diff
@@ -1011,17 +1011,19 @@
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
```

### Comparing `google-cloud-appengine-admin-1.9.2/tests/unit/gapic/appengine_admin_v1/test_versions.py` & `google-cloud-appengine-admin-1.9.3/tests/unit/gapic/appengine_admin_v1/test_versions.py`

 * *Files 1% similar despite different names*

```diff
@@ -1013,17 +1013,19 @@
                     version.Version(),
                     version.Version(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.list_versions(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
@@ -1061,17 +1063,14 @@
             created_by="created_by_value",
             disk_usage_bytes=1701,
             runtime_api_version="runtime_api_version_value",
             runtime_main_executable_path="runtime_main_executable_path_value",
             service_account="service_account_value",
             nobuild_files_regex="nobuild_files_regex_value",
             version_url="version_url_value",
-            automatic_scaling=version.AutomaticScaling(
-                cool_down_period=duration_pb2.Duration(seconds=751)
-            ),
         )
         response = client.get_version(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
         assert args[0] == appengine.GetVersionRequest()
@@ -1897,17 +1896,14 @@
             created_by="created_by_value",
             disk_usage_bytes=1701,
             runtime_api_version="runtime_api_version_value",
             runtime_main_executable_path="runtime_main_executable_path_value",
             service_account="service_account_value",
             nobuild_files_regex="nobuild_files_regex_value",
             version_url="version_url_value",
-            automatic_scaling=version.AutomaticScaling(
-                cool_down_period=duration_pb2.Duration(seconds=751)
-            ),
         )
 
         # Wrap the value into a proper Response obj
         response_value = Response()
         response_value.status_code = 200
         pb_return_value = version.Version.pb(return_value)
         json_return_value = json_format.MessageToJson(pb_return_value)
```

