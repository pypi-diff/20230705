# Comparing `tmp/idf_component_manager-1.3.1.tar.gz` & `tmp/idf_component_manager-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "idf_component_manager-1.3.1.tar", last modified: Mon Jul  3 18:15:38 2023, max compression
+gzip compressed data, was "idf_component_manager-1.3.2.tar", last modified: Wed Jul  5 06:54:01 2023, max compression
```

## Comparing `idf_component_manager-1.3.1.tar` & `idf_component_manager-1.3.2.tar`

### file list

```diff
@@ -1,108 +1,108 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 18:15:38.537039 idf_component_manager-1.3.1/
--rw-rw-rw-   0 root         (0) root         (0)    11358 2023-07-03 04:23:51.000000 idf_component_manager-1.3.1/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-03 04:23:51.000000 idf_component_manager-1.3.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)    10652 2023-07-03 18:15:38.537039 idf_component_manager-1.3.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     9376 2023-07-03 04:23:51.000000 idf_component_manager-1.3.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 18:15:38.533039 idf_component_manager-1.3.1/idf_component_manager/
--rw-rw-rw-   0 root         (0) root         (0)      285 2023-07-03 04:23:51.000000 idf_component_manager-1.3.1/idf_component_manager/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4463 2023-07-03 17:50:30.000000 idf_component_manager-1.3.1/idf_component_manager/__main__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 18:15:38.533039 idf_component_manager-1.3.1/idf_component_manager/cli/
--rw-rw-rw-   0 root         (0) root         (0)      161 2023-07-03 04:23:51.000000 idf_component_manager-1.3.1/idf_component_manager/cli/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6243 2023-07-03 17:50:30.000000 idf_component_manager-1.3.1/idf_component_manager/cli/autocompletion.py
--rw-rw-rw-   0 root         (0) root         (0)     1199 2023-07-03 04:23:51.000000 idf_component_manager-1.3.1/idf_component_manager/cli/cache.py
--rw-rw-rw-   0 root         (0) root         (0)     4464 2023-07-03 17:50:30.000000 idf_component_manager-1.3.1/idf_component_manager/cli/component.py
--rw-rw-rw-   0 root         (0) root         (0)     1671 2023-07-03 17:50:30.000000 idf_component_manager-1.3.1/idf_component_manager/cli/constants.py
--rw-rw-rw-   0 root         (0) root         (0)     1865 2023-07-03 17:50:30.000000 idf_component_manager-1.3.1/idf_component_manager/cli/core.py
--rw-rw-rw-   0 root         (0) root         (0)     2841 2023-07-03 17:50:30.000000 idf_component_manager-1.3.1/idf_component_manager/cli/manifest.py
--rw-rw-rw-   0 root         (0) root         (0)     1418 2023-07-03 17:50:30.000000 idf_component_manager-1.3.1/idf_component_manager/cli/project.py
--rw-rw-rw-   0 root         (0) root         (0)     3602 2023-07-03 17:50:30.000000 idf_component_manager-1.3.1/idf_component_manager/cli/registry.py
--rw-rw-rw-   0 root         (0) root         (0)      275 2023-07-03 04:23:51.000000 idf_component_manager-1.3.1/idf_component_manager/cli/utils.py
--rw-rw-rw-   0 root         (0) root         (0)     6568 2023-07-03 04:23:51.000000 idf_component_manager-1.3.1/idf_component_manager/cmake_component_requirements.py
--rw-rw-rw-   0 root         (0) root         (0)    27373 2023-07-03 17:50:30.000000 idf_component_manager-1.3.1/idf_component_manager/core.py
--rw-rw-rw-   0 root         (0) root         (0)     6209 2023-07-03 17:50:30.000000 idf_component_manager-1.3.1/idf_component_manager/core_utils.py
--rw-rw-rw-   0 root         (0) root         (0)    10024 2023-07-03 17:50:30.000000 idf_component_manager-1.3.1/idf_component_manager/dependencies.py
--rwxrwxrwx   0 root         (0) root         (0)     8695 2023-07-03 17:50:30.000000 idf_component_manager-1.3.1/idf_component_manager/idf_extensions.py
--rw-rw-rw-   0 root         (0) root         (0)      903 2023-07-03 17:50:30.000000 idf_component_manager-1.3.1/idf_component_manager/local_component_list.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 18:15:38.533039 idf_component_manager-1.3.1/idf_component_manager/prepare_components/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-03 04:23:51.000000 idf_component_manager-1.3.1/idf_component_manager/prepare_components/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      140 2023-07-03 04:23:51.000000 idf_component_manager-1.3.1/idf_component_manager/prepare_components/__main__.py
--rwxrwxrwx   0 root         (0) root         (0)     4014 2023-07-03 17:50:30.000000 idf_component_manager-1.3.1/idf_component_manager/prepare_components/prepare.py
--rw-rw-rw-   0 root         (0) root         (0)     3390 2023-07-03 17:50:31.000000 idf_component_manager-1.3.1/idf_component_manager/service_details.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 18:15:38.533039 idf_component_manager-1.3.1/idf_component_manager/templates/
--rw-rw-rw-   0 root         (0) root         (0)      559 2023-07-03 04:23:51.000000 idf_component_manager-1.3.1/idf_component_manager/templates/idf_component_template.yml
--rw-rw-rw-   0 root         (0) root         (0)     1587 2023-07-03 17:50:31.000000 idf_component_manager-1.3.1/idf_component_manager/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 18:15:38.533039 idf_component_manager-1.3.1/idf_component_manager/version_solver/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-03 04:23:51.000000 idf_component_manager-1.3.1/idf_component_manager/version_solver/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6279 2023-07-03 17:50:31.000000 idf_component_manager-1.3.1/idf_component_manager/version_solver/helper.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 18:15:38.533039 idf_component_manager-1.3.1/idf_component_manager/version_solver/mixology/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-03 04:23:51.000000 idf_component_manager-1.3.1/idf_component_manager/version_solver/mixology/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1839 2023-07-03 17:50:31.000000 idf_component_manager-1.3.1/idf_component_manager/version_solver/mixology/assignment.py
--rw-rw-rw-   0 root         (0) root         (0)     3904 2023-07-03 17:50:31.000000 idf_component_manager-1.3.1/idf_component_manager/version_solver/mixology/constraint.py
--rw-rw-rw-   0 root         (0) root         (0)     9409 2023-07-03 17:50:31.000000 idf_component_manager-1.3.1/idf_component_manager/version_solver/mixology/failure.py
--rw-rw-rw-   0 root         (0) root         (0)    14629 2023-07-03 17:50:31.000000 idf_component_manager-1.3.1/idf_component_manager/version_solver/mixology/incompatibility.py
--rw-rw-rw-   0 root         (0) root         (0)     1595 2023-07-03 17:50:31.000000 idf_component_manager-1.3.1/idf_component_manager/version_solver/mixology/incompatibility_cause.py
--rw-rw-rw-   0 root         (0) root         (0)     1428 2023-07-03 17:50:31.000000 idf_component_manager-1.3.1/idf_component_manager/version_solver/mixology/package.py
--rw-rw-rw-   0 root         (0) root         (0)     4188 2023-07-03 17:50:31.000000 idf_component_manager-1.3.1/idf_component_manager/version_solver/mixology/package_source.py
--rw-rw-rw-   0 root         (0) root         (0)     7477 2023-07-03 17:50:31.000000 idf_component_manager-1.3.1/idf_component_manager/version_solver/mixology/partial_solution.py
--rw-rw-rw-   0 root         (0) root         (0)    12692 2023-07-03 17:50:31.000000 idf_component_manager-1.3.1/idf_component_manager/version_solver/mixology/range.py
--rw-rw-rw-   0 root         (0) root         (0)      846 2023-07-03 17:50:31.000000 idf_component_manager-1.3.1/idf_component_manager/version_solver/mixology/result.py
--rw-rw-rw-   0 root         (0) root         (0)      352 2023-07-03 04:23:51.000000 idf_component_manager-1.3.1/idf_component_manager/version_solver/mixology/set_relation.py
--rw-rw-rw-   0 root         (0) root         (0)     6444 2023-07-03 17:50:31.000000 idf_component_manager-1.3.1/idf_component_manager/version_solver/mixology/term.py
--rw-rw-rw-   0 root         (0) root         (0)     6996 2023-07-03 17:50:31.000000 idf_component_manager-1.3.1/idf_component_manager/version_solver/mixology/union.py
--rw-rw-rw-   0 root         (0) root         (0)    15350 2023-07-03 17:50:31.000000 idf_component_manager-1.3.1/idf_component_manager/version_solver/mixology/version_solver.py
--rw-rw-rw-   0 root         (0) root         (0)     6158 2023-07-03 17:50:31.000000 idf_component_manager-1.3.1/idf_component_manager/version_solver/version_solver.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 18:15:38.533039 idf_component_manager-1.3.1/idf_component_manager.egg-info/
--rw-r--r--   0 root         (0) root         (0)    10652 2023-07-03 18:15:38.000000 idf_component_manager-1.3.1/idf_component_manager.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3872 2023-07-03 18:15:38.000000 idf_component_manager-1.3.1/idf_component_manager.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-03 18:15:38.000000 idf_component_manager-1.3.1/idf_component_manager.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       63 2023-07-03 18:15:38.000000 idf_component_manager-1.3.1/idf_component_manager.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      586 2023-07-03 18:15:38.000000 idf_component_manager-1.3.1/idf_component_manager.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       42 2023-07-03 18:15:38.000000 idf_component_manager-1.3.1/idf_component_manager.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 18:15:38.537039 idf_component_manager-1.3.1/idf_component_tools/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-03 04:23:51.000000 idf_component_manager-1.3.1/idf_component_tools/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      167 2023-07-03 17:56:09.000000 idf_component_manager-1.3.1/idf_component_tools/__version__.py
--rw-rw-rw-   0 root         (0) root         (0)    18685 2023-07-03 17:56:09.000000 idf_component_manager-1.3.1/idf_component_tools/api_client.py
--rw-rw-rw-   0 root         (0) root         (0)      585 2023-07-03 04:23:51.000000 idf_component_manager-1.3.1/idf_component_tools/api_client_errors.py
--rw-rw-rw-   0 root         (0) root         (0)     1984 2023-07-03 17:50:31.000000 idf_component_manager-1.3.1/idf_component_tools/api_schemas.py
--rw-rw-rw-   0 root         (0) root         (0)     2965 2023-07-03 17:50:31.000000 idf_component_manager-1.3.1/idf_component_tools/archive_tools.py
--rw-rw-rw-   0 root         (0) root         (0)     3105 2023-07-03 17:50:31.000000 idf_component_manager-1.3.1/idf_component_tools/build_system_tools.py
--rw-rw-rw-   0 root         (0) root         (0)     5273 2023-07-03 17:50:31.000000 idf_component_manager-1.3.1/idf_component_tools/config.py
--rw-rw-rw-   0 root         (0) root         (0)     1366 2023-07-03 17:50:31.000000 idf_component_manager-1.3.1/idf_component_tools/constants.py
--rw-rw-rw-   0 root         (0) root         (0)      730 2023-07-03 04:23:51.000000 idf_component_manager-1.3.1/idf_component_tools/environment.py
--rw-rw-rw-   0 root         (0) root         (0)     2939 2023-07-03 17:50:31.000000 idf_component_manager-1.3.1/idf_component_tools/errors.py
--rw-rw-rw-   0 root         (0) root         (0)     6240 2023-07-03 17:50:31.000000 idf_component_manager-1.3.1/idf_component_tools/file_cache.py
--rw-rw-rw-   0 root         (0) root         (0)     5324 2023-07-03 17:50:31.000000 idf_component_manager-1.3.1/idf_component_tools/file_tools.py
--rw-rw-rw-   0 root         (0) root         (0)     8366 2023-07-03 17:50:31.000000 idf_component_manager-1.3.1/idf_component_tools/git_client.py
--rw-rw-rw-   0 root         (0) root         (0)     3422 2023-07-03 17:50:31.000000 idf_component_manager-1.3.1/idf_component_tools/hash_tools.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 18:15:38.537039 idf_component_manager-1.3.1/idf_component_tools/lock/
--rw-rw-rw-   0 root         (0) root         (0)      208 2023-07-03 04:23:51.000000 idf_component_manager-1.3.1/idf_component_tools/lock/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4018 2023-07-03 17:50:31.000000 idf_component_manager-1.3.1/idf_component_tools/lock/manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 18:15:38.537039 idf_component_manager-1.3.1/idf_component_tools/manifest/
--rw-rw-rw-   0 root         (0) root         (0)     1059 2023-07-03 17:50:31.000000 idf_component_manager-1.3.1/idf_component_tools/manifest/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1688 2023-07-03 17:50:31.000000 idf_component_manager-1.3.1/idf_component_tools/manifest/constants.py
--rw-rw-rw-   0 root         (0) root         (0)     2190 2023-07-03 17:56:09.000000 idf_component_manager-1.3.1/idf_component_tools/manifest/env_expander.py
--rw-rw-rw-   0 root         (0) root         (0)     5112 2023-07-03 17:56:09.000000 idf_component_manager-1.3.1/idf_component_tools/manifest/if_parser.py
--rw-rw-rw-   0 root         (0) root         (0)     5012 2023-07-03 17:56:09.000000 idf_component_manager-1.3.1/idf_component_tools/manifest/manager.py
--rw-rw-rw-   0 root         (0) root         (0)    11197 2023-07-03 17:50:31.000000 idf_component_manager-1.3.1/idf_component_tools/manifest/manifest.py
--rw-rw-rw-   0 root         (0) root         (0)     4489 2023-07-03 17:50:31.000000 idf_component_manager-1.3.1/idf_component_tools/manifest/metadata.py
--rw-rw-rw-   0 root         (0) root         (0)     9176 2023-07-03 17:50:31.000000 idf_component_manager-1.3.1/idf_component_tools/manifest/schemas.py
--rw-rw-rw-   0 root         (0) root         (0)     2304 2023-07-03 17:50:31.000000 idf_component_manager-1.3.1/idf_component_tools/manifest/solved_component.py
--rw-rw-rw-   0 root         (0) root         (0)     1739 2023-07-03 17:50:31.000000 idf_component_manager-1.3.1/idf_component_tools/manifest/solved_manifest.py
--rw-rw-rw-   0 root         (0) root         (0)     7648 2023-07-03 17:50:31.000000 idf_component_manager-1.3.1/idf_component_tools/manifest/validator.py
--rw-rw-rw-   0 root         (0) root         (0)      345 2023-07-03 04:23:51.000000 idf_component_manager-1.3.1/idf_component_tools/network_tools.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 18:15:38.537039 idf_component_manager-1.3.1/idf_component_tools/semver/
--rw-rw-rw-   0 root         (0) root         (0)      452 2023-07-03 04:23:51.000000 idf_component_manager-1.3.1/idf_component_tools/semver/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    33154 2023-07-03 17:50:31.000000 idf_component_manager-1.3.1/idf_component_tools/semver/base.py
--rw-rw-rw-   0 root         (0) root         (0)     2753 2023-07-03 17:50:31.000000 idf_component_manager-1.3.1/idf_component_tools/serialization.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 18:15:38.537039 idf_component_manager-1.3.1/idf_component_tools/sources/
--rw-rw-rw-   0 root         (0) root         (0)      565 2023-07-03 17:50:31.000000 idf_component_manager-1.3.1/idf_component_tools/sources/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6591 2023-07-03 17:50:31.000000 idf_component_manager-1.3.1/idf_component_tools/sources/base.py
--rw-rw-rw-   0 root         (0) root         (0)     2486 2023-07-03 17:50:31.000000 idf_component_manager-1.3.1/idf_component_tools/sources/fetcher.py
--rw-rw-rw-   0 root         (0) root         (0)     7222 2023-07-03 17:50:31.000000 idf_component_manager-1.3.1/idf_component_tools/sources/git.py
--rw-rw-rw-   0 root         (0) root         (0)     1206 2023-07-03 04:23:51.000000 idf_component_manager-1.3.1/idf_component_tools/sources/idf.py
--rw-rw-rw-   0 root         (0) root         (0)     5179 2023-07-03 17:50:31.000000 idf_component_manager-1.3.1/idf_component_tools/sources/local.py
--rw-rw-rw-   0 root         (0) root         (0)      287 2023-07-03 04:23:51.000000 idf_component_manager-1.3.1/idf_component_tools/sources/utils.py
--rw-rw-rw-   0 root         (0) root         (0)     9847 2023-07-03 17:50:31.000000 idf_component_manager-1.3.1/idf_component_tools/sources/web_service.py
--rw-rw-rw-   0 root         (0) root         (0)     1787 2023-07-03 17:56:09.000000 idf_component_manager-1.3.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-03 18:15:38.537039 idf_component_manager-1.3.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     3165 2023-07-03 17:50:31.000000 idf_component_manager-1.3.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 06:54:01.269265 idf_component_manager-1.3.2/
+-rw-rw-rw-   0 root         (0) root         (0)    11358 2023-07-05 06:28:03.000000 idf_component_manager-1.3.2/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-05 06:28:03.000000 idf_component_manager-1.3.2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)    10652 2023-07-05 06:54:01.265265 idf_component_manager-1.3.2/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     9376 2023-07-05 06:28:03.000000 idf_component_manager-1.3.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 06:54:01.241264 idf_component_manager-1.3.2/idf_component_manager/
+-rw-rw-rw-   0 root         (0) root         (0)      285 2023-07-05 06:28:03.000000 idf_component_manager-1.3.2/idf_component_manager/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4463 2023-07-05 06:28:03.000000 idf_component_manager-1.3.2/idf_component_manager/__main__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 06:54:01.245264 idf_component_manager-1.3.2/idf_component_manager/cli/
+-rw-rw-rw-   0 root         (0) root         (0)      161 2023-07-05 06:28:03.000000 idf_component_manager-1.3.2/idf_component_manager/cli/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6243 2023-07-05 06:28:03.000000 idf_component_manager-1.3.2/idf_component_manager/cli/autocompletion.py
+-rw-rw-rw-   0 root         (0) root         (0)     1199 2023-07-05 06:28:03.000000 idf_component_manager-1.3.2/idf_component_manager/cli/cache.py
+-rw-rw-rw-   0 root         (0) root         (0)     4464 2023-07-05 06:28:03.000000 idf_component_manager-1.3.2/idf_component_manager/cli/component.py
+-rw-rw-rw-   0 root         (0) root         (0)     1671 2023-07-05 06:28:03.000000 idf_component_manager-1.3.2/idf_component_manager/cli/constants.py
+-rw-rw-rw-   0 root         (0) root         (0)     1865 2023-07-05 06:28:03.000000 idf_component_manager-1.3.2/idf_component_manager/cli/core.py
+-rw-rw-rw-   0 root         (0) root         (0)     2841 2023-07-05 06:28:03.000000 idf_component_manager-1.3.2/idf_component_manager/cli/manifest.py
+-rw-rw-rw-   0 root         (0) root         (0)     1418 2023-07-05 06:28:03.000000 idf_component_manager-1.3.2/idf_component_manager/cli/project.py
+-rw-rw-rw-   0 root         (0) root         (0)     3602 2023-07-05 06:28:03.000000 idf_component_manager-1.3.2/idf_component_manager/cli/registry.py
+-rw-rw-rw-   0 root         (0) root         (0)      275 2023-07-05 06:28:03.000000 idf_component_manager-1.3.2/idf_component_manager/cli/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     6568 2023-07-05 06:28:03.000000 idf_component_manager-1.3.2/idf_component_manager/cmake_component_requirements.py
+-rw-rw-rw-   0 root         (0) root         (0)    27373 2023-07-05 06:28:03.000000 idf_component_manager-1.3.2/idf_component_manager/core.py
+-rw-rw-rw-   0 root         (0) root         (0)     6209 2023-07-05 06:28:03.000000 idf_component_manager-1.3.2/idf_component_manager/core_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)    10024 2023-07-05 06:28:03.000000 idf_component_manager-1.3.2/idf_component_manager/dependencies.py
+-rwxrwxrwx   0 root         (0) root         (0)     8695 2023-07-05 06:28:03.000000 idf_component_manager-1.3.2/idf_component_manager/idf_extensions.py
+-rw-rw-rw-   0 root         (0) root         (0)      903 2023-07-05 06:28:03.000000 idf_component_manager-1.3.2/idf_component_manager/local_component_list.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 06:54:01.245264 idf_component_manager-1.3.2/idf_component_manager/prepare_components/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 06:28:03.000000 idf_component_manager-1.3.2/idf_component_manager/prepare_components/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      140 2023-07-05 06:28:03.000000 idf_component_manager-1.3.2/idf_component_manager/prepare_components/__main__.py
+-rwxrwxrwx   0 root         (0) root         (0)     4014 2023-07-05 06:28:03.000000 idf_component_manager-1.3.2/idf_component_manager/prepare_components/prepare.py
+-rw-rw-rw-   0 root         (0) root         (0)     3390 2023-07-05 06:28:03.000000 idf_component_manager-1.3.2/idf_component_manager/service_details.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 06:54:01.245264 idf_component_manager-1.3.2/idf_component_manager/templates/
+-rw-rw-rw-   0 root         (0) root         (0)      559 2023-07-05 06:28:03.000000 idf_component_manager-1.3.2/idf_component_manager/templates/idf_component_template.yml
+-rw-rw-rw-   0 root         (0) root         (0)     1587 2023-07-05 06:28:03.000000 idf_component_manager-1.3.2/idf_component_manager/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 06:54:01.249265 idf_component_manager-1.3.2/idf_component_manager/version_solver/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 06:28:03.000000 idf_component_manager-1.3.2/idf_component_manager/version_solver/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6466 2023-07-05 06:28:03.000000 idf_component_manager-1.3.2/idf_component_manager/version_solver/helper.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 06:54:01.253265 idf_component_manager-1.3.2/idf_component_manager/version_solver/mixology/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 06:28:03.000000 idf_component_manager-1.3.2/idf_component_manager/version_solver/mixology/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1839 2023-07-05 06:28:03.000000 idf_component_manager-1.3.2/idf_component_manager/version_solver/mixology/assignment.py
+-rw-rw-rw-   0 root         (0) root         (0)     3904 2023-07-05 06:28:03.000000 idf_component_manager-1.3.2/idf_component_manager/version_solver/mixology/constraint.py
+-rw-rw-rw-   0 root         (0) root         (0)     9409 2023-07-05 06:28:03.000000 idf_component_manager-1.3.2/idf_component_manager/version_solver/mixology/failure.py
+-rw-rw-rw-   0 root         (0) root         (0)    14629 2023-07-05 06:28:03.000000 idf_component_manager-1.3.2/idf_component_manager/version_solver/mixology/incompatibility.py
+-rw-rw-rw-   0 root         (0) root         (0)     1595 2023-07-05 06:28:03.000000 idf_component_manager-1.3.2/idf_component_manager/version_solver/mixology/incompatibility_cause.py
+-rw-rw-rw-   0 root         (0) root         (0)     1428 2023-07-05 06:28:03.000000 idf_component_manager-1.3.2/idf_component_manager/version_solver/mixology/package.py
+-rw-rw-rw-   0 root         (0) root         (0)     4188 2023-07-05 06:28:03.000000 idf_component_manager-1.3.2/idf_component_manager/version_solver/mixology/package_source.py
+-rw-rw-rw-   0 root         (0) root         (0)     7477 2023-07-05 06:28:03.000000 idf_component_manager-1.3.2/idf_component_manager/version_solver/mixology/partial_solution.py
+-rw-rw-rw-   0 root         (0) root         (0)    12692 2023-07-05 06:28:03.000000 idf_component_manager-1.3.2/idf_component_manager/version_solver/mixology/range.py
+-rw-rw-rw-   0 root         (0) root         (0)      846 2023-07-05 06:28:03.000000 idf_component_manager-1.3.2/idf_component_manager/version_solver/mixology/result.py
+-rw-rw-rw-   0 root         (0) root         (0)      352 2023-07-05 06:28:03.000000 idf_component_manager-1.3.2/idf_component_manager/version_solver/mixology/set_relation.py
+-rw-rw-rw-   0 root         (0) root         (0)     6444 2023-07-05 06:28:03.000000 idf_component_manager-1.3.2/idf_component_manager/version_solver/mixology/term.py
+-rw-rw-rw-   0 root         (0) root         (0)     6996 2023-07-05 06:28:03.000000 idf_component_manager-1.3.2/idf_component_manager/version_solver/mixology/union.py
+-rw-rw-rw-   0 root         (0) root         (0)    15350 2023-07-05 06:28:03.000000 idf_component_manager-1.3.2/idf_component_manager/version_solver/mixology/version_solver.py
+-rw-rw-rw-   0 root         (0) root         (0)     6130 2023-07-05 06:28:03.000000 idf_component_manager-1.3.2/idf_component_manager/version_solver/version_solver.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 06:54:01.241264 idf_component_manager-1.3.2/idf_component_manager.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    10652 2023-07-05 06:54:01.000000 idf_component_manager-1.3.2/idf_component_manager.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3872 2023-07-05 06:54:01.000000 idf_component_manager-1.3.2/idf_component_manager.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-05 06:54:01.000000 idf_component_manager-1.3.2/idf_component_manager.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       63 2023-07-05 06:54:01.000000 idf_component_manager-1.3.2/idf_component_manager.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      586 2023-07-05 06:54:01.000000 idf_component_manager-1.3.2/idf_component_manager.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       42 2023-07-05 06:54:01.000000 idf_component_manager-1.3.2/idf_component_manager.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 06:54:01.257265 idf_component_manager-1.3.2/idf_component_tools/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 06:28:03.000000 idf_component_manager-1.3.2/idf_component_tools/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      167 2023-07-05 06:28:03.000000 idf_component_manager-1.3.2/idf_component_tools/__version__.py
+-rw-rw-rw-   0 root         (0) root         (0)    18685 2023-07-05 06:28:03.000000 idf_component_manager-1.3.2/idf_component_tools/api_client.py
+-rw-rw-rw-   0 root         (0) root         (0)      585 2023-07-05 06:28:03.000000 idf_component_manager-1.3.2/idf_component_tools/api_client_errors.py
+-rw-rw-rw-   0 root         (0) root         (0)     1984 2023-07-05 06:28:03.000000 idf_component_manager-1.3.2/idf_component_tools/api_schemas.py
+-rw-rw-rw-   0 root         (0) root         (0)     3013 2023-07-05 06:28:03.000000 idf_component_manager-1.3.2/idf_component_tools/archive_tools.py
+-rw-rw-rw-   0 root         (0) root         (0)     3105 2023-07-05 06:28:03.000000 idf_component_manager-1.3.2/idf_component_tools/build_system_tools.py
+-rw-rw-rw-   0 root         (0) root         (0)     5273 2023-07-05 06:28:03.000000 idf_component_manager-1.3.2/idf_component_tools/config.py
+-rw-rw-rw-   0 root         (0) root         (0)     1366 2023-07-05 06:28:03.000000 idf_component_manager-1.3.2/idf_component_tools/constants.py
+-rw-rw-rw-   0 root         (0) root         (0)      730 2023-07-05 06:28:03.000000 idf_component_manager-1.3.2/idf_component_tools/environment.py
+-rw-rw-rw-   0 root         (0) root         (0)     2939 2023-07-05 06:28:03.000000 idf_component_manager-1.3.2/idf_component_tools/errors.py
+-rw-rw-rw-   0 root         (0) root         (0)     6240 2023-07-05 06:28:03.000000 idf_component_manager-1.3.2/idf_component_tools/file_cache.py
+-rw-rw-rw-   0 root         (0) root         (0)     5324 2023-07-05 06:28:03.000000 idf_component_manager-1.3.2/idf_component_tools/file_tools.py
+-rw-rw-rw-   0 root         (0) root         (0)     8366 2023-07-05 06:28:03.000000 idf_component_manager-1.3.2/idf_component_tools/git_client.py
+-rw-rw-rw-   0 root         (0) root         (0)     3422 2023-07-05 06:28:03.000000 idf_component_manager-1.3.2/idf_component_tools/hash_tools.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 06:54:01.257265 idf_component_manager-1.3.2/idf_component_tools/lock/
+-rw-rw-rw-   0 root         (0) root         (0)      208 2023-07-05 06:28:03.000000 idf_component_manager-1.3.2/idf_component_tools/lock/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4018 2023-07-05 06:28:03.000000 idf_component_manager-1.3.2/idf_component_tools/lock/manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 06:54:01.261265 idf_component_manager-1.3.2/idf_component_tools/manifest/
+-rw-rw-rw-   0 root         (0) root         (0)     1059 2023-07-05 06:28:03.000000 idf_component_manager-1.3.2/idf_component_tools/manifest/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1688 2023-07-05 06:28:03.000000 idf_component_manager-1.3.2/idf_component_tools/manifest/constants.py
+-rw-rw-rw-   0 root         (0) root         (0)     2190 2023-07-05 06:28:03.000000 idf_component_manager-1.3.2/idf_component_tools/manifest/env_expander.py
+-rw-rw-rw-   0 root         (0) root         (0)     6019 2023-07-05 06:28:03.000000 idf_component_manager-1.3.2/idf_component_tools/manifest/if_parser.py
+-rw-rw-rw-   0 root         (0) root         (0)     5012 2023-07-05 06:28:03.000000 idf_component_manager-1.3.2/idf_component_tools/manifest/manager.py
+-rw-rw-rw-   0 root         (0) root         (0)    11218 2023-07-05 06:28:03.000000 idf_component_manager-1.3.2/idf_component_tools/manifest/manifest.py
+-rw-rw-rw-   0 root         (0) root         (0)     4489 2023-07-05 06:28:03.000000 idf_component_manager-1.3.2/idf_component_tools/manifest/metadata.py
+-rw-rw-rw-   0 root         (0) root         (0)     9176 2023-07-05 06:28:03.000000 idf_component_manager-1.3.2/idf_component_tools/manifest/schemas.py
+-rw-rw-rw-   0 root         (0) root         (0)     2304 2023-07-05 06:28:03.000000 idf_component_manager-1.3.2/idf_component_tools/manifest/solved_component.py
+-rw-rw-rw-   0 root         (0) root         (0)     1739 2023-07-05 06:28:03.000000 idf_component_manager-1.3.2/idf_component_tools/manifest/solved_manifest.py
+-rw-rw-rw-   0 root         (0) root         (0)     7648 2023-07-05 06:28:03.000000 idf_component_manager-1.3.2/idf_component_tools/manifest/validator.py
+-rw-rw-rw-   0 root         (0) root         (0)      345 2023-07-05 06:28:03.000000 idf_component_manager-1.3.2/idf_component_tools/network_tools.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 06:54:01.261265 idf_component_manager-1.3.2/idf_component_tools/semver/
+-rw-rw-rw-   0 root         (0) root         (0)      452 2023-07-05 06:28:03.000000 idf_component_manager-1.3.2/idf_component_tools/semver/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    33154 2023-07-05 06:28:03.000000 idf_component_manager-1.3.2/idf_component_tools/semver/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     2753 2023-07-05 06:28:03.000000 idf_component_manager-1.3.2/idf_component_tools/serialization.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 06:54:01.265265 idf_component_manager-1.3.2/idf_component_tools/sources/
+-rw-rw-rw-   0 root         (0) root         (0)      565 2023-07-05 06:28:03.000000 idf_component_manager-1.3.2/idf_component_tools/sources/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6591 2023-07-05 06:28:03.000000 idf_component_manager-1.3.2/idf_component_tools/sources/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     2486 2023-07-05 06:28:03.000000 idf_component_manager-1.3.2/idf_component_tools/sources/fetcher.py
+-rw-rw-rw-   0 root         (0) root         (0)     7222 2023-07-05 06:28:03.000000 idf_component_manager-1.3.2/idf_component_tools/sources/git.py
+-rw-rw-rw-   0 root         (0) root         (0)     1206 2023-07-05 06:28:03.000000 idf_component_manager-1.3.2/idf_component_tools/sources/idf.py
+-rw-rw-rw-   0 root         (0) root         (0)     5179 2023-07-05 06:28:03.000000 idf_component_manager-1.3.2/idf_component_tools/sources/local.py
+-rw-rw-rw-   0 root         (0) root         (0)      287 2023-07-05 06:28:03.000000 idf_component_manager-1.3.2/idf_component_tools/sources/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     9847 2023-07-05 06:28:03.000000 idf_component_manager-1.3.2/idf_component_tools/sources/web_service.py
+-rw-rw-rw-   0 root         (0) root         (0)     1787 2023-07-05 06:28:03.000000 idf_component_manager-1.3.2/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-05 06:54:01.269265 idf_component_manager-1.3.2/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     3165 2023-07-05 06:28:03.000000 idf_component_manager-1.3.2/setup.py
```

### Comparing `idf_component_manager-1.3.1/LICENSE` & `idf_component_manager-1.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `idf_component_manager-1.3.1/PKG-INFO` & `idf_component_manager-1.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idf_component_manager
-Version: 1.3.1
+Version: 1.3.2
 Summary: The component manager for ESP-IDF
 Home-page: https://github.com/espressif/idf-component-manager
 Author: Sergei Silnov
 Author-email: sergei.silnov@espressif.com
 Maintainer: Sergei Silnov
 License: Apache License 2.0
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `idf_component_manager-1.3.1/README.md` & `idf_component_manager-1.3.2/README.md`

 * *Files identical despite different names*

### Comparing `idf_component_manager-1.3.1/idf_component_manager/__main__.py` & `idf_component_manager-1.3.2/idf_component_manager/__main__.py`

 * *Files identical despite different names*

### Comparing `idf_component_manager-1.3.1/idf_component_manager/cli/autocompletion.py` & `idf_component_manager-1.3.2/idf_component_manager/cli/autocompletion.py`

 * *Files identical despite different names*

### Comparing `idf_component_manager-1.3.1/idf_component_manager/cli/cache.py` & `idf_component_manager-1.3.2/idf_component_manager/cli/cache.py`

 * *Files identical despite different names*

### Comparing `idf_component_manager-1.3.1/idf_component_manager/cli/component.py` & `idf_component_manager-1.3.2/idf_component_manager/cli/component.py`

 * *Files identical despite different names*

### Comparing `idf_component_manager-1.3.1/idf_component_manager/cli/constants.py` & `idf_component_manager-1.3.2/idf_component_manager/cli/constants.py`

 * *Files identical despite different names*

### Comparing `idf_component_manager-1.3.1/idf_component_manager/cli/core.py` & `idf_component_manager-1.3.2/idf_component_manager/cli/core.py`

 * *Files identical despite different names*

### Comparing `idf_component_manager-1.3.1/idf_component_manager/cli/manifest.py` & `idf_component_manager-1.3.2/idf_component_manager/cli/manifest.py`

 * *Files identical despite different names*

### Comparing `idf_component_manager-1.3.1/idf_component_manager/cli/project.py` & `idf_component_manager-1.3.2/idf_component_manager/cli/project.py`

 * *Files identical despite different names*

### Comparing `idf_component_manager-1.3.1/idf_component_manager/cli/registry.py` & `idf_component_manager-1.3.2/idf_component_manager/cli/registry.py`

 * *Files identical despite different names*

### Comparing `idf_component_manager-1.3.1/idf_component_manager/cmake_component_requirements.py` & `idf_component_manager-1.3.2/idf_component_manager/cmake_component_requirements.py`

 * *Files identical despite different names*

### Comparing `idf_component_manager-1.3.1/idf_component_manager/core.py` & `idf_component_manager-1.3.2/idf_component_manager/core.py`

 * *Files identical despite different names*

### Comparing `idf_component_manager-1.3.1/idf_component_manager/core_utils.py` & `idf_component_manager-1.3.2/idf_component_manager/core_utils.py`

 * *Files identical despite different names*

### Comparing `idf_component_manager-1.3.1/idf_component_manager/dependencies.py` & `idf_component_manager-1.3.2/idf_component_manager/dependencies.py`

 * *Files identical despite different names*

### Comparing `idf_component_manager-1.3.1/idf_component_manager/idf_extensions.py` & `idf_component_manager-1.3.2/idf_component_manager/idf_extensions.py`

 * *Files identical despite different names*

### Comparing `idf_component_manager-1.3.1/idf_component_manager/local_component_list.py` & `idf_component_manager-1.3.2/idf_component_manager/local_component_list.py`

 * *Files identical despite different names*

### Comparing `idf_component_manager-1.3.1/idf_component_manager/prepare_components/prepare.py` & `idf_component_manager-1.3.2/idf_component_manager/prepare_components/prepare.py`

 * *Files identical despite different names*

### Comparing `idf_component_manager-1.3.1/idf_component_manager/service_details.py` & `idf_component_manager-1.3.2/idf_component_manager/service_details.py`

 * *Files identical despite different names*

### Comparing `idf_component_manager-1.3.1/idf_component_manager/templates/idf_component_template.yml` & `idf_component_manager-1.3.2/idf_component_manager/templates/idf_component_template.yml`

 * *Files identical despite different names*

### Comparing `idf_component_manager-1.3.1/idf_component_manager/utils.py` & `idf_component_manager-1.3.2/idf_component_manager/utils.py`

 * *Files identical despite different names*

### Comparing `idf_component_manager-1.3.1/idf_component_manager/version_solver/helper.py` & `idf_component_manager-1.3.2/idf_component_manager/version_solver/helper.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# SPDX-FileCopyrightText: 2022 Espressif Systems (Shanghai) CO LTD
+# SPDX-FileCopyrightText: 2022-2023 Espressif Systems (Shanghai) CO LTD
 # SPDX-License-Identifier: Apache-2.0
 
 from idf_component_tools.manifest import HashedComponentVersion
 
 from .mixology.failure import SolverFailure
 
 try:
