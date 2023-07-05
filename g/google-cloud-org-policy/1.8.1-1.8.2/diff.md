# Comparing `tmp/google-cloud-org-policy-1.8.1.tar.gz` & `tmp/google-cloud-org-policy-1.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-cloud-org-policy-1.8.1.tar", last modified: Mon Mar 27 14:54:04 2023, max compression
+gzip compressed data, was "google-cloud-org-policy-1.8.2.tar", last modified: Wed Jul  5 15:21:42 2023, max compression
```

## Comparing `google-cloud-org-policy-1.8.1.tar` & `google-cloud-org-policy-1.8.2.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:54:04.603484 google-cloud-org-policy-1.8.1/
--rw-rw-r--   0 root         (0)     1003    11358 2023-03-27 14:51:26.000000 google-cloud-org-policy-1.8.1/LICENSE
--rw-rw-r--   0 root         (0)     1003      860 2023-03-27 14:51:26.000000 google-cloud-org-policy-1.8.1/MANIFEST.in
--rw-r--r--   0 root         (0)     1003     4836 2023-03-27 14:54:04.603484 google-cloud-org-policy-1.8.1/PKG-INFO
--rw-rw-r--   0 root         (0)     1003     3911 2023-03-27 14:51:26.000000 google-cloud-org-policy-1.8.1/README.rst
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:54:04.599482 google-cloud-org-policy-1.8.1/google/
--rw-rw-r--   0 root         (0)     1003      774 2023-03-27 14:51:26.000000 google-cloud-org-policy-1.8.1/google/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:54:04.599482 google-cloud-org-policy-1.8.1/google/cloud/
--rw-rw-r--   0 root         (0)     1003      774 2023-03-27 14:51:26.000000 google-cloud-org-policy-1.8.1/google/cloud/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:54:04.599482 google-cloud-org-policy-1.8.1/google/cloud/orgpolicy/
--rw-rw-r--   0 root         (0)     1003     2236 2023-03-27 14:51:26.000000 google-cloud-org-policy-1.8.1/google/cloud/orgpolicy/__init__.py
--rw-rw-r--   0 root         (0)     1003      652 2023-03-27 14:51:26.000000 google-cloud-org-policy-1.8.1/google/cloud/orgpolicy/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       84 2023-03-27 14:51:26.000000 google-cloud-org-policy-1.8.1/google/cloud/orgpolicy/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:54:04.599482 google-cloud-org-policy-1.8.1/google/cloud/orgpolicy/v1/
--rw-rw-r--   0 root         (0)     1003      919 2023-03-27 14:51:26.000000 google-cloud-org-policy-1.8.1/google/cloud/orgpolicy/v1/__init__.py
--rw-rw-r--   0 root         (0)     1003    14416 2023-03-27 14:51:26.000000 google-cloud-org-policy-1.8.1/google/cloud/orgpolicy/v1/orgpolicy.proto
--rw-rw-r--   0 root         (0)     1003     5783 2023-03-27 14:51:26.000000 google-cloud-org-policy-1.8.1/google/cloud/orgpolicy/v1/orgpolicy_pb2.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:54:04.599482 google-cloud-org-policy-1.8.1/google/cloud/orgpolicy_v2/
--rw-rw-r--   0 root         (0)     1003     1835 2023-03-27 14:51:26.000000 google-cloud-org-policy-1.8.1/google/cloud/orgpolicy_v2/__init__.py
--rw-rw-r--   0 root         (0)     1003     3199 2023-03-27 14:51:26.000000 google-cloud-org-policy-1.8.1/google/cloud/orgpolicy_v2/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003      652 2023-03-27 14:51:26.000000 google-cloud-org-policy-1.8.1/google/cloud/orgpolicy_v2/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       84 2023-03-27 14:51:26.000000 google-cloud-org-policy-1.8.1/google/cloud/orgpolicy_v2/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:54:04.599482 google-cloud-org-policy-1.8.1/google/cloud/orgpolicy_v2/services/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 14:51:26.000000 google-cloud-org-policy-1.8.1/google/cloud/orgpolicy_v2/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:54:04.599482 google-cloud-org-policy-1.8.1/google/cloud/orgpolicy_v2/services/org_policy/
--rw-rw-r--   0 root         (0)     1003      749 2023-03-27 14:51:26.000000 google-cloud-org-policy-1.8.1/google/cloud/orgpolicy_v2/services/org_policy/__init__.py
--rw-rw-r--   0 root         (0)     1003    44686 2023-03-27 14:51:26.000000 google-cloud-org-policy-1.8.1/google/cloud/orgpolicy_v2/services/org_policy/async_client.py
--rw-rw-r--   0 root         (0)     1003    52631 2023-03-27 14:51:26.000000 google-cloud-org-policy-1.8.1/google/cloud/orgpolicy_v2/services/org_policy/client.py
--rw-rw-r--   0 root         (0)     1003    10791 2023-03-27 14:51:26.000000 google-cloud-org-policy-1.8.1/google/cloud/orgpolicy_v2/services/org_policy/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:54:04.599482 google-cloud-org-policy-1.8.1/google/cloud/orgpolicy_v2/services/org_policy/transports/
--rw-rw-r--   0 root         (0)     1003     1348 2023-03-27 14:51:26.000000 google-cloud-org-policy-1.8.1/google/cloud/orgpolicy_v2/services/org_policy/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003    11416 2023-03-27 14:51:26.000000 google-cloud-org-policy-1.8.1/google/cloud/orgpolicy_v2/services/org_policy/transports/base.py
--rw-rw-r--   0 root         (0)     1003    20621 2023-03-27 14:51:26.000000 google-cloud-org-policy-1.8.1/google/cloud/orgpolicy_v2/services/org_policy/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    20982 2023-03-27 14:51:26.000000 google-cloud-org-policy-1.8.1/google/cloud/orgpolicy_v2/services/org_policy/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    45192 2023-03-27 14:51:26.000000 google-cloud-org-policy-1.8.1/google/cloud/orgpolicy_v2/services/org_policy/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:54:04.599482 google-cloud-org-policy-1.8.1/google/cloud/orgpolicy_v2/types/
--rw-rw-r--   0 root         (0)     1003     1306 2023-03-27 14:51:26.000000 google-cloud-org-policy-1.8.1/google/cloud/orgpolicy_v2/types/__init__.py
--rw-rw-r--   0 root         (0)     1003     6656 2023-03-27 14:51:26.000000 google-cloud-org-policy-1.8.1/google/cloud/orgpolicy_v2/types/constraint.py
--rw-rw-r--   0 root         (0)     1003    18977 2023-03-27 14:51:26.000000 google-cloud-org-policy-1.8.1/google/cloud/orgpolicy_v2/types/orgpolicy.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:54:04.603484 google-cloud-org-policy-1.8.1/google_cloud_org_policy.egg-info/
--rw-r--r--   0 root         (0)     1003     4836 2023-03-27 14:54:04.000000 google-cloud-org-policy-1.8.1/google_cloud_org_policy.egg-info/PKG-INFO
--rw-r--r--   0 root         (0)     1003     1733 2023-03-27 14:54:04.000000 google-cloud-org-policy-1.8.1/google_cloud_org_policy.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0)     1003        1 2023-03-27 14:54:04.000000 google-cloud-org-policy-1.8.1/google_cloud_org_policy.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0)     1003       20 2023-03-27 14:54:04.000000 google-cloud-org-policy-1.8.1/google_cloud_org_policy.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0)     1003        1 2023-03-27 14:54:04.000000 google-cloud-org-policy-1.8.1/google_cloud_org_policy.egg-info/not-zip-safe
--rw-r--r--   0 root         (0)     1003      315 2023-03-27 14:54:04.000000 google-cloud-org-policy-1.8.1/google_cloud_org_policy.egg-info/requires.txt
--rw-r--r--   0 root         (0)     1003        7 2023-03-27 14:54:04.000000 google-cloud-org-policy-1.8.1/google_cloud_org_policy.egg-info/top_level.txt
--rw-rw-r--   0 root         (0)     1003       67 2023-03-27 14:54:04.603484 google-cloud-org-policy-1.8.1/setup.cfg
--rw-rw-r--   0 root         (0)     1003     2932 2023-03-27 14:51:26.000000 google-cloud-org-policy-1.8.1/setup.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:54:04.603484 google-cloud-org-policy-1.8.1/tests/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 14:51:26.000000 google-cloud-org-policy-1.8.1/tests/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:54:04.603484 google-cloud-org-policy-1.8.1/tests/unit/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 14:51:26.000000 google-cloud-org-policy-1.8.1/tests/unit/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:54:04.603484 google-cloud-org-policy-1.8.1/tests/unit/gapic/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 14:51:26.000000 google-cloud-org-policy-1.8.1/tests/unit/gapic/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:54:04.603484 google-cloud-org-policy-1.8.1/tests/unit/gapic/orgpolicy_v2/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 14:51:26.000000 google-cloud-org-policy-1.8.1/tests/unit/gapic/orgpolicy_v2/__init__.py
--rw-rw-r--   0 root         (0)     1003   197124 2023-03-27 14:51:26.000000 google-cloud-org-policy-1.8.1/tests/unit/gapic/orgpolicy_v2/test_org_policy.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:21:42.625350 google-cloud-org-policy-1.8.2/
+-rw-rw-r--   0 root         (0)     1003    11358 2023-07-05 15:19:18.000000 google-cloud-org-policy-1.8.2/LICENSE
+-rw-rw-r--   0 root         (0)     1003      860 2023-07-05 15:19:18.000000 google-cloud-org-policy-1.8.2/MANIFEST.in
+-rw-r--r--   0 root         (0)     1003     4836 2023-07-05 15:21:42.625350 google-cloud-org-policy-1.8.2/PKG-INFO
+-rw-rw-r--   0 root         (0)     1003     3911 2023-07-05 15:19:18.000000 google-cloud-org-policy-1.8.2/README.rst
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:21:42.617354 google-cloud-org-policy-1.8.2/google/
+-rw-rw-r--   0 root         (0)     1003      774 2023-07-05 15:19:18.000000 google-cloud-org-policy-1.8.2/google/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:21:42.617354 google-cloud-org-policy-1.8.2/google/cloud/
+-rw-rw-r--   0 root         (0)     1003      774 2023-07-05 15:19:18.000000 google-cloud-org-policy-1.8.2/google/cloud/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:21:42.617354 google-cloud-org-policy-1.8.2/google/cloud/orgpolicy/
+-rw-rw-r--   0 root         (0)     1003     2236 2023-07-05 15:19:18.000000 google-cloud-org-policy-1.8.2/google/cloud/orgpolicy/__init__.py
+-rw-rw-r--   0 root         (0)     1003      652 2023-07-05 15:19:18.000000 google-cloud-org-policy-1.8.2/google/cloud/orgpolicy/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       84 2023-07-05 15:19:18.000000 google-cloud-org-policy-1.8.2/google/cloud/orgpolicy/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:21:42.617354 google-cloud-org-policy-1.8.2/google/cloud/orgpolicy/v1/
+-rw-rw-r--   0 root         (0)     1003      919 2023-07-05 15:19:18.000000 google-cloud-org-policy-1.8.2/google/cloud/orgpolicy/v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003    14416 2023-07-05 15:19:18.000000 google-cloud-org-policy-1.8.2/google/cloud/orgpolicy/v1/orgpolicy.proto
+-rw-rw-r--   0 root         (0)     1003     5783 2023-07-05 15:19:18.000000 google-cloud-org-policy-1.8.2/google/cloud/orgpolicy/v1/orgpolicy_pb2.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:21:42.621352 google-cloud-org-policy-1.8.2/google/cloud/orgpolicy_v2/
+-rw-rw-r--   0 root         (0)     1003     1835 2023-07-05 15:19:18.000000 google-cloud-org-policy-1.8.2/google/cloud/orgpolicy_v2/__init__.py
+-rw-rw-r--   0 root         (0)     1003     3199 2023-07-05 15:19:18.000000 google-cloud-org-policy-1.8.2/google/cloud/orgpolicy_v2/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      652 2023-07-05 15:19:18.000000 google-cloud-org-policy-1.8.2/google/cloud/orgpolicy_v2/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       84 2023-07-05 15:19:18.000000 google-cloud-org-policy-1.8.2/google/cloud/orgpolicy_v2/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:21:42.621352 google-cloud-org-policy-1.8.2/google/cloud/orgpolicy_v2/services/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:19:18.000000 google-cloud-org-policy-1.8.2/google/cloud/orgpolicy_v2/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:21:42.621352 google-cloud-org-policy-1.8.2/google/cloud/orgpolicy_v2/services/org_policy/
+-rw-rw-r--   0 root         (0)     1003      749 2023-07-05 15:19:18.000000 google-cloud-org-policy-1.8.2/google/cloud/orgpolicy_v2/services/org_policy/__init__.py
+-rw-rw-r--   0 root         (0)     1003    44712 2023-07-05 15:19:18.000000 google-cloud-org-policy-1.8.2/google/cloud/orgpolicy_v2/services/org_policy/async_client.py
+-rw-rw-r--   0 root         (0)     1003    52631 2023-07-05 15:19:18.000000 google-cloud-org-policy-1.8.2/google/cloud/orgpolicy_v2/services/org_policy/client.py
+-rw-rw-r--   0 root         (0)     1003    10791 2023-07-05 15:19:18.000000 google-cloud-org-policy-1.8.2/google/cloud/orgpolicy_v2/services/org_policy/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:21:42.621352 google-cloud-org-policy-1.8.2/google/cloud/orgpolicy_v2/services/org_policy/transports/
+-rw-rw-r--   0 root         (0)     1003     1348 2023-07-05 15:19:18.000000 google-cloud-org-policy-1.8.2/google/cloud/orgpolicy_v2/services/org_policy/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003    11416 2023-07-05 15:19:18.000000 google-cloud-org-policy-1.8.2/google/cloud/orgpolicy_v2/services/org_policy/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    20621 2023-07-05 15:19:18.000000 google-cloud-org-policy-1.8.2/google/cloud/orgpolicy_v2/services/org_policy/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    20982 2023-07-05 15:19:18.000000 google-cloud-org-policy-1.8.2/google/cloud/orgpolicy_v2/services/org_policy/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    45192 2023-07-05 15:19:18.000000 google-cloud-org-policy-1.8.2/google/cloud/orgpolicy_v2/services/org_policy/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:21:42.621352 google-cloud-org-policy-1.8.2/google/cloud/orgpolicy_v2/types/
+-rw-rw-r--   0 root         (0)     1003     1306 2023-07-05 15:19:18.000000 google-cloud-org-policy-1.8.2/google/cloud/orgpolicy_v2/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003     6656 2023-07-05 15:19:18.000000 google-cloud-org-policy-1.8.2/google/cloud/orgpolicy_v2/types/constraint.py
+-rw-rw-r--   0 root         (0)     1003    18977 2023-07-05 15:19:18.000000 google-cloud-org-policy-1.8.2/google/cloud/orgpolicy_v2/types/orgpolicy.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:21:42.625350 google-cloud-org-policy-1.8.2/google_cloud_org_policy.egg-info/
+-rw-r--r--   0 root         (0)     1003     4836 2023-07-05 15:21:42.000000 google-cloud-org-policy-1.8.2/google_cloud_org_policy.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0)     1003     1733 2023-07-05 15:21:42.000000 google-cloud-org-policy-1.8.2/google_cloud_org_policy.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-07-05 15:21:42.000000 google-cloud-org-policy-1.8.2/google_cloud_org_policy.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0)     1003       20 2023-07-05 15:21:42.000000 google-cloud-org-policy-1.8.2/google_cloud_org_policy.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-07-05 15:21:42.000000 google-cloud-org-policy-1.8.2/google_cloud_org_policy.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0)     1003      315 2023-07-05 15:21:42.000000 google-cloud-org-policy-1.8.2/google_cloud_org_policy.egg-info/requires.txt
+-rw-r--r--   0 root         (0)     1003        7 2023-07-05 15:21:42.000000 google-cloud-org-policy-1.8.2/google_cloud_org_policy.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0)     1003       67 2023-07-05 15:21:42.625350 google-cloud-org-policy-1.8.2/setup.cfg
+-rw-rw-r--   0 root         (0)     1003     2932 2023-07-05 15:19:18.000000 google-cloud-org-policy-1.8.2/setup.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:21:42.625350 google-cloud-org-policy-1.8.2/tests/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:19:18.000000 google-cloud-org-policy-1.8.2/tests/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:21:42.625350 google-cloud-org-policy-1.8.2/tests/unit/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:19:18.000000 google-cloud-org-policy-1.8.2/tests/unit/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:21:42.625350 google-cloud-org-policy-1.8.2/tests/unit/gapic/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:19:18.000000 google-cloud-org-policy-1.8.2/tests/unit/gapic/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:21:42.625350 google-cloud-org-policy-1.8.2/tests/unit/gapic/orgpolicy_v2/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:19:18.000000 google-cloud-org-policy-1.8.2/tests/unit/gapic/orgpolicy_v2/__init__.py
+-rw-rw-r--   0 root         (0)     1003   197522 2023-07-05 15:19:18.000000 google-cloud-org-policy-1.8.2/tests/unit/gapic/orgpolicy_v2/test_org_policy.py
```

### Comparing `google-cloud-org-policy-1.8.1/LICENSE` & `google-cloud-org-policy-1.8.2/LICENSE`

 * *Files identical despite different names*

### Comparing `google-cloud-org-policy-1.8.1/MANIFEST.in` & `google-cloud-org-policy-1.8.2/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `google-cloud-org-policy-1.8.1/PKG-INFO` & `google-cloud-org-policy-1.8.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-org-policy
-Version: 1.8.1
+Version: 1.8.2
 Summary: Google Cloud Org Policy API client library
 Home-page: https://github.com/googleapis/python-org-policy
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `google-cloud-org-policy-1.8.1/README.rst` & `google-cloud-org-policy-1.8.2/README.rst`

 * *Files identical despite different names*

### Comparing `google-cloud-org-policy-1.8.1/google/__init__.py` & `google-cloud-org-policy-1.8.2/google/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-org-policy-1.8.1/google/cloud/__init__.py` & `google-cloud-org-policy-1.8.2/google/cloud/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-org-policy-1.8.1/google/cloud/orgpolicy/__init__.py` & `google-cloud-org-policy-1.8.2/google/cloud/orgpolicy/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-org-policy-1.8.1/google/cloud/orgpolicy/gapic_version.py` & `google-cloud-org-policy-1.8.2/google/cloud/orgpolicy/gapic_version.py`

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

### Comparing `google-cloud-org-policy-1.8.1/google/cloud/orgpolicy/v1/__init__.py` & `google-cloud-org-policy-1.8.2/google/cloud/orgpolicy/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-org-policy-1.8.1/google/cloud/orgpolicy/v1/orgpolicy.proto` & `google-cloud-org-policy-1.8.2/google/cloud/orgpolicy/v1/orgpolicy.proto`

 * *Files identical despite different names*

### Comparing `google-cloud-org-policy-1.8.1/google/cloud/orgpolicy/v1/orgpolicy_pb2.py` & `google-cloud-org-policy-1.8.2/google/cloud/orgpolicy/v1/orgpolicy_pb2.py`

 * *Files identical despite different names*

### Comparing `google-cloud-org-policy-1.8.1/google/cloud/orgpolicy_v2/__init__.py` & `google-cloud-org-policy-1.8.2/google/cloud/orgpolicy_v2/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-org-policy-1.8.1/google/cloud/orgpolicy_v2/gapic_metadata.json` & `google-cloud-org-policy-1.8.2/google/cloud/orgpolicy_v2/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-cloud-org-policy-1.8.1/google/cloud/orgpolicy_v2/gapic_version.py` & `google-cloud-org-policy-1.8.2/google/cloud/orgpolicy_v2/gapic_version.py`

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

### Comparing `google-cloud-org-policy-1.8.1/google/cloud/orgpolicy_v2/services/__init__.py` & `google-cloud-org-policy-1.8.2/google/cloud/orgpolicy_v2/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-org-policy-1.8.1/google/cloud/orgpolicy_v2/services/org_policy/__init__.py` & `google-cloud-org-policy-1.8.2/google/cloud/orgpolicy_v2/services/org_policy/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-org-policy-1.8.1/google/cloud/orgpolicy_v2/services/org_policy/async_client.py` & `google-cloud-org-policy-1.8.2/google/cloud/orgpolicy_v2/services/org_policy/async_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1088,15 +1088,15 @@
         await rpc(
             request,
             retry=retry,
             timeout=timeout,
             metadata=metadata,
         )
 
