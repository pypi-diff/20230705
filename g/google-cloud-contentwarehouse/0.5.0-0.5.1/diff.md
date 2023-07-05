# Comparing `tmp/google-cloud-contentwarehouse-0.5.0.tar.gz` & `tmp/google-cloud-contentwarehouse-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-cloud-contentwarehouse-0.5.0.tar", last modified: Wed Apr  5 20:24:21 2023, max compression
+gzip compressed data, was "google-cloud-contentwarehouse-0.5.1.tar", last modified: Wed Jul  5 15:51:41 2023, max compression
```

## Comparing `google-cloud-contentwarehouse-0.5.0.tar` & `google-cloud-contentwarehouse-0.5.1.tar`

### file list

```diff
@@ -1,114 +1,114 @@
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-05 20:24:21.025852 google-cloud-contentwarehouse-0.5.0/
--rw-rw-r--   0 root         (0)     1003    11358 2023-04-05 20:21:34.000000 google-cloud-contentwarehouse-0.5.0/LICENSE
--rw-rw-r--   0 root         (0)     1003      860 2023-04-05 20:21:34.000000 google-cloud-contentwarehouse-0.5.0/MANIFEST.in
--rw-r--r--   0 root         (0)     1003     4613 2023-04-05 20:24:21.025852 google-cloud-contentwarehouse-0.5.0/PKG-INFO
--rw-rw-r--   0 root         (0)     1003     3687 2023-04-05 20:21:34.000000 google-cloud-contentwarehouse-0.5.0/README.rst
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-05 20:24:21.001859 google-cloud-contentwarehouse-0.5.0/google/
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-05 20:24:21.001859 google-cloud-contentwarehouse-0.5.0/google/cloud/
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-05 20:24:21.005858 google-cloud-contentwarehouse-0.5.0/google/cloud/contentwarehouse/
--rw-rw-r--   0 root         (0)     1003     8283 2023-04-05 20:21:34.000000 google-cloud-contentwarehouse-0.5.0/google/cloud/contentwarehouse/__init__.py
--rw-rw-r--   0 root         (0)     1003      653 2023-04-05 20:21:34.000000 google-cloud-contentwarehouse-0.5.0/google/cloud/contentwarehouse/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       90 2023-04-05 20:21:34.000000 google-cloud-contentwarehouse-0.5.0/google/cloud/contentwarehouse/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-05 20:24:21.005858 google-cloud-contentwarehouse-0.5.0/google/cloud/contentwarehouse_v1/
--rw-rw-r--   0 root         (0)     1003     7162 2023-04-05 20:21:34.000000 google-cloud-contentwarehouse-0.5.0/google/cloud/contentwarehouse_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003    12557 2023-04-05 20:21:34.000000 google-cloud-contentwarehouse-0.5.0/google/cloud/contentwarehouse_v1/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003      653 2023-04-05 20:21:34.000000 google-cloud-contentwarehouse-0.5.0/google/cloud/contentwarehouse_v1/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       90 2023-04-05 20:21:34.000000 google-cloud-contentwarehouse-0.5.0/google/cloud/contentwarehouse_v1/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-05 20:24:21.005858 google-cloud-contentwarehouse-0.5.0/google/cloud/contentwarehouse_v1/services/
--rw-rw-r--   0 root         (0)     1003      600 2023-04-05 20:21:34.000000 google-cloud-contentwarehouse-0.5.0/google/cloud/contentwarehouse_v1/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-05 20:24:21.009857 google-cloud-contentwarehouse-0.5.0/google/cloud/contentwarehouse_v1/services/document_link_service/
--rw-rw-r--   0 root         (0)     1003      789 2023-04-05 20:21:34.000000 google-cloud-contentwarehouse-0.5.0/google/cloud/contentwarehouse_v1/services/document_link_service/__init__.py
--rw-rw-r--   0 root         (0)     1003    29813 2023-04-05 20:21:34.000000 google-cloud-contentwarehouse-0.5.0/google/cloud/contentwarehouse_v1/services/document_link_service/async_client.py
--rw-rw-r--   0 root         (0)     1003    40134 2023-04-05 20:21:34.000000 google-cloud-contentwarehouse-0.5.0/google/cloud/contentwarehouse_v1/services/document_link_service/client.py
--rw-rw-r--   0 root         (0)     1003     6138 2023-04-05 20:21:34.000000 google-cloud-contentwarehouse-0.5.0/google/cloud/contentwarehouse_v1/services/document_link_service/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-05 20:24:21.009857 google-cloud-contentwarehouse-0.5.0/google/cloud/contentwarehouse_v1/services/document_link_service/transports/
--rw-rw-r--   0 root         (0)     1003     1478 2023-04-05 20:21:34.000000 google-cloud-contentwarehouse-0.5.0/google/cloud/contentwarehouse_v1/services/document_link_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     8009 2023-04-05 20:21:34.000000 google-cloud-contentwarehouse-0.5.0/google/cloud/contentwarehouse_v1/services/document_link_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    16643 2023-04-05 20:21:34.000000 google-cloud-contentwarehouse-0.5.0/google/cloud/contentwarehouse_v1/services/document_link_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    16933 2023-04-05 20:21:34.000000 google-cloud-contentwarehouse-0.5.0/google/cloud/contentwarehouse_v1/services/document_link_service/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    32219 2023-04-05 20:21:34.000000 google-cloud-contentwarehouse-0.5.0/google/cloud/contentwarehouse_v1/services/document_link_service/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-05 20:24:21.009857 google-cloud-contentwarehouse-0.5.0/google/cloud/contentwarehouse_v1/services/document_schema_service/
--rw-rw-r--   0 root         (0)     1003      797 2023-04-05 20:21:34.000000 google-cloud-contentwarehouse-0.5.0/google/cloud/contentwarehouse_v1/services/document_schema_service/__init__.py
--rw-rw-r--   0 root         (0)     1003    35792 2023-04-05 20:21:34.000000 google-cloud-contentwarehouse-0.5.0/google/cloud/contentwarehouse_v1/services/document_schema_service/async_client.py
--rw-rw-r--   0 root         (0)     1003    45455 2023-04-05 20:21:34.000000 google-cloud-contentwarehouse-0.5.0/google/cloud/contentwarehouse_v1/services/document_schema_service/client.py
--rw-rw-r--   0 root         (0)     1003     6242 2023-04-05 20:21:34.000000 google-cloud-contentwarehouse-0.5.0/google/cloud/contentwarehouse_v1/services/document_schema_service/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-05 20:24:21.009857 google-cloud-contentwarehouse-0.5.0/google/cloud/contentwarehouse_v1/services/document_schema_service/transports/
--rw-rw-r--   0 root         (0)     1003     1519 2023-04-05 20:21:34.000000 google-cloud-contentwarehouse-0.5.0/google/cloud/contentwarehouse_v1/services/document_schema_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     9384 2023-04-05 20:21:34.000000 google-cloud-contentwarehouse-0.5.0/google/cloud/contentwarehouse_v1/services/document_schema_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    18582 2023-04-05 20:21:34.000000 google-cloud-contentwarehouse-0.5.0/google/cloud/contentwarehouse_v1/services/document_schema_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    18891 2023-04-05 20:21:34.000000 google-cloud-contentwarehouse-0.5.0/google/cloud/contentwarehouse_v1/services/document_schema_service/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    37177 2023-04-05 20:21:34.000000 google-cloud-contentwarehouse-0.5.0/google/cloud/contentwarehouse_v1/services/document_schema_service/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-05 20:24:21.013856 google-cloud-contentwarehouse-0.5.0/google/cloud/contentwarehouse_v1/services/document_service/
--rw-rw-r--   0 root         (0)     1003      773 2023-04-05 20:21:34.000000 google-cloud-contentwarehouse-0.5.0/google/cloud/contentwarehouse_v1/services/document_service/__init__.py
--rw-rw-r--   0 root         (0)     1003    50186 2023-04-05 20:21:34.000000 google-cloud-contentwarehouse-0.5.0/google/cloud/contentwarehouse_v1/services/document_service/async_client.py
--rw-rw-r--   0 root         (0)     1003    61015 2023-04-05 20:21:34.000000 google-cloud-contentwarehouse-0.5.0/google/cloud/contentwarehouse_v1/services/document_service/client.py
--rw-rw-r--   0 root         (0)     1003     6167 2023-04-05 20:21:34.000000 google-cloud-contentwarehouse-0.5.0/google/cloud/contentwarehouse_v1/services/document_service/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-05 20:24:21.013856 google-cloud-contentwarehouse-0.5.0/google/cloud/contentwarehouse_v1/services/document_service/transports/
--rw-rw-r--   0 root         (0)     1003     1414 2023-04-05 20:21:34.000000 google-cloud-contentwarehouse-0.5.0/google/cloud/contentwarehouse_v1/services/document_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003    10507 2023-04-05 20:21:34.000000 google-cloud-contentwarehouse-0.5.0/google/cloud/contentwarehouse_v1/services/document_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    21464 2023-04-05 20:21:34.000000 google-cloud-contentwarehouse-0.5.0/google/cloud/contentwarehouse_v1/services/document_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    21870 2023-04-05 20:21:34.000000 google-cloud-contentwarehouse-0.5.0/google/cloud/contentwarehouse_v1/services/document_service/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    53838 2023-04-05 20:21:34.000000 google-cloud-contentwarehouse-0.5.0/google/cloud/contentwarehouse_v1/services/document_service/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-05 20:24:21.013856 google-cloud-contentwarehouse-0.5.0/google/cloud/contentwarehouse_v1/services/rule_set_service/
--rw-rw-r--   0 root         (0)     1003      769 2023-04-05 20:21:34.000000 google-cloud-contentwarehouse-0.5.0/google/cloud/contentwarehouse_v1/services/rule_set_service/__init__.py
--rw-rw-r--   0 root         (0)     1003    33981 2023-04-05 20:21:34.000000 google-cloud-contentwarehouse-0.5.0/google/cloud/contentwarehouse_v1/services/rule_set_service/async_client.py
--rw-rw-r--   0 root         (0)     1003    44220 2023-04-05 20:21:34.000000 google-cloud-contentwarehouse-0.5.0/google/cloud/contentwarehouse_v1/services/rule_set_service/client.py
--rw-rw-r--   0 root         (0)     1003     5971 2023-04-05 20:21:34.000000 google-cloud-contentwarehouse-0.5.0/google/cloud/contentwarehouse_v1/services/rule_set_service/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-05 20:24:21.013856 google-cloud-contentwarehouse-0.5.0/google/cloud/contentwarehouse_v1/services/rule_set_service/transports/
--rw-rw-r--   0 root         (0)     1003     1400 2023-04-05 20:21:34.000000 google-cloud-contentwarehouse-0.5.0/google/cloud/contentwarehouse_v1/services/rule_set_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     8882 2023-04-05 20:21:34.000000 google-cloud-contentwarehouse-0.5.0/google/cloud/contentwarehouse_v1/services/rule_set_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    17339 2023-04-05 20:21:34.000000 google-cloud-contentwarehouse-0.5.0/google/cloud/contentwarehouse_v1/services/rule_set_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    17688 2023-04-05 20:21:34.000000 google-cloud-contentwarehouse-0.5.0/google/cloud/contentwarehouse_v1/services/rule_set_service/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    35361 2023-04-05 20:21:34.000000 google-cloud-contentwarehouse-0.5.0/google/cloud/contentwarehouse_v1/services/rule_set_service/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-05 20:24:21.017854 google-cloud-contentwarehouse-0.5.0/google/cloud/contentwarehouse_v1/services/synonym_set_service/
--rw-rw-r--   0 root         (0)     1003      781 2023-04-05 20:21:34.000000 google-cloud-contentwarehouse-0.5.0/google/cloud/contentwarehouse_v1/services/synonym_set_service/__init__.py
--rw-rw-r--   0 root         (0)     1003    35804 2023-04-05 20:21:34.000000 google-cloud-contentwarehouse-0.5.0/google/cloud/contentwarehouse_v1/services/synonym_set_service/async_client.py
--rw-rw-r--   0 root         (0)     1003    45498 2023-04-05 20:21:34.000000 google-cloud-contentwarehouse-0.5.0/google/cloud/contentwarehouse_v1/services/synonym_set_service/client.py
--rw-rw-r--   0 root         (0)     1003     6132 2023-04-05 20:21:34.000000 google-cloud-contentwarehouse-0.5.0/google/cloud/contentwarehouse_v1/services/synonym_set_service/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-05 20:24:21.017854 google-cloud-contentwarehouse-0.5.0/google/cloud/contentwarehouse_v1/services/synonym_set_service/transports/
--rw-rw-r--   0 root         (0)     1003     1442 2023-04-05 20:21:34.000000 google-cloud-contentwarehouse-0.5.0/google/cloud/contentwarehouse_v1/services/synonym_set_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     9005 2023-04-05 20:21:34.000000 google-cloud-contentwarehouse-0.5.0/google/cloud/contentwarehouse_v1/services/synonym_set_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    17951 2023-04-05 20:21:34.000000 google-cloud-contentwarehouse-0.5.0/google/cloud/contentwarehouse_v1/services/synonym_set_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    18274 2023-04-05 20:21:34.000000 google-cloud-contentwarehouse-0.5.0/google/cloud/contentwarehouse_v1/services/synonym_set_service/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    37468 2023-04-05 20:21:34.000000 google-cloud-contentwarehouse-0.5.0/google/cloud/contentwarehouse_v1/services/synonym_set_service/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-05 20:24:21.021853 google-cloud-contentwarehouse-0.5.0/google/cloud/contentwarehouse_v1/types/
--rw-rw-r--   0 root         (0)     1003     6097 2023-04-05 20:21:34.000000 google-cloud-contentwarehouse-0.5.0/google/cloud/contentwarehouse_v1/types/__init__.py
--rw-rw-r--   0 root         (0)     1003     1176 2023-04-05 20:21:34.000000 google-cloud-contentwarehouse-0.5.0/google/cloud/contentwarehouse_v1/types/async_document_service_request.py
--rw-rw-r--   0 root         (0)     1003     8758 2023-04-05 20:21:34.000000 google-cloud-contentwarehouse-0.5.0/google/cloud/contentwarehouse_v1/types/common.py
--rw-rw-r--   0 root         (0)     1003    21142 2023-04-05 20:21:34.000000 google-cloud-contentwarehouse-0.5.0/google/cloud/contentwarehouse_v1/types/document.py
--rw-rw-r--   0 root         (0)     1003    10012 2023-04-05 20:21:34.000000 google-cloud-contentwarehouse-0.5.0/google/cloud/contentwarehouse_v1/types/document_link_service.py
--rw-rw-r--   0 root         (0)     1003    12245 2023-04-05 20:21:34.000000 google-cloud-contentwarehouse-0.5.0/google/cloud/contentwarehouse_v1/types/document_schema.py
--rw-rw-r--   0 root         (0)     1003     5266 2023-04-05 20:21:34.000000 google-cloud-contentwarehouse-0.5.0/google/cloud/contentwarehouse_v1/types/document_schema_service.py
--rw-rw-r--   0 root         (0)     1003    11127 2023-04-05 20:21:34.000000 google-cloud-contentwarehouse-0.5.0/google/cloud/contentwarehouse_v1/types/document_service.py
--rw-rw-r--   0 root         (0)     1003    20277 2023-04-05 20:21:34.000000 google-cloud-contentwarehouse-0.5.0/google/cloud/contentwarehouse_v1/types/document_service_request.py
--rw-rw-r--   0 root         (0)     1003    15827 2023-04-05 20:21:34.000000 google-cloud-contentwarehouse-0.5.0/google/cloud/contentwarehouse_v1/types/filters.py
--rw-rw-r--   0 root         (0)     1003     5515 2023-04-05 20:21:34.000000 google-cloud-contentwarehouse-0.5.0/google/cloud/contentwarehouse_v1/types/histogram.py
--rw-rw-r--   0 root         (0)     1003    17339 2023-04-05 20:21:34.000000 google-cloud-contentwarehouse-0.5.0/google/cloud/contentwarehouse_v1/types/rule_engine.py
--rw-rw-r--   0 root         (0)     1003      775 2023-04-05 20:21:34.000000 google-cloud-contentwarehouse-0.5.0/google/cloud/contentwarehouse_v1/types/ruleset_service.py
--rw-rw-r--   0 root         (0)     1003     4980 2023-04-05 20:21:34.000000 google-cloud-contentwarehouse-0.5.0/google/cloud/contentwarehouse_v1/types/ruleset_service_request.py
--rw-rw-r--   0 root         (0)     1003     2501 2023-04-05 20:21:34.000000 google-cloud-contentwarehouse-0.5.0/google/cloud/contentwarehouse_v1/types/synonymset.py
--rw-rw-r--   0 root         (0)     1003      775 2023-04-05 20:21:34.000000 google-cloud-contentwarehouse-0.5.0/google/cloud/contentwarehouse_v1/types/synonymset_service.py
--rw-rw-r--   0 root         (0)     1003     5315 2023-04-05 20:21:34.000000 google-cloud-contentwarehouse-0.5.0/google/cloud/contentwarehouse_v1/types/synonymset_service_request.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-05 20:24:21.021853 google-cloud-contentwarehouse-0.5.0/google_cloud_contentwarehouse.egg-info/
--rw-r--r--   0 root         (0)     1003     4613 2023-04-05 20:24:20.000000 google-cloud-contentwarehouse-0.5.0/google_cloud_contentwarehouse.egg-info/PKG-INFO
--rw-r--r--   0 root         (0)     1003     5799 2023-04-05 20:24:20.000000 google-cloud-contentwarehouse-0.5.0/google_cloud_contentwarehouse.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0)     1003        1 2023-04-05 20:24:20.000000 google-cloud-contentwarehouse-0.5.0/google_cloud_contentwarehouse.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0)     1003       20 2023-04-05 20:24:20.000000 google-cloud-contentwarehouse-0.5.0/google_cloud_contentwarehouse.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0)     1003        1 2023-04-05 20:24:20.000000 google-cloud-contentwarehouse-0.5.0/google_cloud_contentwarehouse.egg-info/not-zip-safe
--rw-r--r--   0 root         (0)     1003      393 2023-04-05 20:24:20.000000 google-cloud-contentwarehouse-0.5.0/google_cloud_contentwarehouse.egg-info/requires.txt
--rw-r--r--   0 root         (0)     1003        7 2023-04-05 20:24:20.000000 google-cloud-contentwarehouse-0.5.0/google_cloud_contentwarehouse.egg-info/top_level.txt
--rw-r--r--   0 root         (0)     1003       38 2023-04-05 20:24:21.025852 google-cloud-contentwarehouse-0.5.0/setup.cfg
--rw-rw-r--   0 root         (0)     1003     3057 2023-04-05 20:21:34.000000 google-cloud-contentwarehouse-0.5.0/setup.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-05 20:24:21.021853 google-cloud-contentwarehouse-0.5.0/tests/
--rw-rw-r--   0 root         (0)     1003      600 2023-04-05 20:21:34.000000 google-cloud-contentwarehouse-0.5.0/tests/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-05 20:24:21.021853 google-cloud-contentwarehouse-0.5.0/tests/unit/
--rw-rw-r--   0 root         (0)     1003      600 2023-04-05 20:21:34.000000 google-cloud-contentwarehouse-0.5.0/tests/unit/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-05 20:24:21.021853 google-cloud-contentwarehouse-0.5.0/tests/unit/gapic/
--rw-rw-r--   0 root         (0)     1003      600 2023-04-05 20:21:34.000000 google-cloud-contentwarehouse-0.5.0/tests/unit/gapic/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-05 20:24:21.025852 google-cloud-contentwarehouse-0.5.0/tests/unit/gapic/contentwarehouse_v1/
--rw-rw-r--   0 root         (0)     1003      600 2023-04-05 20:21:34.000000 google-cloud-contentwarehouse-0.5.0/tests/unit/gapic/contentwarehouse_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003   149219 2023-04-05 20:21:34.000000 google-cloud-contentwarehouse-0.5.0/tests/unit/gapic/contentwarehouse_v1/test_document_link_service.py
--rw-rw-r--   0 root         (0)     1003   174250 2023-04-05 20:21:34.000000 google-cloud-contentwarehouse-0.5.0/tests/unit/gapic/contentwarehouse_v1/test_document_schema_service.py
--rw-rw-r--   0 root         (0)     1003   228794 2023-04-05 20:21:34.000000 google-cloud-contentwarehouse-0.5.0/tests/unit/gapic/contentwarehouse_v1/test_document_service.py
--rw-rw-r--   0 root         (0)     1003   168913 2023-04-05 20:21:34.000000 google-cloud-contentwarehouse-0.5.0/tests/unit/gapic/contentwarehouse_v1/test_rule_set_service.py
--rw-rw-r--   0 root         (0)     1003   165805 2023-04-05 20:21:34.000000 google-cloud-contentwarehouse-0.5.0/tests/unit/gapic/contentwarehouse_v1/test_synonym_set_service.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:51:41.200482 google-cloud-contentwarehouse-0.5.1/
+-rw-rw-r--   0 root         (0)     1003    11358 2023-07-05 15:46:58.000000 google-cloud-contentwarehouse-0.5.1/LICENSE
+-rw-rw-r--   0 root         (0)     1003      860 2023-07-05 15:46:58.000000 google-cloud-contentwarehouse-0.5.1/MANIFEST.in
+-rw-r--r--   0 root         (0)     1003     4613 2023-07-05 15:51:41.200482 google-cloud-contentwarehouse-0.5.1/PKG-INFO
+-rw-rw-r--   0 root         (0)     1003     3687 2023-07-05 15:46:58.000000 google-cloud-contentwarehouse-0.5.1/README.rst
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:51:41.180482 google-cloud-contentwarehouse-0.5.1/google/
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:51:41.180482 google-cloud-contentwarehouse-0.5.1/google/cloud/
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:51:41.180482 google-cloud-contentwarehouse-0.5.1/google/cloud/contentwarehouse/
+-rw-rw-r--   0 root         (0)     1003     8283 2023-07-05 15:46:58.000000 google-cloud-contentwarehouse-0.5.1/google/cloud/contentwarehouse/__init__.py
+-rw-rw-r--   0 root         (0)     1003      652 2023-07-05 15:46:58.000000 google-cloud-contentwarehouse-0.5.1/google/cloud/contentwarehouse/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       90 2023-07-05 15:46:58.000000 google-cloud-contentwarehouse-0.5.1/google/cloud/contentwarehouse/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:51:41.180482 google-cloud-contentwarehouse-0.5.1/google/cloud/contentwarehouse_v1/
+-rw-rw-r--   0 root         (0)     1003     7162 2023-07-05 15:46:58.000000 google-cloud-contentwarehouse-0.5.1/google/cloud/contentwarehouse_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003    12557 2023-07-05 15:46:58.000000 google-cloud-contentwarehouse-0.5.1/google/cloud/contentwarehouse_v1/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      652 2023-07-05 15:46:58.000000 google-cloud-contentwarehouse-0.5.1/google/cloud/contentwarehouse_v1/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       90 2023-07-05 15:46:58.000000 google-cloud-contentwarehouse-0.5.1/google/cloud/contentwarehouse_v1/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:51:41.184482 google-cloud-contentwarehouse-0.5.1/google/cloud/contentwarehouse_v1/services/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:58.000000 google-cloud-contentwarehouse-0.5.1/google/cloud/contentwarehouse_v1/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:51:41.184482 google-cloud-contentwarehouse-0.5.1/google/cloud/contentwarehouse_v1/services/document_link_service/
+-rw-rw-r--   0 root         (0)     1003      789 2023-07-05 15:46:58.000000 google-cloud-contentwarehouse-0.5.1/google/cloud/contentwarehouse_v1/services/document_link_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003    29849 2023-07-05 15:46:58.000000 google-cloud-contentwarehouse-0.5.1/google/cloud/contentwarehouse_v1/services/document_link_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003    40134 2023-07-05 15:46:58.000000 google-cloud-contentwarehouse-0.5.1/google/cloud/contentwarehouse_v1/services/document_link_service/client.py
+-rw-rw-r--   0 root         (0)     1003     6138 2023-07-05 15:46:58.000000 google-cloud-contentwarehouse-0.5.1/google/cloud/contentwarehouse_v1/services/document_link_service/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:51:41.184482 google-cloud-contentwarehouse-0.5.1/google/cloud/contentwarehouse_v1/services/document_link_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1478 2023-07-05 15:46:58.000000 google-cloud-contentwarehouse-0.5.1/google/cloud/contentwarehouse_v1/services/document_link_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     8009 2023-07-05 15:46:58.000000 google-cloud-contentwarehouse-0.5.1/google/cloud/contentwarehouse_v1/services/document_link_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    16643 2023-07-05 15:46:58.000000 google-cloud-contentwarehouse-0.5.1/google/cloud/contentwarehouse_v1/services/document_link_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    16933 2023-07-05 15:46:58.000000 google-cloud-contentwarehouse-0.5.1/google/cloud/contentwarehouse_v1/services/document_link_service/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    32219 2023-07-05 15:46:58.000000 google-cloud-contentwarehouse-0.5.1/google/cloud/contentwarehouse_v1/services/document_link_service/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:51:41.184482 google-cloud-contentwarehouse-0.5.1/google/cloud/contentwarehouse_v1/services/document_schema_service/
+-rw-rw-r--   0 root         (0)     1003      797 2023-07-05 15:46:58.000000 google-cloud-contentwarehouse-0.5.1/google/cloud/contentwarehouse_v1/services/document_schema_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003    35830 2023-07-05 15:46:58.000000 google-cloud-contentwarehouse-0.5.1/google/cloud/contentwarehouse_v1/services/document_schema_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003    45455 2023-07-05 15:46:58.000000 google-cloud-contentwarehouse-0.5.1/google/cloud/contentwarehouse_v1/services/document_schema_service/client.py
+-rw-rw-r--   0 root         (0)     1003     6242 2023-07-05 15:46:58.000000 google-cloud-contentwarehouse-0.5.1/google/cloud/contentwarehouse_v1/services/document_schema_service/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:51:41.184482 google-cloud-contentwarehouse-0.5.1/google/cloud/contentwarehouse_v1/services/document_schema_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1519 2023-07-05 15:46:58.000000 google-cloud-contentwarehouse-0.5.1/google/cloud/contentwarehouse_v1/services/document_schema_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     9384 2023-07-05 15:46:58.000000 google-cloud-contentwarehouse-0.5.1/google/cloud/contentwarehouse_v1/services/document_schema_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    18582 2023-07-05 15:46:58.000000 google-cloud-contentwarehouse-0.5.1/google/cloud/contentwarehouse_v1/services/document_schema_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    18891 2023-07-05 15:46:58.000000 google-cloud-contentwarehouse-0.5.1/google/cloud/contentwarehouse_v1/services/document_schema_service/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    37177 2023-07-05 15:46:58.000000 google-cloud-contentwarehouse-0.5.1/google/cloud/contentwarehouse_v1/services/document_schema_service/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:51:41.188482 google-cloud-contentwarehouse-0.5.1/google/cloud/contentwarehouse_v1/services/document_service/
+-rw-rw-r--   0 root         (0)     1003      773 2023-07-05 15:46:58.000000 google-cloud-contentwarehouse-0.5.1/google/cloud/contentwarehouse_v1/services/document_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003    50218 2023-07-05 15:46:58.000000 google-cloud-contentwarehouse-0.5.1/google/cloud/contentwarehouse_v1/services/document_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003    61015 2023-07-05 15:46:58.000000 google-cloud-contentwarehouse-0.5.1/google/cloud/contentwarehouse_v1/services/document_service/client.py
+-rw-rw-r--   0 root         (0)     1003     6167 2023-07-05 15:46:58.000000 google-cloud-contentwarehouse-0.5.1/google/cloud/contentwarehouse_v1/services/document_service/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:51:41.188482 google-cloud-contentwarehouse-0.5.1/google/cloud/contentwarehouse_v1/services/document_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1414 2023-07-05 15:46:58.000000 google-cloud-contentwarehouse-0.5.1/google/cloud/contentwarehouse_v1/services/document_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003    10507 2023-07-05 15:46:58.000000 google-cloud-contentwarehouse-0.5.1/google/cloud/contentwarehouse_v1/services/document_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    21464 2023-07-05 15:46:58.000000 google-cloud-contentwarehouse-0.5.1/google/cloud/contentwarehouse_v1/services/document_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    21870 2023-07-05 15:46:58.000000 google-cloud-contentwarehouse-0.5.1/google/cloud/contentwarehouse_v1/services/document_service/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    53838 2023-07-05 15:46:58.000000 google-cloud-contentwarehouse-0.5.1/google/cloud/contentwarehouse_v1/services/document_service/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:51:41.188482 google-cloud-contentwarehouse-0.5.1/google/cloud/contentwarehouse_v1/services/rule_set_service/
+-rw-rw-r--   0 root         (0)     1003      769 2023-07-05 15:46:58.000000 google-cloud-contentwarehouse-0.5.1/google/cloud/contentwarehouse_v1/services/rule_set_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003    34012 2023-07-05 15:46:58.000000 google-cloud-contentwarehouse-0.5.1/google/cloud/contentwarehouse_v1/services/rule_set_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003    44220 2023-07-05 15:46:58.000000 google-cloud-contentwarehouse-0.5.1/google/cloud/contentwarehouse_v1/services/rule_set_service/client.py
+-rw-rw-r--   0 root         (0)     1003     5971 2023-07-05 15:46:58.000000 google-cloud-contentwarehouse-0.5.1/google/cloud/contentwarehouse_v1/services/rule_set_service/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:51:41.188482 google-cloud-contentwarehouse-0.5.1/google/cloud/contentwarehouse_v1/services/rule_set_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1400 2023-07-05 15:46:58.000000 google-cloud-contentwarehouse-0.5.1/google/cloud/contentwarehouse_v1/services/rule_set_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     8882 2023-07-05 15:46:58.000000 google-cloud-contentwarehouse-0.5.1/google/cloud/contentwarehouse_v1/services/rule_set_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    17339 2023-07-05 15:46:58.000000 google-cloud-contentwarehouse-0.5.1/google/cloud/contentwarehouse_v1/services/rule_set_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    17688 2023-07-05 15:46:58.000000 google-cloud-contentwarehouse-0.5.1/google/cloud/contentwarehouse_v1/services/rule_set_service/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    35361 2023-07-05 15:46:58.000000 google-cloud-contentwarehouse-0.5.1/google/cloud/contentwarehouse_v1/services/rule_set_service/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:51:41.192482 google-cloud-contentwarehouse-0.5.1/google/cloud/contentwarehouse_v1/services/synonym_set_service/
+-rw-rw-r--   0 root         (0)     1003      781 2023-07-05 15:46:58.000000 google-cloud-contentwarehouse-0.5.1/google/cloud/contentwarehouse_v1/services/synonym_set_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003    35838 2023-07-05 15:46:58.000000 google-cloud-contentwarehouse-0.5.1/google/cloud/contentwarehouse_v1/services/synonym_set_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003    45498 2023-07-05 15:46:58.000000 google-cloud-contentwarehouse-0.5.1/google/cloud/contentwarehouse_v1/services/synonym_set_service/client.py
+-rw-rw-r--   0 root         (0)     1003     6132 2023-07-05 15:46:58.000000 google-cloud-contentwarehouse-0.5.1/google/cloud/contentwarehouse_v1/services/synonym_set_service/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:51:41.192482 google-cloud-contentwarehouse-0.5.1/google/cloud/contentwarehouse_v1/services/synonym_set_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1442 2023-07-05 15:46:58.000000 google-cloud-contentwarehouse-0.5.1/google/cloud/contentwarehouse_v1/services/synonym_set_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     9005 2023-07-05 15:46:58.000000 google-cloud-contentwarehouse-0.5.1/google/cloud/contentwarehouse_v1/services/synonym_set_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    17951 2023-07-05 15:46:58.000000 google-cloud-contentwarehouse-0.5.1/google/cloud/contentwarehouse_v1/services/synonym_set_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    18274 2023-07-05 15:46:58.000000 google-cloud-contentwarehouse-0.5.1/google/cloud/contentwarehouse_v1/services/synonym_set_service/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    37468 2023-07-05 15:46:58.000000 google-cloud-contentwarehouse-0.5.1/google/cloud/contentwarehouse_v1/services/synonym_set_service/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:51:41.196482 google-cloud-contentwarehouse-0.5.1/google/cloud/contentwarehouse_v1/types/
+-rw-rw-r--   0 root         (0)     1003     6097 2023-07-05 15:46:58.000000 google-cloud-contentwarehouse-0.5.1/google/cloud/contentwarehouse_v1/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003     1176 2023-07-05 15:46:58.000000 google-cloud-contentwarehouse-0.5.1/google/cloud/contentwarehouse_v1/types/async_document_service_request.py
+-rw-rw-r--   0 root         (0)     1003     8758 2023-07-05 15:46:58.000000 google-cloud-contentwarehouse-0.5.1/google/cloud/contentwarehouse_v1/types/common.py
+-rw-rw-r--   0 root         (0)     1003    21142 2023-07-05 15:46:58.000000 google-cloud-contentwarehouse-0.5.1/google/cloud/contentwarehouse_v1/types/document.py
+-rw-rw-r--   0 root         (0)     1003    10012 2023-07-05 15:46:58.000000 google-cloud-contentwarehouse-0.5.1/google/cloud/contentwarehouse_v1/types/document_link_service.py
+-rw-rw-r--   0 root         (0)     1003    12245 2023-07-05 15:46:58.000000 google-cloud-contentwarehouse-0.5.1/google/cloud/contentwarehouse_v1/types/document_schema.py
+-rw-rw-r--   0 root         (0)     1003     5266 2023-07-05 15:46:58.000000 google-cloud-contentwarehouse-0.5.1/google/cloud/contentwarehouse_v1/types/document_schema_service.py
+-rw-rw-r--   0 root         (0)     1003    11127 2023-07-05 15:46:58.000000 google-cloud-contentwarehouse-0.5.1/google/cloud/contentwarehouse_v1/types/document_service.py
+-rw-rw-r--   0 root         (0)     1003    20277 2023-07-05 15:46:58.000000 google-cloud-contentwarehouse-0.5.1/google/cloud/contentwarehouse_v1/types/document_service_request.py
+-rw-rw-r--   0 root         (0)     1003    15827 2023-07-05 15:46:58.000000 google-cloud-contentwarehouse-0.5.1/google/cloud/contentwarehouse_v1/types/filters.py
+-rw-rw-r--   0 root         (0)     1003     5515 2023-07-05 15:46:58.000000 google-cloud-contentwarehouse-0.5.1/google/cloud/contentwarehouse_v1/types/histogram.py
+-rw-rw-r--   0 root         (0)     1003    17339 2023-07-05 15:46:58.000000 google-cloud-contentwarehouse-0.5.1/google/cloud/contentwarehouse_v1/types/rule_engine.py
+-rw-rw-r--   0 root         (0)     1003      775 2023-07-05 15:46:58.000000 google-cloud-contentwarehouse-0.5.1/google/cloud/contentwarehouse_v1/types/ruleset_service.py
+-rw-rw-r--   0 root         (0)     1003     4980 2023-07-05 15:46:58.000000 google-cloud-contentwarehouse-0.5.1/google/cloud/contentwarehouse_v1/types/ruleset_service_request.py
+-rw-rw-r--   0 root         (0)     1003     2501 2023-07-05 15:46:58.000000 google-cloud-contentwarehouse-0.5.1/google/cloud/contentwarehouse_v1/types/synonymset.py
+-rw-rw-r--   0 root         (0)     1003      775 2023-07-05 15:46:58.000000 google-cloud-contentwarehouse-0.5.1/google/cloud/contentwarehouse_v1/types/synonymset_service.py
+-rw-rw-r--   0 root         (0)     1003     5315 2023-07-05 15:46:58.000000 google-cloud-contentwarehouse-0.5.1/google/cloud/contentwarehouse_v1/types/synonymset_service_request.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:51:41.196482 google-cloud-contentwarehouse-0.5.1/google_cloud_contentwarehouse.egg-info/
+-rw-r--r--   0 root         (0)     1003     4613 2023-07-05 15:51:41.000000 google-cloud-contentwarehouse-0.5.1/google_cloud_contentwarehouse.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0)     1003     5799 2023-07-05 15:51:41.000000 google-cloud-contentwarehouse-0.5.1/google_cloud_contentwarehouse.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-07-05 15:51:41.000000 google-cloud-contentwarehouse-0.5.1/google_cloud_contentwarehouse.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0)     1003       20 2023-07-05 15:51:41.000000 google-cloud-contentwarehouse-0.5.1/google_cloud_contentwarehouse.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-07-05 15:51:41.000000 google-cloud-contentwarehouse-0.5.1/google_cloud_contentwarehouse.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0)     1003      393 2023-07-05 15:51:41.000000 google-cloud-contentwarehouse-0.5.1/google_cloud_contentwarehouse.egg-info/requires.txt
+-rw-r--r--   0 root         (0)     1003        7 2023-07-05 15:51:41.000000 google-cloud-contentwarehouse-0.5.1/google_cloud_contentwarehouse.egg-info/top_level.txt
+-rw-r--r--   0 root         (0)     1003       38 2023-07-05 15:51:41.200482 google-cloud-contentwarehouse-0.5.1/setup.cfg
+-rw-rw-r--   0 root         (0)     1003     3057 2023-07-05 15:46:58.000000 google-cloud-contentwarehouse-0.5.1/setup.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:51:41.196482 google-cloud-contentwarehouse-0.5.1/tests/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:58.000000 google-cloud-contentwarehouse-0.5.1/tests/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:51:41.196482 google-cloud-contentwarehouse-0.5.1/tests/unit/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:58.000000 google-cloud-contentwarehouse-0.5.1/tests/unit/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:51:41.196482 google-cloud-contentwarehouse-0.5.1/tests/unit/gapic/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:58.000000 google-cloud-contentwarehouse-0.5.1/tests/unit/gapic/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:51:41.200482 google-cloud-contentwarehouse-0.5.1/tests/unit/gapic/contentwarehouse_v1/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:58.000000 google-cloud-contentwarehouse-0.5.1/tests/unit/gapic/contentwarehouse_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003   149418 2023-07-05 15:46:58.000000 google-cloud-contentwarehouse-0.5.1/tests/unit/gapic/contentwarehouse_v1/test_document_link_service.py
+-rw-rw-r--   0 root         (0)     1003   174449 2023-07-05 15:46:58.000000 google-cloud-contentwarehouse-0.5.1/tests/unit/gapic/contentwarehouse_v1/test_document_schema_service.py
+-rw-rw-r--   0 root         (0)     1003   228993 2023-07-05 15:46:58.000000 google-cloud-contentwarehouse-0.5.1/tests/unit/gapic/contentwarehouse_v1/test_document_service.py
+-rw-rw-r--   0 root         (0)     1003   169112 2023-07-05 15:46:58.000000 google-cloud-contentwarehouse-0.5.1/tests/unit/gapic/contentwarehouse_v1/test_rule_set_service.py
+-rw-rw-r--   0 root         (0)     1003   166004 2023-07-05 15:46:58.000000 google-cloud-contentwarehouse-0.5.1/tests/unit/gapic/contentwarehouse_v1/test_synonym_set_service.py
```

### Comparing `google-cloud-contentwarehouse-0.5.0/LICENSE` & `google-cloud-contentwarehouse-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `google-cloud-contentwarehouse-0.5.0/MANIFEST.in` & `google-cloud-contentwarehouse-0.5.1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `google-cloud-contentwarehouse-0.5.0/PKG-INFO` & `google-cloud-contentwarehouse-0.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-contentwarehouse
-Version: 0.5.0
+Version: 0.5.1
 Summary: Google Cloud Contentwarehouse API client library
 Home-page: https://github.com/googleapis/google-cloud-python
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 4 - Beta
```

### Comparing `google-cloud-contentwarehouse-0.5.0/README.rst` & `google-cloud-contentwarehouse-0.5.1/README.rst`

 * *Files identical despite different names*

### Comparing `google-cloud-contentwarehouse-0.5.0/google/cloud/contentwarehouse/__init__.py` & `google-cloud-contentwarehouse-0.5.1/google/cloud/contentwarehouse/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-contentwarehouse-0.5.0/google/cloud/contentwarehouse/gapic_version.py` & `google-cloud-contentwarehouse-0.5.1/google/cloud/contentwarehouse/gapic_version.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,9 +9,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-
-__version__ = "0.5.0"  # {x-release-please-version}
+__version__ = "0.5.1"  # {x-release-please-version}
```

### Comparing `google-cloud-contentwarehouse-0.5.0/google/cloud/contentwarehouse_v1/__init__.py` & `google-cloud-contentwarehouse-0.5.1/google/cloud/contentwarehouse_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-contentwarehouse-0.5.0/google/cloud/contentwarehouse_v1/gapic_metadata.json` & `google-cloud-contentwarehouse-0.5.1/google/cloud/contentwarehouse_v1/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-cloud-contentwarehouse-0.5.0/google/cloud/contentwarehouse_v1/gapic_version.py` & `google-cloud-contentwarehouse-0.5.1/google/cloud/contentwarehouse_v1/gapic_version.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,9 +9,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-
-__version__ = "0.5.0"  # {x-release-please-version}
+__version__ = "0.5.1"  # {x-release-please-version}
```

### Comparing `google-cloud-contentwarehouse-0.5.0/google/cloud/contentwarehouse_v1/services/__init__.py` & `google-cloud-contentwarehouse-0.5.1/google/cloud/contentwarehouse_v1/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-contentwarehouse-0.5.0/google/cloud/contentwarehouse_v1/services/document_link_service/__init__.py` & `google-cloud-contentwarehouse-0.5.1/google/cloud/contentwarehouse_v1/services/document_link_service/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-contentwarehouse-0.5.0/google/cloud/contentwarehouse_v1/services/document_link_service/async_client.py` & `google-cloud-contentwarehouse-0.5.1/google/cloud/contentwarehouse_v1/services/document_link_service/async_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -708,15 +708,15 @@
             timeout=timeout,
             metadata=metadata,
         )
 
         # Done; return the response.
         return response
 
