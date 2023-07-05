# Comparing `tmp/google-cloud-artifact-registry-1.8.1.tar.gz` & `tmp/google-cloud-artifact-registry-1.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-cloud-artifact-registry-1.8.1.tar", last modified: Mon Mar 27 14:57:42 2023, max compression
+gzip compressed data, was "google-cloud-artifact-registry-1.8.2.tar", last modified: Wed Jul  5 15:50:23 2023, max compression
```

## Comparing `google-cloud-artifact-registry-1.8.1.tar` & `google-cloud-artifact-registry-1.8.2.tar`

### file list

```diff
@@ -1,93 +1,93 @@
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:57:42.434918 google-cloud-artifact-registry-1.8.1/
--rw-rw-r--   0 root         (0)     1003    11358 2023-03-27 14:55:06.000000 google-cloud-artifact-registry-1.8.1/LICENSE
--rw-rw-r--   0 root         (0)     1003      860 2023-03-27 14:55:06.000000 google-cloud-artifact-registry-1.8.1/MANIFEST.in
--rw-r--r--   0 root         (0)     1003     4955 2023-03-27 14:57:42.434918 google-cloud-artifact-registry-1.8.1/PKG-INFO
--rw-rw-r--   0 root         (0)     1003     4009 2023-03-27 14:55:06.000000 google-cloud-artifact-registry-1.8.1/README.rst
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:57:42.414914 google-cloud-artifact-registry-1.8.1/google/
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:57:42.414914 google-cloud-artifact-registry-1.8.1/google/cloud/
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:57:42.414914 google-cloud-artifact-registry-1.8.1/google/cloud/artifactregistry/
--rw-rw-r--   0 root         (0)     1003     5160 2023-03-27 14:55:06.000000 google-cloud-artifact-registry-1.8.1/google/cloud/artifactregistry/__init__.py
--rw-rw-r--   0 root         (0)     1003      652 2023-03-27 14:55:06.000000 google-cloud-artifact-registry-1.8.1/google/cloud/artifactregistry/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       91 2023-03-27 14:55:06.000000 google-cloud-artifact-registry-1.8.1/google/cloud/artifactregistry/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:57:42.418915 google-cloud-artifact-registry-1.8.1/google/cloud/artifactregistry_v1/
--rw-rw-r--   0 root         (0)     1003     4658 2023-03-27 14:55:06.000000 google-cloud-artifact-registry-1.8.1/google/cloud/artifactregistry_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003    13684 2023-03-27 14:55:06.000000 google-cloud-artifact-registry-1.8.1/google/cloud/artifactregistry_v1/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003      652 2023-03-27 14:55:06.000000 google-cloud-artifact-registry-1.8.1/google/cloud/artifactregistry_v1/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       91 2023-03-27 14:55:06.000000 google-cloud-artifact-registry-1.8.1/google/cloud/artifactregistry_v1/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:57:42.418915 google-cloud-artifact-registry-1.8.1/google/cloud/artifactregistry_v1/services/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 14:55:06.000000 google-cloud-artifact-registry-1.8.1/google/cloud/artifactregistry_v1/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:57:42.418915 google-cloud-artifact-registry-1.8.1/google/cloud/artifactregistry_v1/services/artifact_registry/
--rw-rw-r--   0 root         (0)     1003      777 2023-03-27 14:55:06.000000 google-cloud-artifact-registry-1.8.1/google/cloud/artifactregistry_v1/services/artifact_registry/__init__.py
--rw-rw-r--   0 root         (0)     1003   173687 2023-03-27 14:55:06.000000 google-cloud-artifact-registry-1.8.1/google/cloud/artifactregistry_v1/services/artifact_registry/async_client.py
--rw-rw-r--   0 root         (0)     1003   195059 2023-03-27 14:55:06.000000 google-cloud-artifact-registry-1.8.1/google/cloud/artifactregistry_v1/services/artifact_registry/client.py
--rw-rw-r--   0 root         (0)     1003    46028 2023-03-27 14:55:06.000000 google-cloud-artifact-registry-1.8.1/google/cloud/artifactregistry_v1/services/artifact_registry/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:57:42.418915 google-cloud-artifact-registry-1.8.1/google/cloud/artifactregistry_v1/services/artifact_registry/transports/
--rw-rw-r--   0 root         (0)     1003     1428 2023-03-27 14:55:06.000000 google-cloud-artifact-registry-1.8.1/google/cloud/artifactregistry_v1/services/artifact_registry/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003    22688 2023-03-27 14:55:06.000000 google-cloud-artifact-registry-1.8.1/google/cloud/artifactregistry_v1/services/artifact_registry/transports/base.py
--rw-rw-r--   0 root         (0)     1003    54735 2023-03-27 14:55:06.000000 google-cloud-artifact-registry-1.8.1/google/cloud/artifactregistry_v1/services/artifact_registry/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    56058 2023-03-27 14:55:06.000000 google-cloud-artifact-registry-1.8.1/google/cloud/artifactregistry_v1/services/artifact_registry/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003   197642 2023-03-27 14:55:06.000000 google-cloud-artifact-registry-1.8.1/google/cloud/artifactregistry_v1/services/artifact_registry/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:57:42.422916 google-cloud-artifact-registry-1.8.1/google/cloud/artifactregistry_v1/types/
--rw-rw-r--   0 root         (0)     1003     4282 2023-03-27 14:55:06.000000 google-cloud-artifact-registry-1.8.1/google/cloud/artifactregistry_v1/types/__init__.py
--rw-rw-r--   0 root         (0)     1003     6178 2023-03-27 14:55:06.000000 google-cloud-artifact-registry-1.8.1/google/cloud/artifactregistry_v1/types/apt_artifact.py
--rw-rw-r--   0 root         (0)     1003    17062 2023-03-27 14:55:06.000000 google-cloud-artifact-registry-1.8.1/google/cloud/artifactregistry_v1/types/artifact.py
--rw-rw-r--   0 root         (0)     1003     6289 2023-03-27 14:55:06.000000 google-cloud-artifact-registry-1.8.1/google/cloud/artifactregistry_v1/types/file.py
--rw-rw-r--   0 root         (0)     1003     4185 2023-03-27 14:55:06.000000 google-cloud-artifact-registry-1.8.1/google/cloud/artifactregistry_v1/types/package.py
--rw-rw-r--   0 root         (0)     1003    10021 2023-03-27 14:55:06.000000 google-cloud-artifact-registry-1.8.1/google/cloud/artifactregistry_v1/types/repository.py
--rw-rw-r--   0 root         (0)     1003     1012 2023-03-27 14:55:06.000000 google-cloud-artifact-registry-1.8.1/google/cloud/artifactregistry_v1/types/service.py
--rw-rw-r--   0 root         (0)     1003     3484 2023-03-27 14:55:06.000000 google-cloud-artifact-registry-1.8.1/google/cloud/artifactregistry_v1/types/settings.py
--rw-rw-r--   0 root         (0)     1003     5826 2023-03-27 14:55:06.000000 google-cloud-artifact-registry-1.8.1/google/cloud/artifactregistry_v1/types/tag.py
--rw-rw-r--   0 root         (0)     1003     7171 2023-03-27 14:55:06.000000 google-cloud-artifact-registry-1.8.1/google/cloud/artifactregistry_v1/types/version.py
--rw-rw-r--   0 root         (0)     1003     3578 2023-03-27 14:55:06.000000 google-cloud-artifact-registry-1.8.1/google/cloud/artifactregistry_v1/types/vpcsc_config.py
--rw-rw-r--   0 root         (0)     1003     5666 2023-03-27 14:55:06.000000 google-cloud-artifact-registry-1.8.1/google/cloud/artifactregistry_v1/types/yum_artifact.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:57:42.422916 google-cloud-artifact-registry-1.8.1/google/cloud/artifactregistry_v1beta2/
--rw-rw-r--   0 root         (0)     1003     3493 2023-03-27 14:55:06.000000 google-cloud-artifact-registry-1.8.1/google/cloud/artifactregistry_v1beta2/__init__.py
--rw-rw-r--   0 root         (0)     1003     9842 2023-03-27 14:55:06.000000 google-cloud-artifact-registry-1.8.1/google/cloud/artifactregistry_v1beta2/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003      652 2023-03-27 14:55:06.000000 google-cloud-artifact-registry-1.8.1/google/cloud/artifactregistry_v1beta2/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       91 2023-03-27 14:55:06.000000 google-cloud-artifact-registry-1.8.1/google/cloud/artifactregistry_v1beta2/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:57:42.422916 google-cloud-artifact-registry-1.8.1/google/cloud/artifactregistry_v1beta2/services/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 14:55:06.000000 google-cloud-artifact-registry-1.8.1/google/cloud/artifactregistry_v1beta2/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:57:42.426916 google-cloud-artifact-registry-1.8.1/google/cloud/artifactregistry_v1beta2/services/artifact_registry/
--rw-rw-r--   0 root         (0)     1003      777 2023-03-27 14:55:06.000000 google-cloud-artifact-registry-1.8.1/google/cloud/artifactregistry_v1beta2/services/artifact_registry/__init__.py
--rw-rw-r--   0 root         (0)     1003   132737 2023-03-27 14:55:06.000000 google-cloud-artifact-registry-1.8.1/google/cloud/artifactregistry_v1beta2/services/artifact_registry/async_client.py
--rw-rw-r--   0 root         (0)     1003   144067 2023-03-27 14:55:06.000000 google-cloud-artifact-registry-1.8.1/google/cloud/artifactregistry_v1beta2/services/artifact_registry/client.py
--rw-rw-r--   0 root         (0)     1003    25699 2023-03-27 14:55:06.000000 google-cloud-artifact-registry-1.8.1/google/cloud/artifactregistry_v1beta2/services/artifact_registry/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:57:42.426916 google-cloud-artifact-registry-1.8.1/google/cloud/artifactregistry_v1beta2/services/artifact_registry/transports/
--rw-rw-r--   0 root         (0)     1003     1428 2023-03-27 14:55:06.000000 google-cloud-artifact-registry-1.8.1/google/cloud/artifactregistry_v1beta2/services/artifact_registry/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003    22792 2023-03-27 14:55:06.000000 google-cloud-artifact-registry-1.8.1/google/cloud/artifactregistry_v1beta2/services/artifact_registry/transports/base.py
--rw-rw-r--   0 root         (0)     1003    42447 2023-03-27 14:55:06.000000 google-cloud-artifact-registry-1.8.1/google/cloud/artifactregistry_v1beta2/services/artifact_registry/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    43467 2023-03-27 14:55:06.000000 google-cloud-artifact-registry-1.8.1/google/cloud/artifactregistry_v1beta2/services/artifact_registry/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003   141462 2023-03-27 14:55:06.000000 google-cloud-artifact-registry-1.8.1/google/cloud/artifactregistry_v1beta2/services/artifact_registry/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:57:42.430917 google-cloud-artifact-registry-1.8.1/google/cloud/artifactregistry_v1beta2/types/
--rw-rw-r--   0 root         (0)     1003     3141 2023-03-27 14:55:06.000000 google-cloud-artifact-registry-1.8.1/google/cloud/artifactregistry_v1beta2/types/__init__.py
--rw-rw-r--   0 root         (0)     1003     6209 2023-03-27 14:55:06.000000 google-cloud-artifact-registry-1.8.1/google/cloud/artifactregistry_v1beta2/types/apt_artifact.py
--rw-rw-r--   0 root         (0)     1003     5727 2023-03-27 14:55:06.000000 google-cloud-artifact-registry-1.8.1/google/cloud/artifactregistry_v1beta2/types/file.py
--rw-rw-r--   0 root         (0)     1003     4064 2023-03-27 14:55:06.000000 google-cloud-artifact-registry-1.8.1/google/cloud/artifactregistry_v1beta2/types/package.py
--rw-rw-r--   0 root         (0)     1003    10058 2023-03-27 14:55:06.000000 google-cloud-artifact-registry-1.8.1/google/cloud/artifactregistry_v1beta2/types/repository.py
--rw-rw-r--   0 root         (0)     1003     1017 2023-03-27 14:55:06.000000 google-cloud-artifact-registry-1.8.1/google/cloud/artifactregistry_v1beta2/types/service.py
--rw-rw-r--   0 root         (0)     1003     3499 2023-03-27 14:55:06.000000 google-cloud-artifact-registry-1.8.1/google/cloud/artifactregistry_v1beta2/types/settings.py
--rw-rw-r--   0 root         (0)     1003     5846 2023-03-27 14:55:06.000000 google-cloud-artifact-registry-1.8.1/google/cloud/artifactregistry_v1beta2/types/tag.py
--rw-rw-r--   0 root         (0)     1003     6729 2023-03-27 14:55:06.000000 google-cloud-artifact-registry-1.8.1/google/cloud/artifactregistry_v1beta2/types/version.py
--rw-rw-r--   0 root         (0)     1003     5697 2023-03-27 14:55:06.000000 google-cloud-artifact-registry-1.8.1/google/cloud/artifactregistry_v1beta2/types/yum_artifact.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:57:42.430917 google-cloud-artifact-registry-1.8.1/google_cloud_artifact_registry.egg-info/
--rw-r--r--   0 root         (0)     1003     4955 2023-03-27 14:57:42.000000 google-cloud-artifact-registry-1.8.1/google_cloud_artifact_registry.egg-info/PKG-INFO
--rw-r--r--   0 root         (0)     1003     3986 2023-03-27 14:57:42.000000 google-cloud-artifact-registry-1.8.1/google_cloud_artifact_registry.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0)     1003        1 2023-03-27 14:57:42.000000 google-cloud-artifact-registry-1.8.1/google_cloud_artifact_registry.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0)     1003       20 2023-03-27 14:57:42.000000 google-cloud-artifact-registry-1.8.1/google_cloud_artifact_registry.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0)     1003        1 2023-03-27 14:57:42.000000 google-cloud-artifact-registry-1.8.1/google_cloud_artifact_registry.egg-info/not-zip-safe
--rw-r--r--   0 root         (0)     1003      352 2023-03-27 14:57:42.000000 google-cloud-artifact-registry-1.8.1/google_cloud_artifact_registry.egg-info/requires.txt
--rw-r--r--   0 root         (0)     1003        7 2023-03-27 14:57:42.000000 google-cloud-artifact-registry-1.8.1/google_cloud_artifact_registry.egg-info/top_level.txt
--rw-rw-r--   0 root         (0)     1003       67 2023-03-27 14:57:42.434918 google-cloud-artifact-registry-1.8.1/setup.cfg
--rw-rw-r--   0 root         (0)     1003     3013 2023-03-27 14:55:06.000000 google-cloud-artifact-registry-1.8.1/setup.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:57:42.430917 google-cloud-artifact-registry-1.8.1/tests/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 14:55:06.000000 google-cloud-artifact-registry-1.8.1/tests/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:57:42.430917 google-cloud-artifact-registry-1.8.1/tests/unit/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 14:55:06.000000 google-cloud-artifact-registry-1.8.1/tests/unit/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:57:42.430917 google-cloud-artifact-registry-1.8.1/tests/unit/gapic/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 14:55:06.000000 google-cloud-artifact-registry-1.8.1/tests/unit/gapic/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:57:42.430917 google-cloud-artifact-registry-1.8.1/tests/unit/gapic/artifactregistry_v1/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 14:55:06.000000 google-cloud-artifact-registry-1.8.1/tests/unit/gapic/artifactregistry_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003   753860 2023-03-27 14:55:06.000000 google-cloud-artifact-registry-1.8.1/tests/unit/gapic/artifactregistry_v1/test_artifact_registry.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:57:42.434918 google-cloud-artifact-registry-1.8.1/tests/unit/gapic/artifactregistry_v1beta2/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 14:55:06.000000 google-cloud-artifact-registry-1.8.1/tests/unit/gapic/artifactregistry_v1beta2/__init__.py
--rw-rw-r--   0 root         (0)     1003   502510 2023-03-27 14:55:06.000000 google-cloud-artifact-registry-1.8.1/tests/unit/gapic/artifactregistry_v1beta2/test_artifact_registry.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:50:23.040056 google-cloud-artifact-registry-1.8.2/
+-rw-rw-r--   0 root         (0)     1003    11358 2023-07-05 15:46:58.000000 google-cloud-artifact-registry-1.8.2/LICENSE
+-rw-rw-r--   0 root         (0)     1003      860 2023-07-05 15:46:58.000000 google-cloud-artifact-registry-1.8.2/MANIFEST.in
+-rw-r--r--   0 root         (0)     1003     4914 2023-07-05 15:50:23.040056 google-cloud-artifact-registry-1.8.2/PKG-INFO
+-rw-rw-r--   0 root         (0)     1003     3973 2023-07-05 15:46:58.000000 google-cloud-artifact-registry-1.8.2/README.rst
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:50:23.024055 google-cloud-artifact-registry-1.8.2/google/
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:50:23.024055 google-cloud-artifact-registry-1.8.2/google/cloud/
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:50:23.024055 google-cloud-artifact-registry-1.8.2/google/cloud/artifactregistry/
+-rw-rw-r--   0 root         (0)     1003     5160 2023-07-05 15:46:58.000000 google-cloud-artifact-registry-1.8.2/google/cloud/artifactregistry/__init__.py
+-rw-rw-r--   0 root         (0)     1003      652 2023-07-05 15:46:58.000000 google-cloud-artifact-registry-1.8.2/google/cloud/artifactregistry/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       91 2023-07-05 15:46:58.000000 google-cloud-artifact-registry-1.8.2/google/cloud/artifactregistry/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:50:23.028055 google-cloud-artifact-registry-1.8.2/google/cloud/artifactregistry_v1/
+-rw-rw-r--   0 root         (0)     1003     4658 2023-07-05 15:46:58.000000 google-cloud-artifact-registry-1.8.2/google/cloud/artifactregistry_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003    13684 2023-07-05 15:46:58.000000 google-cloud-artifact-registry-1.8.2/google/cloud/artifactregistry_v1/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      652 2023-07-05 15:46:58.000000 google-cloud-artifact-registry-1.8.2/google/cloud/artifactregistry_v1/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       91 2023-07-05 15:46:58.000000 google-cloud-artifact-registry-1.8.2/google/cloud/artifactregistry_v1/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:50:23.028055 google-cloud-artifact-registry-1.8.2/google/cloud/artifactregistry_v1/services/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:58.000000 google-cloud-artifact-registry-1.8.2/google/cloud/artifactregistry_v1/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:50:23.028055 google-cloud-artifact-registry-1.8.2/google/cloud/artifactregistry_v1/services/artifact_registry/
+-rw-rw-r--   0 root         (0)     1003      777 2023-07-05 15:46:58.000000 google-cloud-artifact-registry-1.8.2/google/cloud/artifactregistry_v1/services/artifact_registry/__init__.py
+-rw-rw-r--   0 root         (0)     1003   173720 2023-07-05 15:46:58.000000 google-cloud-artifact-registry-1.8.2/google/cloud/artifactregistry_v1/services/artifact_registry/async_client.py
+-rw-rw-r--   0 root         (0)     1003   195059 2023-07-05 15:46:58.000000 google-cloud-artifact-registry-1.8.2/google/cloud/artifactregistry_v1/services/artifact_registry/client.py
+-rw-rw-r--   0 root         (0)     1003    46028 2023-07-05 15:46:58.000000 google-cloud-artifact-registry-1.8.2/google/cloud/artifactregistry_v1/services/artifact_registry/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:50:23.028055 google-cloud-artifact-registry-1.8.2/google/cloud/artifactregistry_v1/services/artifact_registry/transports/
+-rw-rw-r--   0 root         (0)     1003     1428 2023-07-05 15:46:58.000000 google-cloud-artifact-registry-1.8.2/google/cloud/artifactregistry_v1/services/artifact_registry/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003    22688 2023-07-05 15:46:58.000000 google-cloud-artifact-registry-1.8.2/google/cloud/artifactregistry_v1/services/artifact_registry/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    54735 2023-07-05 15:46:58.000000 google-cloud-artifact-registry-1.8.2/google/cloud/artifactregistry_v1/services/artifact_registry/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    56058 2023-07-05 15:46:58.000000 google-cloud-artifact-registry-1.8.2/google/cloud/artifactregistry_v1/services/artifact_registry/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003   197642 2023-07-05 15:46:58.000000 google-cloud-artifact-registry-1.8.2/google/cloud/artifactregistry_v1/services/artifact_registry/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:50:23.032055 google-cloud-artifact-registry-1.8.2/google/cloud/artifactregistry_v1/types/
+-rw-rw-r--   0 root         (0)     1003     4282 2023-07-05 15:46:58.000000 google-cloud-artifact-registry-1.8.2/google/cloud/artifactregistry_v1/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003     6178 2023-07-05 15:46:58.000000 google-cloud-artifact-registry-1.8.2/google/cloud/artifactregistry_v1/types/apt_artifact.py
+-rw-rw-r--   0 root         (0)     1003    17062 2023-07-05 15:46:58.000000 google-cloud-artifact-registry-1.8.2/google/cloud/artifactregistry_v1/types/artifact.py
+-rw-rw-r--   0 root         (0)     1003     6289 2023-07-05 15:46:58.000000 google-cloud-artifact-registry-1.8.2/google/cloud/artifactregistry_v1/types/file.py
+-rw-rw-r--   0 root         (0)     1003     4185 2023-07-05 15:46:58.000000 google-cloud-artifact-registry-1.8.2/google/cloud/artifactregistry_v1/types/package.py
+-rw-rw-r--   0 root         (0)     1003    10021 2023-07-05 15:46:58.000000 google-cloud-artifact-registry-1.8.2/google/cloud/artifactregistry_v1/types/repository.py
+-rw-rw-r--   0 root         (0)     1003     1012 2023-07-05 15:46:58.000000 google-cloud-artifact-registry-1.8.2/google/cloud/artifactregistry_v1/types/service.py
+-rw-rw-r--   0 root         (0)     1003     3484 2023-07-05 15:46:58.000000 google-cloud-artifact-registry-1.8.2/google/cloud/artifactregistry_v1/types/settings.py
+-rw-rw-r--   0 root         (0)     1003     5826 2023-07-05 15:46:58.000000 google-cloud-artifact-registry-1.8.2/google/cloud/artifactregistry_v1/types/tag.py
+-rw-rw-r--   0 root         (0)     1003     7171 2023-07-05 15:46:58.000000 google-cloud-artifact-registry-1.8.2/google/cloud/artifactregistry_v1/types/version.py
+-rw-rw-r--   0 root         (0)     1003     3578 2023-07-05 15:46:58.000000 google-cloud-artifact-registry-1.8.2/google/cloud/artifactregistry_v1/types/vpcsc_config.py
+-rw-rw-r--   0 root         (0)     1003     5666 2023-07-05 15:46:58.000000 google-cloud-artifact-registry-1.8.2/google/cloud/artifactregistry_v1/types/yum_artifact.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:50:23.032055 google-cloud-artifact-registry-1.8.2/google/cloud/artifactregistry_v1beta2/
+-rw-rw-r--   0 root         (0)     1003     3493 2023-07-05 15:46:58.000000 google-cloud-artifact-registry-1.8.2/google/cloud/artifactregistry_v1beta2/__init__.py
+-rw-rw-r--   0 root         (0)     1003     9842 2023-07-05 15:46:58.000000 google-cloud-artifact-registry-1.8.2/google/cloud/artifactregistry_v1beta2/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      652 2023-07-05 15:46:58.000000 google-cloud-artifact-registry-1.8.2/google/cloud/artifactregistry_v1beta2/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       91 2023-07-05 15:46:58.000000 google-cloud-artifact-registry-1.8.2/google/cloud/artifactregistry_v1beta2/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:50:23.032055 google-cloud-artifact-registry-1.8.2/google/cloud/artifactregistry_v1beta2/services/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:58.000000 google-cloud-artifact-registry-1.8.2/google/cloud/artifactregistry_v1beta2/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:50:23.036056 google-cloud-artifact-registry-1.8.2/google/cloud/artifactregistry_v1beta2/services/artifact_registry/
+-rw-rw-r--   0 root         (0)     1003      777 2023-07-05 15:46:58.000000 google-cloud-artifact-registry-1.8.2/google/cloud/artifactregistry_v1beta2/services/artifact_registry/__init__.py
+-rw-rw-r--   0 root         (0)     1003   132770 2023-07-05 15:46:58.000000 google-cloud-artifact-registry-1.8.2/google/cloud/artifactregistry_v1beta2/services/artifact_registry/async_client.py
+-rw-rw-r--   0 root         (0)     1003   144067 2023-07-05 15:46:58.000000 google-cloud-artifact-registry-1.8.2/google/cloud/artifactregistry_v1beta2/services/artifact_registry/client.py
+-rw-rw-r--   0 root         (0)     1003    25699 2023-07-05 15:46:58.000000 google-cloud-artifact-registry-1.8.2/google/cloud/artifactregistry_v1beta2/services/artifact_registry/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:50:23.036056 google-cloud-artifact-registry-1.8.2/google/cloud/artifactregistry_v1beta2/services/artifact_registry/transports/
+-rw-rw-r--   0 root         (0)     1003     1428 2023-07-05 15:46:58.000000 google-cloud-artifact-registry-1.8.2/google/cloud/artifactregistry_v1beta2/services/artifact_registry/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003    22792 2023-07-05 15:46:58.000000 google-cloud-artifact-registry-1.8.2/google/cloud/artifactregistry_v1beta2/services/artifact_registry/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    42447 2023-07-05 15:46:58.000000 google-cloud-artifact-registry-1.8.2/google/cloud/artifactregistry_v1beta2/services/artifact_registry/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    43467 2023-07-05 15:46:58.000000 google-cloud-artifact-registry-1.8.2/google/cloud/artifactregistry_v1beta2/services/artifact_registry/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003   141462 2023-07-05 15:46:58.000000 google-cloud-artifact-registry-1.8.2/google/cloud/artifactregistry_v1beta2/services/artifact_registry/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:50:23.036056 google-cloud-artifact-registry-1.8.2/google/cloud/artifactregistry_v1beta2/types/
+-rw-rw-r--   0 root         (0)     1003     3141 2023-07-05 15:46:58.000000 google-cloud-artifact-registry-1.8.2/google/cloud/artifactregistry_v1beta2/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003     6209 2023-07-05 15:46:58.000000 google-cloud-artifact-registry-1.8.2/google/cloud/artifactregistry_v1beta2/types/apt_artifact.py
+-rw-rw-r--   0 root         (0)     1003     5727 2023-07-05 15:46:58.000000 google-cloud-artifact-registry-1.8.2/google/cloud/artifactregistry_v1beta2/types/file.py
+-rw-rw-r--   0 root         (0)     1003     4064 2023-07-05 15:46:58.000000 google-cloud-artifact-registry-1.8.2/google/cloud/artifactregistry_v1beta2/types/package.py
+-rw-rw-r--   0 root         (0)     1003    10058 2023-07-05 15:46:58.000000 google-cloud-artifact-registry-1.8.2/google/cloud/artifactregistry_v1beta2/types/repository.py
+-rw-rw-r--   0 root         (0)     1003     1017 2023-07-05 15:46:58.000000 google-cloud-artifact-registry-1.8.2/google/cloud/artifactregistry_v1beta2/types/service.py
+-rw-rw-r--   0 root         (0)     1003     3499 2023-07-05 15:46:58.000000 google-cloud-artifact-registry-1.8.2/google/cloud/artifactregistry_v1beta2/types/settings.py
+-rw-rw-r--   0 root         (0)     1003     5846 2023-07-05 15:46:58.000000 google-cloud-artifact-registry-1.8.2/google/cloud/artifactregistry_v1beta2/types/tag.py
+-rw-rw-r--   0 root         (0)     1003     6729 2023-07-05 15:46:58.000000 google-cloud-artifact-registry-1.8.2/google/cloud/artifactregistry_v1beta2/types/version.py
+-rw-rw-r--   0 root         (0)     1003     5697 2023-07-05 15:46:58.000000 google-cloud-artifact-registry-1.8.2/google/cloud/artifactregistry_v1beta2/types/yum_artifact.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:50:23.040056 google-cloud-artifact-registry-1.8.2/google_cloud_artifact_registry.egg-info/
+-rw-r--r--   0 root         (0)     1003     4914 2023-07-05 15:50:22.000000 google-cloud-artifact-registry-1.8.2/google_cloud_artifact_registry.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0)     1003     3986 2023-07-05 15:50:22.000000 google-cloud-artifact-registry-1.8.2/google_cloud_artifact_registry.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-07-05 15:50:22.000000 google-cloud-artifact-registry-1.8.2/google_cloud_artifact_registry.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0)     1003       20 2023-07-05 15:50:22.000000 google-cloud-artifact-registry-1.8.2/google_cloud_artifact_registry.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-07-05 15:50:22.000000 google-cloud-artifact-registry-1.8.2/google_cloud_artifact_registry.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0)     1003      352 2023-07-05 15:50:22.000000 google-cloud-artifact-registry-1.8.2/google_cloud_artifact_registry.egg-info/requires.txt
+-rw-r--r--   0 root         (0)     1003        7 2023-07-05 15:50:22.000000 google-cloud-artifact-registry-1.8.2/google_cloud_artifact_registry.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0)     1003       67 2023-07-05 15:50:23.044056 google-cloud-artifact-registry-1.8.2/setup.cfg
+-rw-rw-r--   0 root         (0)     1003     3008 2023-07-05 15:46:58.000000 google-cloud-artifact-registry-1.8.2/setup.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:50:23.040056 google-cloud-artifact-registry-1.8.2/tests/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:58.000000 google-cloud-artifact-registry-1.8.2/tests/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:50:23.040056 google-cloud-artifact-registry-1.8.2/tests/unit/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:58.000000 google-cloud-artifact-registry-1.8.2/tests/unit/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:50:23.040056 google-cloud-artifact-registry-1.8.2/tests/unit/gapic/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:58.000000 google-cloud-artifact-registry-1.8.2/tests/unit/gapic/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:50:23.040056 google-cloud-artifact-registry-1.8.2/tests/unit/gapic/artifactregistry_v1/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:58.000000 google-cloud-artifact-registry-1.8.2/tests/unit/gapic/artifactregistry_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003   755115 2023-07-05 15:46:58.000000 google-cloud-artifact-registry-1.8.2/tests/unit/gapic/artifactregistry_v1/test_artifact_registry.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:50:23.040056 google-cloud-artifact-registry-1.8.2/tests/unit/gapic/artifactregistry_v1beta2/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:58.000000 google-cloud-artifact-registry-1.8.2/tests/unit/gapic/artifactregistry_v1beta2/__init__.py
+-rw-rw-r--   0 root         (0)     1003   502969 2023-07-05 15:46:58.000000 google-cloud-artifact-registry-1.8.2/tests/unit/gapic/artifactregistry_v1beta2/test_artifact_registry.py
```

### Comparing `google-cloud-artifact-registry-1.8.1/LICENSE` & `google-cloud-artifact-registry-1.8.2/LICENSE`

 * *Files identical despite different names*

### Comparing `google-cloud-artifact-registry-1.8.1/MANIFEST.in` & `google-cloud-artifact-registry-1.8.2/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `google-cloud-artifact-registry-1.8.1/PKG-INFO` & `google-cloud-artifact-registry-1.8.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: google-cloud-artifact-registry
-Version: 1.8.1
+Version: 1.8.2
 Summary: Google Cloud Artifact Registry API client library
-Home-page: https://github.com/googleapis/python-artifact-registry
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
 
-Python Client for Artifact Registry API
-=======================================
+Python Client for Artifact Registry
+===================================
 
 |stable| |pypi| |versions|
 
-`Artifact Registry API`_: provides a single place for your organization to manage container images and language packages (such as Maven and npm). It is fully integrated with Google Cloud's tooling and runtimes and comes with support for native artifact protocols. This makes it simple to integrate it with your CI/CD tooling to set up automated pipelines.
+`Artifact Registry`_: provides a single place for your organization to manage container images and language packages (such as Maven and npm). It is fully integrated with Google Cloud's tooling and runtimes and comes with support for native artifact protocols. This makes it simple to integrate it with your CI/CD tooling to set up automated pipelines.
 
 - `Client Library Documentation`_
 - `Product Documentation`_
 
 .. |stable| image:: https://img.shields.io/badge/support-stable-gold.svg
    :target: https://github.com/googleapis/google-cloud-python/blob/main/README.rst#stability-levels
 .. |pypi| image:: https://img.shields.io/pypi/v/google-cloud-artifact-registry.svg
    :target: https://pypi.org/project/google-cloud-artifact-registry/
 .. |versions| image:: https://img.shields.io/pypi/pyversions/google-cloud-artifact-registry.svg
    :target: https://pypi.org/project/google-cloud-artifact-registry/
-.. _Artifact Registry API: https://cloud.google.com/artifact-registry
+.. _Artifact Registry: https://cloud.google.com/artifact-registry
 .. _Client Library Documentation: https://cloud.google.com/python/docs/reference/artifactregistry/latest
 .. _Product Documentation:  https://cloud.google.com/artifact-registry
 
 Quick Start
 -----------
 
 In order to use this library, you first need to go through the following steps:
 
 1. `Select or create a Cloud Platform project.`_
 2. `Enable billing for your project.`_
-3. `Enable the Artifact Registry API.`_
+3. `Enable the Artifact Registry.`_
 4. `Setup Authentication.`_
 
 .. _Select or create a Cloud Platform project.: https://console.cloud.google.com/project
 .. _Enable billing for your project.: https://cloud.google.com/billing/docs/how-to/modify-project#enable_billing_for_a_project
-.. _Enable the Artifact Registry API.:  https://cloud.google.com/artifact-registry
+.. _Enable the Artifact Registry.:  https://cloud.google.com/artifact-registry
 .. _Setup Authentication.: https://googleapis.dev/python/google-api-core/latest/auth.html
 
 Installation
 ~~~~~~~~~~~~
 
 Install this library in a `virtualenv`_ using pip. `virtualenv`_ is a tool to
 create isolated Python environments. The basic problem it addresses is one of
@@ -116,16 +116,16 @@
     virtualenv <your-env>
     <your-env>\Scripts\activate
     <your-env>\Scripts\pip.exe install google-cloud-artifact-registry
 
 Next Steps
 ~~~~~~~~~~
 
--  Read the `Client Library Documentation`_ for Artifact Registry API
+-  Read the `Client Library Documentation`_ for Artifact Registry
    to see other available methods on the client.
--  Read the `Artifact Registry API Product documentation`_ to learn
+-  Read the `Artifact Registry Product documentation`_ to learn
    more about the product and see How-to Guides.
 -  View this `README`_ to see the full list of Cloud
    APIs that we cover.
 
-.. _Artifact Registry API Product documentation:  https://cloud.google.com/artifact-registry
+.. _Artifact Registry Product documentation:  https://cloud.google.com/artifact-registry
 .. _README: https://github.com/googleapis/google-cloud-python/blob/main/README.rst
```

