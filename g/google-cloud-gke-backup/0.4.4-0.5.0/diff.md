# Comparing `tmp/google-cloud-gke-backup-0.4.4.tar.gz` & `tmp/google-cloud-gke-backup-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-cloud-gke-backup-0.4.4.tar", last modified: Tue Jun 13 15:00:12 2023, max compression
+gzip compressed data, was "google-cloud-gke-backup-0.5.0.tar", last modified: Wed Jul  5 15:21:41 2023, max compression
```

## Comparing `google-cloud-gke-backup-0.4.4.tar` & `google-cloud-gke-backup-0.5.0.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-13 15:00:12.254714 google-cloud-gke-backup-0.4.4/
--rw-rw-r--   0 root         (0)     1003    11358 2023-06-13 14:58:11.000000 google-cloud-gke-backup-0.4.4/LICENSE
--rw-rw-r--   0 root         (0)     1003      860 2023-06-13 14:58:11.000000 google-cloud-gke-backup-0.4.4/MANIFEST.in
--rw-r--r--   0 root         (0)     1003     4778 2023-06-13 15:00:12.254714 google-cloud-gke-backup-0.4.4/PKG-INFO
--rw-rw-r--   0 root         (0)     1003     3866 2023-06-13 14:58:11.000000 google-cloud-gke-backup-0.4.4/README.rst
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-13 15:00:12.242712 google-cloud-gke-backup-0.4.4/google/
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-13 15:00:12.242712 google-cloud-gke-backup-0.4.4/google/cloud/
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-13 15:00:12.246713 google-cloud-gke-backup-0.4.4/google/cloud/gke_backup/
--rw-rw-r--   0 root         (0)     1003     3498 2023-06-13 14:58:11.000000 google-cloud-gke-backup-0.4.4/google/cloud/gke_backup/__init__.py
--rw-rw-r--   0 root         (0)     1003      652 2023-06-13 14:58:11.000000 google-cloud-gke-backup-0.4.4/google/cloud/gke_backup/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       84 2023-06-13 14:58:11.000000 google-cloud-gke-backup-0.4.4/google/cloud/gke_backup/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-13 15:00:12.246713 google-cloud-gke-backup-0.4.4/google/cloud/gke_backup_v1/
--rw-rw-r--   0 root         (0)     1003     3181 2023-06-13 14:58:11.000000 google-cloud-gke-backup-0.4.4/google/cloud/gke_backup_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003     9647 2023-06-13 14:58:11.000000 google-cloud-gke-backup-0.4.4/google/cloud/gke_backup_v1/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003      652 2023-06-13 14:58:11.000000 google-cloud-gke-backup-0.4.4/google/cloud/gke_backup_v1/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       84 2023-06-13 14:58:11.000000 google-cloud-gke-backup-0.4.4/google/cloud/gke_backup_v1/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-13 15:00:12.246713 google-cloud-gke-backup-0.4.4/google/cloud/gke_backup_v1/services/
--rw-rw-r--   0 root         (0)     1003      600 2023-06-13 14:58:11.000000 google-cloud-gke-backup-0.4.4/google/cloud/gke_backup_v1/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-13 15:00:12.246713 google-cloud-gke-backup-0.4.4/google/cloud/gke_backup_v1/services/backup_for_gke/
--rw-rw-r--   0 root         (0)     1003      761 2023-06-13 14:58:11.000000 google-cloud-gke-backup-0.4.4/google/cloud/gke_backup_v1/services/backup_for_gke/__init__.py
--rw-rw-r--   0 root         (0)     1003   159833 2023-06-13 14:58:11.000000 google-cloud-gke-backup-0.4.4/google/cloud/gke_backup_v1/services/backup_for_gke/async_client.py
--rw-rw-r--   0 root         (0)     1003   173179 2023-06-13 14:58:11.000000 google-cloud-gke-backup-0.4.4/google/cloud/gke_backup_v1/services/backup_for_gke/client.py
--rw-rw-r--   0 root         (0)     1003    31038 2023-06-13 14:58:11.000000 google-cloud-gke-backup-0.4.4/google/cloud/gke_backup_v1/services/backup_for_gke/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-13 15:00:12.250713 google-cloud-gke-backup-0.4.4/google/cloud/gke_backup_v1/services/backup_for_gke/transports/
--rw-rw-r--   0 root         (0)     1003     1372 2023-06-13 14:58:11.000000 google-cloud-gke-backup-0.4.4/google/cloud/gke_backup_v1/services/backup_for_gke/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003    22951 2023-06-13 14:58:11.000000 google-cloud-gke-backup-0.4.4/google/cloud/gke_backup_v1/services/backup_for_gke/transports/base.py
--rw-rw-r--   0 root         (0)     1003    46982 2023-06-13 14:58:11.000000 google-cloud-gke-backup-0.4.4/google/cloud/gke_backup_v1/services/backup_for_gke/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    47961 2023-06-13 14:58:11.000000 google-cloud-gke-backup-0.4.4/google/cloud/gke_backup_v1/services/backup_for_gke/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003   166853 2023-06-13 14:58:11.000000 google-cloud-gke-backup-0.4.4/google/cloud/gke_backup_v1/services/backup_for_gke/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-13 15:00:12.250713 google-cloud-gke-backup-0.4.4/google/cloud/gke_backup_v1/types/
--rw-rw-r--   0 root         (0)     1003     2884 2023-06-13 14:58:11.000000 google-cloud-gke-backup-0.4.4/google/cloud/gke_backup_v1/types/__init__.py
--rw-rw-r--   0 root         (0)     1003    14215 2023-06-13 14:58:11.000000 google-cloud-gke-backup-0.4.4/google/cloud/gke_backup_v1/types/backup.py
--rw-rw-r--   0 root         (0)     1003    11959 2023-06-13 14:58:11.000000 google-cloud-gke-backup-0.4.4/google/cloud/gke_backup_v1/types/backup_plan.py
--rw-rw-r--   0 root         (0)     1003     2520 2023-06-13 14:58:11.000000 google-cloud-gke-backup-0.4.4/google/cloud/gke_backup_v1/types/common.py
--rw-rw-r--   0 root         (0)     1003    36417 2023-06-13 14:58:11.000000 google-cloud-gke-backup-0.4.4/google/cloud/gke_backup_v1/types/gkebackup.py
--rw-rw-r--   0 root         (0)     1003    22577 2023-06-13 14:58:11.000000 google-cloud-gke-backup-0.4.4/google/cloud/gke_backup_v1/types/restore.py
--rw-rw-r--   0 root         (0)     1003     4643 2023-06-13 14:58:11.000000 google-cloud-gke-backup-0.4.4/google/cloud/gke_backup_v1/types/restore_plan.py
--rw-rw-r--   0 root         (0)     1003    12236 2023-06-13 14:58:11.000000 google-cloud-gke-backup-0.4.4/google/cloud/gke_backup_v1/types/volume.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-13 15:00:12.254714 google-cloud-gke-backup-0.4.4/google_cloud_gke_backup.egg-info/
--rw-r--r--   0 root         (0)     1003     4778 2023-06-13 15:00:12.000000 google-cloud-gke-backup-0.4.4/google_cloud_gke_backup.egg-info/PKG-INFO
--rw-r--r--   0 root         (0)     1003     1851 2023-06-13 15:00:12.000000 google-cloud-gke-backup-0.4.4/google_cloud_gke_backup.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0)     1003        1 2023-06-13 15:00:12.000000 google-cloud-gke-backup-0.4.4/google_cloud_gke_backup.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0)     1003       20 2023-06-13 15:00:12.000000 google-cloud-gke-backup-0.4.4/google_cloud_gke_backup.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0)     1003        1 2023-06-13 15:00:12.000000 google-cloud-gke-backup-0.4.4/google_cloud_gke_backup.egg-info/not-zip-safe
--rw-r--r--   0 root         (0)     1003      352 2023-06-13 15:00:12.000000 google-cloud-gke-backup-0.4.4/google_cloud_gke_backup.egg-info/requires.txt
--rw-r--r--   0 root         (0)     1003        7 2023-06-13 15:00:12.000000 google-cloud-gke-backup-0.4.4/google_cloud_gke_backup.egg-info/top_level.txt
--rw-rw-r--   0 root         (0)     1003       67 2023-06-13 15:00:12.254714 google-cloud-gke-backup-0.4.4/setup.cfg
--rw-rw-r--   0 root         (0)     1003     2980 2023-06-13 14:58:11.000000 google-cloud-gke-backup-0.4.4/setup.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-13 15:00:12.254714 google-cloud-gke-backup-0.4.4/tests/
--rw-rw-r--   0 root         (0)     1003      600 2023-06-13 14:58:11.000000 google-cloud-gke-backup-0.4.4/tests/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-13 15:00:12.254714 google-cloud-gke-backup-0.4.4/tests/unit/
--rw-rw-r--   0 root         (0)     1003      600 2023-06-13 14:58:11.000000 google-cloud-gke-backup-0.4.4/tests/unit/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-13 15:00:12.254714 google-cloud-gke-backup-0.4.4/tests/unit/gapic/
--rw-rw-r--   0 root         (0)     1003      600 2023-06-13 14:58:11.000000 google-cloud-gke-backup-0.4.4/tests/unit/gapic/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-13 15:00:12.254714 google-cloud-gke-backup-0.4.4/tests/unit/gapic/gke_backup_v1/
--rw-rw-r--   0 root         (0)     1003      600 2023-06-13 14:58:11.000000 google-cloud-gke-backup-0.4.4/tests/unit/gapic/gke_backup_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003   666141 2023-06-13 14:58:11.000000 google-cloud-gke-backup-0.4.4/tests/unit/gapic/gke_backup_v1/test_backup_for_gke.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:21:41.248927 google-cloud-gke-backup-0.5.0/
+-rw-rw-r--   0 root         (0)     1003    11358 2023-07-05 15:19:45.000000 google-cloud-gke-backup-0.5.0/LICENSE
+-rw-rw-r--   0 root         (0)     1003      860 2023-07-05 15:19:45.000000 google-cloud-gke-backup-0.5.0/MANIFEST.in
+-rw-r--r--   0 root         (0)     1003     4778 2023-07-05 15:21:41.248927 google-cloud-gke-backup-0.5.0/PKG-INFO
+-rw-rw-r--   0 root         (0)     1003     3866 2023-07-05 15:19:45.000000 google-cloud-gke-backup-0.5.0/README.rst
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:21:41.236929 google-cloud-gke-backup-0.5.0/google/
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:21:41.236929 google-cloud-gke-backup-0.5.0/google/cloud/
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:21:41.240929 google-cloud-gke-backup-0.5.0/google/cloud/gke_backup/
+-rw-rw-r--   0 root         (0)     1003     3498 2023-07-05 15:19:45.000000 google-cloud-gke-backup-0.5.0/google/cloud/gke_backup/__init__.py
+-rw-rw-r--   0 root         (0)     1003      652 2023-07-05 15:19:45.000000 google-cloud-gke-backup-0.5.0/google/cloud/gke_backup/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       84 2023-07-05 15:19:45.000000 google-cloud-gke-backup-0.5.0/google/cloud/gke_backup/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:21:41.240929 google-cloud-gke-backup-0.5.0/google/cloud/gke_backup_v1/
+-rw-rw-r--   0 root         (0)     1003     3181 2023-07-05 15:19:45.000000 google-cloud-gke-backup-0.5.0/google/cloud/gke_backup_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003     9647 2023-07-05 15:19:45.000000 google-cloud-gke-backup-0.5.0/google/cloud/gke_backup_v1/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      652 2023-07-05 15:19:45.000000 google-cloud-gke-backup-0.5.0/google/cloud/gke_backup_v1/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       84 2023-07-05 15:19:45.000000 google-cloud-gke-backup-0.5.0/google/cloud/gke_backup_v1/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:21:41.240929 google-cloud-gke-backup-0.5.0/google/cloud/gke_backup_v1/services/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:19:45.000000 google-cloud-gke-backup-0.5.0/google/cloud/gke_backup_v1/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:21:41.240929 google-cloud-gke-backup-0.5.0/google/cloud/gke_backup_v1/services/backup_for_gke/
+-rw-rw-r--   0 root         (0)     1003      761 2023-07-05 15:19:45.000000 google-cloud-gke-backup-0.5.0/google/cloud/gke_backup_v1/services/backup_for_gke/__init__.py
+-rw-rw-r--   0 root         (0)     1003   159862 2023-07-05 15:19:45.000000 google-cloud-gke-backup-0.5.0/google/cloud/gke_backup_v1/services/backup_for_gke/async_client.py
+-rw-rw-r--   0 root         (0)     1003   173179 2023-07-05 15:19:45.000000 google-cloud-gke-backup-0.5.0/google/cloud/gke_backup_v1/services/backup_for_gke/client.py
+-rw-rw-r--   0 root         (0)     1003    31038 2023-07-05 15:19:45.000000 google-cloud-gke-backup-0.5.0/google/cloud/gke_backup_v1/services/backup_for_gke/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:21:41.244928 google-cloud-gke-backup-0.5.0/google/cloud/gke_backup_v1/services/backup_for_gke/transports/
+-rw-rw-r--   0 root         (0)     1003     1372 2023-07-05 15:19:45.000000 google-cloud-gke-backup-0.5.0/google/cloud/gke_backup_v1/services/backup_for_gke/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003    22951 2023-07-05 15:19:45.000000 google-cloud-gke-backup-0.5.0/google/cloud/gke_backup_v1/services/backup_for_gke/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    46982 2023-07-05 15:19:45.000000 google-cloud-gke-backup-0.5.0/google/cloud/gke_backup_v1/services/backup_for_gke/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    47961 2023-07-05 15:19:45.000000 google-cloud-gke-backup-0.5.0/google/cloud/gke_backup_v1/services/backup_for_gke/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003   166817 2023-07-05 15:19:45.000000 google-cloud-gke-backup-0.5.0/google/cloud/gke_backup_v1/services/backup_for_gke/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:21:41.244928 google-cloud-gke-backup-0.5.0/google/cloud/gke_backup_v1/types/
+-rw-rw-r--   0 root         (0)     1003     2884 2023-07-05 15:19:45.000000 google-cloud-gke-backup-0.5.0/google/cloud/gke_backup_v1/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003    14215 2023-07-05 15:19:45.000000 google-cloud-gke-backup-0.5.0/google/cloud/gke_backup_v1/types/backup.py
+-rw-rw-r--   0 root         (0)     1003    13525 2023-07-05 15:19:45.000000 google-cloud-gke-backup-0.5.0/google/cloud/gke_backup_v1/types/backup_plan.py
+-rw-rw-r--   0 root         (0)     1003     2520 2023-07-05 15:19:45.000000 google-cloud-gke-backup-0.5.0/google/cloud/gke_backup_v1/types/common.py
+-rw-rw-r--   0 root         (0)     1003    36417 2023-07-05 15:19:45.000000 google-cloud-gke-backup-0.5.0/google/cloud/gke_backup_v1/types/gkebackup.py
+-rw-rw-r--   0 root         (0)     1003    33144 2023-07-05 15:19:45.000000 google-cloud-gke-backup-0.5.0/google/cloud/gke_backup_v1/types/restore.py
+-rw-rw-r--   0 root         (0)     1003     5892 2023-07-05 15:19:45.000000 google-cloud-gke-backup-0.5.0/google/cloud/gke_backup_v1/types/restore_plan.py
+-rw-rw-r--   0 root         (0)     1003    12236 2023-07-05 15:19:45.000000 google-cloud-gke-backup-0.5.0/google/cloud/gke_backup_v1/types/volume.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:21:41.244928 google-cloud-gke-backup-0.5.0/google_cloud_gke_backup.egg-info/
+-rw-r--r--   0 root         (0)     1003     4778 2023-07-05 15:21:41.000000 google-cloud-gke-backup-0.5.0/google_cloud_gke_backup.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0)     1003     1851 2023-07-05 15:21:41.000000 google-cloud-gke-backup-0.5.0/google_cloud_gke_backup.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-07-05 15:21:41.000000 google-cloud-gke-backup-0.5.0/google_cloud_gke_backup.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0)     1003       20 2023-07-05 15:21:41.000000 google-cloud-gke-backup-0.5.0/google_cloud_gke_backup.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-07-05 15:21:41.000000 google-cloud-gke-backup-0.5.0/google_cloud_gke_backup.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0)     1003      352 2023-07-05 15:21:41.000000 google-cloud-gke-backup-0.5.0/google_cloud_gke_backup.egg-info/requires.txt
+-rw-r--r--   0 root         (0)     1003        7 2023-07-05 15:21:41.000000 google-cloud-gke-backup-0.5.0/google_cloud_gke_backup.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0)     1003       67 2023-07-05 15:21:41.248927 google-cloud-gke-backup-0.5.0/setup.cfg
+-rw-rw-r--   0 root         (0)     1003     2980 2023-07-05 15:19:45.000000 google-cloud-gke-backup-0.5.0/setup.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:21:41.244928 google-cloud-gke-backup-0.5.0/tests/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:19:45.000000 google-cloud-gke-backup-0.5.0/tests/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:21:41.244928 google-cloud-gke-backup-0.5.0/tests/unit/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:19:45.000000 google-cloud-gke-backup-0.5.0/tests/unit/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:21:41.248927 google-cloud-gke-backup-0.5.0/tests/unit/gapic/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:19:45.000000 google-cloud-gke-backup-0.5.0/tests/unit/gapic/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:21:41.248927 google-cloud-gke-backup-0.5.0/tests/unit/gapic/gke_backup_v1/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:19:45.000000 google-cloud-gke-backup-0.5.0/tests/unit/gapic/gke_backup_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003   676567 2023-07-05 15:19:45.000000 google-cloud-gke-backup-0.5.0/tests/unit/gapic/gke_backup_v1/test_backup_for_gke.py
```

### Comparing `google-cloud-gke-backup-0.4.4/LICENSE` & `google-cloud-gke-backup-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `google-cloud-gke-backup-0.4.4/MANIFEST.in` & `google-cloud-gke-backup-0.5.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `google-cloud-gke-backup-0.4.4/PKG-INFO` & `google-cloud-gke-backup-0.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-gke-backup
-Version: 0.4.4
+Version: 0.5.0
 Summary: Google Cloud Gke Backup API client library
 Home-page: https://github.com/googleapis/python-gke-backup
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 4 - Beta
```

### Comparing `google-cloud-gke-backup-0.4.4/README.rst` & `google-cloud-gke-backup-0.5.0/README.rst`

 * *Files identical despite different names*

### Comparing `google-cloud-gke-backup-0.4.4/google/cloud/gke_backup/__init__.py` & `google-cloud-gke-backup-0.5.0/google/cloud/gke_backup/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-gke-backup-0.4.4/google/cloud/gke_backup/gapic_version.py` & `google-cloud-gke-backup-0.5.0/google/cloud/gke_backup/gapic_version.py`

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
-__version__ = "0.4.4"  # {x-release-please-version}
+__version__ = "0.5.0"  # {x-release-please-version}
```