-    async def __aenter__(self):
+    async def __aenter__(self) -> "DocumentLinkServiceAsyncClient":
         return self
 
     async def __aexit__(self, exc_type, exc, tb):
         await self.transport.close()
 
 
 DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
```

### Comparing `google-cloud-contentwarehouse-0.5.0/google/cloud/contentwarehouse_v1/services/document_link_service/client.py` & `google-cloud-contentwarehouse-0.5.1/google/cloud/contentwarehouse_v1/services/document_link_service/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-contentwarehouse-0.5.0/google/cloud/contentwarehouse_v1/services/document_link_service/pagers.py` & `google-cloud-contentwarehouse-0.5.1/google/cloud/contentwarehouse_v1/services/document_link_service/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-contentwarehouse-0.5.0/google/cloud/contentwarehouse_v1/services/document_link_service/transports/__init__.py` & `google-cloud-contentwarehouse-0.5.1/google/cloud/contentwarehouse_v1/services/document_link_service/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-contentwarehouse-0.5.0/google/cloud/contentwarehouse_v1/services/document_link_service/transports/base.py` & `google-cloud-contentwarehouse-0.5.1/google/cloud/contentwarehouse_v1/services/document_link_service/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-contentwarehouse-0.5.0/google/cloud/contentwarehouse_v1/services/document_link_service/transports/grpc.py` & `google-cloud-contentwarehouse-0.5.1/google/cloud/contentwarehouse_v1/services/document_link_service/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-contentwarehouse-0.5.0/google/cloud/contentwarehouse_v1/services/document_link_service/transports/grpc_asyncio.py` & `google-cloud-contentwarehouse-0.5.1/google/cloud/contentwarehouse_v1/services/document_link_service/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-contentwarehouse-0.5.0/google/cloud/contentwarehouse_v1/services/document_link_service/transports/rest.py` & `google-cloud-contentwarehouse-0.5.1/google/cloud/contentwarehouse_v1/services/document_link_service/transports/rest.py`

 * *Files identical despite different names*

### Comparing `google-cloud-contentwarehouse-0.5.0/google/cloud/contentwarehouse_v1/services/document_schema_service/__init__.py` & `google-cloud-contentwarehouse-0.5.1/google/cloud/contentwarehouse_v1/services/document_schema_service/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-contentwarehouse-0.5.0/google/cloud/contentwarehouse_v1/services/document_schema_service/async_client.py` & `google-cloud-contentwarehouse-0.5.1/google/cloud/contentwarehouse_v1/services/document_schema_service/async_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -856,15 +856,15 @@
             timeout=timeout,
             metadata=metadata,
         )
 
         # Done; return the response.
         return response
 