### Comparing `google-cloud-artifact-registry-1.8.1/README.rst` & `google-cloud-artifact-registry-1.8.2/README.rst`

 * *Files 10% similar despite different names*

```diff
@@ -1,40 +1,40 @@
-Python Client for Artifact Registry API
-=======================================
+Python Client for Artifact Registry
+===================================
 
 |stable| |pypi| |versions|
 
-`Artifact Registry API`_: provides a single place for your organization to manage container images and language packages (such as Maven and npm). It is fully integrated with Google Cloud's tooling and runtimes and comes with support for native artifact protocols. This makes it simple to integrate it with your CI/CD tooling to set up automated pipelines.
+`Artifact Registry`_: provides a single place for your organization to manage container images and language packages (such as Maven and npm). It is fully integrated with Google Cloud's tooling and runtimes and comes with support for native artifact protocols. This makes it simple to integrate it with your CI/CD tooling to set up automated pipelines.
 
 - `Client Library Documentation`_
 - `Product Documentation`_
 
 .. |stable| image:: https://img.shields.io/badge/support-stable-gold.svg
    :target: https://github.com/googleapis/google-cloud-python/blob/main/README.rst#stability-levels
 .. |pypi| image:: https://img.shields.io/pypi/v/google-cloud-artifact-registry.svg
    :target: https://pypi.org/project/google-cloud-artifact-registry/
 .. |versions| image:: https://img.shields.io/pypi/pyversions/google-cloud-artifact-registry.svg
    :target: https://pypi.org/project/google-cloud-artifact-registry/
-.. _Artifact Registry API: https://cloud.google.com/artifact-registry
+.. _Artifact Registry: https://cloud.google.com/artifact-registry
 .. _Client Library Documentation: https://cloud.google.com/python/docs/reference/artifactregistry/latest
 .. _Product Documentation:  https://cloud.google.com/artifact-registry
 
 Quick Start
 -----------
 
 In order to use this library, you first need to go through the following steps:
 
 1. `Select or create a Cloud Platform project.`_
 2. `Enable billing for your project.`_
-3. `Enable the Artifact Registry API.`_
+3. `Enable the Artifact Registry.`_
 4. `Setup Authentication.`_
 
 .. _Select or create a Cloud Platform project.: https://console.cloud.google.com/project
 .. _Enable billing for your project.: https://cloud.google.com/billing/docs/how-to/modify-project#enable_billing_for_a_project
-.. _Enable the Artifact Registry API.:  https://cloud.google.com/artifact-registry
+.. _Enable the Artifact Registry.:  https://cloud.google.com/artifact-registry
 .. _Setup Authentication.: https://googleapis.dev/python/google-api-core/latest/auth.html
 
 Installation
 ~~~~~~~~~~~~
 
 Install this library in a `virtualenv`_ using pip. `virtualenv`_ is a tool to
 create isolated Python environments. The basic problem it addresses is one of
@@ -92,16 +92,16 @@
     virtualenv <your-env>
     <your-env>\Scripts\activate
     <your-env>\Scripts\pip.exe install google-cloud-artifact-registry
 
 Next Steps
 ~~~~~~~~~~
 
--  Read the `Client Library Documentation`_ for Artifact Registry API
+-  Read the `Client Library Documentation`_ for Artifact Registry
    to see other available methods on the client.
--  Read the `Artifact Registry API Product documentation`_ to learn
+-  Read the `Artifact Registry Product documentation`_ to learn
    more about the product and see How-to Guides.
 -  View this `README`_ to see the full list of Cloud
    APIs that we cover.
 
-.. _Artifact Registry API Product documentation:  https://cloud.google.com/artifact-registry
+.. _Artifact Registry Product documentation:  https://cloud.google.com/artifact-registry
 .. _README: https://github.com/googleapis/google-cloud-python/blob/main/README.rst
```