### Comparing `google-cloud-gke-backup-0.4.4/google/cloud/gke_backup_v1/__init__.py` & `google-cloud-gke-backup-0.5.0/google/cloud/gke_backup_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-gke-backup-0.4.4/google/cloud/gke_backup_v1/gapic_metadata.json` & `google-cloud-gke-backup-0.5.0/google/cloud/gke_backup_v1/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-cloud-gke-backup-0.4.4/google/cloud/gke_backup_v1/gapic_version.py` & `google-cloud-gke-backup-0.5.0/google/cloud/gke_backup_v1/gapic_version.py`

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
-__version__ = "0.4.4"  # {x-release-please-version}
+__version__ = "0.5.0"  # {x-release-please-version}
```

### Comparing `google-cloud-gke-backup-0.4.4/google/cloud/gke_backup_v1/services/__init__.py` & `google-cloud-gke-backup-0.5.0/google/cloud/gke_backup_v1/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-gke-backup-0.4.4/google/cloud/gke_backup_v1/services/backup_for_gke/__init__.py` & `google-cloud-gke-backup-0.5.0/google/cloud/gke_backup_v1/services/backup_for_gke/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-gke-backup-0.4.4/google/cloud/gke_backup_v1/services/backup_for_gke/async_client.py` & `google-cloud-gke-backup-0.5.0/google/cloud/gke_backup_v1/services/backup_for_gke/async_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1869,15 +1869,15 @@
 
         Returns:
             google.api_core.operation_async.AsyncOperation:
                 An object representing a long-running operation.
 
                 The result type for the operation will be :class:`google.cloud.gke_backup_v1.types.RestorePlan` The configuration of a potential series of Restore operations to be performed
                    against Backups belong to a particular BackupPlan.
