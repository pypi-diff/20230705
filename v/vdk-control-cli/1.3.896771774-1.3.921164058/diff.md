# Comparing `tmp/vdk-control-cli-1.3.896771774.tar.gz` & `tmp/vdk-control-cli-1.3.921164058.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/vdk-control-cli-1.3.896771774.tar", last modified: Mon Jun 12 08:45:26 2023, max compression
+gzip compressed data, was "dist/vdk-control-cli-1.3.921164058.tar", last modified: Wed Jul  5 06:50:36 2023, max compression
```

## Comparing `vdk-control-cli-1.3.896771774.tar` & `vdk-control-cli-1.3.921164058.tar`

### file list

```diff
@@ -1,74 +1,75 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 08:45:26.000000 vdk-control-cli-1.3.896771774/
--rw-rw-rw-   0 root         (0) root         (0)      270 2023-06-12 08:45:11.000000 vdk-control-cli-1.3.896771774/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     5153 2023-06-12 08:45:26.000000 vdk-control-cli-1.3.896771774/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     4192 2023-06-12 08:45:11.000000 vdk-control-cli-1.3.896771774/README.md
--rw-rw-rw-   0 root         (0) root         (0)     1747 2023-06-12 08:45:26.000000 vdk-control-cli-1.3.896771774/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      460 2023-06-12 08:45:11.000000 vdk-control-cli-1.3.896771774/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 08:45:26.000000 vdk-control-cli-1.3.896771774/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 08:45:26.000000 vdk-control-cli-1.3.896771774/src/vdk/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 08:45:26.000000 vdk-control-cli-1.3.896771774/src/vdk/api/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 08:45:26.000000 vdk-control-cli-1.3.896771774/src/vdk/api/control/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 08:45:26.000000 vdk-control-cli-1.3.896771774/src/vdk/api/control/plugin/
--rw-rw-rw-   0 root         (0) root         (0)      717 2023-06-12 08:45:11.000000 vdk-control-cli-1.3.896771774/src/vdk/api/control/plugin/markers.py
--rw-rw-rw-   0 root         (0) root         (0)     1423 2023-06-12 08:45:11.000000 vdk-control-cli-1.3.896771774/src/vdk/api/control/plugin/specs.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 08:45:26.000000 vdk-control-cli-1.3.896771774/src/vdk/internal/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 08:45:26.000000 vdk-control-cli-1.3.896771774/src/vdk/internal/control/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 08:45:26.000000 vdk-control-cli-1.3.896771774/src/vdk/internal/control/command_groups/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 08:45:26.000000 vdk-control-cli-1.3.896771774/src/vdk/internal/control/command_groups/common_group/
--rw-rw-rw-   0 root         (0) root         (0)     2284 2023-06-12 08:45:11.000000 vdk-control-cli-1.3.896771774/src/vdk/internal/control/command_groups/common_group/default.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 08:45:26.000000 vdk-control-cli-1.3.896771774/src/vdk/internal/control/command_groups/info_group/
--rw-rw-rw-   0 root         (0) root         (0)     1868 2023-06-12 08:45:11.000000 vdk-control-cli-1.3.896771774/src/vdk/internal/control/command_groups/info_group/info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 08:45:26.000000 vdk-control-cli-1.3.896771774/src/vdk/internal/control/command_groups/job/
--rw-rw-rw-   0 root         (0) root         (0)    12776 2023-06-12 08:45:11.000000 vdk-control-cli-1.3.896771774/src/vdk/internal/control/command_groups/job/create.py
--rw-rw-rw-   0 root         (0) root         (0)     2121 2023-06-12 08:45:11.000000 vdk-control-cli-1.3.896771774/src/vdk/internal/control/command_groups/job/delete.py
--rw-rw-rw-   0 root         (0) root         (0)     7121 2023-06-12 08:45:11.000000 vdk-control-cli-1.3.896771774/src/vdk/internal/control/command_groups/job/deploy_cli.py
--rw-rw-rw-   0 root         (0) root         (0)    14343 2023-06-12 08:45:11.000000 vdk-control-cli-1.3.896771774/src/vdk/internal/control/command_groups/job/deploy_cli_impl.py
--rw-rw-rw-   0 root         (0) root         (0)     5129 2023-06-12 08:45:11.000000 vdk-control-cli-1.3.896771774/src/vdk/internal/control/command_groups/job/download_job.py
--rw-rw-rw-   0 root         (0) root         (0)     2678 2023-06-12 08:45:11.000000 vdk-control-cli-1.3.896771774/src/vdk/internal/control/command_groups/job/download_key.py
--rw-rw-rw-   0 root         (0) root         (0)    12207 2023-06-12 08:45:11.000000 vdk-control-cli-1.3.896771774/src/vdk/internal/control/command_groups/job/execute.py
--rw-rw-rw-   0 root         (0) root         (0)     8735 2023-06-12 08:45:11.000000 vdk-control-cli-1.3.896771774/src/vdk/internal/control/command_groups/job/list.py
--rw-rw-rw-   0 root         (0) root         (0)    12040 2023-06-12 08:45:11.000000 vdk-control-cli-1.3.896771774/src/vdk/internal/control/command_groups/job/properties.py
--rw-rw-rw-   0 root         (0) root         (0)     3403 2023-06-12 08:45:11.000000 vdk-control-cli-1.3.896771774/src/vdk/internal/control/command_groups/job/show.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 08:45:26.000000 vdk-control-cli-1.3.896771774/src/vdk/internal/control/command_groups/login_group/
--rw-rw-rw-   0 root         (0) root         (0)     6510 2023-06-12 08:45:11.000000 vdk-control-cli-1.3.896771774/src/vdk/internal/control/command_groups/login_group/login.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 08:45:26.000000 vdk-control-cli-1.3.896771774/src/vdk/internal/control/command_groups/logout_group/
--rw-rw-rw-   0 root         (0) root         (0)      410 2023-06-12 08:45:11.000000 vdk-control-cli-1.3.896771774/src/vdk/internal/control/command_groups/logout_group/logout.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 08:45:26.000000 vdk-control-cli-1.3.896771774/src/vdk/internal/control/command_groups/version_group/
--rw-rw-rw-   0 root         (0) root         (0)      772 2023-06-12 08:45:11.000000 vdk-control-cli-1.3.896771774/src/vdk/internal/control/command_groups/version_group/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 08:45:26.000000 vdk-control-cli-1.3.896771774/src/vdk/internal/control/configuration/
--rw-rw-rw-   0 root         (0) root         (0)      424 2023-06-12 08:45:11.000000 vdk-control-cli-1.3.896771774/src/vdk/internal/control/configuration/default_options.py
--rw-rw-rw-   0 root         (0) root         (0)     1221 2023-06-12 08:45:11.000000 vdk-control-cli-1.3.896771774/src/vdk/internal/control/configuration/defaults_config.py
--rw-rw-rw-   0 root         (0) root         (0)     2272 2023-06-12 08:45:11.000000 vdk-control-cli-1.3.896771774/src/vdk/internal/control/configuration/log_config.py
--rw-rw-rw-   0 root         (0) root         (0)     9551 2023-06-12 08:45:11.000000 vdk-control-cli-1.3.896771774/src/vdk/internal/control/configuration/vdk_config.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 08:45:26.000000 vdk-control-cli-1.3.896771774/src/vdk/internal/control/exception/
--rw-rw-rw-   0 root         (0) root         (0)      649 2023-06-12 08:45:11.000000 vdk-control-cli-1.3.896771774/src/vdk/internal/control/exception/vdk_exception.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 08:45:26.000000 vdk-control-cli-1.3.896771774/src/vdk/internal/control/job/
--rw-rw-rw-   0 root         (0) root         (0)     1930 2023-06-12 08:45:11.000000 vdk-control-cli-1.3.896771774/src/vdk/internal/control/job/job_archive.py
--rw-rw-rw-   0 root         (0) root         (0)     4871 2023-06-12 08:45:11.000000 vdk-control-cli-1.3.896771774/src/vdk/internal/control/job/job_config.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 08:45:26.000000 vdk-control-cli-1.3.896771774/src/vdk/internal/control/job/sample_job/
--rw-rw-rw-   0 root         (0) root         (0)      579 2023-06-12 08:45:11.000000 vdk-control-cli-1.3.896771774/src/vdk/internal/control/job/sample_job/10_sql_step.sql
--rw-rw-rw-   0 root         (0) root         (0)      816 2023-06-12 08:45:11.000000 vdk-control-cli-1.3.896771774/src/vdk/internal/control/job/sample_job/20_python_step.py
--rw-rw-rw-   0 root         (0) root         (0)     1446 2023-06-12 08:45:11.000000 vdk-control-cli-1.3.896771774/src/vdk/internal/control/job/sample_job/README.md
--rw-rw-rw-   0 root         (0) root         (0)     2902 2023-06-12 08:45:11.000000 vdk-control-cli-1.3.896771774/src/vdk/internal/control/job/sample_job/config.ini
--rw-rw-rw-   0 root         (0) root         (0)      243 2023-06-12 08:45:11.000000 vdk-control-cli-1.3.896771774/src/vdk/internal/control/job/sample_job/requirements.txt
--rw-rw-rw-   0 root         (0) root         (0)     3553 2023-06-12 08:45:11.000000 vdk-control-cli-1.3.896771774/src/vdk/internal/control/main.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 08:45:26.000000 vdk-control-cli-1.3.896771774/src/vdk/internal/control/plugin/
--rw-rw-rw-   0 root         (0) root         (0)     3715 2023-06-12 08:45:11.000000 vdk-control-cli-1.3.896771774/src/vdk/internal/control/plugin/control_plugin_manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 08:45:26.000000 vdk-control-cli-1.3.896771774/src/vdk/internal/control/rest_lib/
--rw-rw-rw-   0 root         (0) root         (0)     3077 2023-06-12 08:45:11.000000 vdk-control-cli-1.3.896771774/src/vdk/internal/control/rest_lib/factory.py
--rw-rw-rw-   0 root         (0) root         (0)     3845 2023-06-12 08:45:11.000000 vdk-control-cli-1.3.896771774/src/vdk/internal/control/rest_lib/rest_client_errors.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 08:45:26.000000 vdk-control-cli-1.3.896771774/src/vdk/internal/control/utils/
--rw-rw-rw-   0 root         (0) root         (0)     7297 2023-06-12 08:45:11.000000 vdk-control-cli-1.3.896771774/src/vdk/internal/control/utils/cli_utils.py
--rw-rw-rw-   0 root         (0) root         (0)     1413 2023-06-12 08:45:11.000000 vdk-control-cli-1.3.896771774/src/vdk/internal/control/utils/control_utils.py
--rw-rw-rw-   0 root         (0) root         (0)     3690 2023-06-12 08:45:11.000000 vdk-control-cli-1.3.896771774/src/vdk/internal/control/utils/output_printer.py
--rw-rw-rw-   0 root         (0) root         (0)      819 2023-06-12 08:45:11.000000 vdk-control-cli-1.3.896771774/src/vdk/internal/control/utils/version_utils.py
--rw-rw-rw-   0 root         (0) root         (0)      181 2023-06-12 08:45:15.000000 vdk-control-cli-1.3.896771774/src/vdk/internal/control/vdk_control_build_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 08:45:26.000000 vdk-control-cli-1.3.896771774/src/vdk_control_cli.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5153 2023-06-12 08:45:26.000000 vdk-control-cli-1.3.896771774/src/vdk_control_cli.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2371 2023-06-12 08:45:26.000000 vdk-control-cli-1.3.896771774/src/vdk_control_cli.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-12 08:45:26.000000 vdk-control-cli-1.3.896771774/src/vdk_control_cli.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       57 2023-06-12 08:45:26.000000 vdk-control-cli-1.3.896771774/src/vdk_control_cli.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-12 08:45:26.000000 vdk-control-cli-1.3.896771774/src/vdk_control_cli.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      185 2023-06-12 08:45:26.000000 vdk-control-cli-1.3.896771774/src/vdk_control_cli.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        4 2023-06-12 08:45:26.000000 vdk-control-cli-1.3.896771774/src/vdk_control_cli.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)       14 2023-06-12 08:45:15.000000 vdk-control-cli-1.3.896771774/version.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 06:50:36.000000 vdk-control-cli-1.3.921164058/
+-rw-rw-rw-   0 root         (0) root         (0)      270 2023-07-05 06:50:20.000000 vdk-control-cli-1.3.921164058/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     5153 2023-07-05 06:50:36.000000 vdk-control-cli-1.3.921164058/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     4192 2023-07-05 06:50:20.000000 vdk-control-cli-1.3.921164058/README.md
+-rw-rw-rw-   0 root         (0) root         (0)     1747 2023-07-05 06:50:36.000000 vdk-control-cli-1.3.921164058/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      460 2023-07-05 06:50:20.000000 vdk-control-cli-1.3.921164058/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 06:50:36.000000 vdk-control-cli-1.3.921164058/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 06:50:36.000000 vdk-control-cli-1.3.921164058/src/vdk/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 06:50:36.000000 vdk-control-cli-1.3.921164058/src/vdk/api/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 06:50:36.000000 vdk-control-cli-1.3.921164058/src/vdk/api/control/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 06:50:36.000000 vdk-control-cli-1.3.921164058/src/vdk/api/control/plugin/
+-rw-rw-rw-   0 root         (0) root         (0)      717 2023-07-05 06:50:20.000000 vdk-control-cli-1.3.921164058/src/vdk/api/control/plugin/markers.py
+-rw-rw-rw-   0 root         (0) root         (0)     1423 2023-07-05 06:50:20.000000 vdk-control-cli-1.3.921164058/src/vdk/api/control/plugin/specs.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 06:50:36.000000 vdk-control-cli-1.3.921164058/src/vdk/internal/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 06:50:36.000000 vdk-control-cli-1.3.921164058/src/vdk/internal/control/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 06:50:36.000000 vdk-control-cli-1.3.921164058/src/vdk/internal/control/command_groups/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 06:50:36.000000 vdk-control-cli-1.3.921164058/src/vdk/internal/control/command_groups/common_group/
+-rw-rw-rw-   0 root         (0) root         (0)     2284 2023-07-05 06:50:20.000000 vdk-control-cli-1.3.921164058/src/vdk/internal/control/command_groups/common_group/default.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 06:50:36.000000 vdk-control-cli-1.3.921164058/src/vdk/internal/control/command_groups/info_group/
+-rw-rw-rw-   0 root         (0) root         (0)     1868 2023-07-05 06:50:20.000000 vdk-control-cli-1.3.921164058/src/vdk/internal/control/command_groups/info_group/info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 06:50:36.000000 vdk-control-cli-1.3.921164058/src/vdk/internal/control/command_groups/job/
+-rw-rw-rw-   0 root         (0) root         (0)    12776 2023-07-05 06:50:20.000000 vdk-control-cli-1.3.921164058/src/vdk/internal/control/command_groups/job/create.py
+-rw-rw-rw-   0 root         (0) root         (0)     2121 2023-07-05 06:50:20.000000 vdk-control-cli-1.3.921164058/src/vdk/internal/control/command_groups/job/delete.py
+-rw-rw-rw-   0 root         (0) root         (0)     7121 2023-07-05 06:50:20.000000 vdk-control-cli-1.3.921164058/src/vdk/internal/control/command_groups/job/deploy_cli.py
+-rw-rw-rw-   0 root         (0) root         (0)    14343 2023-07-05 06:50:20.000000 vdk-control-cli-1.3.921164058/src/vdk/internal/control/command_groups/job/deploy_cli_impl.py
+-rw-rw-rw-   0 root         (0) root         (0)     5129 2023-07-05 06:50:20.000000 vdk-control-cli-1.3.921164058/src/vdk/internal/control/command_groups/job/download_job.py
+-rw-rw-rw-   0 root         (0) root         (0)     2678 2023-07-05 06:50:20.000000 vdk-control-cli-1.3.921164058/src/vdk/internal/control/command_groups/job/download_key.py
+-rw-rw-rw-   0 root         (0) root         (0)    12207 2023-07-05 06:50:20.000000 vdk-control-cli-1.3.921164058/src/vdk/internal/control/command_groups/job/execute.py
+-rw-rw-rw-   0 root         (0) root         (0)     8735 2023-07-05 06:50:20.000000 vdk-control-cli-1.3.921164058/src/vdk/internal/control/command_groups/job/list.py
+-rw-rw-rw-   0 root         (0) root         (0)    12040 2023-07-05 06:50:20.000000 vdk-control-cli-1.3.921164058/src/vdk/internal/control/command_groups/job/properties.py
+-rw-rw-rw-   0 root         (0) root         (0)    11456 2023-07-05 06:50:20.000000 vdk-control-cli-1.3.921164058/src/vdk/internal/control/command_groups/job/secrets.py
+-rw-rw-rw-   0 root         (0) root         (0)     3403 2023-07-05 06:50:20.000000 vdk-control-cli-1.3.921164058/src/vdk/internal/control/command_groups/job/show.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 06:50:36.000000 vdk-control-cli-1.3.921164058/src/vdk/internal/control/command_groups/login_group/
+-rw-rw-rw-   0 root         (0) root         (0)     6510 2023-07-05 06:50:20.000000 vdk-control-cli-1.3.921164058/src/vdk/internal/control/command_groups/login_group/login.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 06:50:36.000000 vdk-control-cli-1.3.921164058/src/vdk/internal/control/command_groups/logout_group/
+-rw-rw-rw-   0 root         (0) root         (0)      410 2023-07-05 06:50:20.000000 vdk-control-cli-1.3.921164058/src/vdk/internal/control/command_groups/logout_group/logout.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 06:50:36.000000 vdk-control-cli-1.3.921164058/src/vdk/internal/control/command_groups/version_group/
+-rw-rw-rw-   0 root         (0) root         (0)      772 2023-07-05 06:50:20.000000 vdk-control-cli-1.3.921164058/src/vdk/internal/control/command_groups/version_group/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 06:50:36.000000 vdk-control-cli-1.3.921164058/src/vdk/internal/control/configuration/
+-rw-rw-rw-   0 root         (0) root         (0)      424 2023-07-05 06:50:20.000000 vdk-control-cli-1.3.921164058/src/vdk/internal/control/configuration/default_options.py
+-rw-rw-rw-   0 root         (0) root         (0)     1221 2023-07-05 06:50:20.000000 vdk-control-cli-1.3.921164058/src/vdk/internal/control/configuration/defaults_config.py
+-rw-rw-rw-   0 root         (0) root         (0)     2272 2023-07-05 06:50:20.000000 vdk-control-cli-1.3.921164058/src/vdk/internal/control/configuration/log_config.py
+-rw-rw-rw-   0 root         (0) root         (0)     9551 2023-07-05 06:50:20.000000 vdk-control-cli-1.3.921164058/src/vdk/internal/control/configuration/vdk_config.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 06:50:36.000000 vdk-control-cli-1.3.921164058/src/vdk/internal/control/exception/
+-rw-rw-rw-   0 root         (0) root         (0)      649 2023-07-05 06:50:20.000000 vdk-control-cli-1.3.921164058/src/vdk/internal/control/exception/vdk_exception.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 06:50:36.000000 vdk-control-cli-1.3.921164058/src/vdk/internal/control/job/
+-rw-rw-rw-   0 root         (0) root         (0)     1930 2023-07-05 06:50:20.000000 vdk-control-cli-1.3.921164058/src/vdk/internal/control/job/job_archive.py
+-rw-rw-rw-   0 root         (0) root         (0)     4871 2023-07-05 06:50:20.000000 vdk-control-cli-1.3.921164058/src/vdk/internal/control/job/job_config.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 06:50:36.000000 vdk-control-cli-1.3.921164058/src/vdk/internal/control/job/sample_job/
+-rw-rw-rw-   0 root         (0) root         (0)      579 2023-07-05 06:50:20.000000 vdk-control-cli-1.3.921164058/src/vdk/internal/control/job/sample_job/10_sql_step.sql
+-rw-rw-rw-   0 root         (0) root         (0)      816 2023-07-05 06:50:20.000000 vdk-control-cli-1.3.921164058/src/vdk/internal/control/job/sample_job/20_python_step.py
+-rw-rw-rw-   0 root         (0) root         (0)     1446 2023-07-05 06:50:20.000000 vdk-control-cli-1.3.921164058/src/vdk/internal/control/job/sample_job/README.md
+-rw-rw-rw-   0 root         (0) root         (0)     2902 2023-07-05 06:50:20.000000 vdk-control-cli-1.3.921164058/src/vdk/internal/control/job/sample_job/config.ini
+-rw-rw-rw-   0 root         (0) root         (0)      243 2023-07-05 06:50:20.000000 vdk-control-cli-1.3.921164058/src/vdk/internal/control/job/sample_job/requirements.txt
+-rw-rw-rw-   0 root         (0) root         (0)     3666 2023-07-05 06:50:20.000000 vdk-control-cli-1.3.921164058/src/vdk/internal/control/main.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 06:50:36.000000 vdk-control-cli-1.3.921164058/src/vdk/internal/control/plugin/
+-rw-rw-rw-   0 root         (0) root         (0)     3715 2023-07-05 06:50:20.000000 vdk-control-cli-1.3.921164058/src/vdk/internal/control/plugin/control_plugin_manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 06:50:36.000000 vdk-control-cli-1.3.921164058/src/vdk/internal/control/rest_lib/
+-rw-rw-rw-   0 root         (0) root         (0)     3239 2023-07-05 06:50:20.000000 vdk-control-cli-1.3.921164058/src/vdk/internal/control/rest_lib/factory.py
+-rw-rw-rw-   0 root         (0) root         (0)     3845 2023-07-05 06:50:20.000000 vdk-control-cli-1.3.921164058/src/vdk/internal/control/rest_lib/rest_client_errors.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 06:50:36.000000 vdk-control-cli-1.3.921164058/src/vdk/internal/control/utils/
+-rw-rw-rw-   0 root         (0) root         (0)     7297 2023-07-05 06:50:20.000000 vdk-control-cli-1.3.921164058/src/vdk/internal/control/utils/cli_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     1413 2023-07-05 06:50:20.000000 vdk-control-cli-1.3.921164058/src/vdk/internal/control/utils/control_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     3690 2023-07-05 06:50:20.000000 vdk-control-cli-1.3.921164058/src/vdk/internal/control/utils/output_printer.py
+-rw-rw-rw-   0 root         (0) root         (0)      819 2023-07-05 06:50:20.000000 vdk-control-cli-1.3.921164058/src/vdk/internal/control/utils/version_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)      181 2023-07-05 06:50:24.000000 vdk-control-cli-1.3.921164058/src/vdk/internal/control/vdk_control_build_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 06:50:36.000000 vdk-control-cli-1.3.921164058/src/vdk_control_cli.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5153 2023-07-05 06:50:36.000000 vdk-control-cli-1.3.921164058/src/vdk_control_cli.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2426 2023-07-05 06:50:36.000000 vdk-control-cli-1.3.921164058/src/vdk_control_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-05 06:50:36.000000 vdk-control-cli-1.3.921164058/src/vdk_control_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       57 2023-07-05 06:50:36.000000 vdk-control-cli-1.3.921164058/src/vdk_control_cli.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-05 06:50:36.000000 vdk-control-cli-1.3.921164058/src/vdk_control_cli.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      185 2023-07-05 06:50:36.000000 vdk-control-cli-1.3.921164058/src/vdk_control_cli.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        4 2023-07-05 06:50:36.000000 vdk-control-cli-1.3.921164058/src/vdk_control_cli.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)       14 2023-07-05 06:50:24.000000 vdk-control-cli-1.3.921164058/version.txt
```

### Comparing `vdk-control-cli-1.3.896771774/PKG-INFO` & `vdk-control-cli-1.3.921164058/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vdk-control-cli
-Version: 1.3.896771774
+Version: 1.3.921164058
 Summary: VDK Control CLI allows user to create, delete, manage and their Data Jobs in Kubernetes runtime.
 Home-page: https://github.com/vmware/versatile-data-kit
 Author: VMware Inc.
 Author-email: aivanov@vmware.com
 Project-URL: Documentation, https://github.com/vmware/versatile-data-kit/wiki
 Project-URL: Source, https://github.com/vmware/versatile-data-kit/projects/vdk-control-cli
 Platform: any