### Comparing `google-cloud-artifact-registry-1.8.1/google/cloud/artifactregistry/__init__.py` & `google-cloud-artifact-registry-1.8.2/google/cloud/artifactregistry/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-artifact-registry-1.8.1/google/cloud/artifactregistry/gapic_version.py` & `google-cloud-artifact-registry-1.8.2/google/cloud/artifactregistry/gapic_version.py`

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

### Comparing `google-cloud-artifact-registry-1.8.1/google/cloud/artifactregistry_v1/__init__.py` & `google-cloud-artifact-registry-1.8.2/google/cloud/artifactregistry_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-artifact-registry-1.8.1/google/cloud/artifactregistry_v1/gapic_metadata.json` & `google-cloud-artifact-registry-1.8.2/google/cloud/artifactregistry_v1/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-cloud-artifact-registry-1.8.1/google/cloud/artifactregistry_v1/gapic_version.py` & `google-cloud-artifact-registry-1.8.2/google/cloud/artifactregistry_v1/gapic_version.py`

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

### Comparing `google-cloud-artifact-registry-1.8.1/google/cloud/artifactregistry_v1/services/__init__.py` & `google-cloud-artifact-registry-1.8.2/google/cloud/artifactregistry_v1/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-artifact-registry-1.8.1/google/cloud/artifactregistry_v1/services/artifact_registry/__init__.py` & `google-cloud-artifact-registry-1.8.2/google/cloud/artifactregistry_v1/services/artifact_registry/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-artifact-registry-1.8.1/google/cloud/artifactregistry_v1/services/artifact_registry/async_client.py` & `google-cloud-artifact-registry-1.8.2/google/cloud/artifactregistry_v1/services/artifact_registry/async_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -4311,15 +4311,15 @@
             timeout=timeout,
             metadata=metadata,
         )
 
         # Done; return the response.
         return response
 