@@ -102,14 +102,17 @@
             self._packages[package] = {}
 
         if version in self._packages[package]:
             return
 
         dependencies = []
         for dep_package, spec in deps.items():
+            if dep_package.source:
+                spec = dep_package.source.normalize_spec(spec)
+
             dependencies.append(Dependency(dep_package, spec))
 
         self._packages[package][version] = dependencies
 
     def override_dependencies(self, overriders):  # type: (set[str]) -> None
         for package in list(self._packages.keys()):
             if not package.source.is_overrider and package.name in overriders:
@@ -119,14 +122,17 @@
             for version in self._packages[package].keys():
                 self._packages[package][version] = [
                     elem for elem in self._packages[package][version]
                     if elem.package.source.is_overrider or elem.package.name not in overriders
                 ]
 
     def root_dep(self, package, spec):  # type: (Package, str) -> None
+        if package.source:
+            spec = package.source.normalize_spec(spec)
+
         self._root_dependencies.append(Dependency(package, spec))
 
     def _versions_for(self, package, constraint=None):  # type: (Package, Any) -> List[HashedComponentVersion]
         if package not in self._packages:
             return []
 
         versions = []
```

### Comparing `idf_component_manager-1.3.1/idf_component_manager/version_solver/mixology/assignment.py` & `idf_component_manager-1.3.2/idf_component_manager/version_solver/mixology/assignment.py`

 * *Files identical despite different names*

### Comparing `idf_component_manager-1.3.1/idf_component_manager/version_solver/mixology/constraint.py` & `idf_component_manager-1.3.2/idf_component_manager/version_solver/mixology/constraint.py`

 * *Files identical despite different names*

### Comparing `idf_component_manager-1.3.1/idf_component_manager/version_solver/mixology/failure.py` & `idf_component_manager-1.3.2/idf_component_manager/version_solver/mixology/failure.py`

 * *Files identical despite different names*

### Comparing `idf_component_manager-1.3.1/idf_component_manager/version_solver/mixology/incompatibility.py` & `idf_component_manager-1.3.2/idf_component_manager/version_solver/mixology/incompatibility.py`

 * *Files identical despite different names*

### Comparing `idf_component_manager-1.3.1/idf_component_manager/version_solver/mixology/incompatibility_cause.py` & `idf_component_manager-1.3.2/idf_component_manager/version_solver/mixology/incompatibility_cause.py`

 * *Files identical despite different names*

### Comparing `idf_component_manager-1.3.1/idf_component_manager/version_solver/mixology/package.py` & `idf_component_manager-1.3.2/idf_component_manager/version_solver/mixology/package.py`

 * *Files identical despite different names*

### Comparing `idf_component_manager-1.3.1/idf_component_manager/version_solver/mixology/package_source.py` & `idf_component_manager-1.3.2/idf_component_manager/version_solver/mixology/package_source.py`

 * *Files identical despite different names*

### Comparing `idf_component_manager-1.3.1/idf_component_manager/version_solver/mixology/partial_solution.py` & `idf_component_manager-1.3.2/idf_component_manager/version_solver/mixology/partial_solution.py`

 * *Files identical despite different names*

### Comparing `idf_component_manager-1.3.1/idf_component_manager/version_solver/mixology/range.py` & `idf_component_manager-1.3.2/idf_component_manager/version_solver/mixology/range.py`

 * *Files identical despite different names*

### Comparing `idf_component_manager-1.3.1/idf_component_manager/version_solver/mixology/result.py` & `idf_component_manager-1.3.2/idf_component_manager/version_solver/mixology/result.py`

 * *Files identical despite different names*

### Comparing `idf_component_manager-1.3.1/idf_component_manager/version_solver/mixology/term.py` & `idf_component_manager-1.3.2/idf_component_manager/version_solver/mixology/term.py`

 * *Files identical despite different names*

### Comparing `idf_component_manager-1.3.1/idf_component_manager/version_solver/mixology/union.py` & `idf_component_manager-1.3.2/idf_component_manager/version_solver/mixology/union.py`

 * *Files identical despite different names*

### Comparing `idf_component_manager-1.3.1/idf_component_manager/version_solver/mixology/version_solver.py` & `idf_component_manager-1.3.2/idf_component_manager/version_solver/mixology/version_solver.py`

 * *Files identical despite different names*

### Comparing `idf_component_manager-1.3.1/idf_component_manager/version_solver/version_solver.py` & `idf_component_manager-1.3.2/idf_component_manager/version_solver/version_solver.py`

 * *Files 1% similar despite different names*

```diff
@@ -113,15 +113,15 @@
                             req,
                             self._local_root_requirements[req.name],
                         ))
                     _req = self._local_root_requirements[req.name]
                 else:
                     _req = req
 