-    async def __aenter__(self):
+    async def __aenter__(self) -> "DocumentSchemaServiceAsyncClient":
         return self
 
     async def __aexit__(self, exc_type, exc, tb):
         await self.transport.close()
 
 
 DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
```

### Comparing `google-cloud-contentwarehouse-0.5.0/google/cloud/contentwarehouse_v1/services/document_schema_service/client.py` & `google-cloud-contentwarehouse-0.5.1/google/cloud/contentwarehouse_v1/services/document_schema_service/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-contentwarehouse-0.5.0/google/cloud/contentwarehouse_v1/services/document_schema_service/pagers.py` & `google-cloud-contentwarehouse-0.5.1/google/cloud/contentwarehouse_v1/services/document_schema_service/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-contentwarehouse-0.5.0/google/cloud/contentwarehouse_v1/services/document_schema_service/transports/__init__.py` & `google-cloud-contentwarehouse-0.5.1/google/cloud/contentwarehouse_v1/services/document_schema_service/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-contentwarehouse-0.5.0/google/cloud/contentwarehouse_v1/services/document_schema_service/transports/base.py` & `google-cloud-contentwarehouse-0.5.1/google/cloud/contentwarehouse_v1/services/document_schema_service/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-contentwarehouse-0.5.0/google/cloud/contentwarehouse_v1/services/document_schema_service/transports/grpc.py` & `google-cloud-contentwarehouse-0.5.1/google/cloud/contentwarehouse_v1/services/document_schema_service/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-contentwarehouse-0.5.0/google/cloud/contentwarehouse_v1/services/document_schema_service/transports/grpc_asyncio.py` & `google-cloud-contentwarehouse-0.5.1/google/cloud/contentwarehouse_v1/services/document_schema_service/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-contentwarehouse-0.5.0/google/cloud/contentwarehouse_v1/services/document_schema_service/transports/rest.py` & `google-cloud-contentwarehouse-0.5.1/google/cloud/contentwarehouse_v1/services/document_schema_service/transports/rest.py`

 * *Files identical despite different names*

### Comparing `google-cloud-contentwarehouse-0.5.0/google/cloud/contentwarehouse_v1/services/document_service/__init__.py` & `google-cloud-contentwarehouse-0.5.1/google/cloud/contentwarehouse_v1/services/document_service/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-contentwarehouse-0.5.0/google/cloud/contentwarehouse_v1/services/document_service/async_client.py` & `google-cloud-contentwarehouse-0.5.1/google/cloud/contentwarehouse_v1/services/document_service/async_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1211,15 +1211,15 @@
             timeout=timeout,
             metadata=metadata,
         )
 
         # Done; return the response.
         return response
 