-    async def __aenter__(self):
+    async def __aenter__(self) -> "ArtifactRegistryAsyncClient":
         return self
 
     async def __aexit__(self, exc_type, exc, tb):
         await self.transport.close()
 
 
 DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
```

### Comparing `google-cloud-artifact-registry-1.8.1/google/cloud/artifactregistry_v1/services/artifact_registry/client.py` & `google-cloud-artifact-registry-1.8.2/google/cloud/artifactregistry_v1/services/artifact_registry/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-artifact-registry-1.8.1/google/cloud/artifactregistry_v1/services/artifact_registry/pagers.py` & `google-cloud-artifact-registry-1.8.2/google/cloud/artifactregistry_v1/services/artifact_registry/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-artifact-registry-1.8.1/google/cloud/artifactregistry_v1/services/artifact_registry/transports/__init__.py` & `google-cloud-artifact-registry-1.8.2/google/cloud/artifactregistry_v1/services/artifact_registry/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-artifact-registry-1.8.1/google/cloud/artifactregistry_v1/services/artifact_registry/transports/base.py` & `google-cloud-artifact-registry-1.8.2/google/cloud/artifactregistry_v1/services/artifact_registry/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-artifact-registry-1.8.1/google/cloud/artifactregistry_v1/services/artifact_registry/transports/grpc.py` & `google-cloud-artifact-registry-1.8.2/google/cloud/artifactregistry_v1/services/artifact_registry/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-artifact-registry-1.8.1/google/cloud/artifactregistry_v1/services/artifact_registry/transports/grpc_asyncio.py` & `google-cloud-artifact-registry-1.8.2/google/cloud/artifactregistry_v1/services/artifact_registry/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-artifact-registry-1.8.1/google/cloud/artifactregistry_v1/services/artifact_registry/transports/rest.py` & `google-cloud-artifact-registry-1.8.2/google/cloud/artifactregistry_v1/services/artifact_registry/transports/rest.py`

 * *Files identical despite different names*

### Comparing `google-cloud-artifact-registry-1.8.1/google/cloud/artifactregistry_v1/types/__init__.py` & `google-cloud-artifact-registry-1.8.2/google/cloud/artifactregistry_v1/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-artifact-registry-1.8.1/google/cloud/artifactregistry_v1/types/apt_artifact.py` & `google-cloud-artifact-registry-1.8.2/google/cloud/artifactregistry_v1/types/apt_artifact.py`

 * *Files identical despite different names*

### Comparing `google-cloud-artifact-registry-1.8.1/google/cloud/artifactregistry_v1/types/artifact.py` & `google-cloud-artifact-registry-1.8.2/google/cloud/artifactregistry_v1/types/artifact.py`

 * *Files identical despite different names*

### Comparing `google-cloud-artifact-registry-1.8.1/google/cloud/artifactregistry_v1/types/file.py` & `google-cloud-artifact-registry-1.8.2/google/cloud/artifactregistry_v1/types/file.py`

 * *Files identical despite different names*

### Comparing `google-cloud-artifact-registry-1.8.1/google/cloud/artifactregistry_v1/types/package.py` & `google-cloud-artifact-registry-1.8.2/google/cloud/artifactregistry_v1/types/package.py`

 * *Files identical despite different names*

### Comparing `google-cloud-artifact-registry-1.8.1/google/cloud/artifactregistry_v1/types/repository.py` & `google-cloud-artifact-registry-1.8.2/google/cloud/artifactregistry_v1/types/repository.py`

 * *Files identical despite different names*

### Comparing `google-cloud-artifact-registry-1.8.1/google/cloud/artifactregistry_v1/types/service.py` & `google-cloud-artifact-registry-1.8.2/google/cloud/artifactregistry_v1/types/service.py`

 * *Files identical despite different names*

### Comparing `google-cloud-artifact-registry-1.8.1/google/cloud/artifactregistry_v1/types/settings.py` & `google-cloud-artifact-registry-1.8.2/google/cloud/artifactregistry_v1/types/settings.py`

 * *Files identical despite different names*

### Comparing `google-cloud-artifact-registry-1.8.1/google/cloud/artifactregistry_v1/types/tag.py` & `google-cloud-artifact-registry-1.8.2/google/cloud/artifactregistry_v1/types/tag.py`

 * *Files identical despite different names*

### Comparing `google-cloud-artifact-registry-1.8.1/google/cloud/artifactregistry_v1/types/version.py` & `google-cloud-artifact-registry-1.8.2/google/cloud/artifactregistry_v1/types/version.py`

 * *Files identical despite different names*

### Comparing `google-cloud-artifact-registry-1.8.1/google/cloud/artifactregistry_v1/types/vpcsc_config.py` & `google-cloud-artifact-registry-1.8.2/google/cloud/artifactregistry_v1/types/vpcsc_config.py`

 * *Files identical despite different names*

### Comparing `google-cloud-artifact-registry-1.8.1/google/cloud/artifactregistry_v1/types/yum_artifact.py` & `google-cloud-artifact-registry-1.8.2/google/cloud/artifactregistry_v1/types/yum_artifact.py`

 * *Files identical despite different names*

### Comparing `google-cloud-artifact-registry-1.8.1/google/cloud/artifactregistry_v1beta2/__init__.py` & `google-cloud-artifact-registry-1.8.2/google/cloud/artifactregistry_v1beta2/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-artifact-registry-1.8.1/google/cloud/artifactregistry_v1beta2/gapic_metadata.json` & `google-cloud-artifact-registry-1.8.2/google/cloud/artifactregistry_v1beta2/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-cloud-artifact-registry-1.8.1/google/cloud/artifactregistry_v1beta2/gapic_version.py` & `google-cloud-artifact-registry-1.8.2/google/cloud/artifactregistry_v1beta2/gapic_version.py`

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

### Comparing `google-cloud-artifact-registry-1.8.1/google/cloud/artifactregistry_v1beta2/services/__init__.py` & `google-cloud-artifact-registry-1.8.2/google/cloud/artifactregistry_v1beta2/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-artifact-registry-1.8.1/google/cloud/artifactregistry_v1beta2/services/artifact_registry/__init__.py` & `google-cloud-artifact-registry-1.8.2/google/cloud/artifactregistry_v1beta2/services/artifact_registry/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-artifact-registry-1.8.1/google/cloud/artifactregistry_v1beta2/services/artifact_registry/async_client.py` & `google-cloud-artifact-registry-1.8.2/google/cloud/artifactregistry_v1beta2/services/artifact_registry/async_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -3277,15 +3277,15 @@
             timeout=timeout,
             metadata=metadata,
         )
 
         # Done; return the response.
         return response
 
