# Comparing `tmp/prismacloud-api-5.2.4.tar.gz` & `tmp/prismacloud-api-5.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prismacloud-api-5.2.4.tar", last modified: Thu Jun 22 15:51:39 2023, max compression
+gzip compressed data, was "prismacloud-api-5.2.5.tar", last modified: Wed Jul  5 15:21:13 2023, max compression
```

## Comparing `prismacloud-api-5.2.4.tar` & `prismacloud-api-5.2.5.tar`

### file list

```diff
@@ -1,60 +1,60 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 15:51:39.736184 prismacloud-api-5.2.4/
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-06-22 15:51:20.000000 prismacloud-api-5.2.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2854 2023-06-22 15:51:39.732184 prismacloud-api-5.2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2332 2023-06-22 15:51:20.000000 prismacloud-api-5.2.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 15:51:39.716184 prismacloud-api-5.2.4/prismacloud/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 15:51:39.724184 prismacloud-api-5.2.4/prismacloud/api/
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-06-22 15:51:20.000000 prismacloud-api-5.2.4/prismacloud/api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 15:51:39.724184 prismacloud-api-5.2.4/prismacloud/api/cspm/
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-06-22 15:51:20.000000 prismacloud-api-5.2.4/prismacloud/api/cspm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18687 2023-06-22 15:51:20.000000 prismacloud-api-5.2.4/prismacloud/api/cspm/_endpoints.py
--rw-r--r--   0 runner    (1001) docker     (123)     3372 2023-06-22 15:51:20.000000 prismacloud-api-5.2.4/prismacloud/api/cspm/_extended.py
--rw-r--r--   0 runner    (1001) docker     (123)     8604 2023-06-22 15:51:20.000000 prismacloud-api-5.2.4/prismacloud/api/cspm/cspm.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 15:51:39.728184 prismacloud-api-5.2.4/prismacloud/api/cwpp/
--rw-r--r--   0 runner    (1001) docker     (123)      823 2023-06-22 15:51:20.000000 prismacloud-api-5.2.4/prismacloud/api/cwpp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2996 2023-06-22 15:51:20.000000 prismacloud-api-5.2.4/prismacloud/api/cwpp/_audits.py
--rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-06-22 15:51:20.000000 prismacloud-api-5.2.4/prismacloud/api/cwpp/_cloud.py
--rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-06-22 15:51:20.000000 prismacloud-api-5.2.4/prismacloud/api/cwpp/_collections.py
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-06-22 15:51:20.000000 prismacloud-api-5.2.4/prismacloud/api/cwpp/_containers.py
--rw-r--r--   0 runner    (1001) docker     (123)      877 2023-06-22 15:51:20.000000 prismacloud-api-5.2.4/prismacloud/api/cwpp/_credentials.py
--rw-r--r--   0 runner    (1001) docker     (123)      571 2023-06-22 15:51:20.000000 prismacloud-api-5.2.4/prismacloud/api/cwpp/_defenders.py
--rw-r--r--   0 runner    (1001) docker     (123)     2824 2023-06-22 15:51:20.000000 prismacloud-api-5.2.4/prismacloud/api/cwpp/_feeds.py
--rw-r--r--   0 runner    (1001) docker     (123)      888 2023-06-22 15:51:20.000000 prismacloud-api-5.2.4/prismacloud/api/cwpp/_hosts.py
--rw-r--r--   0 runner    (1001) docker     (123)      739 2023-06-22 15:51:20.000000 prismacloud-api-5.2.4/prismacloud/api/cwpp/_images.py
--rw-r--r--   0 runner    (1001) docker     (123)      938 2023-06-22 15:51:20.000000 prismacloud-api-5.2.4/prismacloud/api/cwpp/_logs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-06-22 15:51:20.000000 prismacloud-api-5.2.4/prismacloud/api/cwpp/_policies.py
--rw-r--r--   0 runner    (1001) docker     (123)      889 2023-06-22 15:51:20.000000 prismacloud-api-5.2.4/prismacloud/api/cwpp/_registry.py
--rw-r--r--   0 runner    (1001) docker     (123)      527 2023-06-22 15:51:20.000000 prismacloud-api-5.2.4/prismacloud/api/cwpp/_scans.py
--rw-r--r--   0 runner    (1001) docker     (123)     1431 2023-06-22 15:51:20.000000 prismacloud-api-5.2.4/prismacloud/api/cwpp/_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     3619 2023-06-22 15:51:20.000000 prismacloud-api-5.2.4/prismacloud/api/cwpp/_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)      376 2023-06-22 15:51:20.000000 prismacloud-api-5.2.4/prismacloud/api/cwpp/_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-06-22 15:51:20.000000 prismacloud-api-5.2.4/prismacloud/api/cwpp/_tags.py
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-06-22 15:51:20.000000 prismacloud-api-5.2.4/prismacloud/api/cwpp/_vms.py
--rw-r--r--   0 runner    (1001) docker     (123)     6316 2023-06-22 15:51:20.000000 prismacloud-api-5.2.4/prismacloud/api/cwpp/cwpp.py
--rw-r--r--   0 runner    (1001) docker     (123)     3422 2023-06-22 15:51:20.000000 prismacloud-api-5.2.4/prismacloud/api/pc_lib_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    17122 2023-06-22 15:51:20.000000 prismacloud-api-5.2.4/prismacloud/api/pc_lib_utility.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 15:51:39.732184 prismacloud-api-5.2.4/prismacloud/api/pccs/
--rw-r--r--   0 runner    (1001) docker     (123)      630 2023-06-22 15:51:20.000000 prismacloud-api-5.2.4/prismacloud/api/pccs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      342 2023-06-22 15:51:20.000000 prismacloud-api-5.2.4/prismacloud/api/pccs/_checkov_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-06-22 15:51:20.000000 prismacloud-api-5.2.4/prismacloud/api/pccs/_errors.py
--rw-r--r--   0 runner    (1001) docker     (123)      461 2023-06-22 15:51:20.000000 prismacloud-api-5.2.4/prismacloud/api/pccs/_fixes.py
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-06-22 15:51:20.000000 prismacloud-api-5.2.4/prismacloud/api/pccs/_packages.py
--rw-r--r--   0 runner    (1001) docker     (123)      873 2023-06-22 15:51:20.000000 prismacloud-api-5.2.4/prismacloud/api/pccs/_repositories.py
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-06-22 15:51:20.000000 prismacloud-api-5.2.4/prismacloud/api/pccs/_scans.py
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-22 15:51:20.000000 prismacloud-api-5.2.4/prismacloud/api/pccs/_suppressions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5277 2023-06-22 15:51:20.000000 prismacloud-api-5.2.4/prismacloud/api/pccs/pccs.py
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-22 15:51:20.000000 prismacloud-api-5.2.4/prismacloud/api/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 15:51:39.732184 prismacloud-api-5.2.4/prismacloud_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2854 2023-06-22 15:51:39.000000 prismacloud-api-5.2.4/prismacloud_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-06-22 15:51:39.000000 prismacloud-api-5.2.4/prismacloud_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 15:51:39.000000 prismacloud-api-5.2.4/prismacloud_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-22 15:51:39.000000 prismacloud-api-5.2.4/prismacloud_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-22 15:51:39.000000 prismacloud-api-5.2.4/prismacloud_api.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-06-22 15:51:20.000000 prismacloud-api-5.2.4/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 15:51:39.720184 prismacloud-api-5.2.4/scripts/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 15:51:39.732184 prismacloud-api-5.2.4/scripts/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     5394 2023-06-22 15:51:20.000000 prismacloud-api-5.2.4/scripts/examples/pcs_vuln_container_with_cve_2022_22965.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-22 15:51:39.736184 prismacloud-api-5.2.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-06-22 15:51:20.000000 prismacloud-api-5.2.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 15:51:39.732184 prismacloud-api-5.2.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2096 2023-06-22 15:51:20.000000 prismacloud-api-5.2.4/tests/unit.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 15:21:13.805801 prismacloud-api-5.2.5/
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-07-05 15:20:52.000000 prismacloud-api-5.2.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2854 2023-07-05 15:21:13.805801 prismacloud-api-5.2.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2332 2023-07-05 15:20:52.000000 prismacloud-api-5.2.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 15:21:13.797801 prismacloud-api-5.2.5/prismacloud/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 15:21:13.801801 prismacloud-api-5.2.5/prismacloud/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-07-05 15:20:52.000000 prismacloud-api-5.2.5/prismacloud/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 15:21:13.801801 prismacloud-api-5.2.5/prismacloud/api/cspm/
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-07-05 15:20:52.000000 prismacloud-api-5.2.5/prismacloud/api/cspm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18880 2023-07-05 15:20:52.000000 prismacloud-api-5.2.5/prismacloud/api/cspm/_endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3372 2023-07-05 15:20:52.000000 prismacloud-api-5.2.5/prismacloud/api/cspm/_extended.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8604 2023-07-05 15:20:52.000000 prismacloud-api-5.2.5/prismacloud/api/cspm/cspm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 15:21:13.805801 prismacloud-api-5.2.5/prismacloud/api/cwpp/
+-rw-r--r--   0 runner    (1001) docker     (123)      823 2023-07-05 15:20:52.000000 prismacloud-api-5.2.5/prismacloud/api/cwpp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2996 2023-07-05 15:20:52.000000 prismacloud-api-5.2.5/prismacloud/api/cwpp/_audits.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-07-05 15:20:52.000000 prismacloud-api-5.2.5/prismacloud/api/cwpp/_cloud.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-07-05 15:20:52.000000 prismacloud-api-5.2.5/prismacloud/api/cwpp/_collections.py
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-07-05 15:20:52.000000 prismacloud-api-5.2.5/prismacloud/api/cwpp/_containers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      877 2023-07-05 15:20:52.000000 prismacloud-api-5.2.5/prismacloud/api/cwpp/_credentials.py
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-07-05 15:20:52.000000 prismacloud-api-5.2.5/prismacloud/api/cwpp/_defenders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2824 2023-07-05 15:20:52.000000 prismacloud-api-5.2.5/prismacloud/api/cwpp/_feeds.py
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-07-05 15:20:52.000000 prismacloud-api-5.2.5/prismacloud/api/cwpp/_hosts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-07-05 15:20:52.000000 prismacloud-api-5.2.5/prismacloud/api/cwpp/_images.py
+-rw-r--r--   0 runner    (1001) docker     (123)      938 2023-07-05 15:20:52.000000 prismacloud-api-5.2.5/prismacloud/api/cwpp/_logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-07-05 15:20:52.000000 prismacloud-api-5.2.5/prismacloud/api/cwpp/_policies.py
+-rw-r--r--   0 runner    (1001) docker     (123)      889 2023-07-05 15:20:52.000000 prismacloud-api-5.2.5/prismacloud/api/cwpp/_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      527 2023-07-05 15:20:52.000000 prismacloud-api-5.2.5/prismacloud/api/cwpp/_scans.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1431 2023-07-05 15:20:52.000000 prismacloud-api-5.2.5/prismacloud/api/cwpp/_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3619 2023-07-05 15:20:52.000000 prismacloud-api-5.2.5/prismacloud/api/cwpp/_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-07-05 15:20:52.000000 prismacloud-api-5.2.5/prismacloud/api/cwpp/_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-07-05 15:20:52.000000 prismacloud-api-5.2.5/prismacloud/api/cwpp/_tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-07-05 15:20:52.000000 prismacloud-api-5.2.5/prismacloud/api/cwpp/_vms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6316 2023-07-05 15:20:52.000000 prismacloud-api-5.2.5/prismacloud/api/cwpp/cwpp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3422 2023-07-05 15:20:52.000000 prismacloud-api-5.2.5/prismacloud/api/pc_lib_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17122 2023-07-05 15:20:52.000000 prismacloud-api-5.2.5/prismacloud/api/pc_lib_utility.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 15:21:13.805801 prismacloud-api-5.2.5/prismacloud/api/pccs/
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-07-05 15:20:52.000000 prismacloud-api-5.2.5/prismacloud/api/pccs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-07-05 15:20:52.000000 prismacloud-api-5.2.5/prismacloud/api/pccs/_checkov_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-07-05 15:20:52.000000 prismacloud-api-5.2.5/prismacloud/api/pccs/_errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      461 2023-07-05 15:20:52.000000 prismacloud-api-5.2.5/prismacloud/api/pccs/_fixes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-07-05 15:20:52.000000 prismacloud-api-5.2.5/prismacloud/api/pccs/_packages.py
+-rw-r--r--   0 runner    (1001) docker     (123)      873 2023-07-05 15:20:52.000000 prismacloud-api-5.2.5/prismacloud/api/pccs/_repositories.py
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-07-05 15:20:52.000000 prismacloud-api-5.2.5/prismacloud/api/pccs/_scans.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-05 15:20:52.000000 prismacloud-api-5.2.5/prismacloud/api/pccs/_suppressions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5277 2023-07-05 15:20:52.000000 prismacloud-api-5.2.5/prismacloud/api/pccs/pccs.py
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-05 15:20:52.000000 prismacloud-api-5.2.5/prismacloud/api/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 15:21:13.805801 prismacloud-api-5.2.5/prismacloud_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2854 2023-07-05 15:21:13.000000 prismacloud-api-5.2.5/prismacloud_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-07-05 15:21:13.000000 prismacloud-api-5.2.5/prismacloud_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 15:21:13.000000 prismacloud-api-5.2.5/prismacloud_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-05 15:21:13.000000 prismacloud-api-5.2.5/prismacloud_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-05 15:21:13.000000 prismacloud-api-5.2.5/prismacloud_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-07-05 15:20:52.000000 prismacloud-api-5.2.5/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 15:21:13.797801 prismacloud-api-5.2.5/scripts/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 15:21:13.805801 prismacloud-api-5.2.5/scripts/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     5394 2023-07-05 15:20:52.000000 prismacloud-api-5.2.5/scripts/examples/pcs_vuln_container_with_cve_2022_22965.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-05 15:21:13.805801 prismacloud-api-5.2.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-07-05 15:20:52.000000 prismacloud-api-5.2.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 15:21:13.805801 prismacloud-api-5.2.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2096 2023-07-05 15:20:52.000000 prismacloud-api-5.2.5/tests/unit.py
```

### Comparing `prismacloud-api-5.2.4/LICENSE` & `prismacloud-api-5.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `prismacloud-api-5.2.4/PKG-INFO` & `prismacloud-api-5.2.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prismacloud-api
-Version: 5.2.4
+Version: 5.2.5
 Summary: Prisma Cloud API SDK for Python
 Home-page: https://github.com/PaloAltoNetworks/prismacloud-api-python
 Author: Tom Kishel
 Author-email: tkishel@paloaltonetworks.com
 Keywords: prisma cloud api
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `prismacloud-api-5.2.4/README.md` & `prismacloud-api-5.2.5/README.md`

 * *Files identical despite different names*

### Comparing `prismacloud-api-5.2.4/prismacloud/api/cspm/_endpoints.py` & `prismacloud-api-5.2.5/prismacloud/api/cspm/_endpoints.py`

 * *Files 0% similar despite different names*

```diff
@@ -331,19 +331,23 @@
     [x] LIST
     [ ] CREATE
     [ ] READ
     [ ] UPDATE
     [ ] DELETE
     Additional:
     [x] LIST (v2)