-    async def __aenter__(self):
+    async def __aenter__(self) -> "DocumentServiceAsyncClient":
         return self
 
     async def __aexit__(self, exc_type, exc, tb):
         await self.transport.close()
 
 
 DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
```

### Comparing `google-cloud-contentwarehouse-0.5.0/google/cloud/contentwarehouse_v1/services/document_service/client.py` & `google-cloud-contentwarehouse-0.5.1/google/cloud/contentwarehouse_v1/services/document_service/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-contentwarehouse-0.5.0/google/cloud/contentwarehouse_v1/services/document_service/pagers.py` & `google-cloud-contentwarehouse-0.5.1/google/cloud/contentwarehouse_v1/services/document_service/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-contentwarehouse-0.5.0/google/cloud/contentwarehouse_v1/services/document_service/transports/__init__.py` & `google-cloud-contentwarehouse-0.5.1/google/cloud/contentwarehouse_v1/services/document_service/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-contentwarehouse-0.5.0/google/cloud/contentwarehouse_v1/services/document_service/transports/base.py` & `google-cloud-contentwarehouse-0.5.1/google/cloud/contentwarehouse_v1/services/document_service/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-contentwarehouse-0.5.0/google/cloud/contentwarehouse_v1/services/document_service/transports/grpc.py` & `google-cloud-contentwarehouse-0.5.1/google/cloud/contentwarehouse_v1/services/document_service/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-contentwarehouse-0.5.0/google/cloud/contentwarehouse_v1/services/document_service/transports/grpc_asyncio.py` & `google-cloud-contentwarehouse-0.5.1/google/cloud/contentwarehouse_v1/services/document_service/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-contentwarehouse-0.5.0/google/cloud/contentwarehouse_v1/services/document_service/transports/rest.py` & `google-cloud-contentwarehouse-0.5.1/google/cloud/contentwarehouse_v1/services/document_service/transports/rest.py`

 * *Files identical despite different names*

### Comparing `google-cloud-contentwarehouse-0.5.0/google/cloud/contentwarehouse_v1/services/rule_set_service/__init__.py` & `google-cloud-contentwarehouse-0.5.1/google/cloud/contentwarehouse_v1/services/rule_set_service/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-contentwarehouse-0.5.0/google/cloud/contentwarehouse_v1/services/rule_set_service/async_client.py` & `google-cloud-contentwarehouse-0.5.1/google/cloud/contentwarehouse_v1/services/rule_set_service/async_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -828,15 +828,15 @@
             timeout=timeout,
             metadata=metadata,
         )
 
         # Done; return the response.
         return response
 