-                   Next id: 11
+                   Next id: 13
 
         """
         # Create or coerce a protobuf request object.
         # Quick check: If we got a request object, we should *not* have
         # gotten any keyword arguments that map to the request.
         has_flattened_params = any([parent, restore_plan, restore_plan_id])
         if request is not None and has_flattened_params:
@@ -2107,15 +2107,15 @@
                 sent along with the request as metadata.
 
         Returns:
             google.cloud.gke_backup_v1.types.RestorePlan:
                 The configuration of a potential
                 series of Restore operations to be
                 performed against Backups belong to a
-                particular BackupPlan. Next id: 11
+                particular BackupPlan. Next id: 13
 
         """
         # Create or coerce a protobuf request object.
         # Quick check: If we got a request object, we should *not* have
         # gotten any keyword arguments that map to the request.
         has_flattened_params = any([name])
         if request is not None and has_flattened_params:
@@ -2247,15 +2247,15 @@
 
         Returns:
             google.api_core.operation_async.AsyncOperation:
                 An object representing a long-running operation.
 
                 The result type for the operation will be :class:`google.cloud.gke_backup_v1.types.RestorePlan` The configuration of a potential series of Restore operations to be performed
                    against Backups belong to a particular BackupPlan.
-                   Next id: 11
+                   Next id: 13
 
         """
         # Create or coerce a protobuf request object.
         # Quick check: If we got a request object, we should *not* have
         # gotten any keyword arguments that map to the request.
         has_flattened_params = any([restore_plan, update_mask])
         if request is not None and has_flattened_params:
@@ -3935,15 +3935,15 @@
             timeout=timeout,
             metadata=metadata,
         )
 
         # Done; return the response.
         return response
 
-    async def __aenter__(self):
+    async def __aenter__(self) -> "BackupForGKEAsyncClient":
         return self
 
     async def __aexit__(self, exc_type, exc, tb):
         await self.transport.close()
 
 
 DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
```

### Comparing `google-cloud-gke-backup-0.4.4/google/cloud/gke_backup_v1/services/backup_for_gke/client.py` & `google-cloud-gke-backup-0.5.0/google/cloud/gke_backup_v1/services/backup_for_gke/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -2200,15 +2200,15 @@
 
         Returns:
             google.api_core.operation.Operation:
                 An object representing a long-running operation.
 
                 The result type for the operation will be :class:`google.cloud.gke_backup_v1.types.RestorePlan` The configuration of a potential series of Restore operations to be performed
                    against Backups belong to a particular BackupPlan.
-                   Next id: 11
+                   Next id: 13
 
         """
         # Create or coerce a protobuf request object.
         # Quick check: If we got a request object, we should *not* have
         # gotten any keyword arguments that map to the request.
         has_flattened_params = any([parent, restore_plan, restore_plan_id])
         if request is not None and has_flattened_params:
@@ -2429,15 +2429,15 @@
                 sent along with the request as metadata.
 
         Returns:
             google.cloud.gke_backup_v1.types.RestorePlan:
                 The configuration of a potential
                 series of Restore operations to be
                 performed against Backups belong to a
-                particular BackupPlan. Next id: 11
+                particular BackupPlan. Next id: 13
 
         """
         # Create or coerce a protobuf request object.
         # Quick check: If we got a request object, we should *not* have
         # gotten any keyword arguments that map to the request.
         has_flattened_params = any([name])
         if request is not None and has_flattened_params:
@@ -2560,15 +2560,15 @@
 
         Returns:
             google.api_core.operation.Operation:
                 An object representing a long-running operation.
 
                 The result type for the operation will be :class:`google.cloud.gke_backup_v1.types.RestorePlan` The configuration of a potential series of Restore operations to be performed
                    against Backups belong to a particular BackupPlan.
-                   Next id: 11
+                   Next id: 13
 
         """
         # Create or coerce a protobuf request object.
         # Quick check: If we got a request object, we should *not* have
         # gotten any keyword arguments that map to the request.
         has_flattened_params = any([restore_plan, update_mask])
         if request is not None and has_flattened_params:
```

### Comparing `google-cloud-gke-backup-0.4.4/google/cloud/gke_backup_v1/services/backup_for_gke/pagers.py` & `google-cloud-gke-backup-0.5.0/google/cloud/gke_backup_v1/services/backup_for_gke/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-gke-backup-0.4.4/google/cloud/gke_backup_v1/services/backup_for_gke/transports/__init__.py` & `google-cloud-gke-backup-0.5.0/google/cloud/gke_backup_v1/services/backup_for_gke/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-gke-backup-0.4.4/google/cloud/gke_backup_v1/services/backup_for_gke/transports/base.py` & `google-cloud-gke-backup-0.5.0/google/cloud/gke_backup_v1/services/backup_for_gke/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-gke-backup-0.4.4/google/cloud/gke_backup_v1/services/backup_for_gke/transports/grpc.py` & `google-cloud-gke-backup-0.5.0/google/cloud/gke_backup_v1/services/backup_for_gke/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-gke-backup-0.4.4/google/cloud/gke_backup_v1/services/backup_for_gke/transports/grpc_asyncio.py` & `google-cloud-gke-backup-0.5.0/google/cloud/gke_backup_v1/services/backup_for_gke/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-gke-backup-0.4.4/google/cloud/gke_backup_v1/services/backup_for_gke/transports/rest.py` & `google-cloud-gke-backup-0.5.0/google/cloud/gke_backup_v1/services/backup_for_gke/transports/rest.py`

 * *Files 0% similar despite different names*

```diff
@@ -2228,15 +2228,15 @@
                     sent along with the request as metadata.
 
             Returns:
                 ~.restore_plan.RestorePlan:
                     The configuration of a potential
                 series of Restore operations to be
                 performed against Backups belong to a
