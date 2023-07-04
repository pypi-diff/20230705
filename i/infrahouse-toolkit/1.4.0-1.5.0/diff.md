# Comparing `tmp/infrahouse-toolkit-1.4.0.tar.gz` & `tmp/infrahouse-toolkit-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "infrahouse-toolkit-1.4.0.tar", last modified: Tue Jul  4 22:19:18 2023, max compression
+gzip compressed data, was "infrahouse-toolkit-1.5.0.tar", last modified: Tue Jul  4 22:51:05 2023, max compression
```

## Comparing `infrahouse-toolkit-1.4.0.tar` & `infrahouse-toolkit-1.5.0.tar`

### file list

```diff
@@ -1,102 +1,102 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 22:19:18.059818 infrahouse-toolkit-1.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-07-04 22:18:45.000000 infrahouse-toolkit-1.4.0/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2965 2023-07-04 22:18:45.000000 infrahouse-toolkit-1.4.0/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-07-04 22:18:45.000000 infrahouse-toolkit-1.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-07-04 22:18:45.000000 infrahouse-toolkit-1.4.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-07-04 22:19:18.059818 infrahouse-toolkit-1.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-07-04 22:18:45.000000 infrahouse-toolkit-1.4.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 22:19:18.051818 infrahouse-toolkit-1.4.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      619 2023-07-04 22:18:45.000000 infrahouse-toolkit-1.4.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-04 22:18:45.000000 infrahouse-toolkit-1.4.0/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4940 2023-07-04 22:18:45.000000 infrahouse-toolkit-1.4.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-04 22:18:45.000000 infrahouse-toolkit-1.4.0/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      312 2023-07-04 22:18:45.000000 infrahouse-toolkit-1.4.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-07-04 22:18:45.000000 infrahouse-toolkit-1.4.0/docs/infrahouse_toolkit.cli.ih_plan.cmd_download.rst
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-07-04 22:18:45.000000 infrahouse-toolkit-1.4.0/docs/infrahouse_toolkit.cli.ih_plan.cmd_publish.rst
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-07-04 22:18:45.000000 infrahouse-toolkit-1.4.0/docs/infrahouse_toolkit.cli.ih_plan.cmd_remove.rst
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-07-04 22:18:45.000000 infrahouse-toolkit-1.4.0/docs/infrahouse_toolkit.cli.ih_plan.cmd_upload.rst
--rw-r--r--   0 runner    (1001) docker     (123)      456 2023-07-04 22:18:45.000000 infrahouse-toolkit-1.4.0/docs/infrahouse_toolkit.cli.ih_plan.rst
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-07-04 22:18:45.000000 infrahouse-toolkit-1.4.0/docs/infrahouse_toolkit.cli.rst
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-07-04 22:18:45.000000 infrahouse-toolkit-1.4.0/docs/infrahouse_toolkit.cli.tests.rst
--rw-r--r--   0 runner    (1001) docker     (123)      293 2023-07-04 22:18:45.000000 infrahouse-toolkit-1.4.0/docs/infrahouse_toolkit.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-07-04 22:18:45.000000 infrahouse-toolkit-1.4.0/docs/infrahouse_toolkit.terraform.backends.rst
--rw-r--r--   0 runner    (1001) docker     (123)      665 2023-07-04 22:18:45.000000 infrahouse-toolkit-1.4.0/docs/infrahouse_toolkit.terraform.backends.tests.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-07-04 22:18:45.000000 infrahouse-toolkit-1.4.0/docs/infrahouse_toolkit.terraform.backends.tests.s3backend.rst
--rw-r--r--   0 runner    (1001) docker     (123)      771 2023-07-04 22:18:45.000000 infrahouse-toolkit-1.4.0/docs/infrahouse_toolkit.terraform.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-07-04 22:18:45.000000 infrahouse-toolkit-1.4.0/docs/infrahouse_toolkit.terraform.tests.github_pr.rst
--rw-r--r--   0 runner    (1001) docker     (123)      898 2023-07-04 22:18:45.000000 infrahouse-toolkit-1.4.0/docs/infrahouse_toolkit.terraform.tests.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1589 2023-07-04 22:18:45.000000 infrahouse-toolkit-1.4.0/docs/infrahouse_toolkit.terraform.tests.status.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-07-04 22:18:45.000000 infrahouse-toolkit-1.4.0/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-04 22:18:45.000000 infrahouse-toolkit-1.4.0/docs/modules.rst
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-04 22:18:45.000000 infrahouse-toolkit-1.4.0/docs/readme.rst
--rw-r--r--   0 runner    (1001) docker     (123)      982 2023-07-04 22:18:45.000000 infrahouse-toolkit-1.4.0/docs/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 22:19:18.051818 infrahouse-toolkit-1.4.0/infrahouse_toolkit/
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-07-04 22:18:45.000000 infrahouse-toolkit-1.4.0/infrahouse_toolkit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 22:19:18.055818 infrahouse-toolkit-1.4.0/infrahouse_toolkit/cli/
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-07-04 22:18:45.000000 infrahouse-toolkit-1.4.0/infrahouse_toolkit/cli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 22:19:18.055818 infrahouse-toolkit-1.4.0/infrahouse_toolkit/cli/ih_plan/
--rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-07-04 22:18:45.000000 infrahouse-toolkit-1.4.0/infrahouse_toolkit/cli/ih_plan/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 22:19:18.055818 infrahouse-toolkit-1.4.0/infrahouse_toolkit/cli/ih_plan/cmd_download/
--rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-07-04 22:18:45.000000 infrahouse-toolkit-1.4.0/infrahouse_toolkit/cli/ih_plan/cmd_download/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 22:19:18.055818 infrahouse-toolkit-1.4.0/infrahouse_toolkit/cli/ih_plan/cmd_min_permissions/
--rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-07-04 22:18:45.000000 infrahouse-toolkit-1.4.0/infrahouse_toolkit/cli/ih_plan/cmd_min_permissions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 22:19:18.055818 infrahouse-toolkit-1.4.0/infrahouse_toolkit/cli/ih_plan/cmd_publish/
--rw-r--r--   0 runner    (1001) docker     (123)     2390 2023-07-04 22:18:45.000000 infrahouse-toolkit-1.4.0/infrahouse_toolkit/cli/ih_plan/cmd_publish/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 22:19:18.055818 infrahouse-toolkit-1.4.0/infrahouse_toolkit/cli/ih_plan/cmd_remove/
--rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-07-04 22:18:45.000000 infrahouse-toolkit-1.4.0/infrahouse_toolkit/cli/ih_plan/cmd_remove/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 22:19:18.055818 infrahouse-toolkit-1.4.0/infrahouse_toolkit/cli/ih_plan/cmd_upload/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-04 22:18:45.000000 infrahouse-toolkit-1.4.0/infrahouse_toolkit/cli/ih_plan/cmd_upload/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-07-04 22:18:45.000000 infrahouse-toolkit-1.4.0/infrahouse_toolkit/cli/lib.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 22:19:18.055818 infrahouse-toolkit-1.4.0/infrahouse_toolkit/cli/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 22:18:45.000000 infrahouse-toolkit-1.4.0/infrahouse_toolkit/cli/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      700 2023-07-04 22:18:45.000000 infrahouse-toolkit-1.4.0/infrahouse_toolkit/cli/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-07-04 22:18:45.000000 infrahouse-toolkit-1.4.0/infrahouse_toolkit/cli/tests/test_get_bucket.py
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-07-04 22:18:45.000000 infrahouse-toolkit-1.4.0/infrahouse_toolkit/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-07-04 22:18:45.000000 infrahouse-toolkit-1.4.0/infrahouse_toolkit/logging.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 22:19:18.055818 infrahouse-toolkit-1.4.0/infrahouse_toolkit/terraform/
--rw-r--r--   0 runner    (1001) docker     (123)     8365 2023-07-04 22:18:45.000000 infrahouse-toolkit-1.4.0/infrahouse_toolkit/terraform/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 22:19:18.055818 infrahouse-toolkit-1.4.0/infrahouse_toolkit/terraform/backends/
--rw-r--r--   0 runner    (1001) docker     (123)      907 2023-07-04 22:18:45.000000 infrahouse-toolkit-1.4.0/infrahouse_toolkit/terraform/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-07-04 22:18:45.000000 infrahouse-toolkit-1.4.0/infrahouse_toolkit/terraform/backends/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1453 2023-07-04 22:18:45.000000 infrahouse-toolkit-1.4.0/infrahouse_toolkit/terraform/backends/s3backend.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 22:19:18.055818 infrahouse-toolkit-1.4.0/infrahouse_toolkit/terraform/backends/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 22:18:45.000000 infrahouse-toolkit-1.4.0/infrahouse_toolkit/terraform/backends/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 22:19:18.055818 infrahouse-toolkit-1.4.0/infrahouse_toolkit/terraform/backends/tests/s3backend/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 22:18:45.000000 infrahouse-toolkit-1.4.0/infrahouse_toolkit/terraform/backends/tests/s3backend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-07-04 22:18:45.000000 infrahouse-toolkit-1.4.0/infrahouse_toolkit/terraform/backends/tests/s3backend/test_eq.py
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-04 22:18:45.000000 infrahouse-toolkit-1.4.0/infrahouse_toolkit/terraform/backends/tests/s3backend/test_init.py
--rw-r--r--   0 runner    (1001) docker     (123)      695 2023-07-04 22:18:45.000000 infrahouse-toolkit-1.4.0/infrahouse_toolkit/terraform/backends/tests/s3backend/test_region.py
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-07-04 22:18:45.000000 infrahouse-toolkit-1.4.0/infrahouse_toolkit/terraform/backends/tests/test_get_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-07-04 22:18:45.000000 infrahouse-toolkit-1.4.0/infrahouse_toolkit/terraform/backends/tfbackend.py
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-07-04 22:18:45.000000 infrahouse-toolkit-1.4.0/infrahouse_toolkit/terraform/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3145 2023-07-04 22:18:45.000000 infrahouse-toolkit-1.4.0/infrahouse_toolkit/terraform/githubpr.py
--rw-r--r--   0 runner    (1001) docker     (123)     5155 2023-07-04 22:18:45.000000 infrahouse-toolkit-1.4.0/infrahouse_toolkit/terraform/status.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 22:19:18.055818 infrahouse-toolkit-1.4.0/infrahouse_toolkit/terraform/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 22:18:45.000000 infrahouse-toolkit-1.4.0/infrahouse_toolkit/terraform/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 22:19:18.055818 infrahouse-toolkit-1.4.0/infrahouse_toolkit/terraform/tests/github_pr/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 22:18:45.000000 infrahouse-toolkit-1.4.0/infrahouse_toolkit/terraform/tests/github_pr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      950 2023-07-04 22:18:45.000000 infrahouse-toolkit-1.4.0/infrahouse_toolkit/terraform/tests/github_pr/test_find_comment_by_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-07-04 22:18:45.000000 infrahouse-toolkit-1.4.0/infrahouse_toolkit/terraform/tests/github_pr/test_init.py
--rw-r--r--   0 runner    (1001) docker     (123)      933 2023-07-04 22:18:45.000000 infrahouse-toolkit-1.4.0/infrahouse_toolkit/terraform/tests/github_pr/test_publish_comment.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 22:19:18.059818 infrahouse-toolkit-1.4.0/infrahouse_toolkit/terraform/tests/status/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 22:18:45.000000 infrahouse-toolkit-1.4.0/infrahouse_toolkit/terraform/tests/status/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-07-04 22:18:45.000000 infrahouse-toolkit-1.4.0/infrahouse_toolkit/terraform/tests/status/test_comment.py
--rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-07-04 22:18:45.000000 infrahouse-toolkit-1.4.0/infrahouse_toolkit/terraform/tests/status/test_eq.py
--rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-07-04 22:18:45.000000 infrahouse-toolkit-1.4.0/infrahouse_toolkit/terraform/tests/status/test_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)      531 2023-07-04 22:18:45.000000 infrahouse-toolkit-1.4.0/infrahouse_toolkit/terraform/tests/status/test_summary_counts.py
--rw-r--r--   0 runner    (1001) docker     (123)      650 2023-07-04 22:18:45.000000 infrahouse-toolkit-1.4.0/infrahouse_toolkit/terraform/tests/status/test_summary_resources.py
--rw-r--r--   0 runner    (1001) docker     (123)     2601 2023-07-04 22:18:45.000000 infrahouse-toolkit-1.4.0/infrahouse_toolkit/terraform/tests/test_parse_comment.py
--rw-r--r--   0 runner    (1001) docker     (123)     2369 2023-07-04 22:18:45.000000 infrahouse-toolkit-1.4.0/infrahouse_toolkit/terraform/tests/test_parse_plan.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 22:19:18.055818 infrahouse-toolkit-1.4.0/infrahouse_toolkit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-07-04 22:19:18.000000 infrahouse-toolkit-1.4.0/infrahouse_toolkit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3417 2023-07-04 22:19:18.000000 infrahouse-toolkit-1.4.0/infrahouse_toolkit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 22:19:18.000000 infrahouse-toolkit-1.4.0/infrahouse_toolkit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-04 22:19:18.000000 infrahouse-toolkit-1.4.0/infrahouse_toolkit.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 22:19:13.000000 infrahouse-toolkit-1.4.0/infrahouse_toolkit.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-04 22:19:18.000000 infrahouse-toolkit-1.4.0/infrahouse_toolkit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-04 22:19:18.000000 infrahouse-toolkit-1.4.0/infrahouse_toolkit.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-04 22:18:45.000000 infrahouse-toolkit-1.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-07-04 22:18:45.000000 infrahouse-toolkit-1.4.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-07-04 22:18:45.000000 infrahouse-toolkit-1.4.0/requirements_dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)      466 2023-07-04 22:19:18.059818 infrahouse-toolkit-1.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-07-04 22:18:45.000000 infrahouse-toolkit-1.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 22:51:05.374645 infrahouse-toolkit-1.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-07-04 22:50:33.000000 infrahouse-toolkit-1.5.0/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2965 2023-07-04 22:50:33.000000 infrahouse-toolkit-1.5.0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-07-04 22:50:33.000000 infrahouse-toolkit-1.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-07-04 22:50:33.000000 infrahouse-toolkit-1.5.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-07-04 22:51:05.374645 infrahouse-toolkit-1.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-07-04 22:50:33.000000 infrahouse-toolkit-1.5.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 22:51:05.366644 infrahouse-toolkit-1.5.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      619 2023-07-04 22:50:33.000000 infrahouse-toolkit-1.5.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-04 22:50:33.000000 infrahouse-toolkit-1.5.0/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4940 2023-07-04 22:50:33.000000 infrahouse-toolkit-1.5.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-04 22:50:33.000000 infrahouse-toolkit-1.5.0/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      312 2023-07-04 22:50:33.000000 infrahouse-toolkit-1.5.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-07-04 22:50:33.000000 infrahouse-toolkit-1.5.0/docs/infrahouse_toolkit.cli.ih_plan.cmd_download.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-07-04 22:50:33.000000 infrahouse-toolkit-1.5.0/docs/infrahouse_toolkit.cli.ih_plan.cmd_publish.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-07-04 22:50:33.000000 infrahouse-toolkit-1.5.0/docs/infrahouse_toolkit.cli.ih_plan.cmd_remove.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-07-04 22:50:33.000000 infrahouse-toolkit-1.5.0/docs/infrahouse_toolkit.cli.ih_plan.cmd_upload.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      456 2023-07-04 22:50:33.000000 infrahouse-toolkit-1.5.0/docs/infrahouse_toolkit.cli.ih_plan.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-07-04 22:50:33.000000 infrahouse-toolkit-1.5.0/docs/infrahouse_toolkit.cli.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-07-04 22:50:33.000000 infrahouse-toolkit-1.5.0/docs/infrahouse_toolkit.cli.tests.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-07-04 22:50:33.000000 infrahouse-toolkit-1.5.0/docs/infrahouse_toolkit.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-07-04 22:50:33.000000 infrahouse-toolkit-1.5.0/docs/infrahouse_toolkit.terraform.backends.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-07-04 22:50:33.000000 infrahouse-toolkit-1.5.0/docs/infrahouse_toolkit.terraform.backends.tests.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-07-04 22:50:33.000000 infrahouse-toolkit-1.5.0/docs/infrahouse_toolkit.terraform.backends.tests.s3backend.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-07-04 22:50:33.000000 infrahouse-toolkit-1.5.0/docs/infrahouse_toolkit.terraform.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-07-04 22:50:33.000000 infrahouse-toolkit-1.5.0/docs/infrahouse_toolkit.terraform.tests.github_pr.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      898 2023-07-04 22:50:33.000000 infrahouse-toolkit-1.5.0/docs/infrahouse_toolkit.terraform.tests.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1589 2023-07-04 22:50:33.000000 infrahouse-toolkit-1.5.0/docs/infrahouse_toolkit.terraform.tests.status.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-07-04 22:50:33.000000 infrahouse-toolkit-1.5.0/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-04 22:50:33.000000 infrahouse-toolkit-1.5.0/docs/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-04 22:50:33.000000 infrahouse-toolkit-1.5.0/docs/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      982 2023-07-04 22:50:33.000000 infrahouse-toolkit-1.5.0/docs/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 22:51:05.366644 infrahouse-toolkit-1.5.0/infrahouse_toolkit/
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-07-04 22:50:33.000000 infrahouse-toolkit-1.5.0/infrahouse_toolkit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 22:51:05.370645 infrahouse-toolkit-1.5.0/infrahouse_toolkit/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-07-04 22:50:33.000000 infrahouse-toolkit-1.5.0/infrahouse_toolkit/cli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 22:51:05.370645 infrahouse-toolkit-1.5.0/infrahouse_toolkit/cli/ih_plan/
+-rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-07-04 22:50:33.000000 infrahouse-toolkit-1.5.0/infrahouse_toolkit/cli/ih_plan/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 22:51:05.370645 infrahouse-toolkit-1.5.0/infrahouse_toolkit/cli/ih_plan/cmd_download/
+-rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-07-04 22:50:33.000000 infrahouse-toolkit-1.5.0/infrahouse_toolkit/cli/ih_plan/cmd_download/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 22:51:05.370645 infrahouse-toolkit-1.5.0/infrahouse_toolkit/cli/ih_plan/cmd_min_permissions/
+-rw-r--r--   0 runner    (1001) docker     (123)     2092 2023-07-04 22:50:33.000000 infrahouse-toolkit-1.5.0/infrahouse_toolkit/cli/ih_plan/cmd_min_permissions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 22:51:05.370645 infrahouse-toolkit-1.5.0/infrahouse_toolkit/cli/ih_plan/cmd_publish/
+-rw-r--r--   0 runner    (1001) docker     (123)     2390 2023-07-04 22:50:33.000000 infrahouse-toolkit-1.5.0/infrahouse_toolkit/cli/ih_plan/cmd_publish/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 22:51:05.370645 infrahouse-toolkit-1.5.0/infrahouse_toolkit/cli/ih_plan/cmd_remove/
+-rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-07-04 22:50:33.000000 infrahouse-toolkit-1.5.0/infrahouse_toolkit/cli/ih_plan/cmd_remove/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 22:51:05.370645 infrahouse-toolkit-1.5.0/infrahouse_toolkit/cli/ih_plan/cmd_upload/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-04 22:50:33.000000 infrahouse-toolkit-1.5.0/infrahouse_toolkit/cli/ih_plan/cmd_upload/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-07-04 22:50:33.000000 infrahouse-toolkit-1.5.0/infrahouse_toolkit/cli/lib.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 22:51:05.370645 infrahouse-toolkit-1.5.0/infrahouse_toolkit/cli/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 22:50:33.000000 infrahouse-toolkit-1.5.0/infrahouse_toolkit/cli/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-07-04 22:50:33.000000 infrahouse-toolkit-1.5.0/infrahouse_toolkit/cli/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-07-04 22:50:33.000000 infrahouse-toolkit-1.5.0/infrahouse_toolkit/cli/tests/test_get_bucket.py
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-07-04 22:50:33.000000 infrahouse-toolkit-1.5.0/infrahouse_toolkit/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-07-04 22:50:33.000000 infrahouse-toolkit-1.5.0/infrahouse_toolkit/logging.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 22:51:05.370645 infrahouse-toolkit-1.5.0/infrahouse_toolkit/terraform/
+-rw-r--r--   0 runner    (1001) docker     (123)     8365 2023-07-04 22:50:33.000000 infrahouse-toolkit-1.5.0/infrahouse_toolkit/terraform/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 22:51:05.370645 infrahouse-toolkit-1.5.0/infrahouse_toolkit/terraform/backends/
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-07-04 22:50:33.000000 infrahouse-toolkit-1.5.0/infrahouse_toolkit/terraform/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-07-04 22:50:33.000000 infrahouse-toolkit-1.5.0/infrahouse_toolkit/terraform/backends/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1453 2023-07-04 22:50:33.000000 infrahouse-toolkit-1.5.0/infrahouse_toolkit/terraform/backends/s3backend.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 22:51:05.370645 infrahouse-toolkit-1.5.0/infrahouse_toolkit/terraform/backends/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 22:50:33.000000 infrahouse-toolkit-1.5.0/infrahouse_toolkit/terraform/backends/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 22:51:05.370645 infrahouse-toolkit-1.5.0/infrahouse_toolkit/terraform/backends/tests/s3backend/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 22:50:33.000000 infrahouse-toolkit-1.5.0/infrahouse_toolkit/terraform/backends/tests/s3backend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-07-04 22:50:33.000000 infrahouse-toolkit-1.5.0/infrahouse_toolkit/terraform/backends/tests/s3backend/test_eq.py
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-04 22:50:33.000000 infrahouse-toolkit-1.5.0/infrahouse_toolkit/terraform/backends/tests/s3backend/test_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)      695 2023-07-04 22:50:33.000000 infrahouse-toolkit-1.5.0/infrahouse_toolkit/terraform/backends/tests/s3backend/test_region.py
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-07-04 22:50:33.000000 infrahouse-toolkit-1.5.0/infrahouse_toolkit/terraform/backends/tests/test_get_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-07-04 22:50:33.000000 infrahouse-toolkit-1.5.0/infrahouse_toolkit/terraform/backends/tfbackend.py
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-07-04 22:50:33.000000 infrahouse-toolkit-1.5.0/infrahouse_toolkit/terraform/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3145 2023-07-04 22:50:33.000000 infrahouse-toolkit-1.5.0/infrahouse_toolkit/terraform/githubpr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5155 2023-07-04 22:50:33.000000 infrahouse-toolkit-1.5.0/infrahouse_toolkit/terraform/status.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 22:51:05.370645 infrahouse-toolkit-1.5.0/infrahouse_toolkit/terraform/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 22:50:33.000000 infrahouse-toolkit-1.5.0/infrahouse_toolkit/terraform/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 22:51:05.370645 infrahouse-toolkit-1.5.0/infrahouse_toolkit/terraform/tests/github_pr/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 22:50:33.000000 infrahouse-toolkit-1.5.0/infrahouse_toolkit/terraform/tests/github_pr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      950 2023-07-04 22:50:33.000000 infrahouse-toolkit-1.5.0/infrahouse_toolkit/terraform/tests/github_pr/test_find_comment_by_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-07-04 22:50:33.000000 infrahouse-toolkit-1.5.0/infrahouse_toolkit/terraform/tests/github_pr/test_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)      933 2023-07-04 22:50:33.000000 infrahouse-toolkit-1.5.0/infrahouse_toolkit/terraform/tests/github_pr/test_publish_comment.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 22:51:05.374645 infrahouse-toolkit-1.5.0/infrahouse_toolkit/terraform/tests/status/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 22:50:33.000000 infrahouse-toolkit-1.5.0/infrahouse_toolkit/terraform/tests/status/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-07-04 22:50:33.000000 infrahouse-toolkit-1.5.0/infrahouse_toolkit/terraform/tests/status/test_comment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-07-04 22:50:33.000000 infrahouse-toolkit-1.5.0/infrahouse_toolkit/terraform/tests/status/test_eq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-07-04 22:50:33.000000 infrahouse-toolkit-1.5.0/infrahouse_toolkit/terraform/tests/status/test_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-07-04 22:50:33.000000 infrahouse-toolkit-1.5.0/infrahouse_toolkit/terraform/tests/status/test_summary_counts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-07-04 22:50:33.000000 infrahouse-toolkit-1.5.0/infrahouse_toolkit/terraform/tests/status/test_summary_resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2601 2023-07-04 22:50:33.000000 infrahouse-toolkit-1.5.0/infrahouse_toolkit/terraform/tests/test_parse_comment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2369 2023-07-04 22:50:33.000000 infrahouse-toolkit-1.5.0/infrahouse_toolkit/terraform/tests/test_parse_plan.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 22:51:05.370645 infrahouse-toolkit-1.5.0/infrahouse_toolkit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-07-04 22:51:05.000000 infrahouse-toolkit-1.5.0/infrahouse_toolkit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3417 2023-07-04 22:51:05.000000 infrahouse-toolkit-1.5.0/infrahouse_toolkit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 22:51:05.000000 infrahouse-toolkit-1.5.0/infrahouse_toolkit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-04 22:51:05.000000 infrahouse-toolkit-1.5.0/infrahouse_toolkit.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 22:51:00.000000 infrahouse-toolkit-1.5.0/infrahouse_toolkit.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-04 22:51:05.000000 infrahouse-toolkit-1.5.0/infrahouse_toolkit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-04 22:51:05.000000 infrahouse-toolkit-1.5.0/infrahouse_toolkit.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-04 22:50:33.000000 infrahouse-toolkit-1.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-07-04 22:50:33.000000 infrahouse-toolkit-1.5.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-07-04 22:50:33.000000 infrahouse-toolkit-1.5.0/requirements_dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2023-07-04 22:51:05.374645 infrahouse-toolkit-1.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-07-04 22:50:33.000000 infrahouse-toolkit-1.5.0/setup.py
```

### Comparing `infrahouse-toolkit-1.4.0/CONTRIBUTING.rst` & `infrahouse-toolkit-1.5.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-1.4.0/LICENSE` & `infrahouse-toolkit-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-1.4.0/PKG-INFO` & `infrahouse-toolkit-1.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: infrahouse-toolkit
-Version: 1.4.0
+Version: 1.5.0
 Summary: A collection of tools for building infrastructure.
 Home-page: https://github.com/infrahouse/infrahouse-toolkit
 Author: Oleksandr Kuzminskyi
 Author-email: aleks@infrahouse.com
 License: Apache Software License 2.0
 Keywords: infrahouse-toolkit
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `infrahouse-toolkit-1.4.0/README.rst` & `infrahouse-toolkit-1.5.0/README.rst`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-1.4.0/docs/Makefile` & `infrahouse-toolkit-1.5.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-1.4.0/docs/conf.py` & `infrahouse-toolkit-1.5.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-1.4.0/docs/infrahouse_toolkit.cli.tests.rst` & `infrahouse-toolkit-1.5.0/docs/infrahouse_toolkit.cli.tests.rst`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-1.4.0/docs/infrahouse_toolkit.terraform.backends.rst` & `infrahouse-toolkit-1.5.0/docs/infrahouse_toolkit.terraform.backends.rst`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-1.4.0/docs/infrahouse_toolkit.terraform.backends.tests.rst` & `infrahouse-toolkit-1.5.0/docs/infrahouse_toolkit.terraform.backends.tests.rst`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-1.4.0/docs/infrahouse_toolkit.terraform.backends.tests.s3backend.rst` & `infrahouse-toolkit-1.5.0/docs/infrahouse_toolkit.terraform.backends.tests.s3backend.rst`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-1.4.0/docs/infrahouse_toolkit.terraform.rst` & `infrahouse-toolkit-1.5.0/docs/infrahouse_toolkit.terraform.rst`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-1.4.0/docs/infrahouse_toolkit.terraform.tests.github_pr.rst` & `infrahouse-toolkit-1.5.0/docs/infrahouse_toolkit.terraform.tests.github_pr.rst`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-1.4.0/docs/infrahouse_toolkit.terraform.tests.rst` & `infrahouse-toolkit-1.5.0/docs/infrahouse_toolkit.terraform.tests.rst`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-1.4.0/docs/infrahouse_toolkit.terraform.tests.status.rst` & `infrahouse-toolkit-1.5.0/docs/infrahouse_toolkit.terraform.tests.status.rst`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-1.4.0/docs/installation.rst` & `infrahouse-toolkit-1.5.0/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-1.4.0/docs/usage.rst` & `infrahouse-toolkit-1.5.0/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-1.4.0/infrahouse_toolkit/cli/ih_plan/__init__.py` & `infrahouse-toolkit-1.5.0/infrahouse_toolkit/cli/ih_plan/__init__.py`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-1.4.0/infrahouse_toolkit/cli/ih_plan/cmd_download/__init__.py` & `infrahouse-toolkit-1.5.0/infrahouse_toolkit/cli/ih_plan/cmd_download/__init__.py`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-1.4.0/infrahouse_toolkit/cli/ih_plan/cmd_min_permissions/__init__.py` & `infrahouse-toolkit-1.5.0/infrahouse_toolkit/cli/ih_plan/cmd_min_permissions/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -2,24 +2,26 @@
 .. topic:: ``ih-plan min-permissions``
 
     A ``ih-plan min-permissions`` subcommand.
 
     See ``ih-plan min-permissions --help`` for more details.
 """
 import json
+from copy import deepcopy
 from json import JSONDecodeError
 
 import click
 
 from infrahouse_toolkit import DEFAULT_OPEN_ENCODING
 
 
 @click.command(name="min-permissions")
+@click.option("--existing-actions", help="A file with permissions.", default=None)
 @click.argument("trace_file")
-def cmd_min_permissions(trace_file):
+def cmd_min_permissions(existing_actions, trace_file):
     """
     Parse Terraform trace file and produce an action list from the trace.
 
     The trace file contains entries with AWS actions. The command
     finds the actions and AWS services to generate a list that
     you can add to an AWS policy.
     It's useful to prepare the least privileges policy.