-    async def __aenter__(self):
+    async def __aenter__(self) -> "RuleSetServiceAsyncClient":
         return self
 
     async def __aexit__(self, exc_type, exc, tb):
         await self.transport.close()
 
 
 DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
```

### Comparing `google-cloud-contentwarehouse-0.5.0/google/cloud/contentwarehouse_v1/services/rule_set_service/client.py` & `google-cloud-contentwarehouse-0.5.1/google/cloud/contentwarehouse_v1/services/rule_set_service/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-contentwarehouse-0.5.0/google/cloud/contentwarehouse_v1/services/rule_set_service/pagers.py` & `google-cloud-contentwarehouse-0.5.1/google/cloud/contentwarehouse_v1/services/rule_set_service/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-contentwarehouse-0.5.0/google/cloud/contentwarehouse_v1/services/rule_set_service/transports/__init__.py` & `google-cloud-contentwarehouse-0.5.1/google/cloud/contentwarehouse_v1/services/rule_set_service/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-contentwarehouse-0.5.0/google/cloud/contentwarehouse_v1/services/rule_set_service/transports/base.py` & `google-cloud-contentwarehouse-0.5.1/google/cloud/contentwarehouse_v1/services/rule_set_service/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-contentwarehouse-0.5.0/google/cloud/contentwarehouse_v1/services/rule_set_service/transports/grpc.py` & `google-cloud-contentwarehouse-0.5.1/google/cloud/contentwarehouse_v1/services/rule_set_service/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-contentwarehouse-0.5.0/google/cloud/contentwarehouse_v1/services/rule_set_service/transports/grpc_asyncio.py` & `google-cloud-contentwarehouse-0.5.1/google/cloud/contentwarehouse_v1/services/rule_set_service/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-contentwarehouse-0.5.0/google/cloud/contentwarehouse_v1/services/rule_set_service/transports/rest.py` & `google-cloud-contentwarehouse-0.5.1/google/cloud/contentwarehouse_v1/services/rule_set_service/transports/rest.py`

 * *Files identical despite different names*

### Comparing `google-cloud-contentwarehouse-0.5.0/google/cloud/contentwarehouse_v1/services/synonym_set_service/__init__.py` & `google-cloud-contentwarehouse-0.5.1/google/cloud/contentwarehouse_v1/services/synonym_set_service/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-contentwarehouse-0.5.0/google/cloud/contentwarehouse_v1/services/synonym_set_service/async_client.py` & `google-cloud-contentwarehouse-0.5.1/google/cloud/contentwarehouse_v1/services/synonym_set_service/async_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -863,15 +863,15 @@
             timeout=timeout,
             metadata=metadata,
         )
 
         # Done; return the response.
         return response
 