-    async def __aenter__(self):
+    async def __aenter__(self) -> "ArtifactRegistryAsyncClient":
         return self
 
     async def __aexit__(self, exc_type, exc, tb):
         await self.transport.close()
 
 
 DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
```

### Comparing `google-cloud-artifact-registry-1.8.1/google/cloud/artifactregistry_v1beta2/services/artifact_registry/client.py` & `google-cloud-artifact-registry-1.8.2/google/cloud/artifactregistry_v1beta2/services/artifact_registry/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-artifact-registry-1.8.1/google/cloud/artifactregistry_v1beta2/services/artifact_registry/pagers.py` & `google-cloud-artifact-registry-1.8.2/google/cloud/artifactregistry_v1beta2/services/artifact_registry/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-artifact-registry-1.8.1/google/cloud/artifactregistry_v1beta2/services/artifact_registry/transports/__init__.py` & `google-cloud-artifact-registry-1.8.2/google/cloud/artifactregistry_v1beta2/services/artifact_registry/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-artifact-registry-1.8.1/google/cloud/artifactregistry_v1beta2/services/artifact_registry/transports/base.py` & `google-cloud-artifact-registry-1.8.2/google/cloud/artifactregistry_v1beta2/services/artifact_registry/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-artifact-registry-1.8.1/google/cloud/artifactregistry_v1beta2/services/artifact_registry/transports/grpc.py` & `google-cloud-artifact-registry-1.8.2/google/cloud/artifactregistry_v1beta2/services/artifact_registry/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-artifact-registry-1.8.1/google/cloud/artifactregistry_v1beta2/services/artifact_registry/transports/grpc_asyncio.py` & `google-cloud-artifact-registry-1.8.2/google/cloud/artifactregistry_v1beta2/services/artifact_registry/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-artifact-registry-1.8.1/google/cloud/artifactregistry_v1beta2/services/artifact_registry/transports/rest.py` & `google-cloud-artifact-registry-1.8.2/google/cloud/artifactregistry_v1beta2/services/artifact_registry/transports/rest.py`

 * *Files identical despite different names*

### Comparing `google-cloud-artifact-registry-1.8.1/google/cloud/artifactregistry_v1beta2/types/__init__.py` & `google-cloud-artifact-registry-1.8.2/google/cloud/artifactregistry_v1beta2/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-artifact-registry-1.8.1/google/cloud/artifactregistry_v1beta2/types/apt_artifact.py` & `google-cloud-artifact-registry-1.8.2/google/cloud/artifactregistry_v1beta2/types/apt_artifact.py`

 * *Files identical despite different names*

### Comparing `google-cloud-artifact-registry-1.8.1/google/cloud/artifactregistry_v1beta2/types/file.py` & `google-cloud-artifact-registry-1.8.2/google/cloud/artifactregistry_v1beta2/types/file.py`

 * *Files identical despite different names*

### Comparing `google-cloud-artifact-registry-1.8.1/google/cloud/artifactregistry_v1beta2/types/package.py` & `google-cloud-artifact-registry-1.8.2/google/cloud/artifactregistry_v1beta2/types/package.py`

 * *Files identical despite different names*

### Comparing `google-cloud-artifact-registry-1.8.1/google/cloud/artifactregistry_v1beta2/types/repository.py` & `google-cloud-artifact-registry-1.8.2/google/cloud/artifactregistry_v1beta2/types/repository.py`

 * *Files identical despite different names*

### Comparing `google-cloud-artifact-registry-1.8.1/google/cloud/artifactregistry_v1beta2/types/service.py` & `google-cloud-artifact-registry-1.8.2/google/cloud/artifactregistry_v1beta2/types/service.py`

 * *Files identical despite different names*

### Comparing `google-cloud-artifact-registry-1.8.1/google/cloud/artifactregistry_v1beta2/types/settings.py` & `google-cloud-artifact-registry-1.8.2/google/cloud/artifactregistry_v1beta2/types/settings.py`

 * *Files identical despite different names*

### Comparing `google-cloud-artifact-registry-1.8.1/google/cloud/artifactregistry_v1beta2/types/tag.py` & `google-cloud-artifact-registry-1.8.2/google/cloud/artifactregistry_v1beta2/types/tag.py`

 * *Files identical despite different names*

### Comparing `google-cloud-artifact-registry-1.8.1/google/cloud/artifactregistry_v1beta2/types/version.py` & `google-cloud-artifact-registry-1.8.2/google/cloud/artifactregistry_v1beta2/types/version.py`

 * *Files identical despite different names*

### Comparing `google-cloud-artifact-registry-1.8.1/google/cloud/artifactregistry_v1beta2/types/yum_artifact.py` & `google-cloud-artifact-registry-1.8.2/google/cloud/artifactregistry_v1beta2/types/yum_artifact.py`

 * *Files identical despite different names*

### Comparing `google-cloud-artifact-registry-1.8.1/google_cloud_artifact_registry.egg-info/PKG-INFO` & `google-cloud-artifact-registry-1.8.2/google_cloud_artifact_registry.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: google-cloud-artifact-registry
-Version: 1.8.1
+Version: 1.8.2
 Summary: Google Cloud Artifact Registry API client library