-                particular BackupPlan. Next id: 11
+                particular BackupPlan. Next id: 13
 
             """
 
             http_options: List[Dict[str, str]] = [
                 {
                     "method": "get",
                     "uri": "/v1/{name=projects/*/locations/*/restorePlans/*}",
@@ -3871,15 +3871,15 @@
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
@@ -3968,15 +3968,15 @@
 
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
@@ -4037,15 +4037,15 @@
 
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

### Comparing `google-cloud-gke-backup-0.4.4/google/cloud/gke_backup_v1/types/__init__.py` & `google-cloud-gke-backup-0.5.0/google/cloud/gke_backup_v1/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-gke-backup-0.4.4/google/cloud/gke_backup_v1/types/backup.py` & `google-cloud-gke-backup-0.5.0/google/cloud/gke_backup_v1/types/backup.py`

 * *Files identical despite different names*

### Comparing `google-cloud-gke-backup-0.4.4/google/cloud/gke_backup_v1/types/backup_plan.py` & `google-cloud-gke-backup-0.5.0/google/cloud/gke_backup_v1/types/backup_plan.py`

 * *Files 13% similar despite different names*

```diff
@@ -89,16 +89,55 @@
         backup_config (google.cloud.gke_backup_v1.types.BackupPlan.BackupConfig):
             Defines the configuration of Backups created
             via this BackupPlan.
         protected_pod_count (int):
             Output only. The number of Kubernetes Pods
             backed up in the last successful Backup created
             via this BackupPlan.
+        state (google.cloud.gke_backup_v1.types.BackupPlan.State):
+            Output only. State of the BackupPlan. This
+            State field reflects the various stages a
+            BackupPlan can be in during the Create
+            operation. It will be set to "DEACTIVATED" if
+            the BackupPlan is deactivated on an Update
+        state_reason (str):
+            Output only. Human-readable description of why BackupPlan is
+            in the current ``state``
     """
 
+    class State(proto.Enum):
+        r"""State
+
+        Values:
+            STATE_UNSPECIFIED (0):
+                Default first value for Enums.
+            CLUSTER_PENDING (1):
+                Waiting for cluster state to be RUNNING.
+            PROVISIONING (2):
+                The BackupPlan is in the process of being
+                created.
+            READY (3):
+                The BackupPlan has successfully been created
+                and is ready for Backups.
+            FAILED (4):
+                BackupPlan creation has failed.
+            DEACTIVATED (5):
+                The BackupPlan has been deactivated.
+            DELETING (6):
+                The BackupPlan is in the process of being
+                deleted.
+        """
+        STATE_UNSPECIFIED = 0
+        CLUSTER_PENDING = 1
+        PROVISIONING = 2
+        READY = 3
+        FAILED = 4
+        DEACTIVATED = 5
+        DELETING = 6
+
     class RetentionPolicy(proto.Message):
         r"""RetentionPolicy defines a Backup retention policy for a
         BackupPlan.
 
         Attributes:
             backup_delete_lock_days (int):
                 Minimum age for Backups created via this BackupPlan (in
@@ -148,16 +187,16 @@
         )
         locked: bool = proto.Field(
             proto.BOOL,
             number=3,
         )
 
     class Schedule(proto.Message):
-        r"""Schedule defines scheduling parameters for automatically
-        creating Backups via this BackupPlan.
+        r"""Defines scheduling parameters for automatically creating
+        Backups via this BackupPlan.
 
         Attributes:
             cron_schedule (str):
                 A standard `cron <https://wikipedia.com/wiki/cron>`__ string
                 that defines a repeating schedule for creating Backups via
                 this BackupPlan. If this is defined, then
                 [backup_retain_days][google.cloud.gkebackup.v1.BackupPlan.RetentionPolicy.backup_retain_days]
@@ -311,10 +350,19 @@
         number=12,
         message=BackupConfig,
     )
     protected_pod_count: int = proto.Field(
         proto.INT32,
         number=13,
     )
+    state: State = proto.Field(
+        proto.ENUM,
+        number=14,
+        enum=State,
+    )
+    state_reason: str = proto.Field(
+        proto.STRING,
+        number=15,
+    )
 
 
 __all__ = tuple(sorted(__protobuf__.manifest))
```

### Comparing `google-cloud-gke-backup-0.4.4/google/cloud/gke_backup_v1/types/common.py` & `google-cloud-gke-backup-0.5.0/google/cloud/gke_backup_v1/types/common.py`

 * *Files identical despite different names*

### Comparing `google-cloud-gke-backup-0.4.4/google/cloud/gke_backup_v1/types/gkebackup.py` & `google-cloud-gke-backup-0.5.0/google/cloud/gke_backup_v1/types/gkebackup.py`

 * *Files identical despite different names*

### Comparing `google-cloud-gke-backup-0.4.4/google/cloud/gke_backup_v1/types/restore.py` & `google-cloud-gke-backup-0.5.0/google/cloud/gke_backup_v1/types/restore.py`

 * *Files 20% similar despite different names*

```diff
@@ -215,15 +215,15 @@
         proto.STRING,
         number=17,
     )
 
 
 class RestoreConfig(proto.Message):
     r"""Configuration of a restore.
-    Next id: 9
+    Next id: 12
 
     This message has `oneof`_ fields (mutually exclusive fields).
     For each oneof, at most one member field can be set at the same time.
     Setting any member of the oneof automatically clears all other
     members.
 
     .. _oneof: https://proto-plus-python.readthedocs.io/en/stable/fields.html#oneofs-mutually-exclusive-fields
@@ -264,22 +264,42 @@
         selected_applications (google.cloud.gke_backup_v1.types.NamespacedNames):
             A list of selected ProtectedApplications to
             restore. The listed ProtectedApplications and
             all the resources to which they refer will be
             restored.
 
             This field is a member of `oneof`_ ``namespaced_resource_restore_scope``.
+        no_namespaces (bool):
+            Do not restore any namespaced resources if
+            set to "True". Specifying this field to "False"
+            is not allowed.
+
+            This field is a member of `oneof`_ ``namespaced_resource_restore_scope``.
+        excluded_namespaces (google.cloud.gke_backup_v1.types.Namespaces):
+            A list of selected namespaces excluded from
+            restoration. All namespaces except those in this
+            list will be restored.
+
+            This field is a member of `oneof`_ ``namespaced_resource_restore_scope``.
         substitution_rules (MutableSequence[google.cloud.gke_backup_v1.types.RestoreConfig.SubstitutionRule]):
             A list of transformation rules to be applied
             against Kubernetes resources as they are
             selected for restoration from a Backup. Rules
             are executed in order defined - this order
             matters, as changes made by a rule may impact
             the filtering logic of subsequent rules. An
             empty list means no substitution will occur.
+        transformation_rules (MutableSequence[google.cloud.gke_backup_v1.types.RestoreConfig.TransformationRule]):
+            A list of transformation rules to be applied
+            against Kubernetes resources as they are
+            selected for restoration from a Backup. Rules
+            are executed in order defined - this order
+            matters, as changes made by a rule may impact
+            the filtering logic of subsequent rules. An
+            empty list means no transformation will occur.
     """
 
     class VolumeDataRestorePolicy(proto.Enum):
         r"""Defines how volume data should be restored.
 
         Values:
             VOLUME_DATA_RESTORE_POLICY_UNSPECIFIED (0):
@@ -412,23 +432,54 @@
         Attributes:
             selected_group_kinds (MutableSequence[google.cloud.gke_backup_v1.types.RestoreConfig.GroupKind]):
                 A list of cluster-scoped resource group kinds
                 to restore from the backup. If specified, only
                 the selected resources will be restored.
                 Mutually exclusive to any other field in the
                 message.
+            excluded_group_kinds (MutableSequence[google.cloud.gke_backup_v1.types.RestoreConfig.GroupKind]):
+                A list of cluster-scoped resource group kinds
+                to NOT restore from the backup. If specified,
+                all valid cluster-scoped resources will be
+                restored except for those specified in the list.
+                Mutually exclusive to any other field in the
+                message.
+            all_group_kinds (bool):
+                If True, all valid cluster-scoped resources
+                will be restored. Mutually exclusive to any
+                other field in the message.
+            no_group_kinds (bool):
+                If True, no cluster-scoped resources will be
+                restored. This has the same restore scope as if
+                the message is not defined. Mutually exclusive
+                to any other field in the message.
         """
 
         selected_group_kinds: MutableSequence[
             "RestoreConfig.GroupKind"
         ] = proto.RepeatedField(
             proto.MESSAGE,
             number=1,
             message="RestoreConfig.GroupKind",
         )
+        excluded_group_kinds: MutableSequence[
+            "RestoreConfig.GroupKind"
+        ] = proto.RepeatedField(
+            proto.MESSAGE,
+            number=2,
+            message="RestoreConfig.GroupKind",
+        )
+        all_group_kinds: bool = proto.Field(
+            proto.BOOL,
+            number=3,
+        )
+        no_group_kinds: bool = proto.Field(
+            proto.BOOL,
+            number=4,
+        )
 
     class SubstitutionRule(proto.Message):
         r"""A transformation rule to be applied against Kubernetes
         resources as they are selected for restoration from a Backup. A
         rule contains both filtering logic (which resources are subject
         to substitution) and substitution logic.
 
@@ -499,14 +550,192 @@
             number=4,
         )
         new_value: str = proto.Field(
             proto.STRING,
             number=5,
         )
 