-    async def __aenter__(self):
+    async def __aenter__(self) -> "SynonymSetServiceAsyncClient":
         return self
 
     async def __aexit__(self, exc_type, exc, tb):
         await self.transport.close()
 
 
 DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
```

### Comparing `google-cloud-contentwarehouse-0.5.0/google/cloud/contentwarehouse_v1/services/synonym_set_service/client.py` & `google-cloud-contentwarehouse-0.5.1/google/cloud/contentwarehouse_v1/services/synonym_set_service/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-contentwarehouse-0.5.0/google/cloud/contentwarehouse_v1/services/synonym_set_service/pagers.py` & `google-cloud-contentwarehouse-0.5.1/google/cloud/contentwarehouse_v1/services/synonym_set_service/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-contentwarehouse-0.5.0/google/cloud/contentwarehouse_v1/services/synonym_set_service/transports/__init__.py` & `google-cloud-contentwarehouse-0.5.1/google/cloud/contentwarehouse_v1/services/synonym_set_service/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-contentwarehouse-0.5.0/google/cloud/contentwarehouse_v1/services/synonym_set_service/transports/base.py` & `google-cloud-contentwarehouse-0.5.1/google/cloud/contentwarehouse_v1/services/synonym_set_service/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-contentwarehouse-0.5.0/google/cloud/contentwarehouse_v1/services/synonym_set_service/transports/grpc.py` & `google-cloud-contentwarehouse-0.5.1/google/cloud/contentwarehouse_v1/services/synonym_set_service/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-contentwarehouse-0.5.0/google/cloud/contentwarehouse_v1/services/synonym_set_service/transports/grpc_asyncio.py` & `google-cloud-contentwarehouse-0.5.1/google/cloud/contentwarehouse_v1/services/synonym_set_service/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-contentwarehouse-0.5.0/google/cloud/contentwarehouse_v1/services/synonym_set_service/transports/rest.py` & `google-cloud-contentwarehouse-0.5.1/google/cloud/contentwarehouse_v1/services/synonym_set_service/transports/rest.py`

 * *Files identical despite different names*

### Comparing `google-cloud-contentwarehouse-0.5.0/google/cloud/contentwarehouse_v1/types/__init__.py` & `google-cloud-contentwarehouse-0.5.1/google/cloud/contentwarehouse_v1/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-contentwarehouse-0.5.0/google/cloud/contentwarehouse_v1/types/async_document_service_request.py` & `google-cloud-contentwarehouse-0.5.1/google/cloud/contentwarehouse_v1/types/async_document_service_request.py`

 * *Files identical despite different names*

### Comparing `google-cloud-contentwarehouse-0.5.0/google/cloud/contentwarehouse_v1/types/common.py` & `google-cloud-contentwarehouse-0.5.1/google/cloud/contentwarehouse_v1/types/common.py`

 * *Files identical despite different names*

### Comparing `google-cloud-contentwarehouse-0.5.0/google/cloud/contentwarehouse_v1/types/document.py` & `google-cloud-contentwarehouse-0.5.1/google/cloud/contentwarehouse_v1/types/document.py`

 * *Files identical despite different names*

### Comparing `google-cloud-contentwarehouse-0.5.0/google/cloud/contentwarehouse_v1/types/document_link_service.py` & `google-cloud-contentwarehouse-0.5.1/google/cloud/contentwarehouse_v1/types/document_link_service.py`

 * *Files identical despite different names*

### Comparing `google-cloud-contentwarehouse-0.5.0/google/cloud/contentwarehouse_v1/types/document_schema.py` & `google-cloud-contentwarehouse-0.5.1/google/cloud/contentwarehouse_v1/types/document_schema.py`

 * *Files identical despite different names*

### Comparing `google-cloud-contentwarehouse-0.5.0/google/cloud/contentwarehouse_v1/types/document_schema_service.py` & `google-cloud-contentwarehouse-0.5.1/google/cloud/contentwarehouse_v1/types/document_schema_service.py`

 * *Files identical despite different names*

### Comparing `google-cloud-contentwarehouse-0.5.0/google/cloud/contentwarehouse_v1/types/document_service.py` & `google-cloud-contentwarehouse-0.5.1/google/cloud/contentwarehouse_v1/types/document_service.py`

 * *Files identical despite different names*

### Comparing `google-cloud-contentwarehouse-0.5.0/google/cloud/contentwarehouse_v1/types/document_service_request.py` & `google-cloud-contentwarehouse-0.5.1/google/cloud/contentwarehouse_v1/types/document_service_request.py`

 * *Files identical despite different names*

### Comparing `google-cloud-contentwarehouse-0.5.0/google/cloud/contentwarehouse_v1/types/filters.py` & `google-cloud-contentwarehouse-0.5.1/google/cloud/contentwarehouse_v1/types/filters.py`

 * *Files identical despite different names*

### Comparing `google-cloud-contentwarehouse-0.5.0/google/cloud/contentwarehouse_v1/types/histogram.py` & `google-cloud-contentwarehouse-0.5.1/google/cloud/contentwarehouse_v1/types/histogram.py`

 * *Files identical despite different names*

### Comparing `google-cloud-contentwarehouse-0.5.0/google/cloud/contentwarehouse_v1/types/rule_engine.py` & `google-cloud-contentwarehouse-0.5.1/google/cloud/contentwarehouse_v1/types/rule_engine.py`

 * *Files identical despite different names*

### Comparing `google-cloud-contentwarehouse-0.5.0/google/cloud/contentwarehouse_v1/types/ruleset_service.py` & `google-cloud-contentwarehouse-0.5.1/google/cloud/contentwarehouse_v1/types/ruleset_service.py`

 * *Files identical despite different names*

### Comparing `google-cloud-contentwarehouse-0.5.0/google/cloud/contentwarehouse_v1/types/ruleset_service_request.py` & `google-cloud-contentwarehouse-0.5.1/google/cloud/contentwarehouse_v1/types/ruleset_service_request.py`

 * *Files identical despite different names*

### Comparing `google-cloud-contentwarehouse-0.5.0/google/cloud/contentwarehouse_v1/types/synonymset.py` & `google-cloud-contentwarehouse-0.5.1/google/cloud/contentwarehouse_v1/types/synonymset.py`

 * *Files identical despite different names*

### Comparing `google-cloud-contentwarehouse-0.5.0/google/cloud/contentwarehouse_v1/types/synonymset_service.py` & `google-cloud-contentwarehouse-0.5.1/google/cloud/contentwarehouse_v1/types/synonymset_service.py`

 * *Files identical despite different names*

### Comparing `google-cloud-contentwarehouse-0.5.0/google/cloud/contentwarehouse_v1/types/synonymset_service_request.py` & `google-cloud-contentwarehouse-0.5.1/google/cloud/contentwarehouse_v1/types/synonymset_service_request.py`

 * *Files identical despite different names*

### Comparing `google-cloud-contentwarehouse-0.5.0/google_cloud_contentwarehouse.egg-info/PKG-INFO` & `google-cloud-contentwarehouse-0.5.1/google_cloud_contentwarehouse.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-contentwarehouse
-Version: 0.5.0
+Version: 0.5.1
 Summary: Google Cloud Contentwarehouse API client library
 Home-page: https://github.com/googleapis/google-cloud-python
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 4 - Beta
```

### Comparing `google-cloud-contentwarehouse-0.5.0/google_cloud_contentwarehouse.egg-info/SOURCES.txt` & `google-cloud-contentwarehouse-0.5.1/google_cloud_contentwarehouse.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `google-cloud-contentwarehouse-0.5.0/setup.py` & `google-cloud-contentwarehouse-0.5.1/setup.py`

 * *Files identical despite different names*