-                deps[Package(_req.name, _req.source)] = _req.source.normalize_spec(_req.version_spec)
+                deps[Package(_req.name, _req.source)] = _req.version_spec
 
             self._source.add(
                 Package(requirement.name, requirement.source),
                 version,
                 deps=deps,
             )
```

### Comparing `idf_component_manager-1.3.1/idf_component_manager.egg-info/PKG-INFO` & `idf_component_manager-1.3.2/idf_component_manager.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idf-component-manager
-Version: 1.3.1
+Version: 1.3.2
 Summary: The component manager for ESP-IDF
 Home-page: https://github.com/espressif/idf-component-manager
 Author: Sergei Silnov
 Author-email: sergei.silnov@espressif.com
 Maintainer: Sergei Silnov
 License: Apache License 2.0
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `idf_component_manager-1.3.1/idf_component_manager.egg-info/SOURCES.txt` & `idf_component_manager-1.3.2/idf_component_manager.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `idf_component_manager-1.3.1/idf_component_manager.egg-info/requires.txt` & `idf_component_manager-1.3.2/idf_component_manager.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `idf_component_manager-1.3.1/idf_component_tools/api_client.py` & `idf_component_manager-1.3.2/idf_component_tools/api_client.py`

 * *Files identical despite different names*

### Comparing `idf_component_manager-1.3.1/idf_component_tools/api_client_errors.py` & `idf_component_manager-1.3.2/idf_component_tools/api_client_errors.py`

 * *Files identical despite different names*