```

### Comparing `vdk-control-cli-1.3.896771774/README.md` & `vdk-control-cli-1.3.921164058/README.md`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.896771774/setup.cfg` & `vdk-control-cli-1.3.921164058/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 install_requires = 
 	click==8.*
 	click-log==0.*
 	click-spinner==0.*
 	requests>=2.25
 	setuptools>=47.0
 	pluggy
-	vdk-control-service-api==1.0.10
+	vdk-control-service-api==1.0.11
 	tabulate
 	requests_oauthlib>=1.0
 	urllib3>=1.26.5
 	vdk-control-api-auth
 python_requires = >=3.7, <4
 
 [options.packages.find]
```

### Comparing `vdk-control-cli-1.3.896771774/src/vdk/api/control/plugin/markers.py` & `vdk-control-cli-1.3.921164058/src/vdk/api/control/plugin/markers.py`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.896771774/src/vdk/api/control/plugin/specs.py` & `vdk-control-cli-1.3.921164058/src/vdk/api/control/plugin/specs.py`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.896771774/src/vdk/internal/control/command_groups/common_group/default.py` & `vdk-control-cli-1.3.921164058/src/vdk/internal/control/command_groups/common_group/default.py`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.896771774/src/vdk/internal/control/command_groups/info_group/info.py` & `vdk-control-cli-1.3.921164058/src/vdk/internal/control/command_groups/info_group/info.py`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.896771774/src/vdk/internal/control/command_groups/job/create.py` & `vdk-control-cli-1.3.921164058/src/vdk/internal/control/command_groups/job/create.py`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.896771774/src/vdk/internal/control/command_groups/job/delete.py` & `vdk-control-cli-1.3.921164058/src/vdk/internal/control/command_groups/job/delete.py`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.896771774/src/vdk/internal/control/command_groups/job/deploy_cli.py` & `vdk-control-cli-1.3.921164058/src/vdk/internal/control/command_groups/job/deploy_cli.py`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.896771774/src/vdk/internal/control/command_groups/job/deploy_cli_impl.py` & `vdk-control-cli-1.3.921164058/src/vdk/internal/control/command_groups/job/deploy_cli_impl.py`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.896771774/src/vdk/internal/control/command_groups/job/download_job.py` & `vdk-control-cli-1.3.921164058/src/vdk/internal/control/command_groups/job/download_job.py`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.896771774/src/vdk/internal/control/command_groups/job/download_key.py` & `vdk-control-cli-1.3.921164058/src/vdk/internal/control/command_groups/job/download_key.py`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.896771774/src/vdk/internal/control/command_groups/job/execute.py` & `vdk-control-cli-1.3.921164058/src/vdk/internal/control/command_groups/job/execute.py`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.896771774/src/vdk/internal/control/command_groups/job/list.py` & `vdk-control-cli-1.3.921164058/src/vdk/internal/control/command_groups/job/list.py`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.896771774/src/vdk/internal/control/command_groups/job/properties.py` & `vdk-control-cli-1.3.921164058/src/vdk/internal/control/command_groups/job/properties.py`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.896771774/src/vdk/internal/control/command_groups/job/show.py` & `vdk-control-cli-1.3.921164058/src/vdk/internal/control/command_groups/job/show.py`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.896771774/src/vdk/internal/control/command_groups/login_group/login.py` & `vdk-control-cli-1.3.921164058/src/vdk/internal/control/command_groups/login_group/login.py`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.896771774/src/vdk/internal/control/command_groups/version_group/version.py` & `vdk-control-cli-1.3.921164058/src/vdk/internal/control/command_groups/version_group/version.py`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.896771774/src/vdk/internal/control/configuration/defaults_config.py` & `vdk-control-cli-1.3.921164058/src/vdk/internal/control/configuration/defaults_config.py`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.896771774/src/vdk/internal/control/configuration/log_config.py` & `vdk-control-cli-1.3.921164058/src/vdk/internal/control/configuration/log_config.py`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.896771774/src/vdk/internal/control/configuration/vdk_config.py` & `vdk-control-cli-1.3.921164058/src/vdk/internal/control/configuration/vdk_config.py`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.896771774/src/vdk/internal/control/exception/vdk_exception.py` & `vdk-control-cli-1.3.921164058/src/vdk/internal/control/exception/vdk_exception.py`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.896771774/src/vdk/internal/control/job/job_archive.py` & `vdk-control-cli-1.3.921164058/src/vdk/internal/control/job/job_archive.py`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.896771774/src/vdk/internal/control/job/job_config.py` & `vdk-control-cli-1.3.921164058/src/vdk/internal/control/job/job_config.py`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.896771774/src/vdk/internal/control/job/sample_job/10_sql_step.sql` & `vdk-control-cli-1.3.921164058/src/vdk/internal/control/job/sample_job/10_sql_step.sql`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.896771774/src/vdk/internal/control/job/sample_job/20_python_step.py` & `vdk-control-cli-1.3.921164058/src/vdk/internal/control/job/sample_job/20_python_step.py`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.896771774/src/vdk/internal/control/job/sample_job/README.md` & `vdk-control-cli-1.3.921164058/src/vdk/internal/control/job/sample_job/README.md`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.896771774/src/vdk/internal/control/job/sample_job/config.ini` & `vdk-control-cli-1.3.921164058/src/vdk/internal/control/job/sample_job/config.ini`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.896771774/src/vdk/internal/control/main.py` & `vdk-control-cli-1.3.921164058/src/vdk/internal/control/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 from vdk.internal.control.command_groups.job.delete import delete
 from vdk.internal.control.command_groups.job.deploy_cli import deploy
 from vdk.internal.control.command_groups.job.download_job import download_job
 from vdk.internal.control.command_groups.job.download_key import download_key
 from vdk.internal.control.command_groups.job.execute import execute
 from vdk.internal.control.command_groups.job.list import list_command
 from vdk.internal.control.command_groups.job.properties import properties_command