### Comparing `google-cloud-contentwarehouse-0.5.0/tests/__init__.py` & `google-cloud-contentwarehouse-0.5.1/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-contentwarehouse-0.5.0/tests/unit/__init__.py` & `google-cloud-contentwarehouse-0.5.1/tests/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-contentwarehouse-0.5.0/tests/unit/gapic/__init__.py` & `google-cloud-contentwarehouse-0.5.1/tests/unit/gapic/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-contentwarehouse-0.5.0/tests/unit/gapic/contentwarehouse_v1/__init__.py` & `google-cloud-contentwarehouse-0.5.1/tests/unit/gapic/contentwarehouse_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-contentwarehouse-0.5.0/tests/unit/gapic/contentwarehouse_v1/test_document_link_service.py` & `google-cloud-contentwarehouse-0.5.1/tests/unit/gapic/contentwarehouse_v1/test_document_link_service.py`

 * *Files 0% similar despite different names*

```diff
@@ -1433,17 +1433,19 @@
                     document_link_service.DocumentLink(),
                     document_link_service.DocumentLink(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.list_linked_sources(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
```

### Comparing `google-cloud-contentwarehouse-0.5.0/tests/unit/gapic/contentwarehouse_v1/test_document_schema_service.py` & `google-cloud-contentwarehouse-0.5.1/tests/unit/gapic/contentwarehouse_v1/test_document_schema_service.py`

 * *Files 0% similar despite different names*