### Comparing `idf_component_manager-1.3.1/idf_component_tools/api_schemas.py` & `idf_component_manager-1.3.2/idf_component_tools/api_schemas.py`

 * *Files identical despite different names*

### Comparing `idf_component_manager-1.3.1/idf_component_tools/archive_tools.py` & `idf_component_manager-1.3.2/idf_component_tools/archive_tools.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# SPDX-FileCopyrightText: 2022 Espressif Systems (Shanghai) CO LTD
+# SPDX-FileCopyrightText: 2022-2023 Espressif Systems (Shanghai) CO LTD
 # SPDX-License-Identifier: Apache-2.0
 """Set of tools to work with archives"""
 
 import re
 import tarfile
 from pathlib import Path
 from shutil import get_archive_formats
@@ -90,15 +90,15 @@
     prepare_empty_directory(destination_directory)
 
     with zipfile.ZipFile(file) as archive:
         for item in archive.infolist():
             archive.extract(item, destination_directory)
 
 
-def unpack_archive(file, destination_directory):
+def unpack_archive(file, destination_directory):  # type: (Union[Text, Path], Text) -> None
     prepare_empty_directory(destination_directory)
     archive_format, ext, handler = get_format_from_path(file)
     if not is_known_format(archive_format):
         raise ArchiveError('.%s files are not supported on your system' % ext)
     handler(file, destination_directory)