+    class TransformationRuleAction(proto.Message):
+        r"""TransformationRuleAction defines a TransformationRule action
+        based on the JSON Patch RFC
+        (https://www.rfc-editor.org/rfc/rfc6902)
+
+        Attributes:
+            op (google.cloud.gke_backup_v1.types.RestoreConfig.TransformationRuleAction.Op):
+                Required. op specifies the operation to
+                perform.
+            from_path (str):
+                A string containing a JSON Pointer value that
+                references the location in the target document
+                to move the value from.
+            path (str):
+                A string containing a JSON-Pointer value that
+                references a location within the target document
+                where the operation is performed.
+            value (str):
+                A string that specifies the desired value in
+                string format to use for transformation.
+        """
+
+        class Op(proto.Enum):
+            r"""Possible values for operations of a transformation rule
+            action.
+
+            Values:
+                OP_UNSPECIFIED (0):
+                    Unspecified operation
+                REMOVE (1):
+                    The "remove" operation removes the value at
+                    the target location.
+                MOVE (2):
+                    The "move" operation removes the value at a
+                    specified location and adds it to the target
+                    location.
+                COPY (3):
+                    The "copy" operation copies the value at a
+                    specified location to the target location.
+                ADD (4):
+                    The "add" operation performs one of the
+                    following functions, depending upon what the
+                    target location references: 1. If the target
+                    location specifies an array index, a new value
+                    is inserted into the array at the specified
+                    index. 2. If the target location specifies an
+                    object member that does not already exist, a new
+                    member is added to the object. 3. If the target
+                    location specifies an object member that does
+                    exist, that member's value is replaced.
+                TEST (5):
+                    The "test" operation tests that a value at
+                    the target location is equal to a specified
+                    value.
+                REPLACE (6):
+                    The "replace" operation replaces the value at
+                    the target location with a new value.  The
+                    operation object MUST contain a "value" member
+                    whose content specifies the replacement value.
+            """
+            OP_UNSPECIFIED = 0
+            REMOVE = 1
+            MOVE = 2
+            COPY = 3
+            ADD = 4
+            TEST = 5
+            REPLACE = 6
+
+        op: "RestoreConfig.TransformationRuleAction.Op" = proto.Field(
+            proto.ENUM,
+            number=1,
+            enum="RestoreConfig.TransformationRuleAction.Op",
+        )
+        from_path: str = proto.Field(
+            proto.STRING,
+            number=2,
+        )
+        path: str = proto.Field(
+            proto.STRING,
+            number=3,
+        )
+        value: str = proto.Field(
+            proto.STRING,
+            number=4,
+        )
+
+    class ResourceFilter(proto.Message):
+        r"""ResourceFilter specifies matching criteria to limit the scope
+        of a change to a specific set of kubernetes resources that are
+        selected for restoration from a backup.
+
+        Attributes:
+            namespaces (MutableSequence[str]):
+                (Filtering parameter) Any resource subject to
+                transformation must be contained within one of
+                the listed Kubernetes Namespace in the Backup.
+                If this field is not provided, no namespace
+                filtering will be performed (all resources in
+                all Namespaces, including all cluster-scoped
+                resources, will be candidates for
+                transformation).
+                To mix cluster-scoped and namespaced resources
+                in the same rule, use an empty string ("") as
+                one of the target namespaces.
+            group_kinds (MutableSequence[google.cloud.gke_backup_v1.types.RestoreConfig.GroupKind]):
+                (Filtering parameter) Any resource subject to
+                transformation must belong to one of the listed
+                "types". If this field is not provided, no type
+                filtering will be performed (all resources of
+                all types matching previous filtering parameters
+                will be candidates for transformation).
+            json_path (str):
+                This is a [JSONPath]
+                (https://github.com/json-path/JsonPath/blob/master/README.md)
+                expression that matches specific fields of candidate
+                resources and it operates as a filtering parameter
+                (resources that are not matched with this expression will
+                not be candidates for transformation).
+        """
+
+        namespaces: MutableSequence[str] = proto.RepeatedField(
+            proto.STRING,
+            number=1,
+        )
+        group_kinds: MutableSequence["RestoreConfig.GroupKind"] = proto.RepeatedField(
+            proto.MESSAGE,
+            number=2,
+            message="RestoreConfig.GroupKind",
+        )
+        json_path: str = proto.Field(
+            proto.STRING,
+            number=3,
+        )
+
+    class TransformationRule(proto.Message):
+        r"""A transformation rule to be applied against Kubernetes
+        resources as they are selected for restoration from a Backup. A
+        rule contains both filtering logic (which resources are subject
+        to transform) and transformation logic.
+
+        Attributes:
+            field_actions (MutableSequence[google.cloud.gke_backup_v1.types.RestoreConfig.TransformationRuleAction]):
+                Required. A list of transformation rule
+                actions to take against candidate resources.
+                Actions are executed in order defined - this
+                order matters, as they could potentially
+                interfere with each other and the first
+                operation could affect the outcome of the second
+                operation.
+            resource_filter (google.cloud.gke_backup_v1.types.RestoreConfig.ResourceFilter):
+                This field is used to specify a set of fields
+                that should be used to determine which resources
+                in backup should be acted upon by the supplied
+                transformation rule actions, and this will
+                ensure that only specific resources are affected
+                by transformation rule actions.
+            description (str):
+                The description is a user specified string
+                description of the transformation rule.
+        """
+
+        field_actions: MutableSequence[
+            "RestoreConfig.TransformationRuleAction"
+        ] = proto.RepeatedField(
+            proto.MESSAGE,
+            number=1,
+            message="RestoreConfig.TransformationRuleAction",
+        )
+        resource_filter: "RestoreConfig.ResourceFilter" = proto.Field(
+            proto.MESSAGE,
+            number=2,
+            message="RestoreConfig.ResourceFilter",
+        )
+        description: str = proto.Field(
+            proto.STRING,
+            number=3,
+        )
+
     volume_data_restore_policy: VolumeDataRestorePolicy = proto.Field(
         proto.ENUM,
         number=1,
         enum=VolumeDataRestorePolicy,
     )
     cluster_resource_conflict_policy: ClusterResourceConflictPolicy = proto.Field(
         proto.ENUM,
@@ -536,15 +765,31 @@
     )
     selected_applications: common.NamespacedNames = proto.Field(
         proto.MESSAGE,
         number=7,
         oneof="namespaced_resource_restore_scope",
         message=common.NamespacedNames,
     )
+    no_namespaces: bool = proto.Field(
+        proto.BOOL,
+        number=9,
+        oneof="namespaced_resource_restore_scope",
+    )
+    excluded_namespaces: common.Namespaces = proto.Field(
+        proto.MESSAGE,
+        number=10,
+        oneof="namespaced_resource_restore_scope",
+        message=common.Namespaces,
+    )
     substitution_rules: MutableSequence[SubstitutionRule] = proto.RepeatedField(
         proto.MESSAGE,
         number=8,
         message=SubstitutionRule,
     )
+    transformation_rules: MutableSequence[TransformationRule] = proto.RepeatedField(
+        proto.MESSAGE,
+        number=11,
+        message=TransformationRule,
+    )
 
 
 __all__ = tuple(sorted(__protobuf__.manifest))
```

### Comparing `google-cloud-gke-backup-0.4.4/google/cloud/gke_backup_v1/types/restore_plan.py` & `google-cloud-gke-backup-0.5.0/google/cloud/gke_backup_v1/types/restore_plan.py`

 * *Files 20% similar despite different names*

```diff
@@ -29,15 +29,15 @@
     },
 )
 
 
 class RestorePlan(proto.Message):
     r"""The configuration of a potential series of Restore operations
     to be performed against Backups belong to a particular
-    BackupPlan. Next id: 11
+    BackupPlan. Next id: 13
 
     Attributes:
         name (str):
             Output only. The full name of the RestorePlan resource.
             Format: ``projects/*/locations/*/restorePlans/*``.
         uid (str):
             Output only. Server generated global unique identifier of
@@ -78,16 +78,47 @@
             suggested that systems make use of the ``etag`` in the
             read-modify-write cycle to perform restore updates in order
             to avoid race conditions: An ``etag`` is returned in the
             response to ``GetRestorePlan``, and systems are expected to
             put that etag in the request to ``UpdateRestorePlan`` or
             ``DeleteRestorePlan`` to ensure that their change will be
             applied to the same version of the resource.
+        state (google.cloud.gke_backup_v1.types.RestorePlan.State):
+            Output only. State of the RestorePlan. This
+            State field reflects the various stages a
+            RestorePlan can be in during the Create
+            operation.
+        state_reason (str):
+            Output only. Human-readable description of why RestorePlan
+            is in the current ``state``
     """
 
+    class State(proto.Enum):
+        r"""State
+
+        Values:
+            STATE_UNSPECIFIED (0):
+                Default first value for Enums.
+            CLUSTER_PENDING (1):
+                Waiting for cluster state to be RUNNING.
+            READY (2):
+                The RestorePlan has successfully been created
+                and is ready for Restores.
+            FAILED (3):
+                RestorePlan creation has failed.
+            DELETING (4):
+                The RestorePlan is in the process of being
+                deleted.
+        """
+        STATE_UNSPECIFIED = 0
+        CLUSTER_PENDING = 1
+        READY = 2
+        FAILED = 3
+        DELETING = 4
+
     name: str = proto.Field(
         proto.STRING,
         number=1,
     )
     uid: str = proto.Field(
         proto.STRING,
         number=2,
@@ -124,10 +155,19 @@
         proto.STRING,
         number=9,
     )
     etag: str = proto.Field(
         proto.STRING,
         number=10,
     )