```diff
@@ -2217,17 +2217,19 @@
                     document_schema.DocumentSchema(),
                     document_schema.DocumentSchema(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.list_document_schemas(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
```

### Comparing `google-cloud-contentwarehouse-0.5.0/tests/unit/gapic/contentwarehouse_v1/test_document_service.py` & `google-cloud-contentwarehouse-0.5.1/tests/unit/gapic/contentwarehouse_v1/test_document_service.py`

 * *Files 0% similar despite different names*

```diff
@@ -2163,17 +2163,19 @@
                     document_service.SearchDocumentsResponse.MatchingDocument(),
                     document_service.SearchDocumentsResponse.MatchingDocument(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.search_documents(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
```

### Comparing `google-cloud-contentwarehouse-0.5.0/tests/unit/gapic/contentwarehouse_v1/test_rule_set_service.py` & `google-cloud-contentwarehouse-0.5.1/tests/unit/gapic/contentwarehouse_v1/test_rule_set_service.py`

 * *Files 0% similar despite different names*

```diff
@@ -2070,17 +2070,19 @@
                     rule_engine.RuleSet(),
                     rule_engine.RuleSet(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.list_rule_sets(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
```

### Comparing `google-cloud-contentwarehouse-0.5.0/tests/unit/gapic/contentwarehouse_v1/test_synonym_set_service.py` & `google-cloud-contentwarehouse-0.5.1/tests/unit/gapic/contentwarehouse_v1/test_synonym_set_service.py`

 * *Files 0% similar despite different names*

```diff
@@ -2161,17 +2161,19 @@
                     synonymset.SynonymSet(),
                     synonymset.SynonymSet(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.list_synonym_sets(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
```