```

### Comparing `idf_component_manager-1.3.1/idf_component_tools/build_system_tools.py` & `idf_component_manager-1.3.2/idf_component_tools/build_system_tools.py`

 * *Files identical despite different names*

### Comparing `idf_component_manager-1.3.1/idf_component_tools/config.py` & `idf_component_manager-1.3.2/idf_component_tools/config.py`

 * *Files identical despite different names*

### Comparing `idf_component_manager-1.3.1/idf_component_tools/constants.py` & `idf_component_manager-1.3.2/idf_component_tools/constants.py`

 * *Files identical despite different names*

### Comparing `idf_component_manager-1.3.1/idf_component_tools/environment.py` & `idf_component_manager-1.3.2/idf_component_tools/environment.py`

 * *Files identical despite different names*

### Comparing `idf_component_manager-1.3.1/idf_component_tools/errors.py` & `idf_component_manager-1.3.2/idf_component_tools/errors.py`

 * *Files identical despite different names*

### Comparing `idf_component_manager-1.3.1/idf_component_tools/file_cache.py` & `idf_component_manager-1.3.2/idf_component_tools/file_cache.py`

 * *Files identical despite different names*

### Comparing `idf_component_manager-1.3.1/idf_component_tools/file_tools.py` & `idf_component_manager-1.3.2/idf_component_tools/file_tools.py`

 * *Files identical despite different names*

### Comparing `idf_component_manager-1.3.1/idf_component_tools/git_client.py` & `idf_component_manager-1.3.2/idf_component_tools/git_client.py`

 * *Files identical despite different names*

### Comparing `idf_component_manager-1.3.1/idf_component_tools/hash_tools.py` & `idf_component_manager-1.3.2/idf_component_tools/hash_tools.py`

 * *Files identical despite different names*

### Comparing `idf_component_manager-1.3.1/idf_component_tools/lock/manager.py` & `idf_component_manager-1.3.2/idf_component_tools/lock/manager.py`

 * *Files identical despite different names*

### Comparing `idf_component_manager-1.3.1/idf_component_tools/manifest/__init__.py` & `idf_component_manager-1.3.2/idf_component_tools/manifest/__init__.py`

 * *Files identical despite different names*

### Comparing `idf_component_manager-1.3.1/idf_component_tools/manifest/constants.py` & `idf_component_manager-1.3.2/idf_component_tools/manifest/constants.py`

 * *Files identical despite different names*

### Comparing `idf_component_manager-1.3.1/idf_component_tools/manifest/env_expander.py` & `idf_component_manager-1.3.2/idf_component_tools/manifest/env_expander.py`

 * *Files identical despite different names*

### Comparing `idf_component_manager-1.3.1/idf_component_tools/manifest/if_parser.py` & `idf_component_manager-1.3.2/idf_component_tools/manifest/if_parser.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,130 +1,169 @@
 # SPDX-FileCopyrightText: 2022-2023 Espressif Systems (Shanghai) CO LTD
 # SPDX-License-Identifier: Apache-2.0
