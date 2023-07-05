# Comparing `tmp/xpanse-2.0.0rc4.tar.gz` & `tmp/xpanse-2.0.0rc5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xpanse-2.0.0rc4.tar", last modified: Wed Jun 14 17:25:08 2023, max compression
+gzip compressed data, was "xpanse-2.0.0rc5.tar", last modified: Wed Jul  5 14:20:47 2023, max compression
```

## Comparing `xpanse-2.0.0rc4.tar` & `xpanse-2.0.0rc5.tar`

### file list

```diff
@@ -1,80 +1,80 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 17:25:08.180911 xpanse-2.0.0rc4/
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-06-14 17:24:34.000000 xpanse-2.0.0rc4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-06-14 17:24:34.000000 xpanse-2.0.0rc4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4011 2023-06-14 17:25:08.180911 xpanse-2.0.0rc4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3119 2023-06-14 17:24:34.000000 xpanse-2.0.0rc4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 17:25:08.172911 xpanse-2.0.0rc4/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      791 2023-06-14 17:24:34.000000 xpanse-2.0.0rc4/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      656 2023-06-14 17:24:34.000000 xpanse-2.0.0rc4/docs/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 17:25:08.176911 xpanse-2.0.0rc4/docs/_source/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 17:25:08.176911 xpanse-2.0.0rc4/docs/_source/_static/
--rw-r--r--   0 runner    (1001) docker     (123)    17992 2023-06-14 17:24:34.000000 xpanse-2.0.0rc4/docs/_source/_static/xpanse_banner.png
--rw-r--r--   0 runner    (1001) docker     (123)     3531 2023-06-14 17:24:34.000000 xpanse-2.0.0rc4/docs/_source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     2247 2023-06-14 17:24:34.000000 xpanse-2.0.0rc4/docs/_source/cover.rst
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-06-14 17:24:34.000000 xpanse-2.0.0rc4/docs/_source/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      714 2023-06-14 17:24:34.000000 xpanse-2.0.0rc4/docs/_source/xpanse.api.asset_management.rst
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-06-14 17:24:34.000000 xpanse-2.0.0rc4/docs/_source/xpanse.api.attack_surface_rules.rst
--rw-r--r--   0 runner    (1001) docker     (123)      512 2023-06-14 17:24:34.000000 xpanse-2.0.0rc4/docs/_source/xpanse.api.incident_management.rst
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-06-14 17:24:34.000000 xpanse-2.0.0rc4/docs/_source/xpanse.api.rst
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-06-14 17:24:34.000000 xpanse-2.0.0rc4/docs/_source/xpanse.api.tags.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-06-14 17:24:34.000000 xpanse-2.0.0rc4/docs/_source/xpanse.rst
--rw-r--r--   0 runner    (1001) docker     (123)      618 2023-06-14 17:24:34.000000 xpanse-2.0.0rc4/docs/requirements-docs.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 17:25:08.172911 xpanse-2.0.0rc4/examples/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 17:25:08.176911 xpanse-2.0.0rc4/examples/asset_management/
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-06-14 17:24:34.000000 xpanse-2.0.0rc4/examples/asset_management/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     3418 2023-06-14 17:24:34.000000 xpanse-2.0.0rc4/examples/asset_management/get_services_by_asset.py
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-14 17:24:34.000000 xpanse-2.0.0rc4/examples/asset_management/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 17:25:08.176911 xpanse-2.0.0rc4/examples/incident_management/
--rw-r--r--   0 runner    (1001) docker     (123)      457 2023-06-14 17:24:34.000000 xpanse-2.0.0rc4/examples/incident_management/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-14 17:24:34.000000 xpanse-2.0.0rc4/examples/incident_management/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3557 2023-06-14 17:24:34.000000 xpanse-2.0.0rc4/examples/incident_management/update_incidents.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 17:25:08.176911 xpanse-2.0.0rc4/examples/tags/
--rw-r--r--   0 runner    (1001) docker     (123)      351 2023-06-14 17:24:34.000000 xpanse-2.0.0rc4/examples/tags/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2771 2023-06-14 17:24:34.000000 xpanse-2.0.0rc4/examples/tags/assign_and_remove_tags.py
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-14 17:24:34.000000 xpanse-2.0.0rc4/examples/tags/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 17:25:08.180911 xpanse-2.0.0rc4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-06-14 17:24:34.000000 xpanse-2.0.0rc4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 17:25:08.176911 xpanse-2.0.0rc4/xpanse/
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-06-14 17:24:34.000000 xpanse-2.0.0rc4/xpanse/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 17:25:08.176911 xpanse-2.0.0rc4/xpanse/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 17:24:34.000000 xpanse-2.0.0rc4/xpanse/api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 17:25:08.176911 xpanse-2.0.0rc4/xpanse/api/asset_management/
--rw-r--r--   0 runner    (1001) docker     (123)      968 2023-06-14 17:24:34.000000 xpanse-2.0.0rc4/xpanse/api/asset_management/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4080 2023-06-14 17:24:34.000000 xpanse-2.0.0rc4/xpanse/api/asset_management/assets_management_base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 17:25:08.176911 xpanse-2.0.0rc4/xpanse/api/asset_management/v1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 17:24:34.000000 xpanse-2.0.0rc4/xpanse/api/asset_management/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6859 2023-06-14 17:24:34.000000 xpanse-2.0.0rc4/xpanse/api/asset_management/v1/assets.py
--rw-r--r--   0 runner    (1001) docker     (123)     5412 2023-06-14 17:24:34.000000 xpanse-2.0.0rc4/xpanse/api/asset_management/v1/owned_ip_ranges.py
--rw-r--r--   0 runner    (1001) docker     (123)     5230 2023-06-14 17:24:34.000000 xpanse-2.0.0rc4/xpanse/api/asset_management/v1/services.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 17:25:08.176911 xpanse-2.0.0rc4/xpanse/api/attack_surface_rules/
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-06-14 17:24:34.000000 xpanse-2.0.0rc4/xpanse/api/attack_surface_rules/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 17:25:08.176911 xpanse-2.0.0rc4/xpanse/api/attack_surface_rules/v1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 17:24:34.000000 xpanse-2.0.0rc4/xpanse/api/attack_surface_rules/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6034 2023-06-14 17:24:34.000000 xpanse-2.0.0rc4/xpanse/api/attack_surface_rules/v1/attack_surface_rules.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 17:25:08.176911 xpanse-2.0.0rc4/xpanse/api/incident_management/
--rw-r--r--   0 runner    (1001) docker     (123)      635 2023-06-14 17:24:34.000000 xpanse-2.0.0rc4/xpanse/api/incident_management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 17:25:08.176911 xpanse-2.0.0rc4/xpanse/api/incident_management/v1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 17:24:34.000000 xpanse-2.0.0rc4/xpanse/api/incident_management/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7612 2023-06-14 17:24:34.000000 xpanse-2.0.0rc4/xpanse/api/incident_management/v1/incidents.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 17:25:08.180911 xpanse-2.0.0rc4/xpanse/api/incident_management/v2/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 17:24:34.000000 xpanse-2.0.0rc4/xpanse/api/incident_management/v2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5239 2023-06-14 17:24:34.000000 xpanse-2.0.0rc4/xpanse/api/incident_management/v2/alerts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 17:25:08.180911 xpanse-2.0.0rc4/xpanse/api/tags/
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-06-14 17:24:34.000000 xpanse-2.0.0rc4/xpanse/api/tags/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 17:25:08.180911 xpanse-2.0.0rc4/xpanse/api/tags/v1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 17:24:34.000000 xpanse-2.0.0rc4/xpanse/api/tags/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6754 2023-06-14 17:24:34.000000 xpanse-2.0.0rc4/xpanse/api/tags/v1/tags.py
--rw-r--r--   0 runner    (1001) docker     (123)    16292 2023-06-14 17:24:34.000000 xpanse-2.0.0rc4/xpanse/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3500 2023-06-14 17:24:34.000000 xpanse-2.0.0rc4/xpanse/const.py
--rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-06-14 17:24:34.000000 xpanse-2.0.0rc4/xpanse/endpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-06-14 17:24:34.000000 xpanse-2.0.0rc4/xpanse/error.py
--rw-r--r--   0 runner    (1001) docker     (123)     6309 2023-06-14 17:24:34.000000 xpanse-2.0.0rc4/xpanse/iterator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-06-14 17:24:34.000000 xpanse-2.0.0rc4/xpanse/response.py
--rw-r--r--   0 runner    (1001) docker     (123)      978 2023-06-14 17:24:34.000000 xpanse-2.0.0rc4/xpanse/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     2947 2023-06-14 17:24:34.000000 xpanse-2.0.0rc4/xpanse/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 17:25:08.176911 xpanse-2.0.0rc4/xpanse.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4011 2023-06-14 17:25:08.000000 xpanse-2.0.0rc4/xpanse.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1848 2023-06-14 17:25:08.000000 xpanse-2.0.0rc4/xpanse.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 17:25:08.000000 xpanse-2.0.0rc4/xpanse.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-14 17:25:08.000000 xpanse-2.0.0rc4/xpanse.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-14 17:25:08.000000 xpanse-2.0.0rc4/xpanse.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:20:47.929791 xpanse-2.0.0rc5/
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-07-05 14:20:16.000000 xpanse-2.0.0rc5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-07-05 14:20:16.000000 xpanse-2.0.0rc5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4011 2023-07-05 14:20:47.929791 xpanse-2.0.0rc5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3119 2023-07-05 14:20:16.000000 xpanse-2.0.0rc5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:20:47.925791 xpanse-2.0.0rc5/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      791 2023-07-05 14:20:16.000000 xpanse-2.0.0rc5/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      656 2023-07-05 14:20:16.000000 xpanse-2.0.0rc5/docs/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:20:47.925791 xpanse-2.0.0rc5/docs/_source/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:20:47.929791 xpanse-2.0.0rc5/docs/_source/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)    17992 2023-07-05 14:20:16.000000 xpanse-2.0.0rc5/docs/_source/_static/xpanse_banner.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3531 2023-07-05 14:20:16.000000 xpanse-2.0.0rc5/docs/_source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2247 2023-07-05 14:20:16.000000 xpanse-2.0.0rc5/docs/_source/cover.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-07-05 14:20:16.000000 xpanse-2.0.0rc5/docs/_source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      714 2023-07-05 14:20:16.000000 xpanse-2.0.0rc5/docs/_source/xpanse.api.asset_management.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-07-05 14:20:16.000000 xpanse-2.0.0rc5/docs/_source/xpanse.api.attack_surface_rules.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      512 2023-07-05 14:20:16.000000 xpanse-2.0.0rc5/docs/_source/xpanse.api.incident_management.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-07-05 14:20:16.000000 xpanse-2.0.0rc5/docs/_source/xpanse.api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-07-05 14:20:16.000000 xpanse-2.0.0rc5/docs/_source/xpanse.api.tags.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-07-05 14:20:16.000000 xpanse-2.0.0rc5/docs/_source/xpanse.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-07-05 14:20:16.000000 xpanse-2.0.0rc5/docs/requirements-docs.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:20:47.925791 xpanse-2.0.0rc5/examples/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:20:47.929791 xpanse-2.0.0rc5/examples/asset_management/
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-07-05 14:20:16.000000 xpanse-2.0.0rc5/examples/asset_management/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3418 2023-07-05 14:20:16.000000 xpanse-2.0.0rc5/examples/asset_management/get_services_by_asset.py
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-05 14:20:16.000000 xpanse-2.0.0rc5/examples/asset_management/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:20:47.929791 xpanse-2.0.0rc5/examples/incident_management/
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-07-05 14:20:16.000000 xpanse-2.0.0rc5/examples/incident_management/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-05 14:20:16.000000 xpanse-2.0.0rc5/examples/incident_management/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3557 2023-07-05 14:20:16.000000 xpanse-2.0.0rc5/examples/incident_management/update_incidents.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:20:47.929791 xpanse-2.0.0rc5/examples/tags/
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-07-05 14:20:16.000000 xpanse-2.0.0rc5/examples/tags/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2771 2023-07-05 14:20:16.000000 xpanse-2.0.0rc5/examples/tags/assign_and_remove_tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-05 14:20:16.000000 xpanse-2.0.0rc5/examples/tags/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-05 14:20:47.929791 xpanse-2.0.0rc5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-07-05 14:20:16.000000 xpanse-2.0.0rc5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:20:47.929791 xpanse-2.0.0rc5/xpanse/
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-07-05 14:20:16.000000 xpanse-2.0.0rc5/xpanse/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:20:47.929791 xpanse-2.0.0rc5/xpanse/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 14:20:16.000000 xpanse-2.0.0rc5/xpanse/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:20:47.929791 xpanse-2.0.0rc5/xpanse/api/asset_management/
+-rw-r--r--   0 runner    (1001) docker     (123)      968 2023-07-05 14:20:16.000000 xpanse-2.0.0rc5/xpanse/api/asset_management/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4080 2023-07-05 14:20:16.000000 xpanse-2.0.0rc5/xpanse/api/asset_management/assets_management_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:20:47.929791 xpanse-2.0.0rc5/xpanse/api/asset_management/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 14:20:16.000000 xpanse-2.0.0rc5/xpanse/api/asset_management/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6859 2023-07-05 14:20:16.000000 xpanse-2.0.0rc5/xpanse/api/asset_management/v1/assets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5412 2023-07-05 14:20:16.000000 xpanse-2.0.0rc5/xpanse/api/asset_management/v1/owned_ip_ranges.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5230 2023-07-05 14:20:16.000000 xpanse-2.0.0rc5/xpanse/api/asset_management/v1/services.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:20:47.929791 xpanse-2.0.0rc5/xpanse/api/attack_surface_rules/
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-07-05 14:20:16.000000 xpanse-2.0.0rc5/xpanse/api/attack_surface_rules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:20:47.929791 xpanse-2.0.0rc5/xpanse/api/attack_surface_rules/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 14:20:16.000000 xpanse-2.0.0rc5/xpanse/api/attack_surface_rules/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6034 2023-07-05 14:20:16.000000 xpanse-2.0.0rc5/xpanse/api/attack_surface_rules/v1/attack_surface_rules.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:20:47.929791 xpanse-2.0.0rc5/xpanse/api/incident_management/
+-rw-r--r--   0 runner    (1001) docker     (123)      635 2023-07-05 14:20:16.000000 xpanse-2.0.0rc5/xpanse/api/incident_management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:20:47.929791 xpanse-2.0.0rc5/xpanse/api/incident_management/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 14:20:16.000000 xpanse-2.0.0rc5/xpanse/api/incident_management/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7612 2023-07-05 14:20:16.000000 xpanse-2.0.0rc5/xpanse/api/incident_management/v1/incidents.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:20:47.929791 xpanse-2.0.0rc5/xpanse/api/incident_management/v2/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 14:20:16.000000 xpanse-2.0.0rc5/xpanse/api/incident_management/v2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5239 2023-07-05 14:20:16.000000 xpanse-2.0.0rc5/xpanse/api/incident_management/v2/alerts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:20:47.929791 xpanse-2.0.0rc5/xpanse/api/tags/
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-07-05 14:20:16.000000 xpanse-2.0.0rc5/xpanse/api/tags/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:20:47.929791 xpanse-2.0.0rc5/xpanse/api/tags/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 14:20:16.000000 xpanse-2.0.0rc5/xpanse/api/tags/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6754 2023-07-05 14:20:16.000000 xpanse-2.0.0rc5/xpanse/api/tags/v1/tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16292 2023-07-05 14:20:16.000000 xpanse-2.0.0rc5/xpanse/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3500 2023-07-05 14:20:16.000000 xpanse-2.0.0rc5/xpanse/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-07-05 14:20:16.000000 xpanse-2.0.0rc5/xpanse/endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-07-05 14:20:16.000000 xpanse-2.0.0rc5/xpanse/error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6309 2023-07-05 14:20:16.000000 xpanse-2.0.0rc5/xpanse/iterator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-07-05 14:20:16.000000 xpanse-2.0.0rc5/xpanse/response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      978 2023-07-05 14:20:16.000000 xpanse-2.0.0rc5/xpanse/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2947 2023-07-05 14:20:16.000000 xpanse-2.0.0rc5/xpanse/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:20:47.929791 xpanse-2.0.0rc5/xpanse.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4011 2023-07-05 14:20:47.000000 xpanse-2.0.0rc5/xpanse.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1848 2023-07-05 14:20:47.000000 xpanse-2.0.0rc5/xpanse.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 14:20:47.000000 xpanse-2.0.0rc5/xpanse.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-05 14:20:47.000000 xpanse-2.0.0rc5/xpanse.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-05 14:20:47.000000 xpanse-2.0.0rc5/xpanse.egg-info/top_level.txt
```

### Comparing `xpanse-2.0.0rc4/LICENSE` & `xpanse-2.0.0rc5/LICENSE`

 * *Files identical despite different names*

### Comparing `xpanse-2.0.0rc4/PKG-INFO` & `xpanse-2.0.0rc5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xpanse
-Version: 2.0.0rc4
+Version: 2.0.0rc5
 Summary: Python library is an interface to the Cortex Xpanse API.
 Home-page: UNKNOWN
 Author: Palo Alto Cortex Xpanse
 Author-email: xpanse-integrations@paloaltonetworks.com
 License: ISC
 Keywords: xpanse iom
 Platform: UNKNOWN
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: xpanse Version: 2.0.0rc4 Summary: Python library is
+Metadata-Version: 2.1 Name: xpanse Version: 2.0.0rc5 Summary: Python library is
 an interface to the Cortex Xpanse API. Home-page: UNKNOWN Author: Palo Alto
 Cortex Xpanse Author-email: xpanse-integrations@paloaltonetworks.com License:
 ISC Keywords: xpanse iom Platform: UNKNOWN Classifier: Development Status :: 5
 - Production/Stable Classifier: Intended Audience :: Developers Classifier:
 Topic :: Software Development Classifier: Topic :: Software Development ::
 Libraries Classifier: Topic :: Software Development :: Libraries :: Application
 Frameworks Classifier: Programming Language :: Python :: 3 Classifier:
```

### Comparing `xpanse-2.0.0rc4/README.md` & `xpanse-2.0.0rc5/README.md`

 * *Files identical despite different names*

### Comparing `xpanse-2.0.0rc4/docs/Makefile` & `xpanse-2.0.0rc5/docs/Makefile`

 * *Files identical despite different names*

### Comparing `xpanse-2.0.0rc4/docs/README.md` & `xpanse-2.0.0rc5/docs/README.md`

 * *Files identical despite different names*

### Comparing `xpanse-2.0.0rc4/docs/_source/_static/xpanse_banner.png` & `xpanse-2.0.0rc5/docs/_source/_static/xpanse_banner.png`

 * *Files identical despite different names*

### Comparing `xpanse-2.0.0rc4/docs/_source/conf.py` & `xpanse-2.0.0rc5/docs/_source/conf.py`

 * *Files identical despite different names*

### Comparing `xpanse-2.0.0rc4/docs/_source/cover.rst` & `xpanse-2.0.0rc5/docs/_source/cover.rst`

 * *Files identical despite different names*

### Comparing `xpanse-2.0.0rc4/docs/_source/xpanse.api.asset_management.rst` & `xpanse-2.0.0rc5/docs/_source/xpanse.api.asset_management.rst`

 * *Files identical despite different names*

### Comparing `xpanse-2.0.0rc4/docs/_source/xpanse.api.incident_management.rst` & `xpanse-2.0.0rc5/docs/_source/xpanse.api.incident_management.rst`

 * *Files identical despite different names*

### Comparing `xpanse-2.0.0rc4/docs/_source/xpanse.api.rst` & `xpanse-2.0.0rc5/docs/_source/xpanse.api.rst`

 * *Files identical despite different names*

### Comparing `xpanse-2.0.0rc4/docs/_source/xpanse.rst` & `xpanse-2.0.0rc5/docs/_source/xpanse.rst`

 * *Files identical despite different names*

### Comparing `xpanse-2.0.0rc4/docs/requirements-docs.txt` & `xpanse-2.0.0rc5/docs/requirements-docs.txt`

 * *Files identical despite different names*

### Comparing `xpanse-2.0.0rc4/examples/asset_management/get_services_by_asset.py` & `xpanse-2.0.0rc5/examples/asset_management/get_services_by_asset.py`

 * *Files identical despite different names*

### Comparing `xpanse-2.0.0rc4/examples/incident_management/update_incidents.py` & `xpanse-2.0.0rc5/examples/incident_management/update_incidents.py`

 * *Files identical despite different names*

### Comparing `xpanse-2.0.0rc4/examples/tags/assign_and_remove_tags.py` & `xpanse-2.0.0rc5/examples/tags/assign_and_remove_tags.py`

 * *Files identical despite different names*

### Comparing `xpanse-2.0.0rc4/setup.py` & `xpanse-2.0.0rc5/setup.py`

 * *Files identical despite different names*

### Comparing `xpanse-2.0.0rc4/xpanse/api/asset_management/__init__.py` & `xpanse-2.0.0rc5/xpanse/api/asset_management/__init__.py`

 * *Files identical despite different names*

### Comparing `xpanse-2.0.0rc4/xpanse/api/asset_management/assets_management_base.py` & `xpanse-2.0.0rc5/xpanse/api/asset_management/assets_management_base.py`

 * *Files identical despite different names*

### Comparing `xpanse-2.0.0rc4/xpanse/api/asset_management/v1/assets.py` & `xpanse-2.0.0rc5/xpanse/api/asset_management/v1/assets.py`

 * *Files identical despite different names*

### Comparing `xpanse-2.0.0rc4/xpanse/api/asset_management/v1/owned_ip_ranges.py` & `xpanse-2.0.0rc5/xpanse/api/asset_management/v1/owned_ip_ranges.py`

 * *Files identical despite different names*

### Comparing `xpanse-2.0.0rc4/xpanse/api/asset_management/v1/services.py` & `xpanse-2.0.0rc5/xpanse/api/asset_management/v1/services.py`

 * *Files identical despite different names*

### Comparing `xpanse-2.0.0rc4/xpanse/api/attack_surface_rules/v1/attack_surface_rules.py` & `xpanse-2.0.0rc5/xpanse/api/attack_surface_rules/v1/attack_surface_rules.py`

 * *Files identical despite different names*

### Comparing `xpanse-2.0.0rc4/xpanse/api/incident_management/__init__.py` & `xpanse-2.0.0rc5/xpanse/api/incident_management/__init__.py`

 * *Files identical despite different names*

### Comparing `xpanse-2.0.0rc4/xpanse/api/incident_management/v1/incidents.py` & `xpanse-2.0.0rc5/xpanse/api/incident_management/v1/incidents.py`

 * *Files identical despite different names*

### Comparing `xpanse-2.0.0rc4/xpanse/api/incident_management/v2/alerts.py` & `xpanse-2.0.0rc5/xpanse/api/incident_management/v2/alerts.py`

 * *Files identical despite different names*

### Comparing `xpanse-2.0.0rc4/xpanse/api/tags/v1/tags.py` & `xpanse-2.0.0rc5/xpanse/api/tags/v1/tags.py`

 * *Files identical despite different names*

### Comparing `xpanse-2.0.0rc4/xpanse/client.py` & `xpanse-2.0.0rc5/xpanse/client.py`

 * *Files identical despite different names*

### Comparing `xpanse-2.0.0rc4/xpanse/const.py` & `xpanse-2.0.0rc5/xpanse/const.py`

 * *Files identical despite different names*

### Comparing `xpanse-2.0.0rc4/xpanse/endpoint.py` & `xpanse-2.0.0rc5/xpanse/endpoint.py`

 * *Files identical despite different names*

### Comparing `xpanse-2.0.0rc4/xpanse/error.py` & `xpanse-2.0.0rc5/xpanse/error.py`

 * *Files identical despite different names*

### Comparing `xpanse-2.0.0rc4/xpanse/iterator.py` & `xpanse-2.0.0rc5/xpanse/iterator.py`

 * *Files identical despite different names*

### Comparing `xpanse-2.0.0rc4/xpanse/response.py` & `xpanse-2.0.0rc5/xpanse/response.py`

 * *Files identical despite different names*

### Comparing `xpanse-2.0.0rc4/xpanse/types.py` & `xpanse-2.0.0rc5/xpanse/types.py`

 * *Files identical despite different names*

### Comparing `xpanse-2.0.0rc4/xpanse/utils.py` & `xpanse-2.0.0rc5/xpanse/utils.py`

 * *Files identical despite different names*

### Comparing `xpanse-2.0.0rc4/xpanse.egg-info/PKG-INFO` & `xpanse-2.0.0rc5/xpanse.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xpanse
-Version: 2.0.0rc4
+Version: 2.0.0rc5
 Summary: Python library is an interface to the Cortex Xpanse API.
 Home-page: UNKNOWN
 Author: Palo Alto Cortex Xpanse
 Author-email: xpanse-integrations@paloaltonetworks.com
 License: ISC
 Keywords: xpanse iom
 Platform: UNKNOWN
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: xpanse Version: 2.0.0rc4 Summary: Python library is
+Metadata-Version: 2.1 Name: xpanse Version: 2.0.0rc5 Summary: Python library is
 an interface to the Cortex Xpanse API. Home-page: UNKNOWN Author: Palo Alto
 Cortex Xpanse Author-email: xpanse-integrations@paloaltonetworks.com License:
 ISC Keywords: xpanse iom Platform: UNKNOWN Classifier: Development Status :: 5
 - Production/Stable Classifier: Intended Audience :: Developers Classifier:
 Topic :: Software Development Classifier: Topic :: Software Development ::
 Libraries Classifier: Topic :: Software Development :: Libraries :: Application
 Frameworks Classifier: Programming Language :: Python :: 3 Classifier:
```

### Comparing `xpanse-2.0.0rc4/xpanse.egg-info/SOURCES.txt` & `xpanse-2.0.0rc5/xpanse.egg-info/SOURCES.txt`

 * *Files identical despite different names*