-Home-page: https://github.com/googleapis/python-artifact-registry
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
 
-Python Client for Artifact Registry API
-=======================================
+Python Client for Artifact Registry
+===================================
 
 |stable| |pypi| |versions|
 
-`Artifact Registry API`_: provides a single place for your organization to manage container images and language packages (such as Maven and npm). It is fully integrated with Google Cloud's tooling and runtimes and comes with support for native artifact protocols. This makes it simple to integrate it with your CI/CD tooling to set up automated pipelines.
+`Artifact Registry`_: provides a single place for your organization to manage container images and language packages (such as Maven and npm). It is fully integrated with Google Cloud's tooling and runtimes and comes with support for native artifact protocols. This makes it simple to integrate it with your CI/CD tooling to set up automated pipelines.
 
 - `Client Library Documentation`_
 - `Product Documentation`_
 
 .. |stable| image:: https://img.shields.io/badge/support-stable-gold.svg
    :target: https://github.com/googleapis/google-cloud-python/blob/main/README.rst#stability-levels
 .. |pypi| image:: https://img.shields.io/pypi/v/google-cloud-artifact-registry.svg
    :target: https://pypi.org/project/google-cloud-artifact-registry/
 .. |versions| image:: https://img.shields.io/pypi/pyversions/google-cloud-artifact-registry.svg
    :target: https://pypi.org/project/google-cloud-artifact-registry/