+
 import re
 from ast import literal_eval
 
 from schema import SchemaError
 
 from idf_component_tools.build_system_tools import get_env_idf_target, get_idf_version
 from idf_component_tools.errors import FetchingError, ProcessingError
 from idf_component_tools.manifest.constants import IF_IDF_VERSION_REGEX, IF_TARGET_REGEX
 from idf_component_tools.semver import SimpleSpec, Version
 from idf_component_tools.serialization import serializable
 
+try:
+    from typing import Literal
+except ImportError:
+    pass
+
 IF_IDF_VERSION_REGEX_COMPILED = re.compile(IF_IDF_VERSION_REGEX)
 IF_TARGET_REGEX_COMPILED = re.compile(IF_TARGET_REGEX)
 
 
 @serializable
 class IfClause:
     _serialization_properties = [
         'clause',
         'bool_value',
     ]
 
-    def __init__(self, clause, bool_value):  # type: (str, bool) -> None
-        self.clause = clause
-        self.bool_value = bool_value
+    @staticmethod
+    def eval_str(s):  # type: (str) -> str
+        _s = s.strip()
+        if not (_s[0] == _s[-1] == '"'):
+            _s = '"{}"'.format(_s.replace('"', r'\"'))
+
+        try:
+            return literal_eval(_s)
+        except (ValueError, SyntaxError):
+            raise SchemaError(None, 'Invalid string "{}" in "if" clause'.format(s))
 