+    [x] LIST WITH FILTERS(v2)
     """
 
     def asset_inventory_list_read(self, query_params=None):
         return self.execute('GET', 'v2/inventory', query_params=query_params)
 
+    def asset_inventory_list_read_post(self, body_params=None):
+        return self.execute('POST', 'v2/inventory', body_params=body_params)
+
     """
     (Assets) Resources
 
     [ ] LIST
     [ ] CREATE
     [x] READ
     [ ] UPDATE
@@ -483,15 +487,15 @@
         api_response = self.execute(
             'POST', 'search/config', body_params=search_params)
         if 'data' in api_response and 'items' in api_response['data']:
             result = api_response['data']['items']
             next_page_token = api_response['data'].pop('nextPageToken', None)
         while next_page_token:
             api_response = self.execute(
-                'POST', 'search/config/page', body_params={'limit':1000,'pageToken': next_page_token, 'withResourceJson':'true'})
+                'POST', 'search/config/page', body_params={'limit': 1000, 'pageToken': next_page_token, 'withResourceJson': 'true'})
             if 'items' in api_response:
                 result.extend(api_response['items'])
             next_page_token = api_response.pop('nextPageToken', None)
         return result
 
     def search_network_read(self, search_params, filtered=False):
         search_url = 'search'
@@ -508,30 +512,31 @@
         api_response = self.execute(
             'POST', search_url, body_params=search_params)
         if 'data' in api_response and 'items' in api_response['data']:
             result = api_response['data']['items']
             next_page_token = api_response['data'].pop('nextPageToken', None)
         while next_page_token:
             api_response = self.execute(
-                'POST', 'search/config/page', body_params={'limit':1000,'pageToken': next_page_token})
+                'POST', 'search/config/page', body_params={'limit': 1000, 'pageToken': next_page_token})
             if 'items' in api_response:
                 result.extend(api_response['items'])
             next_page_token = api_response.pop('nextPageToken', None)
         return result
 
     def search_iam_read(self, search_params):
         result = []
         next_page_token = None