-.. _Artifact Registry API: https://cloud.google.com/artifact-registry
+.. _Artifact Registry: https://cloud.google.com/artifact-registry
 .. _Client Library Documentation: https://cloud.google.com/python/docs/reference/artifactregistry/latest
 .. _Product Documentation:  https://cloud.google.com/artifact-registry
 
 Quick Start
 -----------
 
 In order to use this library, you first need to go through the following steps:
 
 1. `Select or create a Cloud Platform project.`_
 2. `Enable billing for your project.`_
-3. `Enable the Artifact Registry API.`_
+3. `Enable the Artifact Registry.`_
 4. `Setup Authentication.`_
 
 .. _Select or create a Cloud Platform project.: https://console.cloud.google.com/project
 .. _Enable billing for your project.: https://cloud.google.com/billing/docs/how-to/modify-project#enable_billing_for_a_project
-.. _Enable the Artifact Registry API.:  https://cloud.google.com/artifact-registry
+.. _Enable the Artifact Registry.:  https://cloud.google.com/artifact-registry
 .. _Setup Authentication.: https://googleapis.dev/python/google-api-core/latest/auth.html
 
 Installation
 ~~~~~~~~~~~~
 
 Install this library in a `virtualenv`_ using pip. `virtualenv`_ is a tool to
 create isolated Python environments. The basic problem it addresses is one of
@@ -116,16 +116,16 @@
     virtualenv <your-env>
     <your-env>\Scripts\activate
     <your-env>\Scripts\pip.exe install google-cloud-artifact-registry
 
 Next Steps
 ~~~~~~~~~~
 
--  Read the `Client Library Documentation`_ for Artifact Registry API
+-  Read the `Client Library Documentation`_ for Artifact Registry
    to see other available methods on the client.
--  Read the `Artifact Registry API Product documentation`_ to learn
+-  Read the `Artifact Registry Product documentation`_ to learn
    more about the product and see How-to Guides.
 -  View this `README`_ to see the full list of Cloud
    APIs that we cover.
 
-.. _Artifact Registry API Product documentation:  https://cloud.google.com/artifact-registry
+.. _Artifact Registry Product documentation:  https://cloud.google.com/artifact-registry
 .. _README: https://github.com/googleapis/google-cloud-python/blob/main/README.rst
```

### Comparing `google-cloud-artifact-registry-1.8.1/google_cloud_artifact_registry.egg-info/SOURCES.txt` & `google-cloud-artifact-registry-1.8.2/google_cloud_artifact_registry.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `google-cloud-artifact-registry-1.8.1/setup.py` & `google-cloud-artifact-registry-1.8.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 dependencies = [
     "google-api-core[grpc] >= 1.34.0, <3.0.0dev,!=2.0.*,!=2.1.*,!=2.2.*,!=2.3.*,!=2.4.*,!=2.5.*,!=2.6.*,!=2.7.*,!=2.8.*,!=2.9.*,!=2.10.*",
     "proto-plus >= 1.22.0, <2.0.0dev",
     "proto-plus >= 1.22.2, <2.0.0dev; python_version>='3.11'",
     "protobuf>=3.19.5,<5.0.0dev,!=3.20.0,!=3.20.1,!=4.21.0,!=4.21.1,!=4.21.2,!=4.21.3,!=4.21.4,!=4.21.5",
     "grpc-google-iam-v1 >= 0.12.4, <1.0.0dev",
 ]
-url = "https://github.com/googleapis/python-artifact-registry"
+url = "https://github.com/googleapis/google-cloud-python"
 
 package_root = os.path.abspath(os.path.dirname(__file__))
 
 readme_filename = os.path.join(package_root, "README.rst")
 with io.open(readme_filename, encoding="utf-8") as readme_file:
     readme = readme_file.read()
```