-    def __repr__(self):
-        return '{} ({})'.format(self.clause, self.bool_value)
+    @staticmethod
+    def eval_list(s):  # type: (str) -> list[str]
+        _s = s.strip()
+
+        if _s[0] == '[' and _s[-1] == ']':
+            _s = _s[1:-1]
+
+        try:
+            return [IfClause.eval_str(part) for part in _s.split(',')]
+        except (ValueError, SyntaxError):
+            raise SchemaError(None, 'Invalid list "{}" in "if" clause'.format(s))
 
     @staticmethod
     def regex_str():
         if_idf_version = IF_IDF_VERSION_REGEX
         # remove the name group
         if_idf_version = re.sub(r'\(\?P<\w+>', '(?:', if_idf_version)
         # remove the first ^ and the last $ and make it as a group
         if_idf_version = '(' + if_idf_version[1:-1] + ')'
 
         if_target = IF_TARGET_REGEX
         # remove the name group
-        if_target = re.sub(r'\(\?P<\w+>', '(?:', if_idf_version)
+        if_target = re.sub(r'\(\?P<\w+>', '(?:', if_target)
         # remove the first ^ and the last $ and make it as a group
         if_target = '(' + if_target[1:-1] + ')'
 
         return '^{}|{}$'.format(if_idf_version, if_target)
 
+    @classmethod
+    def from_string(cls, s):  # type: (str) -> IfClause
+        return parse_if_clause(s)
 
-def _eval_str(s):  # type: (str) -> str
-    _s = s.strip()
-    if not (_s[0] == _s[-1] == '"'):
-        _s = '"{}"'.format(_s.replace('"', r'\"'))
 
-    try:
-        return literal_eval(_s)
-    except (ValueError, SyntaxError):
-        raise SchemaError(None, 'Invalid string "{}" in "if" clause'.format(s))
+class IfIdfVersionClause(IfClause):
+    def __init__(self, spec):  # type: (str) -> None
+        self.spec = spec
 
+    def __repr__(self):  # type: () -> str
+        return '{} ({})'.format(self.clause, self.bool_value)
 
-def _eval_list(s):  # type: (str) -> list[str]
-    _s = s.strip()
+    @property
+    def clause(self):  # type: () -> str
+        return 'idf_version {}'.format(self.spec)
+
+    @property
+    def bool_value(self):  # type: () -> bool
+        try:
+            idf_version = get_idf_version()
+        except FetchingError:
+            return False
 
-    if _s[0] == '[' and _s[-1] == ']':
-        _s = _s[1:-1]
+        return SimpleSpec(self.spec).match(Version(idf_version))
 
-    try:
-        return [_eval_str(part) for part in _s.split(',')]
-    except (ValueError, SyntaxError):
-        raise SchemaError(None, 'Invalid list "{}" in "if" clause'.format(s))
+
+@serializable
+class IfTargetClause(IfClause):
+    def __init__(self, operator, target_str):  # type: (Literal['==', '!=', 'in', 'not in'], str) -> None
+        self.operator = operator
+        self.target_str = target_str
+
+    def __repr__(self):
+        return '{} ({})'.format(self.clause, self.bool_value)
+
+    @property
+    def clause(self):  # type: () -> str
+        return 'target {} {}'.format(self.operator, self.target_str)
+
+    @property
+    def bool_value(self):
+        try:
+            env_target = get_env_idf_target()
+        except ProcessingError:
+            return False
+
+        if self.operator == '!=':
+            return env_target != self.eval_str(self.target_str)
+
+        if self.operator == '==':
+            return env_target == self.eval_str(self.target_str)
+
+        if self.operator == 'not in':
+            return env_target not in self.eval_list(self.target_str)
+
+        if self.operator == 'in':
+            return env_target in self.eval_list(self.target_str)
 
 
 def _parse_if_idf_version_clause(mat):  # type: (re.Match) -> IfClause
     comparison = mat.group('comparison')
     spec = mat.group('spec')
     spec = ','.join([part.strip() for part in spec.split(',')])
 
     try:
-        simple_spec = SimpleSpec('{}{}'.format(_eval_str(comparison), _eval_str(spec)))
+        simple_spec = SimpleSpec('{}{}'.format(IfClause.eval_str(comparison), IfClause.eval_str(spec)))
     except ValueError:
         raise SchemaError(
-            None, 'Invalid version specification for "idf_version": {clause}. Please use a format like '
+            None,
+            'Invalid version specification for "idf_version": {clause}. Please use a format like '
             '"idf_version >=4.4,<5.3"\nDocumentation: '
             'https://docs.espressif.com/projects/idf-component-manager/en/latest/reference/manifest_file.html#rules'.
-            format(clause=mat.string))
-
-    try:
-        idf_version = get_idf_version()
-    except FetchingError:
-        idf_version = None
-        bool_value = False
-    else:
-        bool_value = simple_spec.match(Version(idf_version))
+            format(clause=mat.string),
+        )
 
-    return IfClause('{} {}'.format(idf_version, simple_spec.expression), bool_value)
+    return IfIdfVersionClause(str(simple_spec))
 
 
 def _parser_if_target_clause(mat):  # type: (re.Match) -> IfClause
-    comparison = mat.group('comparison')
-    targets = mat.group('targets').strip()
+    operator = mat.group('comparison')
+    target_str = mat.group('targets').strip()
 
