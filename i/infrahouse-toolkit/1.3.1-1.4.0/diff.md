# Comparing `tmp/infrahouse-toolkit-1.3.1.tar.gz` & `tmp/infrahouse-toolkit-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "infrahouse-toolkit-1.3.1.tar", last modified: Tue Jul  4 21:40:42 2023, max compression
+gzip compressed data, was "infrahouse-toolkit-1.4.0.tar", last modified: Tue Jul  4 22:19:18 2023, max compression
```

## Comparing `infrahouse-toolkit-1.3.1.tar` & `infrahouse-toolkit-1.4.0.tar`

### file list

```diff
@@ -1,100 +1,102 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 21:40:42.854264 infrahouse-toolkit-1.3.1/
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-07-04 21:40:07.000000 infrahouse-toolkit-1.3.1/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2965 2023-07-04 21:40:07.000000 infrahouse-toolkit-1.3.1/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-07-04 21:40:07.000000 infrahouse-toolkit-1.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-07-04 21:40:07.000000 infrahouse-toolkit-1.3.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-07-04 21:40:42.854264 infrahouse-toolkit-1.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-07-04 21:40:07.000000 infrahouse-toolkit-1.3.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 21:40:42.838264 infrahouse-toolkit-1.3.1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      619 2023-07-04 21:40:07.000000 infrahouse-toolkit-1.3.1/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-04 21:40:07.000000 infrahouse-toolkit-1.3.1/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4940 2023-07-04 21:40:07.000000 infrahouse-toolkit-1.3.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-04 21:40:07.000000 infrahouse-toolkit-1.3.1/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      312 2023-07-04 21:40:07.000000 infrahouse-toolkit-1.3.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-07-04 21:40:07.000000 infrahouse-toolkit-1.3.1/docs/infrahouse_toolkit.cli.ih_plan.cmd_download.rst
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-07-04 21:40:07.000000 infrahouse-toolkit-1.3.1/docs/infrahouse_toolkit.cli.ih_plan.cmd_publish.rst
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-07-04 21:40:07.000000 infrahouse-toolkit-1.3.1/docs/infrahouse_toolkit.cli.ih_plan.cmd_remove.rst
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-07-04 21:40:07.000000 infrahouse-toolkit-1.3.1/docs/infrahouse_toolkit.cli.ih_plan.cmd_upload.rst
--rw-r--r--   0 runner    (1001) docker     (123)      456 2023-07-04 21:40:07.000000 infrahouse-toolkit-1.3.1/docs/infrahouse_toolkit.cli.ih_plan.rst
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-07-04 21:40:07.000000 infrahouse-toolkit-1.3.1/docs/infrahouse_toolkit.cli.rst
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-07-04 21:40:07.000000 infrahouse-toolkit-1.3.1/docs/infrahouse_toolkit.cli.tests.rst
--rw-r--r--   0 runner    (1001) docker     (123)      293 2023-07-04 21:40:07.000000 infrahouse-toolkit-1.3.1/docs/infrahouse_toolkit.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-07-04 21:40:07.000000 infrahouse-toolkit-1.3.1/docs/infrahouse_toolkit.terraform.backends.rst
--rw-r--r--   0 runner    (1001) docker     (123)      665 2023-07-04 21:40:07.000000 infrahouse-toolkit-1.3.1/docs/infrahouse_toolkit.terraform.backends.tests.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-07-04 21:40:07.000000 infrahouse-toolkit-1.3.1/docs/infrahouse_toolkit.terraform.backends.tests.s3backend.rst
--rw-r--r--   0 runner    (1001) docker     (123)      771 2023-07-04 21:40:07.000000 infrahouse-toolkit-1.3.1/docs/infrahouse_toolkit.terraform.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-07-04 21:40:07.000000 infrahouse-toolkit-1.3.1/docs/infrahouse_toolkit.terraform.tests.github_pr.rst
--rw-r--r--   0 runner    (1001) docker     (123)      898 2023-07-04 21:40:07.000000 infrahouse-toolkit-1.3.1/docs/infrahouse_toolkit.terraform.tests.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1589 2023-07-04 21:40:07.000000 infrahouse-toolkit-1.3.1/docs/infrahouse_toolkit.terraform.tests.status.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-07-04 21:40:07.000000 infrahouse-toolkit-1.3.1/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-04 21:40:07.000000 infrahouse-toolkit-1.3.1/docs/modules.rst
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-04 21:40:07.000000 infrahouse-toolkit-1.3.1/docs/readme.rst
--rw-r--r--   0 runner    (1001) docker     (123)      982 2023-07-04 21:40:07.000000 infrahouse-toolkit-1.3.1/docs/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 21:40:42.842264 infrahouse-toolkit-1.3.1/infrahouse_toolkit/
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-07-04 21:40:07.000000 infrahouse-toolkit-1.3.1/infrahouse_toolkit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 21:40:42.842264 infrahouse-toolkit-1.3.1/infrahouse_toolkit/cli/
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-07-04 21:40:07.000000 infrahouse-toolkit-1.3.1/infrahouse_toolkit/cli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 21:40:42.846264 infrahouse-toolkit-1.3.1/infrahouse_toolkit/cli/ih_plan/
--rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-07-04 21:40:07.000000 infrahouse-toolkit-1.3.1/infrahouse_toolkit/cli/ih_plan/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 21:40:42.846264 infrahouse-toolkit-1.3.1/infrahouse_toolkit/cli/ih_plan/cmd_download/
--rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-07-04 21:40:07.000000 infrahouse-toolkit-1.3.1/infrahouse_toolkit/cli/ih_plan/cmd_download/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 21:40:42.846264 infrahouse-toolkit-1.3.1/infrahouse_toolkit/cli/ih_plan/cmd_publish/
--rw-r--r--   0 runner    (1001) docker     (123)     2390 2023-07-04 21:40:07.000000 infrahouse-toolkit-1.3.1/infrahouse_toolkit/cli/ih_plan/cmd_publish/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 21:40:42.846264 infrahouse-toolkit-1.3.1/infrahouse_toolkit/cli/ih_plan/cmd_remove/
--rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-07-04 21:40:07.000000 infrahouse-toolkit-1.3.1/infrahouse_toolkit/cli/ih_plan/cmd_remove/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 21:40:42.846264 infrahouse-toolkit-1.3.1/infrahouse_toolkit/cli/ih_plan/cmd_upload/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-04 21:40:07.000000 infrahouse-toolkit-1.3.1/infrahouse_toolkit/cli/ih_plan/cmd_upload/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-07-04 21:40:07.000000 infrahouse-toolkit-1.3.1/infrahouse_toolkit/cli/lib.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 21:40:42.846264 infrahouse-toolkit-1.3.1/infrahouse_toolkit/cli/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 21:40:07.000000 infrahouse-toolkit-1.3.1/infrahouse_toolkit/cli/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      700 2023-07-04 21:40:07.000000 infrahouse-toolkit-1.3.1/infrahouse_toolkit/cli/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-07-04 21:40:07.000000 infrahouse-toolkit-1.3.1/infrahouse_toolkit/cli/tests/test_get_bucket.py
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-07-04 21:40:07.000000 infrahouse-toolkit-1.3.1/infrahouse_toolkit/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-07-04 21:40:07.000000 infrahouse-toolkit-1.3.1/infrahouse_toolkit/logging.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 21:40:42.850264 infrahouse-toolkit-1.3.1/infrahouse_toolkit/terraform/
--rw-r--r--   0 runner    (1001) docker     (123)     8365 2023-07-04 21:40:07.000000 infrahouse-toolkit-1.3.1/infrahouse_toolkit/terraform/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 21:40:42.850264 infrahouse-toolkit-1.3.1/infrahouse_toolkit/terraform/backends/
--rw-r--r--   0 runner    (1001) docker     (123)      907 2023-07-04 21:40:07.000000 infrahouse-toolkit-1.3.1/infrahouse_toolkit/terraform/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-07-04 21:40:07.000000 infrahouse-toolkit-1.3.1/infrahouse_toolkit/terraform/backends/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1453 2023-07-04 21:40:07.000000 infrahouse-toolkit-1.3.1/infrahouse_toolkit/terraform/backends/s3backend.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 21:40:42.850264 infrahouse-toolkit-1.3.1/infrahouse_toolkit/terraform/backends/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 21:40:07.000000 infrahouse-toolkit-1.3.1/infrahouse_toolkit/terraform/backends/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 21:40:42.850264 infrahouse-toolkit-1.3.1/infrahouse_toolkit/terraform/backends/tests/s3backend/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 21:40:07.000000 infrahouse-toolkit-1.3.1/infrahouse_toolkit/terraform/backends/tests/s3backend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-07-04 21:40:07.000000 infrahouse-toolkit-1.3.1/infrahouse_toolkit/terraform/backends/tests/s3backend/test_eq.py
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-04 21:40:07.000000 infrahouse-toolkit-1.3.1/infrahouse_toolkit/terraform/backends/tests/s3backend/test_init.py
--rw-r--r--   0 runner    (1001) docker     (123)      695 2023-07-04 21:40:07.000000 infrahouse-toolkit-1.3.1/infrahouse_toolkit/terraform/backends/tests/s3backend/test_region.py
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-07-04 21:40:07.000000 infrahouse-toolkit-1.3.1/infrahouse_toolkit/terraform/backends/tests/test_get_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-07-04 21:40:07.000000 infrahouse-toolkit-1.3.1/infrahouse_toolkit/terraform/backends/tfbackend.py
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-07-04 21:40:07.000000 infrahouse-toolkit-1.3.1/infrahouse_toolkit/terraform/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3145 2023-07-04 21:40:07.000000 infrahouse-toolkit-1.3.1/infrahouse_toolkit/terraform/githubpr.py
--rw-r--r--   0 runner    (1001) docker     (123)     5155 2023-07-04 21:40:07.000000 infrahouse-toolkit-1.3.1/infrahouse_toolkit/terraform/status.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 21:40:42.854264 infrahouse-toolkit-1.3.1/infrahouse_toolkit/terraform/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 21:40:07.000000 infrahouse-toolkit-1.3.1/infrahouse_toolkit/terraform/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 21:40:42.854264 infrahouse-toolkit-1.3.1/infrahouse_toolkit/terraform/tests/github_pr/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 21:40:07.000000 infrahouse-toolkit-1.3.1/infrahouse_toolkit/terraform/tests/github_pr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      950 2023-07-04 21:40:07.000000 infrahouse-toolkit-1.3.1/infrahouse_toolkit/terraform/tests/github_pr/test_find_comment_by_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-07-04 21:40:07.000000 infrahouse-toolkit-1.3.1/infrahouse_toolkit/terraform/tests/github_pr/test_init.py
--rw-r--r--   0 runner    (1001) docker     (123)      933 2023-07-04 21:40:07.000000 infrahouse-toolkit-1.3.1/infrahouse_toolkit/terraform/tests/github_pr/test_publish_comment.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 21:40:42.854264 infrahouse-toolkit-1.3.1/infrahouse_toolkit/terraform/tests/status/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 21:40:07.000000 infrahouse-toolkit-1.3.1/infrahouse_toolkit/terraform/tests/status/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-07-04 21:40:07.000000 infrahouse-toolkit-1.3.1/infrahouse_toolkit/terraform/tests/status/test_comment.py
--rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-07-04 21:40:07.000000 infrahouse-toolkit-1.3.1/infrahouse_toolkit/terraform/tests/status/test_eq.py
--rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-07-04 21:40:07.000000 infrahouse-toolkit-1.3.1/infrahouse_toolkit/terraform/tests/status/test_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)      531 2023-07-04 21:40:07.000000 infrahouse-toolkit-1.3.1/infrahouse_toolkit/terraform/tests/status/test_summary_counts.py
--rw-r--r--   0 runner    (1001) docker     (123)      650 2023-07-04 21:40:07.000000 infrahouse-toolkit-1.3.1/infrahouse_toolkit/terraform/tests/status/test_summary_resources.py
--rw-r--r--   0 runner    (1001) docker     (123)     2601 2023-07-04 21:40:07.000000 infrahouse-toolkit-1.3.1/infrahouse_toolkit/terraform/tests/test_parse_comment.py
--rw-r--r--   0 runner    (1001) docker     (123)     2369 2023-07-04 21:40:07.000000 infrahouse-toolkit-1.3.1/infrahouse_toolkit/terraform/tests/test_parse_plan.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 21:40:42.842264 infrahouse-toolkit-1.3.1/infrahouse_toolkit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-07-04 21:40:42.000000 infrahouse-toolkit-1.3.1/infrahouse_toolkit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3354 2023-07-04 21:40:42.000000 infrahouse-toolkit-1.3.1/infrahouse_toolkit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 21:40:42.000000 infrahouse-toolkit-1.3.1/infrahouse_toolkit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-04 21:40:42.000000 infrahouse-toolkit-1.3.1/infrahouse_toolkit.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 21:40:37.000000 infrahouse-toolkit-1.3.1/infrahouse_toolkit.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-04 21:40:42.000000 infrahouse-toolkit-1.3.1/infrahouse_toolkit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-04 21:40:42.000000 infrahouse-toolkit-1.3.1/infrahouse_toolkit.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-04 21:40:07.000000 infrahouse-toolkit-1.3.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-07-04 21:40:07.000000 infrahouse-toolkit-1.3.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-07-04 21:40:07.000000 infrahouse-toolkit-1.3.1/requirements_dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)      466 2023-07-04 21:40:42.854264 infrahouse-toolkit-1.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-07-04 21:40:07.000000 infrahouse-toolkit-1.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 22:19:18.059818 infrahouse-toolkit-1.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-07-04 22:18:45.000000 infrahouse-toolkit-1.4.0/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2965 2023-07-04 22:18:45.000000 infrahouse-toolkit-1.4.0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-07-04 22:18:45.000000 infrahouse-toolkit-1.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-07-04 22:18:45.000000 infrahouse-toolkit-1.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-07-04 22:19:18.059818 infrahouse-toolkit-1.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-07-04 22:18:45.000000 infrahouse-toolkit-1.4.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 22:19:18.051818 infrahouse-toolkit-1.4.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      619 2023-07-04 22:18:45.000000 infrahouse-toolkit-1.4.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-04 22:18:45.000000 infrahouse-toolkit-1.4.0/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4940 2023-07-04 22:18:45.000000 infrahouse-toolkit-1.4.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-04 22:18:45.000000 infrahouse-toolkit-1.4.0/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      312 2023-07-04 22:18:45.000000 infrahouse-toolkit-1.4.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-07-04 22:18:45.000000 infrahouse-toolkit-1.4.0/docs/infrahouse_toolkit.cli.ih_plan.cmd_download.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-07-04 22:18:45.000000 infrahouse-toolkit-1.4.0/docs/infrahouse_toolkit.cli.ih_plan.cmd_publish.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-07-04 22:18:45.000000 infrahouse-toolkit-1.4.0/docs/infrahouse_toolkit.cli.ih_plan.cmd_remove.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-07-04 22:18:45.000000 infrahouse-toolkit-1.4.0/docs/infrahouse_toolkit.cli.ih_plan.cmd_upload.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      456 2023-07-04 22:18:45.000000 infrahouse-toolkit-1.4.0/docs/infrahouse_toolkit.cli.ih_plan.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-07-04 22:18:45.000000 infrahouse-toolkit-1.4.0/docs/infrahouse_toolkit.cli.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-07-04 22:18:45.000000 infrahouse-toolkit-1.4.0/docs/infrahouse_toolkit.cli.tests.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-07-04 22:18:45.000000 infrahouse-toolkit-1.4.0/docs/infrahouse_toolkit.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-07-04 22:18:45.000000 infrahouse-toolkit-1.4.0/docs/infrahouse_toolkit.terraform.backends.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-07-04 22:18:45.000000 infrahouse-toolkit-1.4.0/docs/infrahouse_toolkit.terraform.backends.tests.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-07-04 22:18:45.000000 infrahouse-toolkit-1.4.0/docs/infrahouse_toolkit.terraform.backends.tests.s3backend.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-07-04 22:18:45.000000 infrahouse-toolkit-1.4.0/docs/infrahouse_toolkit.terraform.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-07-04 22:18:45.000000 infrahouse-toolkit-1.4.0/docs/infrahouse_toolkit.terraform.tests.github_pr.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      898 2023-07-04 22:18:45.000000 infrahouse-toolkit-1.4.0/docs/infrahouse_toolkit.terraform.tests.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1589 2023-07-04 22:18:45.000000 infrahouse-toolkit-1.4.0/docs/infrahouse_toolkit.terraform.tests.status.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-07-04 22:18:45.000000 infrahouse-toolkit-1.4.0/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-04 22:18:45.000000 infrahouse-toolkit-1.4.0/docs/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-04 22:18:45.000000 infrahouse-toolkit-1.4.0/docs/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      982 2023-07-04 22:18:45.000000 infrahouse-toolkit-1.4.0/docs/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 22:19:18.051818 infrahouse-toolkit-1.4.0/infrahouse_toolkit/
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-07-04 22:18:45.000000 infrahouse-toolkit-1.4.0/infrahouse_toolkit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 22:19:18.055818 infrahouse-toolkit-1.4.0/infrahouse_toolkit/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-07-04 22:18:45.000000 infrahouse-toolkit-1.4.0/infrahouse_toolkit/cli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 22:19:18.055818 infrahouse-toolkit-1.4.0/infrahouse_toolkit/cli/ih_plan/
+-rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-07-04 22:18:45.000000 infrahouse-toolkit-1.4.0/infrahouse_toolkit/cli/ih_plan/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 22:19:18.055818 infrahouse-toolkit-1.4.0/infrahouse_toolkit/cli/ih_plan/cmd_download/
+-rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-07-04 22:18:45.000000 infrahouse-toolkit-1.4.0/infrahouse_toolkit/cli/ih_plan/cmd_download/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 22:19:18.055818 infrahouse-toolkit-1.4.0/infrahouse_toolkit/cli/ih_plan/cmd_min_permissions/
+-rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-07-04 22:18:45.000000 infrahouse-toolkit-1.4.0/infrahouse_toolkit/cli/ih_plan/cmd_min_permissions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 22:19:18.055818 infrahouse-toolkit-1.4.0/infrahouse_toolkit/cli/ih_plan/cmd_publish/
+-rw-r--r--   0 runner    (1001) docker     (123)     2390 2023-07-04 22:18:45.000000 infrahouse-toolkit-1.4.0/infrahouse_toolkit/cli/ih_plan/cmd_publish/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 22:19:18.055818 infrahouse-toolkit-1.4.0/infrahouse_toolkit/cli/ih_plan/cmd_remove/
+-rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-07-04 22:18:45.000000 infrahouse-toolkit-1.4.0/infrahouse_toolkit/cli/ih_plan/cmd_remove/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 22:19:18.055818 infrahouse-toolkit-1.4.0/infrahouse_toolkit/cli/ih_plan/cmd_upload/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-04 22:18:45.000000 infrahouse-toolkit-1.4.0/infrahouse_toolkit/cli/ih_plan/cmd_upload/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-07-04 22:18:45.000000 infrahouse-toolkit-1.4.0/infrahouse_toolkit/cli/lib.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 22:19:18.055818 infrahouse-toolkit-1.4.0/infrahouse_toolkit/cli/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 22:18:45.000000 infrahouse-toolkit-1.4.0/infrahouse_toolkit/cli/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-07-04 22:18:45.000000 infrahouse-toolkit-1.4.0/infrahouse_toolkit/cli/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-07-04 22:18:45.000000 infrahouse-toolkit-1.4.0/infrahouse_toolkit/cli/tests/test_get_bucket.py
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-07-04 22:18:45.000000 infrahouse-toolkit-1.4.0/infrahouse_toolkit/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-07-04 22:18:45.000000 infrahouse-toolkit-1.4.0/infrahouse_toolkit/logging.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 22:19:18.055818 infrahouse-toolkit-1.4.0/infrahouse_toolkit/terraform/
+-rw-r--r--   0 runner    (1001) docker     (123)     8365 2023-07-04 22:18:45.000000 infrahouse-toolkit-1.4.0/infrahouse_toolkit/terraform/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 22:19:18.055818 infrahouse-toolkit-1.4.0/infrahouse_toolkit/terraform/backends/
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-07-04 22:18:45.000000 infrahouse-toolkit-1.4.0/infrahouse_toolkit/terraform/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-07-04 22:18:45.000000 infrahouse-toolkit-1.4.0/infrahouse_toolkit/terraform/backends/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1453 2023-07-04 22:18:45.000000 infrahouse-toolkit-1.4.0/infrahouse_toolkit/terraform/backends/s3backend.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 22:19:18.055818 infrahouse-toolkit-1.4.0/infrahouse_toolkit/terraform/backends/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 22:18:45.000000 infrahouse-toolkit-1.4.0/infrahouse_toolkit/terraform/backends/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 22:19:18.055818 infrahouse-toolkit-1.4.0/infrahouse_toolkit/terraform/backends/tests/s3backend/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 22:18:45.000000 infrahouse-toolkit-1.4.0/infrahouse_toolkit/terraform/backends/tests/s3backend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-07-04 22:18:45.000000 infrahouse-toolkit-1.4.0/infrahouse_toolkit/terraform/backends/tests/s3backend/test_eq.py
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-04 22:18:45.000000 infrahouse-toolkit-1.4.0/infrahouse_toolkit/terraform/backends/tests/s3backend/test_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)      695 2023-07-04 22:18:45.000000 infrahouse-toolkit-1.4.0/infrahouse_toolkit/terraform/backends/tests/s3backend/test_region.py
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-07-04 22:18:45.000000 infrahouse-toolkit-1.4.0/infrahouse_toolkit/terraform/backends/tests/test_get_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-07-04 22:18:45.000000 infrahouse-toolkit-1.4.0/infrahouse_toolkit/terraform/backends/tfbackend.py
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-07-04 22:18:45.000000 infrahouse-toolkit-1.4.0/infrahouse_toolkit/terraform/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3145 2023-07-04 22:18:45.000000 infrahouse-toolkit-1.4.0/infrahouse_toolkit/terraform/githubpr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5155 2023-07-04 22:18:45.000000 infrahouse-toolkit-1.4.0/infrahouse_toolkit/terraform/status.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 22:19:18.055818 infrahouse-toolkit-1.4.0/infrahouse_toolkit/terraform/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 22:18:45.000000 infrahouse-toolkit-1.4.0/infrahouse_toolkit/terraform/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 22:19:18.055818 infrahouse-toolkit-1.4.0/infrahouse_toolkit/terraform/tests/github_pr/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 22:18:45.000000 infrahouse-toolkit-1.4.0/infrahouse_toolkit/terraform/tests/github_pr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      950 2023-07-04 22:18:45.000000 infrahouse-toolkit-1.4.0/infrahouse_toolkit/terraform/tests/github_pr/test_find_comment_by_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-07-04 22:18:45.000000 infrahouse-toolkit-1.4.0/infrahouse_toolkit/terraform/tests/github_pr/test_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)      933 2023-07-04 22:18:45.000000 infrahouse-toolkit-1.4.0/infrahouse_toolkit/terraform/tests/github_pr/test_publish_comment.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 22:19:18.059818 infrahouse-toolkit-1.4.0/infrahouse_toolkit/terraform/tests/status/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 22:18:45.000000 infrahouse-toolkit-1.4.0/infrahouse_toolkit/terraform/tests/status/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-07-04 22:18:45.000000 infrahouse-toolkit-1.4.0/infrahouse_toolkit/terraform/tests/status/test_comment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-07-04 22:18:45.000000 infrahouse-toolkit-1.4.0/infrahouse_toolkit/terraform/tests/status/test_eq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-07-04 22:18:45.000000 infrahouse-toolkit-1.4.0/infrahouse_toolkit/terraform/tests/status/test_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-07-04 22:18:45.000000 infrahouse-toolkit-1.4.0/infrahouse_toolkit/terraform/tests/status/test_summary_counts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-07-04 22:18:45.000000 infrahouse-toolkit-1.4.0/infrahouse_toolkit/terraform/tests/status/test_summary_resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2601 2023-07-04 22:18:45.000000 infrahouse-toolkit-1.4.0/infrahouse_toolkit/terraform/tests/test_parse_comment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2369 2023-07-04 22:18:45.000000 infrahouse-toolkit-1.4.0/infrahouse_toolkit/terraform/tests/test_parse_plan.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 22:19:18.055818 infrahouse-toolkit-1.4.0/infrahouse_toolkit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-07-04 22:19:18.000000 infrahouse-toolkit-1.4.0/infrahouse_toolkit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3417 2023-07-04 22:19:18.000000 infrahouse-toolkit-1.4.0/infrahouse_toolkit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 22:19:18.000000 infrahouse-toolkit-1.4.0/infrahouse_toolkit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-04 22:19:18.000000 infrahouse-toolkit-1.4.0/infrahouse_toolkit.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 22:19:13.000000 infrahouse-toolkit-1.4.0/infrahouse_toolkit.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-04 22:19:18.000000 infrahouse-toolkit-1.4.0/infrahouse_toolkit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-04 22:19:18.000000 infrahouse-toolkit-1.4.0/infrahouse_toolkit.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-04 22:18:45.000000 infrahouse-toolkit-1.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-07-04 22:18:45.000000 infrahouse-toolkit-1.4.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-07-04 22:18:45.000000 infrahouse-toolkit-1.4.0/requirements_dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2023-07-04 22:19:18.059818 infrahouse-toolkit-1.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-07-04 22:18:45.000000 infrahouse-toolkit-1.4.0/setup.py
```

### Comparing `infrahouse-toolkit-1.3.1/CONTRIBUTING.rst` & `infrahouse-toolkit-1.4.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-1.3.1/LICENSE` & `infrahouse-toolkit-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-1.3.1/PKG-INFO` & `infrahouse-toolkit-1.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: infrahouse-toolkit
-Version: 1.3.1
+Version: 1.4.0
 Summary: A collection of tools for building infrastructure.
 Home-page: https://github.com/infrahouse/infrahouse-toolkit
 Author: Oleksandr Kuzminskyi
 Author-email: aleks@infrahouse.com
 License: Apache Software License 2.0
 Keywords: infrahouse-toolkit
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `infrahouse-toolkit-1.3.1/README.rst` & `infrahouse-toolkit-1.4.0/README.rst`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-1.3.1/docs/Makefile` & `infrahouse-toolkit-1.4.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-1.3.1/docs/conf.py` & `infrahouse-toolkit-1.4.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-1.3.1/docs/infrahouse_toolkit.cli.tests.rst` & `infrahouse-toolkit-1.4.0/docs/infrahouse_toolkit.cli.tests.rst`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-1.3.1/docs/infrahouse_toolkit.terraform.backends.rst` & `infrahouse-toolkit-1.4.0/docs/infrahouse_toolkit.terraform.backends.rst`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-1.3.1/docs/infrahouse_toolkit.terraform.backends.tests.rst` & `infrahouse-toolkit-1.4.0/docs/infrahouse_toolkit.terraform.backends.tests.rst`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-1.3.1/docs/infrahouse_toolkit.terraform.backends.tests.s3backend.rst` & `infrahouse-toolkit-1.4.0/docs/infrahouse_toolkit.terraform.backends.tests.s3backend.rst`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-1.3.1/docs/infrahouse_toolkit.terraform.rst` & `infrahouse-toolkit-1.4.0/docs/infrahouse_toolkit.terraform.rst`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-1.3.1/docs/infrahouse_toolkit.terraform.tests.github_pr.rst` & `infrahouse-toolkit-1.4.0/docs/infrahouse_toolkit.terraform.tests.github_pr.rst`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-1.3.1/docs/infrahouse_toolkit.terraform.tests.rst` & `infrahouse-toolkit-1.4.0/docs/infrahouse_toolkit.terraform.tests.rst`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-1.3.1/docs/infrahouse_toolkit.terraform.tests.status.rst` & `infrahouse-toolkit-1.4.0/docs/infrahouse_toolkit.terraform.tests.status.rst`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-1.3.1/docs/installation.rst` & `infrahouse-toolkit-1.4.0/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-1.3.1/docs/usage.rst` & `infrahouse-toolkit-1.4.0/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-1.3.1/infrahouse_toolkit/cli/ih_plan/__init__.py` & `infrahouse-toolkit-1.4.0/infrahouse_toolkit/cli/ih_plan/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,14 +5,15 @@
     The command can upload the plan to an S3 bucket, download it, and remove.
 
     See ``ih-plan --help`` for more details.
 """
 import click
 
 from infrahouse_toolkit.cli.ih_plan.cmd_download import cmd_download
+from infrahouse_toolkit.cli.ih_plan.cmd_min_permissions import cmd_min_permissions
 from infrahouse_toolkit.cli.ih_plan.cmd_publish import cmd_publish
 from infrahouse_toolkit.cli.ih_plan.cmd_remove import cmd_remove
 from infrahouse_toolkit.cli.ih_plan.cmd_upload import cmd_upload
 from infrahouse_toolkit.cli.lib import DEFAULT_TF_BACKEND_FILE
 
 
 @click.group(name="it-plan")
@@ -37,10 +38,10 @@
 @click.version_option()
 @click.pass_context
 def ih_plan(ctx, bucket, aws_assume_role_arn, tf_backend_file):
     """Terraform plan helpers."""
     ctx.obj = {"aws_assume_role_arn": aws_assume_role_arn, "bucket": bucket, "tf_backend_file": tf_backend_file}
 
 
-for cmd in [cmd_upload, cmd_download, cmd_remove, cmd_publish]:
+for cmd in [cmd_upload, cmd_download, cmd_remove, cmd_publish, cmd_min_permissions]:
     # noinspection PyTypeChecker
     ih_plan.add_command(cmd)
```

### Comparing `infrahouse-toolkit-1.3.1/infrahouse_toolkit/cli/ih_plan/cmd_download/__init__.py` & `infrahouse-toolkit-1.4.0/infrahouse_toolkit/cli/ih_plan/cmd_download/__init__.py`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-1.3.1/infrahouse_toolkit/cli/ih_plan/cmd_publish/__init__.py` & `infrahouse-toolkit-1.4.0/infrahouse_toolkit/cli/ih_plan/cmd_publish/__init__.py`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-1.3.1/infrahouse_toolkit/cli/ih_plan/cmd_remove/__init__.py` & `infrahouse-toolkit-1.4.0/infrahouse_toolkit/cli/ih_plan/cmd_remove/__init__.py`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-1.3.1/infrahouse_toolkit/cli/ih_plan/cmd_upload/__init__.py` & `infrahouse-toolkit-1.4.0/infrahouse_toolkit/cli/ih_plan/cmd_upload/__init__.py`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-1.3.1/infrahouse_toolkit/cli/lib.py` & `infrahouse-toolkit-1.4.0/infrahouse_toolkit/cli/lib.py`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-1.3.1/infrahouse_toolkit/cli/tests/conftest.py` & `infrahouse-toolkit-1.4.0/infrahouse_toolkit/cli/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-1.3.1/infrahouse_toolkit/logging.py` & `infrahouse-toolkit-1.4.0/infrahouse_toolkit/logging.py`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-1.3.1/infrahouse_toolkit/terraform/__init__.py` & `infrahouse-toolkit-1.4.0/infrahouse_toolkit/terraform/__init__.py`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-1.3.1/infrahouse_toolkit/terraform/backends/__init__.py` & `infrahouse-toolkit-1.4.0/infrahouse_toolkit/terraform/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-1.3.1/infrahouse_toolkit/terraform/backends/s3backend.py` & `infrahouse-toolkit-1.4.0/infrahouse_toolkit/terraform/backends/s3backend.py`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-1.3.1/infrahouse_toolkit/terraform/backends/tests/s3backend/test_region.py` & `infrahouse-toolkit-1.4.0/infrahouse_toolkit/terraform/backends/tests/s3backend/test_region.py`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-1.3.1/infrahouse_toolkit/terraform/backends/tfbackend.py` & `infrahouse-toolkit-1.4.0/infrahouse_toolkit/terraform/backends/tfbackend.py`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-1.3.1/infrahouse_toolkit/terraform/githubpr.py` & `infrahouse-toolkit-1.4.0/infrahouse_toolkit/terraform/githubpr.py`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-1.3.1/infrahouse_toolkit/terraform/status.py` & `infrahouse-toolkit-1.4.0/infrahouse_toolkit/terraform/status.py`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-1.3.1/infrahouse_toolkit/terraform/tests/github_pr/test_find_comment_by_backend.py` & `infrahouse-toolkit-1.4.0/infrahouse_toolkit/terraform/tests/github_pr/test_find_comment_by_backend.py`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-1.3.1/infrahouse_toolkit/terraform/tests/github_pr/test_publish_comment.py` & `infrahouse-toolkit-1.4.0/infrahouse_toolkit/terraform/tests/github_pr/test_publish_comment.py`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-1.3.1/infrahouse_toolkit/terraform/tests/status/test_eq.py` & `infrahouse-toolkit-1.4.0/infrahouse_toolkit/terraform/tests/status/test_eq.py`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-1.3.1/infrahouse_toolkit/terraform/tests/status/test_metadata.py` & `infrahouse-toolkit-1.4.0/infrahouse_toolkit/terraform/tests/status/test_metadata.py`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-1.3.1/infrahouse_toolkit/terraform/tests/status/test_summary_counts.py` & `infrahouse-toolkit-1.4.0/infrahouse_toolkit/terraform/tests/status/test_summary_counts.py`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-1.3.1/infrahouse_toolkit/terraform/tests/status/test_summary_resources.py` & `infrahouse-toolkit-1.4.0/infrahouse_toolkit/terraform/tests/status/test_summary_resources.py`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-1.3.1/infrahouse_toolkit/terraform/tests/test_parse_comment.py` & `infrahouse-toolkit-1.4.0/infrahouse_toolkit/terraform/tests/test_parse_comment.py`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-1.3.1/infrahouse_toolkit/terraform/tests/test_parse_plan.py` & `infrahouse-toolkit-1.4.0/infrahouse_toolkit/terraform/tests/test_parse_plan.py`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-1.3.1/infrahouse_toolkit.egg-info/PKG-INFO` & `infrahouse-toolkit-1.4.0/infrahouse_toolkit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: infrahouse-toolkit
-Version: 1.3.1
+Version: 1.4.0
 Summary: A collection of tools for building infrastructure.
 Home-page: https://github.com/infrahouse/infrahouse-toolkit
 Author: Oleksandr Kuzminskyi
 Author-email: aleks@infrahouse.com
 License: Apache Software License 2.0
 Keywords: infrahouse-toolkit
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `infrahouse-toolkit-1.3.1/infrahouse_toolkit.egg-info/SOURCES.txt` & `infrahouse-toolkit-1.4.0/infrahouse_toolkit.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -42,14 +42,15 @@
 infrahouse_toolkit.egg-info/not-zip-safe
 infrahouse_toolkit.egg-info/requires.txt
 infrahouse_toolkit.egg-info/top_level.txt
 infrahouse_toolkit/cli/__init__.py
 infrahouse_toolkit/cli/lib.py
 infrahouse_toolkit/cli/ih_plan/__init__.py
 infrahouse_toolkit/cli/ih_plan/cmd_download/__init__.py
+infrahouse_toolkit/cli/ih_plan/cmd_min_permissions/__init__.py
 infrahouse_toolkit/cli/ih_plan/cmd_publish/__init__.py
 infrahouse_toolkit/cli/ih_plan/cmd_remove/__init__.py
 infrahouse_toolkit/cli/ih_plan/cmd_upload/__init__.py
 infrahouse_toolkit/cli/tests/__init__.py
 infrahouse_toolkit/cli/tests/conftest.py
 infrahouse_toolkit/cli/tests/test_get_bucket.py
 infrahouse_toolkit/terraform/__init__.py
```

### Comparing `infrahouse-toolkit-1.3.1/setup.py` & `infrahouse-toolkit-1.4.0/setup.py`

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
-    version="1.3.1",
+    version="1.4.0",
     zip_safe=False,
 )
```