+    state: State = proto.Field(
+        proto.ENUM,
+        number=11,
+        enum=State,
+    )
+    state_reason: str = proto.Field(
+        proto.STRING,
+        number=12,
+    )
 
 
 __all__ = tuple(sorted(__protobuf__.manifest))
```

### Comparing `google-cloud-gke-backup-0.4.4/google/cloud/gke_backup_v1/types/volume.py` & `google-cloud-gke-backup-0.5.0/google/cloud/gke_backup_v1/types/volume.py`

 * *Files identical despite different names*

### Comparing `google-cloud-gke-backup-0.4.4/google_cloud_gke_backup.egg-info/PKG-INFO` & `google-cloud-gke-backup-0.5.0/google_cloud_gke_backup.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-gke-backup
-Version: 0.4.4
+Version: 0.5.0
 Summary: Google Cloud Gke Backup API client library
 Home-page: https://github.com/googleapis/python-gke-backup
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 4 - Beta
```

### Comparing `google-cloud-gke-backup-0.4.4/google_cloud_gke_backup.egg-info/SOURCES.txt` & `google-cloud-gke-backup-0.5.0/google_cloud_gke_backup.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `google-cloud-gke-backup-0.4.4/setup.py` & `google-cloud-gke-backup-0.5.0/setup.py`

 * *Files identical despite different names*

### Comparing `google-cloud-gke-backup-0.4.4/tests/__init__.py` & `google-cloud-gke-backup-0.5.0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-gke-backup-0.4.4/tests/unit/__init__.py` & `google-cloud-gke-backup-0.5.0/tests/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-gke-backup-0.4.4/tests/unit/gapic/__init__.py` & `google-cloud-gke-backup-0.5.0/tests/unit/gapic/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-gke-backup-0.4.4/tests/unit/gapic/gke_backup_v1/__init__.py` & `google-cloud-gke-backup-0.5.0/tests/unit/gapic/gke_backup_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-gke-backup-0.4.4/tests/unit/gapic/gke_backup_v1/test_backup_for_gke.py` & `google-cloud-gke-backup-0.5.0/tests/unit/gapic/gke_backup_v1/test_backup_for_gke.py`

 * *Files 0% similar despite different names*