-        api_response = self.execute('POST', 'api/v1/permission', body_params=search_params)
+        api_response = self.execute(
+            'POST', 'api/v1/permission', body_params=search_params)
         if 'data' in api_response and 'items' in api_response['data']:
             result = api_response['data']['items']
             next_page_token = api_response['data'].pop('nextPageToken', None)
         while next_page_token:
             api_response = self.execute(
-                'POST', 'api/v1/permission/page', body_params={'limit':1000,'pageToken': next_page_token, 'withResourceJson':'true'})
+                'POST', 'api/v1/permission/page', body_params={'limit': 1000, 'pageToken': next_page_token, 'withResourceJson': 'true'})
             if 'items' in api_response:
                 result.extend(api_response['items'])
             next_page_token = api_response.pop('nextPageToken', None)
         return result
 
     def search_suggest_list_read(self, query_to_suggest):
         return self.execute('POST', 'search/suggest', body_params=query_to_suggest)
```

### Comparing `prismacloud-api-5.2.4/prismacloud/api/cspm/_extended.py` & `prismacloud-api-5.2.5/prismacloud/api/cspm/_extended.py`

 * *Files identical despite different names*

### Comparing `prismacloud-api-5.2.4/prismacloud/api/cspm/cspm.py` & `prismacloud-api-5.2.5/prismacloud/api/cspm/cspm.py`

 * *Files identical despite different names*

### Comparing `prismacloud-api-5.2.4/prismacloud/api/cwpp/__init__.py` & `prismacloud-api-5.2.5/prismacloud/api/cwpp/__init__.py`

 * *Files identical despite different names*

### Comparing `prismacloud-api-5.2.4/prismacloud/api/cwpp/_audits.py` & `prismacloud-api-5.2.5/prismacloud/api/cwpp/_audits.py`

 * *Files identical despite different names*

### Comparing `prismacloud-api-5.2.4/prismacloud/api/cwpp/_cloud.py` & `prismacloud-api-5.2.5/prismacloud/api/cwpp/_cloud.py`

 * *Files identical despite different names*

### Comparing `prismacloud-api-5.2.4/prismacloud/api/cwpp/_collections.py` & `prismacloud-api-5.2.5/prismacloud/api/cwpp/_collections.py`

 * *Files identical despite different names*

### Comparing `prismacloud-api-5.2.4/prismacloud/api/cwpp/_containers.py` & `prismacloud-api-5.2.5/prismacloud/api/cwpp/_containers.py`

 * *Files identical despite different names*

### Comparing `prismacloud-api-5.2.4/prismacloud/api/cwpp/_credentials.py` & `prismacloud-api-5.2.5/prismacloud/api/cwpp/_credentials.py`

 * *Files identical despite different names*

### Comparing `prismacloud-api-5.2.4/prismacloud/api/cwpp/_defenders.py` & `prismacloud-api-5.2.5/prismacloud/api/cwpp/_defenders.py`

 * *Files identical despite different names*

### Comparing `prismacloud-api-5.2.4/prismacloud/api/cwpp/_feeds.py` & `prismacloud-api-5.2.5/prismacloud/api/cwpp/_feeds.py`

 * *Files identical despite different names*

### Comparing `prismacloud-api-5.2.4/prismacloud/api/cwpp/_hosts.py` & `prismacloud-api-5.2.5/prismacloud/api/cwpp/_hosts.py`

 * *Files identical despite different names*

### Comparing `prismacloud-api-5.2.4/prismacloud/api/cwpp/_images.py` & `prismacloud-api-5.2.5/prismacloud/api/cwpp/_images.py`

 * *Files identical despite different names*

### Comparing `prismacloud-api-5.2.4/prismacloud/api/cwpp/_logs.py` & `prismacloud-api-5.2.5/prismacloud/api/cwpp/_logs.py`

 * *Files identical despite different names*

### Comparing `prismacloud-api-5.2.4/prismacloud/api/cwpp/_policies.py` & `prismacloud-api-5.2.5/prismacloud/api/cwpp/_policies.py`

 * *Files identical despite different names*

### Comparing `prismacloud-api-5.2.4/prismacloud/api/cwpp/_registry.py` & `prismacloud-api-5.2.5/prismacloud/api/cwpp/_registry.py`

 * *Files identical despite different names*

### Comparing `prismacloud-api-5.2.4/prismacloud/api/cwpp/_scans.py` & `prismacloud-api-5.2.5/prismacloud/api/cwpp/_scans.py`

 * *Files identical despite different names*

### Comparing `prismacloud-api-5.2.4/prismacloud/api/cwpp/_settings.py` & `prismacloud-api-5.2.5/prismacloud/api/cwpp/_settings.py`

 * *Files identical despite different names*

### Comparing `prismacloud-api-5.2.4/prismacloud/api/cwpp/_stats.py` & `prismacloud-api-5.2.5/prismacloud/api/cwpp/_stats.py`

 * *Files identical despite different names*

### Comparing `prismacloud-api-5.2.4/prismacloud/api/cwpp/_tags.py` & `prismacloud-api-5.2.5/prismacloud/api/cwpp/_tags.py`

 * *Files identical despite different names*

### Comparing `prismacloud-api-5.2.4/prismacloud/api/cwpp/cwpp.py` & `prismacloud-api-5.2.5/prismacloud/api/cwpp/cwpp.py`

 * *Files identical despite different names*

### Comparing `prismacloud-api-5.2.4/prismacloud/api/pc_lib_api.py` & `prismacloud-api-5.2.5/prismacloud/api/pc_lib_api.py`

 * *Files identical despite different names*

### Comparing `prismacloud-api-5.2.4/prismacloud/api/pc_lib_utility.py` & `prismacloud-api-5.2.5/prismacloud/api/pc_lib_utility.py`

 * *Files identical despite different names*

### Comparing `prismacloud-api-5.2.4/prismacloud/api/pccs/__init__.py` & `prismacloud-api-5.2.5/prismacloud/api/pccs/__init__.py`

 * *Files identical despite different names*

### Comparing `prismacloud-api-5.2.4/prismacloud/api/pccs/_errors.py` & `prismacloud-api-5.2.5/prismacloud/api/pccs/_errors.py`

 * *Files identical despite different names*

### Comparing `prismacloud-api-5.2.4/prismacloud/api/pccs/_repositories.py` & `prismacloud-api-5.2.5/prismacloud/api/pccs/_repositories.py`

 * *Files identical despite different names*

### Comparing `prismacloud-api-5.2.4/prismacloud/api/pccs/_suppressions.py` & `prismacloud-api-5.2.5/prismacloud/api/pccs/_suppressions.py`

 * *Files identical despite different names*

### Comparing `prismacloud-api-5.2.4/prismacloud/api/pccs/pccs.py` & `prismacloud-api-5.2.5/prismacloud/api/pccs/pccs.py`

 * *Files identical despite different names*

### Comparing `prismacloud-api-5.2.4/prismacloud_api.egg-info/PKG-INFO` & `prismacloud-api-5.2.5/prismacloud_api.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prismacloud-api
-Version: 5.2.4
+Version: 5.2.5
 Summary: Prisma Cloud API SDK for Python
 Home-page: https://github.com/PaloAltoNetworks/prismacloud-api-python
 Author: Tom Kishel
 Author-email: tkishel@paloaltonetworks.com
 Keywords: prisma cloud api
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `prismacloud-api-5.2.4/prismacloud_api.egg-info/SOURCES.txt` & `prismacloud-api-5.2.5/prismacloud_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `prismacloud-api-5.2.4/scripts/examples/pcs_vuln_container_with_cve_2022_22965.py` & `prismacloud-api-5.2.5/scripts/examples/pcs_vuln_container_with_cve_2022_22965.py`

 * *Files identical despite different names*

### Comparing `prismacloud-api-5.2.4/setup.py` & `prismacloud-api-5.2.5/setup.py`

 * *Files identical despite different names*

### Comparing `prismacloud-api-5.2.4/tests/unit.py` & `prismacloud-api-5.2.5/tests/unit.py`

 * *Files identical despite different names*