-    async def __aenter__(self):
+    async def __aenter__(self) -> "OrgPolicyAsyncClient":
         return self
 
     async def __aexit__(self, exc_type, exc, tb):
         await self.transport.close()
 
 
 DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
```

### Comparing `google-cloud-org-policy-1.8.1/google/cloud/orgpolicy_v2/services/org_policy/client.py` & `google-cloud-org-policy-1.8.2/google/cloud/orgpolicy_v2/services/org_policy/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-org-policy-1.8.1/google/cloud/orgpolicy_v2/services/org_policy/pagers.py` & `google-cloud-org-policy-1.8.2/google/cloud/orgpolicy_v2/services/org_policy/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-org-policy-1.8.1/google/cloud/orgpolicy_v2/services/org_policy/transports/__init__.py` & `google-cloud-org-policy-1.8.2/google/cloud/orgpolicy_v2/services/org_policy/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-org-policy-1.8.1/google/cloud/orgpolicy_v2/services/org_policy/transports/base.py` & `google-cloud-org-policy-1.8.2/google/cloud/orgpolicy_v2/services/org_policy/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-org-policy-1.8.1/google/cloud/orgpolicy_v2/services/org_policy/transports/grpc.py` & `google-cloud-org-policy-1.8.2/google/cloud/orgpolicy_v2/services/org_policy/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-org-policy-1.8.1/google/cloud/orgpolicy_v2/services/org_policy/transports/grpc_asyncio.py` & `google-cloud-org-policy-1.8.2/google/cloud/orgpolicy_v2/services/org_policy/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-org-policy-1.8.1/google/cloud/orgpolicy_v2/services/org_policy/transports/rest.py` & `google-cloud-org-policy-1.8.2/google/cloud/orgpolicy_v2/services/org_policy/transports/rest.py`

 * *Files identical despite different names*

### Comparing `google-cloud-org-policy-1.8.1/google/cloud/orgpolicy_v2/types/__init__.py` & `google-cloud-org-policy-1.8.2/google/cloud/orgpolicy_v2/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-org-policy-1.8.1/google/cloud/orgpolicy_v2/types/constraint.py` & `google-cloud-org-policy-1.8.2/google/cloud/orgpolicy_v2/types/constraint.py`

 * *Files identical despite different names*

### Comparing `google-cloud-org-policy-1.8.1/google/cloud/orgpolicy_v2/types/orgpolicy.py` & `google-cloud-org-policy-1.8.2/google/cloud/orgpolicy_v2/types/orgpolicy.py`

 * *Files identical despite different names*

### Comparing `google-cloud-org-policy-1.8.1/google_cloud_org_policy.egg-info/PKG-INFO` & `google-cloud-org-policy-1.8.2/google_cloud_org_policy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-org-policy
-Version: 1.8.1
+Version: 1.8.2
 Summary: Google Cloud Org Policy API client library
 Home-page: https://github.com/googleapis/python-org-policy
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `google-cloud-org-policy-1.8.1/google_cloud_org_policy.egg-info/SOURCES.txt` & `google-cloud-org-policy-1.8.2/google_cloud_org_policy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `google-cloud-org-policy-1.8.1/setup.py` & `google-cloud-org-policy-1.8.2/setup.py`

 * *Files identical despite different names*

### Comparing `google-cloud-org-policy-1.8.1/tests/__init__.py` & `google-cloud-org-policy-1.8.2/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-org-policy-1.8.1/tests/unit/__init__.py` & `google-cloud-org-policy-1.8.2/tests/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-org-policy-1.8.1/tests/unit/gapic/__init__.py` & `google-cloud-org-policy-1.8.2/tests/unit/gapic/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-org-policy-1.8.1/tests/unit/gapic/orgpolicy_v2/__init__.py` & `google-cloud-org-policy-1.8.2/tests/unit/gapic/orgpolicy_v2/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-org-policy-1.8.1/tests/unit/gapic/orgpolicy_v2/test_org_policy.py` & `google-cloud-org-policy-1.8.2/tests/unit/gapic/orgpolicy_v2/test_org_policy.py`

 * *Files 0% similar despite different names*

```diff
@@ -1091,17 +1091,19 @@
                     constraint.Constraint(),
                     constraint.Constraint(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.list_constraints(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
@@ -1511,17 +1513,19 @@
                     orgpolicy.Policy(),
                     orgpolicy.Policy(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.list_policies(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
```