-    try:
-        env_target = get_env_idf_target()
-    except ProcessingError:
-        env_target = None
-        bool_value = False
-    else:
-        if comparison == '!=':
-            bool_value = env_target != _eval_str(targets)
-        elif comparison == '==':
-            bool_value = env_target == _eval_str(targets)
-        elif comparison == 'not in':
-            bool_value = env_target not in _eval_list(targets)
-        elif comparison == 'in':
-            bool_value = env_target in _eval_list(targets)
-        else:
-            raise SchemaError(
-                None, 'Invalid if clause format for target: {clause}. You can specify rules based on target using '
-                '"==", "!=", "in" or "not in" like: "target in [esp32, esp32c3]", "target == esp32"\n'
-                'Documentation: '
-                'https://docs.espressif.com/projects/idf-component-manager/en/latest/reference'
-                '/manifest_file.html#rules'.format(clause=mat.string))
+    if operator not in ['==', '!=', 'in', 'not in']:
+        raise SchemaError(
+            None,
+            'Invalid if clause format for target: {clause}. You can specify rules based on target using '
+            '"==", "!=", "in" or "not in" like: "target in [esp32, esp32c3]", "target == esp32"\n'
+            'Documentation: '
+            'https://docs.espressif.com/projects/idf-component-manager/en/latest/reference'
+            '/manifest_file.html#rules'.format(clause=mat.string),
+        )
 
-    return IfClause('{} {} {}'.format(env_target, comparison, targets), bool_value)
+    return IfTargetClause(operator, target_str)
 
 
 def parse_if_clause(if_clause):  # type: (str) -> IfClause
     res = IF_IDF_VERSION_REGEX_COMPILED.match(if_clause)
     if res:
         return _parse_if_idf_version_clause(res)
 
@@ -133,8 +172,9 @@
         return _parser_if_target_clause(res)
 
     raise SchemaError(
         None,
         'Invalid if clause format "{clause}". You can specify rules based on current ESP-IDF version or target like: '
         '"idf_version >=3.3,<5.0" or "target in [esp32, esp32c3]"\nDocumentation: '
         'https://docs.espressif.com/projects/idf-component-manager/en/latest/reference/manifest_file.html#rules'.format(
-            clause=if_clause))
+            clause=if_clause),
+    )
```

### Comparing `idf_component_manager-1.3.1/idf_component_tools/manifest/manager.py` & `idf_component_manager-1.3.2/idf_component_tools/manifest/manager.py`

 * *Files identical despite different names*

### Comparing `idf_component_manager-1.3.1/idf_component_tools/manifest/manifest.py` & `idf_component_manager-1.3.2/idf_component_tools/manifest/manifest.py`

 * *Files 2% similar despite different names*

```diff
@@ -131,27 +131,24 @@
                 name,
                 source,
                 version_spec=details.get('version') or '*',
                 public=details.get('public'),
                 if_clauses=details.get('rules'),
                 require=details.get('require', None),
             )
-            if component.meet_optional_dependencies:
-                manifest._dependencies.append(component)
-            else:
-                print('Skipping optional dependency: {}'.format(name))
+            manifest._dependencies.append(component)
 
         links = {link: manifest_tree.get(link, '') for link in LINKS}
         manifest.links = ComponentLinks(**links)
 
         return manifest
 
     @property
     def dependencies(self):  # type: () -> list[ComponentRequirement]
-        return sorted(self._dependencies, key=lambda d: d.name)
+        return sorted([dep for dep in self._dependencies if dep.meet_optional_dependencies], key=lambda d: d.name)
 
     @property
     def manifest_hash(self):  # type: () -> str
         if self._manifest_hash:
             return self._manifest_hash
 
         serialized = self.serialize(serialize_default=False)  # type: ignore
@@ -192,15 +189,15 @@
         self.source = source
         self._name = name
         self.public = None  # type: bool | None
         if require == 'public' or public:
             self.public = True
         elif public is False or require == 'private':
             self.public = False
-        self.if_clauses = if_clauses
+        self.if_clauses = if_clauses or []
         self.require = True if require in ['private', 'public', None] else False
 
     @property
     def meta(self):
         return self.source.meta
 
     @property
@@ -208,15 +205,18 @@
         return self.source.normalized_name(self._name)
 
     @property
     def meet_optional_dependencies(self):
         if not self.if_clauses:
             return True
 
-        return all(if_clause.bool_value for if_clause in self.if_clauses)
+        res = all(if_clause.bool_value for if_clause in self.if_clauses)
+        if not res:
+            print('Skipping optional dependency: {}'.format(self.name))
+        return res
 
     def __repr__(self):  # type: () -> str
         return 'ComponentRequirement("{}", {}, version_spec="{}", public={})'.format(
             self._name, self.source, self.version_spec, self.public)
 
     def __str__(self):  # type: () -> str
         return '{}({})'.format(self._name, self.version_spec)
```

### Comparing `idf_component_manager-1.3.1/idf_component_tools/manifest/metadata.py` & `idf_component_manager-1.3.2/idf_component_tools/manifest/metadata.py`

 * *Files identical despite different names*

### Comparing `idf_component_manager-1.3.1/idf_component_tools/manifest/schemas.py` & `idf_component_manager-1.3.2/idf_component_tools/manifest/schemas.py`

 * *Files identical despite different names*

### Comparing `idf_component_manager-1.3.1/idf_component_tools/manifest/solved_component.py` & `idf_component_manager-1.3.2/idf_component_tools/manifest/solved_component.py`

 * *Files identical despite different names*

### Comparing `idf_component_manager-1.3.1/idf_component_tools/manifest/solved_manifest.py` & `idf_component_manager-1.3.2/idf_component_tools/manifest/solved_manifest.py`

 * *Files identical despite different names*

### Comparing `idf_component_manager-1.3.1/idf_component_tools/manifest/validator.py` & `idf_component_manager-1.3.2/idf_component_tools/manifest/validator.py`

 * *Files identical despite different names*

### Comparing `idf_component_manager-1.3.1/idf_component_tools/semver/base.py` & `idf_component_manager-1.3.2/idf_component_tools/semver/base.py`

 * *Files identical despite different names*

### Comparing `idf_component_manager-1.3.1/idf_component_tools/serialization.py` & `idf_component_manager-1.3.2/idf_component_tools/serialization.py`

 * *Files identical despite different names*

### Comparing `idf_component_manager-1.3.1/idf_component_tools/sources/__init__.py` & `idf_component_manager-1.3.2/idf_component_tools/sources/__init__.py`

 * *Files identical despite different names*

### Comparing `idf_component_manager-1.3.1/idf_component_tools/sources/base.py` & `idf_component_manager-1.3.2/idf_component_tools/sources/base.py`

 * *Files identical despite different names*

### Comparing `idf_component_manager-1.3.1/idf_component_tools/sources/fetcher.py` & `idf_component_manager-1.3.2/idf_component_tools/sources/fetcher.py`

 * *Files identical despite different names*

### Comparing `idf_component_manager-1.3.1/idf_component_tools/sources/git.py` & `idf_component_manager-1.3.2/idf_component_tools/sources/git.py`

 * *Files identical despite different names*

### Comparing `idf_component_manager-1.3.1/idf_component_tools/sources/idf.py` & `idf_component_manager-1.3.2/idf_component_tools/sources/idf.py`

 * *Files identical despite different names*

### Comparing `idf_component_manager-1.3.1/idf_component_tools/sources/local.py` & `idf_component_manager-1.3.2/idf_component_tools/sources/local.py`

 * *Files identical despite different names*

### Comparing `idf_component_manager-1.3.1/idf_component_tools/sources/web_service.py` & `idf_component_manager-1.3.2/idf_component_tools/sources/web_service.py`

 * *Files identical despite different names*

### Comparing `idf_component_manager-1.3.1/pyproject.toml` & `idf_component_manager-1.3.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 
 
 [tool.poetry]
 name = "idf-component-manager"
-version = "1.3.1"
+version = "1.3.2"
 description = "Espressif IDF Component Manager"
 authors = []
 license = "Apache2"
 readme = "README.md"
 packages = [
     { include = "idf_component_manager" },
     { include = "idf_component_tools" },
```

### Comparing `idf_component_manager-1.3.1/setup.py` & `idf_component_manager-1.3.2/setup.py`

 * *Files identical despite different names*