```diff
@@ -1409,17 +1409,19 @@
                     backup_plan.BackupPlan(),
                     backup_plan.BackupPlan(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.list_backup_plans(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
@@ -1445,14 +1447,16 @@
             name="name_value",
             uid="uid_value",
             description="description_value",
             cluster="cluster_value",
             etag="etag_value",
             deactivated=True,
             protected_pod_count=2036,
+            state=backup_plan.BackupPlan.State.CLUSTER_PENDING,
+            state_reason="state_reason_value",
         )
         response = client.get_backup_plan(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
         assert args[0] == gkebackup.GetBackupPlanRequest()
@@ -1462,14 +1466,16 @@
     assert response.name == "name_value"
     assert response.uid == "uid_value"
     assert response.description == "description_value"
     assert response.cluster == "cluster_value"
     assert response.etag == "etag_value"
     assert response.deactivated is True
     assert response.protected_pod_count == 2036
+    assert response.state == backup_plan.BackupPlan.State.CLUSTER_PENDING
+    assert response.state_reason == "state_reason_value"
 
 
 def test_get_backup_plan_empty_call():
     # This test is a coverage failsafe to make sure that totally empty calls,
     # i.e. request == None and no flattened fields passed, work.
     client = BackupForGKEClient(
         credentials=ga_credentials.AnonymousCredentials(),
@@ -1505,14 +1511,16 @@
                 name="name_value",
                 uid="uid_value",
                 description="description_value",
                 cluster="cluster_value",
                 etag="etag_value",
                 deactivated=True,
                 protected_pod_count=2036,
+                state=backup_plan.BackupPlan.State.CLUSTER_PENDING,
+                state_reason="state_reason_value",
             )
         )
         response = await client.get_backup_plan(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls)
         _, args, _ = call.mock_calls[0]
@@ -1523,14 +1531,16 @@
     assert response.name == "name_value"
     assert response.uid == "uid_value"
     assert response.description == "description_value"
     assert response.cluster == "cluster_value"
     assert response.etag == "etag_value"
     assert response.deactivated is True
     assert response.protected_pod_count == 2036
+    assert response.state == backup_plan.BackupPlan.State.CLUSTER_PENDING
+    assert response.state_reason == "state_reason_value"
 
 
 @pytest.mark.asyncio
 async def test_get_backup_plan_async_from_dict():
     await test_get_backup_plan_async(request_type=dict)
 
 
@@ -2821,17 +2831,19 @@
                     backup.Backup(),
                     backup.Backup(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.list_backups(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
@@ -4014,17 +4026,19 @@
                     volume.VolumeBackup(),
                     volume.VolumeBackup(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.list_volume_backups(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
@@ -4998,17 +5012,19 @@
                     restore_plan.RestorePlan(),
                     restore_plan.RestorePlan(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.list_restore_plans(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
@@ -5033,14 +5049,16 @@
         call.return_value = restore_plan.RestorePlan(
             name="name_value",
             uid="uid_value",
             description="description_value",
             backup_plan="backup_plan_value",
             cluster="cluster_value",
             etag="etag_value",
+            state=restore_plan.RestorePlan.State.CLUSTER_PENDING,
+            state_reason="state_reason_value",
         )
         response = client.get_restore_plan(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
         assert args[0] == gkebackup.GetRestorePlanRequest()
@@ -5049,14 +5067,16 @@
     assert isinstance(response, restore_plan.RestorePlan)
     assert response.name == "name_value"
     assert response.uid == "uid_value"
     assert response.description == "description_value"
     assert response.backup_plan == "backup_plan_value"
     assert response.cluster == "cluster_value"
     assert response.etag == "etag_value"
+    assert response.state == restore_plan.RestorePlan.State.CLUSTER_PENDING
+    assert response.state_reason == "state_reason_value"
 
 
 def test_get_restore_plan_empty_call():
     # This test is a coverage failsafe to make sure that totally empty calls,
     # i.e. request == None and no flattened fields passed, work.
     client = BackupForGKEClient(
         credentials=ga_credentials.AnonymousCredentials(),
@@ -5091,14 +5111,16 @@
             restore_plan.RestorePlan(
                 name="name_value",
                 uid="uid_value",
                 description="description_value",
                 backup_plan="backup_plan_value",
                 cluster="cluster_value",
                 etag="etag_value",
+                state=restore_plan.RestorePlan.State.CLUSTER_PENDING,
+                state_reason="state_reason_value",
             )
         )
         response = await client.get_restore_plan(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls)
         _, args, _ = call.mock_calls[0]
@@ -5108,14 +5130,16 @@
     assert isinstance(response, restore_plan.RestorePlan)
     assert response.name == "name_value"
     assert response.uid == "uid_value"
     assert response.description == "description_value"
     assert response.backup_plan == "backup_plan_value"
     assert response.cluster == "cluster_value"
     assert response.etag == "etag_value"
+    assert response.state == restore_plan.RestorePlan.State.CLUSTER_PENDING
+    assert response.state_reason == "state_reason_value"
 
 
 @pytest.mark.asyncio
 async def test_get_restore_plan_async_from_dict():
     await test_get_restore_plan_async(request_type=dict)
 
 
@@ -6410,17 +6434,19 @@
                     restore.Restore(),
                     restore.Restore(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.list_restores(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
@@ -7586,17 +7612,19 @@
                     volume.VolumeRestore(),
                     volume.VolumeRestore(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.list_volume_restores(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
@@ -7916,14 +7944,16 @@
             "include_volume_data": True,
             "include_secrets": True,
             "encryption_key": {
                 "gcp_kms_encryption_key": "gcp_kms_encryption_key_value"
             },
         },
         "protected_pod_count": 2036,
+        "state": 1,
+        "state_reason": "state_reason_value",
     }
     request = request_type(**request_init)
 
     # Mock the http request call within the method and fake a response.
     with mock.patch.object(type(client.transport._session), "request") as req:
         # Designate an appropriate value for the returned response.
         return_value = operations_pb2.Operation(name="operations/spam")
@@ -8148,14 +8178,16 @@
             "include_volume_data": True,
             "include_secrets": True,
             "encryption_key": {
                 "gcp_kms_encryption_key": "gcp_kms_encryption_key_value"
             },
         },
         "protected_pod_count": 2036,
+        "state": 1,
+        "state_reason": "state_reason_value",
     }
     request = request_type(**request_init)
 
     # Mock the http request call within the method and fake a BadRequest error.
     with mock.patch.object(Session, "request") as req, pytest.raises(
         core_exceptions.BadRequest
     ):
@@ -8600,14 +8632,16 @@
             name="name_value",
             uid="uid_value",
             description="description_value",
             cluster="cluster_value",
             etag="etag_value",
             deactivated=True,
             protected_pod_count=2036,
+            state=backup_plan.BackupPlan.State.CLUSTER_PENDING,
+            state_reason="state_reason_value",
         )
 
         # Wrap the value into a proper Response obj
         response_value = Response()
         response_value.status_code = 200
         pb_return_value = backup_plan.BackupPlan.pb(return_value)
         json_return_value = json_format.MessageToJson(pb_return_value)
@@ -8621,14 +8655,16 @@
     assert response.name == "name_value"
     assert response.uid == "uid_value"
     assert response.description == "description_value"
     assert response.cluster == "cluster_value"
     assert response.etag == "etag_value"
     assert response.deactivated is True
     assert response.protected_pod_count == 2036
+    assert response.state == backup_plan.BackupPlan.State.CLUSTER_PENDING
+    assert response.state_reason == "state_reason_value"
 
 
 def test_get_backup_plan_rest_required_fields(
     request_type=gkebackup.GetBackupPlanRequest,
 ):
     transport_class = transports.BackupForGKERestTransport
 
@@ -8904,14 +8940,16 @@
             "include_volume_data": True,
             "include_secrets": True,
             "encryption_key": {
                 "gcp_kms_encryption_key": "gcp_kms_encryption_key_value"
             },
         },
         "protected_pod_count": 2036,
+        "state": 1,
+        "state_reason": "state_reason_value",
     }
     request = request_type(**request_init)
 
     # Mock the http request call within the method and fake a response.
     with mock.patch.object(type(client.transport._session), "request") as req:
         # Designate an appropriate value for the returned response.
         return_value = operations_pb2.Operation(name="operations/spam")
@@ -9113,14 +9151,16 @@
             "include_volume_data": True,
             "include_secrets": True,
             "encryption_key": {
                 "gcp_kms_encryption_key": "gcp_kms_encryption_key_value"
             },
         },
         "protected_pod_count": 2036,
+        "state": 1,
+        "state_reason": "state_reason_value",
     }
     request = request_type(**request_init)
 
     # Mock the http request call within the method and fake a BadRequest error.
     with mock.patch.object(Session, "request") as req, pytest.raises(
         core_exceptions.BadRequest
     ):
@@ -11753,40 +11793,65 @@
             "namespaced_resource_restore_mode": 1,
             "cluster_resource_restore_scope": {
                 "selected_group_kinds": [
                     {
                         "resource_group": "resource_group_value",
                         "resource_kind": "resource_kind_value",
                     }
-                ]
+                ],
+                "excluded_group_kinds": {},
+                "all_group_kinds": True,
+                "no_group_kinds": True,
             },
             "all_namespaces": True,
             "selected_namespaces": {
                 "namespaces": ["namespaces_value1", "namespaces_value2"]
             },
             "selected_applications": {
                 "namespaced_names": [
                     {"namespace": "namespace_value", "name": "name_value"}
                 ]
             },
+            "no_namespaces": True,
+            "excluded_namespaces": {},
             "substitution_rules": [
                 {
                     "target_namespaces": [
                         "target_namespaces_value1",
                         "target_namespaces_value2",
                     ],
                     "target_group_kinds": {},
                     "target_json_path": "target_json_path_value",
                     "original_value_pattern": "original_value_pattern_value",
                     "new_value": "new_value_value",
                 }
             ],
+            "transformation_rules": [
+                {
+                    "field_actions": [
+                        {
+                            "op": 1,
+                            "from_path": "from_path_value",
+                            "path": "path_value",
+                            "value": "value_value",
+                        }
+                    ],
+                    "resource_filter": {
+                        "namespaces": ["namespaces_value1", "namespaces_value2"],
+                        "group_kinds": {},
+                        "json_path": "json_path_value",
+                    },
+                    "description": "description_value",
+                }
+            ],
         },
         "labels": {},
         "etag": "etag_value",
+        "state": 1,
+        "state_reason": "state_reason_value",
     }
     request = request_type(**request_init)
 
     # Mock the http request call within the method and fake a response.
     with mock.patch.object(type(client.transport._session), "request") as req:
         # Designate an appropriate value for the returned response.
         return_value = operations_pb2.Operation(name="operations/spam")
@@ -11996,40 +12061,65 @@
             "namespaced_resource_restore_mode": 1,
             "cluster_resource_restore_scope": {
                 "selected_group_kinds": [
                     {
                         "resource_group": "resource_group_value",
                         "resource_kind": "resource_kind_value",
                     }
-                ]
+                ],
+                "excluded_group_kinds": {},
+                "all_group_kinds": True,
+                "no_group_kinds": True,
             },
             "all_namespaces": True,
             "selected_namespaces": {
                 "namespaces": ["namespaces_value1", "namespaces_value2"]
             },
             "selected_applications": {
                 "namespaced_names": [
                     {"namespace": "namespace_value", "name": "name_value"}
                 ]
             },
+            "no_namespaces": True,
+            "excluded_namespaces": {},
             "substitution_rules": [
                 {
                     "target_namespaces": [
                         "target_namespaces_value1",
                         "target_namespaces_value2",
                     ],
                     "target_group_kinds": {},
                     "target_json_path": "target_json_path_value",
                     "original_value_pattern": "original_value_pattern_value",
                     "new_value": "new_value_value",
                 }
             ],
+            "transformation_rules": [
+                {
+                    "field_actions": [
+                        {
+                            "op": 1,
+                            "from_path": "from_path_value",
+                            "path": "path_value",
+                            "value": "value_value",
+                        }
+                    ],
+                    "resource_filter": {
+                        "namespaces": ["namespaces_value1", "namespaces_value2"],
+                        "group_kinds": {},
+                        "json_path": "json_path_value",
+                    },
+                    "description": "description_value",
+                }
+            ],
         },
         "labels": {},
         "etag": "etag_value",
+        "state": 1,
+        "state_reason": "state_reason_value",
     }
     request = request_type(**request_init)
 
     # Mock the http request call within the method and fake a BadRequest error.
     with mock.patch.object(Session, "request") as req, pytest.raises(
         core_exceptions.BadRequest
     ):
@@ -12475,14 +12565,16 @@
         return_value = restore_plan.RestorePlan(
             name="name_value",
             uid="uid_value",
             description="description_value",
             backup_plan="backup_plan_value",
             cluster="cluster_value",
             etag="etag_value",
+            state=restore_plan.RestorePlan.State.CLUSTER_PENDING,
+            state_reason="state_reason_value",
         )
 
         # Wrap the value into a proper Response obj
         response_value = Response()
         response_value.status_code = 200
         pb_return_value = restore_plan.RestorePlan.pb(return_value)
         json_return_value = json_format.MessageToJson(pb_return_value)
@@ -12495,14 +12587,16 @@
     assert isinstance(response, restore_plan.RestorePlan)
     assert response.name == "name_value"
     assert response.uid == "uid_value"
     assert response.description == "description_value"
     assert response.backup_plan == "backup_plan_value"
     assert response.cluster == "cluster_value"
     assert response.etag == "etag_value"
+    assert response.state == restore_plan.RestorePlan.State.CLUSTER_PENDING
+    assert response.state_reason == "state_reason_value"
 
 
 def test_get_restore_plan_rest_required_fields(
     request_type=gkebackup.GetRestorePlanRequest,
 ):
     transport_class = transports.BackupForGKERestTransport
 
@@ -12765,40 +12859,65 @@
             "namespaced_resource_restore_mode": 1,
             "cluster_resource_restore_scope": {
                 "selected_group_kinds": [
                     {
                         "resource_group": "resource_group_value",
                         "resource_kind": "resource_kind_value",
                     }
-                ]
+                ],
+                "excluded_group_kinds": {},
+                "all_group_kinds": True,
+                "no_group_kinds": True,
             },
             "all_namespaces": True,
             "selected_namespaces": {
                 "namespaces": ["namespaces_value1", "namespaces_value2"]
             },
             "selected_applications": {
                 "namespaced_names": [
                     {"namespace": "namespace_value", "name": "name_value"}
                 ]
             },
+            "no_namespaces": True,
+            "excluded_namespaces": {},
             "substitution_rules": [
                 {
                     "target_namespaces": [
                         "target_namespaces_value1",
                         "target_namespaces_value2",
                     ],
                     "target_group_kinds": {},
                     "target_json_path": "target_json_path_value",
                     "original_value_pattern": "original_value_pattern_value",
                     "new_value": "new_value_value",
                 }
             ],
+            "transformation_rules": [
+                {
+                    "field_actions": [
+                        {
+                            "op": 1,
+                            "from_path": "from_path_value",
+                            "path": "path_value",
+                            "value": "value_value",
+                        }
+                    ],
+                    "resource_filter": {
+                        "namespaces": ["namespaces_value1", "namespaces_value2"],
+                        "group_kinds": {},
+                        "json_path": "json_path_value",
+                    },
+                    "description": "description_value",
+                }
+            ],
         },
         "labels": {},
         "etag": "etag_value",
+        "state": 1,
+        "state_reason": "state_reason_value",
     }
     request = request_type(**request_init)
 
     # Mock the http request call within the method and fake a response.
     with mock.patch.object(type(client.transport._session), "request") as req:
         # Designate an appropriate value for the returned response.
         return_value = operations_pb2.Operation(name="operations/spam")
@@ -12985,40 +13104,65 @@
             "namespaced_resource_restore_mode": 1,
             "cluster_resource_restore_scope": {
                 "selected_group_kinds": [
                     {
                         "resource_group": "resource_group_value",
                         "resource_kind": "resource_kind_value",
                     }
-                ]
+                ],
+                "excluded_group_kinds": {},
+                "all_group_kinds": True,
+                "no_group_kinds": True,
             },
             "all_namespaces": True,
             "selected_namespaces": {
                 "namespaces": ["namespaces_value1", "namespaces_value2"]
             },
             "selected_applications": {
                 "namespaced_names": [
                     {"namespace": "namespace_value", "name": "name_value"}
                 ]
             },
+            "no_namespaces": True,
+            "excluded_namespaces": {},
             "substitution_rules": [
                 {
                     "target_namespaces": [
                         "target_namespaces_value1",
                         "target_namespaces_value2",
                     ],
                     "target_group_kinds": {},
                     "target_json_path": "target_json_path_value",
                     "original_value_pattern": "original_value_pattern_value",
                     "new_value": "new_value_value",
                 }
             ],
+            "transformation_rules": [
+                {
+                    "field_actions": [
+                        {
+                            "op": 1,
+                            "from_path": "from_path_value",
+                            "path": "path_value",
+                            "value": "value_value",
+                        }
+                    ],
+                    "resource_filter": {
+                        "namespaces": ["namespaces_value1", "namespaces_value2"],
+                        "group_kinds": {},
+                        "json_path": "json_path_value",
+                    },
+                    "description": "description_value",
+                }
+            ],
         },
         "labels": {},
         "etag": "etag_value",
+        "state": 1,
+        "state_reason": "state_reason_value",
     }
     request = request_type(**request_init)
 
     # Mock the http request call within the method and fake a BadRequest error.
     with mock.patch.object(Session, "request") as req, pytest.raises(
         core_exceptions.BadRequest
     ):
@@ -13406,37 +13550,60 @@
             "namespaced_resource_restore_mode": 1,
             "cluster_resource_restore_scope": {
                 "selected_group_kinds": [
                     {
                         "resource_group": "resource_group_value",
                         "resource_kind": "resource_kind_value",
                     }
-                ]
+                ],
+                "excluded_group_kinds": {},
+                "all_group_kinds": True,
+                "no_group_kinds": True,
             },
             "all_namespaces": True,
             "selected_namespaces": {
                 "namespaces": ["namespaces_value1", "namespaces_value2"]
             },
             "selected_applications": {
                 "namespaced_names": [
                     {"namespace": "namespace_value", "name": "name_value"}
                 ]
             },
+            "no_namespaces": True,
+            "excluded_namespaces": {},
             "substitution_rules": [
                 {
                     "target_namespaces": [
                         "target_namespaces_value1",
                         "target_namespaces_value2",
                     ],
                     "target_group_kinds": {},
                     "target_json_path": "target_json_path_value",
                     "original_value_pattern": "original_value_pattern_value",
                     "new_value": "new_value_value",
                 }
             ],
+            "transformation_rules": [
+                {
+                    "field_actions": [
+                        {
+                            "op": 1,
+                            "from_path": "from_path_value",
+                            "path": "path_value",
+                            "value": "value_value",
+                        }
+                    ],
+                    "resource_filter": {
+                        "namespaces": ["namespaces_value1", "namespaces_value2"],
+                        "group_kinds": {},
+                        "json_path": "json_path_value",
+                    },
+                    "description": "description_value",
+                }
+            ],
         },
         "labels": {},
         "state": 1,
         "state_reason": "state_reason_value",
         "complete_time": {},
         "resources_restored_count": 2602,
         "resources_excluded_count": 2576,
@@ -13654,37 +13821,60 @@
             "namespaced_resource_restore_mode": 1,
             "cluster_resource_restore_scope": {
                 "selected_group_kinds": [
                     {
                         "resource_group": "resource_group_value",
                         "resource_kind": "resource_kind_value",
                     }
-                ]
+                ],
+                "excluded_group_kinds": {},
+                "all_group_kinds": True,
+                "no_group_kinds": True,
             },
             "all_namespaces": True,
             "selected_namespaces": {
                 "namespaces": ["namespaces_value1", "namespaces_value2"]
             },
             "selected_applications": {
                 "namespaced_names": [
                     {"namespace": "namespace_value", "name": "name_value"}
                 ]
             },
+            "no_namespaces": True,
+            "excluded_namespaces": {},
             "substitution_rules": [
                 {
                     "target_namespaces": [
                         "target_namespaces_value1",
                         "target_namespaces_value2",
                     ],
                     "target_group_kinds": {},
                     "target_json_path": "target_json_path_value",
                     "original_value_pattern": "original_value_pattern_value",
                     "new_value": "new_value_value",
                 }
             ],
+            "transformation_rules": [
+                {
+                    "field_actions": [
+                        {
+                            "op": 1,
+                            "from_path": "from_path_value",
+                            "path": "path_value",
+                            "value": "value_value",
+                        }
+                    ],
+                    "resource_filter": {
+                        "namespaces": ["namespaces_value1", "namespaces_value2"],
+                        "group_kinds": {},
+                        "json_path": "json_path_value",
+                    },
+                    "description": "description_value",
+                }
+            ],
         },
         "labels": {},
         "state": 1,
         "state_reason": "state_reason_value",
         "complete_time": {},
         "resources_restored_count": 2602,
         "resources_excluded_count": 2576,
@@ -14440,37 +14630,60 @@
             "namespaced_resource_restore_mode": 1,
             "cluster_resource_restore_scope": {
                 "selected_group_kinds": [
                     {
                         "resource_group": "resource_group_value",
                         "resource_kind": "resource_kind_value",
                     }
-                ]
+                ],
+                "excluded_group_kinds": {},
+                "all_group_kinds": True,
+                "no_group_kinds": True,
             },
             "all_namespaces": True,
             "selected_namespaces": {
                 "namespaces": ["namespaces_value1", "namespaces_value2"]
             },
             "selected_applications": {
                 "namespaced_names": [
                     {"namespace": "namespace_value", "name": "name_value"}
                 ]
             },
+            "no_namespaces": True,
+            "excluded_namespaces": {},
             "substitution_rules": [
                 {
                     "target_namespaces": [
                         "target_namespaces_value1",
                         "target_namespaces_value2",
                     ],
                     "target_group_kinds": {},
                     "target_json_path": "target_json_path_value",
                     "original_value_pattern": "original_value_pattern_value",
                     "new_value": "new_value_value",
                 }
             ],
+            "transformation_rules": [
+                {
+                    "field_actions": [
+                        {
+                            "op": 1,
+                            "from_path": "from_path_value",
+                            "path": "path_value",
+                            "value": "value_value",
+                        }
+                    ],
+                    "resource_filter": {
+                        "namespaces": ["namespaces_value1", "namespaces_value2"],
+                        "group_kinds": {},
+                        "json_path": "json_path_value",
+                    },
+                    "description": "description_value",
+                }
+            ],
         },
         "labels": {},
         "state": 1,
         "state_reason": "state_reason_value",
         "complete_time": {},
         "resources_restored_count": 2602,
         "resources_excluded_count": 2576,
@@ -14665,37 +14878,60 @@
             "namespaced_resource_restore_mode": 1,
             "cluster_resource_restore_scope": {
                 "selected_group_kinds": [
                     {
                         "resource_group": "resource_group_value",
                         "resource_kind": "resource_kind_value",
                     }
-                ]
+                ],
+                "excluded_group_kinds": {},
+                "all_group_kinds": True,
+                "no_group_kinds": True,
             },
             "all_namespaces": True,
             "selected_namespaces": {
                 "namespaces": ["namespaces_value1", "namespaces_value2"]
             },
             "selected_applications": {
                 "namespaced_names": [
                     {"namespace": "namespace_value", "name": "name_value"}
                 ]
             },
+            "no_namespaces": True,
+            "excluded_namespaces": {},
             "substitution_rules": [
                 {
                     "target_namespaces": [
                         "target_namespaces_value1",
                         "target_namespaces_value2",
                     ],
                     "target_group_kinds": {},
                     "target_json_path": "target_json_path_value",
                     "original_value_pattern": "original_value_pattern_value",
                     "new_value": "new_value_value",
                 }
             ],
+            "transformation_rules": [
+                {
+                    "field_actions": [
+                        {
+                            "op": 1,
+                            "from_path": "from_path_value",
+                            "path": "path_value",
+                            "value": "value_value",
+                        }
+                    ],
+                    "resource_filter": {
+                        "namespaces": ["namespaces_value1", "namespaces_value2"],
+                        "group_kinds": {},
+                        "json_path": "json_path_value",
+                    },
+                    "description": "description_value",
+                }
+            ],
         },
         "labels": {},
         "state": 1,
         "state_reason": "state_reason_value",
         "complete_time": {},
         "resources_restored_count": 2602,
         "resources_excluded_count": 2576,
```