### Comparing `google-cloud-artifact-registry-1.8.1/tests/__init__.py` & `google-cloud-artifact-registry-1.8.2/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-artifact-registry-1.8.1/tests/unit/__init__.py` & `google-cloud-artifact-registry-1.8.2/tests/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-artifact-registry-1.8.1/tests/unit/gapic/__init__.py` & `google-cloud-artifact-registry-1.8.2/tests/unit/gapic/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-artifact-registry-1.8.1/tests/unit/gapic/artifactregistry_v1/__init__.py` & `google-cloud-artifact-registry-1.8.2/tests/unit/gapic/artifactregistry_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-artifact-registry-1.8.1/tests/unit/gapic/artifactregistry_v1/test_artifact_registry.py` & `google-cloud-artifact-registry-1.8.2/tests/unit/gapic/artifactregistry_v1/test_artifact_registry.py`

 * *Files 1% similar despite different names*

```diff
@@ -1193,17 +1193,19 @@
                     artifact.DockerImage(),
                     artifact.DockerImage(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.list_docker_images(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
@@ -1883,17 +1885,19 @@
                     artifact.MavenArtifact(),
                     artifact.MavenArtifact(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.list_maven_artifacts(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
@@ -2587,17 +2591,19 @@
                     artifact.NpmPackage(),
                     artifact.NpmPackage(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.list_npm_packages(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
@@ -3269,17 +3275,19 @@
                     artifact.PythonPackage(),
                     artifact.PythonPackage(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.list_python_packages(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
@@ -4277,17 +4285,19 @@
                     repository.Repository(),
                     repository.Repository(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.list_repositories(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
@@ -4310,17 +4320,14 @@
     with mock.patch.object(type(client.transport.get_repository), "__call__") as call:
         # Designate an appropriate return value for the call.
         call.return_value = repository.Repository(
             name="name_value",
             format_=repository.Repository.Format.DOCKER,
             description="description_value",
             kms_key_name="kms_key_name_value",
-            maven_config=repository.Repository.MavenRepositoryConfig(
-                allow_snapshot_overwrites=True
-            ),
         )
         response = client.get_repository(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
         assert args[0] == repository.GetRepositoryRequest()
@@ -4843,17 +4850,14 @@
     ) as call:
         # Designate an appropriate return value for the call.
         call.return_value = gda_repository.Repository(
             name="name_value",
             format_=gda_repository.Repository.Format.DOCKER,
             description="description_value",
             kms_key_name="kms_key_name_value",
-            maven_config=gda_repository.Repository.MavenRepositoryConfig(
-                allow_snapshot_overwrites=True
-            ),
         )
         response = client.update_repository(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
         assert args[0] == gda_repository.UpdateRepositoryRequest()
@@ -5763,17 +5767,19 @@
                     package.Package(),
                     package.Package(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.list_packages(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
@@ -6641,17 +6647,19 @@
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
@@ -7519,17 +7527,19 @@
                     file.File(),
                     file.File(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.list_files(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
@@ -8175,17 +8185,19 @@
                     tag.Tag(),
                     tag.Tag(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.list_tags(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
@@ -13770,17 +13782,14 @@
     with mock.patch.object(type(client.transport._session), "request") as req:
         # Designate an appropriate value for the returned response.
         return_value = repository.Repository(
             name="name_value",
             format_=repository.Repository.Format.DOCKER,
             description="description_value",
             kms_key_name="kms_key_name_value",
-            maven_config=repository.Repository.MavenRepositoryConfig(
-                allow_snapshot_overwrites=True
-            ),
         )
 
         # Wrap the value into a proper Response obj
         response_value = Response()
         response_value.status_code = 200
         pb_return_value = repository.Repository.pb(return_value)
         json_return_value = json_format.MessageToJson(pb_return_value)
@@ -14361,17 +14370,14 @@
     with mock.patch.object(type(client.transport._session), "request") as req:
         # Designate an appropriate value for the returned response.
         return_value = gda_repository.Repository(
             name="name_value",
             format_=gda_repository.Repository.Format.DOCKER,
             description="description_value",
             kms_key_name="kms_key_name_value",
-            maven_config=gda_repository.Repository.MavenRepositoryConfig(
-                allow_snapshot_overwrites=True
-            ),
         )
 
         # Wrap the value into a proper Response obj
         response_value = Response()
         response_value.status_code = 200
         pb_return_value = gda_repository.Repository.pb(return_value)
         json_return_value = json_format.MessageToJson(pb_return_value)
```

### Comparing `google-cloud-artifact-registry-1.8.1/tests/unit/gapic/artifactregistry_v1beta2/__init__.py` & `google-cloud-artifact-registry-1.8.2/tests/unit/gapic/artifactregistry_v1beta2/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-artifact-registry-1.8.1/tests/unit/gapic/artifactregistry_v1beta2/test_artifact_registry.py` & `google-cloud-artifact-registry-1.8.2/tests/unit/gapic/artifactregistry_v1beta2/test_artifact_registry.py`

 * *Files 1% similar despite different names*

```diff
@@ -1498,17 +1498,19 @@
                     repository.Repository(),
                     repository.Repository(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.list_repositories(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
@@ -1531,17 +1533,14 @@
     with mock.patch.object(type(client.transport.get_repository), "__call__") as call:
         # Designate an appropriate return value for the call.
         call.return_value = repository.Repository(
             name="name_value",
             format_=repository.Repository.Format.DOCKER,
             description="description_value",
             kms_key_name="kms_key_name_value",
-            maven_config=repository.Repository.MavenRepositoryConfig(
-                allow_snapshot_overwrites=True
-            ),
         )
         response = client.get_repository(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
         assert args[0] == repository.GetRepositoryRequest()
@@ -2064,17 +2063,14 @@
     ) as call:
         # Designate an appropriate return value for the call.
         call.return_value = gda_repository.Repository(
             name="name_value",
             format_=gda_repository.Repository.Format.DOCKER,
             description="description_value",
             kms_key_name="kms_key_name_value",
-            maven_config=gda_repository.Repository.MavenRepositoryConfig(
-                allow_snapshot_overwrites=True
-            ),
         )
         response = client.update_repository(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
         assert args[0] == gda_repository.UpdateRepositoryRequest()
@@ -2984,17 +2980,19 @@
                     package.Package(),
                     package.Package(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.list_packages(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
@@ -3862,17 +3860,19 @@
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
@@ -4740,17 +4740,19 @@
                     file.File(),
                     file.File(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.list_files(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
@@ -5396,17 +5398,19 @@
                     tag.Tag(),
                     tag.Tag(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.list_tags(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
@@ -8004,17 +8008,14 @@
     with mock.patch.object(type(client.transport._session), "request") as req:
         # Designate an appropriate value for the returned response.
         return_value = repository.Repository(
             name="name_value",
             format_=repository.Repository.Format.DOCKER,
             description="description_value",
             kms_key_name="kms_key_name_value",
-            maven_config=repository.Repository.MavenRepositoryConfig(
-                allow_snapshot_overwrites=True
-            ),
         )
 
         # Wrap the value into a proper Response obj
         response_value = Response()
         response_value.status_code = 200
         pb_return_value = repository.Repository.pb(return_value)
         json_return_value = json_format.MessageToJson(pb_return_value)
@@ -8595,17 +8596,14 @@
     with mock.patch.object(type(client.transport._session), "request") as req:
         # Designate an appropriate value for the returned response.
         return_value = gda_repository.Repository(
             name="name_value",
             format_=gda_repository.Repository.Format.DOCKER,
             description="description_value",
             kms_key_name="kms_key_name_value",
-            maven_config=gda_repository.Repository.MavenRepositoryConfig(
-                allow_snapshot_overwrites=True
-            ),
         )
 
         # Wrap the value into a proper Response obj
         response_value = Response()
         response_value.status_code = 200
         pb_return_value = gda_repository.Repository.pb(return_value)
         json_return_value = json_format.MessageToJson(pb_return_value)
```