+from vdk.internal.control.command_groups.job.secrets import secrets_command
 from vdk.internal.control.command_groups.job.show import show_command
 from vdk.internal.control.command_groups.login_group.login import login
 from vdk.internal.control.command_groups.logout_group.logout import logout
 from vdk.internal.control.command_groups.version_group.version import version
 from vdk.internal.control.configuration.default_options import DefaultOptions
 from vdk.internal.control.configuration.log_config import configure_loggers
 from vdk.internal.control.configuration.vdk_config import VDKConfig
@@ -88,14 +89,15 @@
     cli.add_command(version)
     cli.add_command(execute)
     cli.add_command(set_default_command)
     cli.add_command(reset_default_command)
     cli.add_command(download_job)
     cli.add_command(show_command)
     cli.add_command(properties_command)
+    cli.add_command(secrets_command)
     cli.add_command(info)
 
     cli()
 
 
 if __name__ == "__main__":
     run()
```

### Comparing `vdk-control-cli-1.3.896771774/src/vdk/internal/control/plugin/control_plugin_manager.py` & `vdk-control-cli-1.3.921164058/src/vdk/internal/control/plugin/control_plugin_manager.py`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.896771774/src/vdk/internal/control/rest_lib/factory.py` & `vdk-control-cli-1.3.921164058/src/vdk/internal/control/rest_lib/factory.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 
 from taurus_datajob_api import ApiClient
 from taurus_datajob_api import Configuration
 from taurus_datajob_api import DataJobsApi
 from taurus_datajob_api import DataJobsDeploymentApi
 from taurus_datajob_api import DataJobsExecutionApi
 from taurus_datajob_api import DataJobsPropertiesApi
+from taurus_datajob_api import DataJobsSecretsApi
 from taurus_datajob_api import DataJobsServiceApi
 from taurus_datajob_api import DataJobsSourcesApi
 from urllib3 import Retry
 from vdk.internal.control.configuration.vdk_config import VDKConfig
 from vdk.plugin.control_api_auth.authentication import Authentication
 
 log = logging.getLogger(__name__)
@@ -64,9 +65,12 @@
 
     def get_execution_api(self) -> DataJobsExecutionApi:
         return DataJobsExecutionApi(self._new_api_client())
 
     def get_properties_api(self) -> DataJobsPropertiesApi:
         return DataJobsPropertiesApi(self._new_api_client())
 
+    def get_secrets_api(self) -> DataJobsSecretsApi:
+        return DataJobsSecretsApi(self._new_api_client())
+
     def get_service_api(self) -> DataJobsServiceApi:
         return DataJobsServiceApi(self._new_api_client())
```