@@ -32,17 +34,33 @@
         "ec2:DescribeAddresses",
         "ec2:DescribeInternetGateways",
         "ec2:DescribeNatGateways",
     ]
 
     """
     actions = []
+    if existing_actions:
+        with open(existing_actions, encoding=DEFAULT_OPEN_ENCODING) as f_desc:
+            actions = json.loads(f_desc.read())
+
+    old_actions = deepcopy(actions)
+    initial_count = len(old_actions)
+
+    print(f"## Existing {initial_count} actions:")
+    print(json.dumps(sorted(old_actions), indent=4))
+
     with open(trace_file, encoding=DEFAULT_OPEN_ENCODING) as f_decs:
         for line in f_decs.readlines():
             try:
                 operation = json.loads(line)
                 if "aws.operation" in operation:
                     actions.append(f'{operation["aws.service"].lower()}:{operation["aws.operation"]}')
             except JSONDecodeError:
                 pass
 
+    new_actions = list(set(actions))
+    final_count = len(new_actions)
+    print(f"## {final_count - initial_count} new action(s):")
+    print(json.dumps([x for x in new_actions if x not in old_actions], indent=4))
+
+    print(f"## Old and new actions together, {final_count} in total:")
     print(json.dumps(sorted(list(set(actions))), indent=4))
```

### Comparing `infrahouse-toolkit-1.4.0/infrahouse_toolkit/cli/ih_plan/cmd_publish/__init__.py` & `infrahouse-toolkit-1.5.0/infrahouse_toolkit/cli/ih_plan/cmd_publish/__init__.py`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-1.4.0/infrahouse_toolkit/cli/ih_plan/cmd_remove/__init__.py` & `infrahouse-toolkit-1.5.0/infrahouse_toolkit/cli/ih_plan/cmd_remove/__init__.py`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-1.4.0/infrahouse_toolkit/cli/ih_plan/cmd_upload/__init__.py` & `infrahouse-toolkit-1.5.0/infrahouse_toolkit/cli/ih_plan/cmd_upload/__init__.py`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-1.4.0/infrahouse_toolkit/cli/lib.py` & `infrahouse-toolkit-1.5.0/infrahouse_toolkit/cli/lib.py`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-1.4.0/infrahouse_toolkit/cli/tests/conftest.py` & `infrahouse-toolkit-1.5.0/infrahouse_toolkit/cli/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-1.4.0/infrahouse_toolkit/logging.py` & `infrahouse-toolkit-1.5.0/infrahouse_toolkit/logging.py`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-1.4.0/infrahouse_toolkit/terraform/__init__.py` & `infrahouse-toolkit-1.5.0/infrahouse_toolkit/terraform/__init__.py`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-1.4.0/infrahouse_toolkit/terraform/backends/__init__.py` & `infrahouse-toolkit-1.5.0/infrahouse_toolkit/terraform/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-1.4.0/infrahouse_toolkit/terraform/backends/s3backend.py` & `infrahouse-toolkit-1.5.0/infrahouse_toolkit/terraform/backends/s3backend.py`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-1.4.0/infrahouse_toolkit/terraform/backends/tests/s3backend/test_region.py` & `infrahouse-toolkit-1.5.0/infrahouse_toolkit/terraform/backends/tests/s3backend/test_region.py`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-1.4.0/infrahouse_toolkit/terraform/backends/tfbackend.py` & `infrahouse-toolkit-1.5.0/infrahouse_toolkit/terraform/backends/tfbackend.py`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-1.4.0/infrahouse_toolkit/terraform/githubpr.py` & `infrahouse-toolkit-1.5.0/infrahouse_toolkit/terraform/githubpr.py`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-1.4.0/infrahouse_toolkit/terraform/status.py` & `infrahouse-toolkit-1.5.0/infrahouse_toolkit/terraform/status.py`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-1.4.0/infrahouse_toolkit/terraform/tests/github_pr/test_find_comment_by_backend.py` & `infrahouse-toolkit-1.5.0/infrahouse_toolkit/terraform/tests/github_pr/test_find_comment_by_backend.py`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-1.4.0/infrahouse_toolkit/terraform/tests/github_pr/test_publish_comment.py` & `infrahouse-toolkit-1.5.0/infrahouse_toolkit/terraform/tests/github_pr/test_publish_comment.py`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-1.4.0/infrahouse_toolkit/terraform/tests/status/test_eq.py` & `infrahouse-toolkit-1.5.0/infrahouse_toolkit/terraform/tests/status/test_eq.py`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-1.4.0/infrahouse_toolkit/terraform/tests/status/test_metadata.py` & `infrahouse-toolkit-1.5.0/infrahouse_toolkit/terraform/tests/status/test_metadata.py`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-1.4.0/infrahouse_toolkit/terraform/tests/status/test_summary_counts.py` & `infrahouse-toolkit-1.5.0/infrahouse_toolkit/terraform/tests/status/test_summary_counts.py`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-1.4.0/infrahouse_toolkit/terraform/tests/status/test_summary_resources.py` & `infrahouse-toolkit-1.5.0/infrahouse_toolkit/terraform/tests/status/test_summary_resources.py`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-1.4.0/infrahouse_toolkit/terraform/tests/test_parse_comment.py` & `infrahouse-toolkit-1.5.0/infrahouse_toolkit/terraform/tests/test_parse_comment.py`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-1.4.0/infrahouse_toolkit/terraform/tests/test_parse_plan.py` & `infrahouse-toolkit-1.5.0/infrahouse_toolkit/terraform/tests/test_parse_plan.py`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-1.4.0/infrahouse_toolkit.egg-info/PKG-INFO` & `infrahouse-toolkit-1.5.0/infrahouse_toolkit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: infrahouse-toolkit
-Version: 1.4.0
+Version: 1.5.0
 Summary: A collection of tools for building infrastructure.
 Home-page: https://github.com/infrahouse/infrahouse-toolkit
 Author: Oleksandr Kuzminskyi
 Author-email: aleks@infrahouse.com
 License: Apache Software License 2.0
 Keywords: infrahouse-toolkit
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `infrahouse-toolkit-1.4.0/infrahouse_toolkit.egg-info/SOURCES.txt` & `infrahouse-toolkit-1.5.0/infrahouse_toolkit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-1.4.0/setup.py` & `infrahouse-toolkit-1.5.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -56,10 +56,10 @@
     include_package_data=True,
     keywords="infrahouse-toolkit",
     name="infrahouse-toolkit",
     packages=find_packages(include=["infrahouse_toolkit", "infrahouse_toolkit.*"]),
     test_suite="tests",
     tests_require=test_requirements,
     url="https://github.com/infrahouse/infrahouse-toolkit",
-    version="1.4.0",
+    version="1.5.0",
     zip_safe=False,
 )
```