### Comparing `vdk-control-cli-1.3.896771774/src/vdk/internal/control/rest_lib/rest_client_errors.py` & `vdk-control-cli-1.3.921164058/src/vdk/internal/control/rest_lib/rest_client_errors.py`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.896771774/src/vdk/internal/control/utils/cli_utils.py` & `vdk-control-cli-1.3.921164058/src/vdk/internal/control/utils/cli_utils.py`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.896771774/src/vdk/internal/control/utils/control_utils.py` & `vdk-control-cli-1.3.921164058/src/vdk/internal/control/utils/control_utils.py`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.896771774/src/vdk/internal/control/utils/output_printer.py` & `vdk-control-cli-1.3.921164058/src/vdk/internal/control/utils/output_printer.py`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.896771774/src/vdk/internal/control/utils/version_utils.py` & `vdk-control-cli-1.3.921164058/src/vdk/internal/control/utils/version_utils.py`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.896771774/src/vdk_control_cli.egg-info/PKG-INFO` & `vdk-control-cli-1.3.921164058/src/vdk_control_cli.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vdk-control-cli
-Version: 1.3.896771774
+Version: 1.3.921164058
 Summary: VDK Control CLI allows user to create, delete, manage and their Data Jobs in Kubernetes runtime.
 Home-page: https://github.com/vmware/versatile-data-kit
 Author: VMware Inc.
 Author-email: aivanov@vmware.com
 Project-URL: Documentation, https://github.com/vmware/versatile-data-kit/wiki
 Project-URL: Source, https://github.com/vmware/versatile-data-kit/projects/vdk-control-cli
 Platform: any
```

### Comparing `vdk-control-cli-1.3.896771774/src/vdk_control_cli.egg-info/SOURCES.txt` & `vdk-control-cli-1.3.921164058/src/vdk_control_cli.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 src/vdk/internal/control/command_groups/job/deploy_cli.py
 src/vdk/internal/control/command_groups/job/deploy_cli_impl.py
 src/vdk/internal/control/command_groups/job/download_job.py
 src/vdk/internal/control/command_groups/job/download_key.py
 src/vdk/internal/control/command_groups/job/execute.py
 src/vdk/internal/control/command_groups/job/list.py
 src/vdk/internal/control/command_groups/job/properties.py
+src/vdk/internal/control/command_groups/job/secrets.py
 src/vdk/internal/control/command_groups/job/show.py
 src/vdk/internal/control/command_groups/login_group/login.py
 src/vdk/internal/control/command_groups/logout_group/logout.py
 src/vdk/internal/control/command_groups/version_group/version.py
 src/vdk/internal/control/configuration/default_options.py
 src/vdk/internal/control/configuration/defaults_config.py
 src/vdk/internal/control/configuration/log_config.py
```

