# Comparing `tmp/hcs-cli-0.1.38.tar.gz` & `tmp/hcs-cli-0.1.39.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hcs-cli-0.1.38.tar", last modified: Wed Jul  5 19:54:20 2023, max compression
+gzip compressed data, was "hcs-cli-0.1.39.tar", last modified: Wed Jul  5 19:55:45 2023, max compression
```

## Comparing `hcs-cli-0.1.38.tar` & `hcs-cli-0.1.39.tar`

### file list

```diff
@@ -1,259 +1,259 @@
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-05 19:54:20.782106 hcs-cli-0.1.38/
--rw-r--r--   0 nanw       (501) staff       (20)     2824 2023-06-21 18:44:48.000000 hcs-cli-0.1.38/.gitignore
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-05 19:54:20.486081 hcs-cli-0.1.38/.vscode/
--rw-r--r--   0 nanw       (501) staff       (20)     2564 2023-07-05 08:21:14.000000 hcs-cli-0.1.38/.vscode/launch.json
--rw-r--r--   0 nanw       (501) staff       (20)       49 2023-06-30 00:59:55.000000 hcs-cli-0.1.38/.vscode/settings.json
--rw-r--r--   0 nanw       (501) staff       (20)       98 2023-06-13 19:57:56.000000 hcs-cli-0.1.38/CHANGELOG.md
--rw-r--r--   0 nanw       (501) staff       (20)     5258 2023-06-13 16:45:49.000000 hcs-cli-0.1.38/CODE_OF_CONDUCT.md
--rw-r--r--   0 nanw       (501) staff       (20)     2706 2023-06-13 18:53:18.000000 hcs-cli-0.1.38/CONTRIBUTING_CLA.md
--rw-r--r--   0 nanw       (501) staff       (20)     6095 2023-04-25 23:13:27.000000 hcs-cli-0.1.38/GOVERNANCE.md
--rw-r--r--   0 nanw       (501) staff       (20)    10449 2023-06-13 16:45:49.000000 hcs-cli-0.1.38/LICENSE
--rw-r--r--   0 nanw       (501) staff       (20)      854 2023-07-03 19:19:46.000000 hcs-cli-0.1.38/Makefile
--rw-r--r--   0 nanw       (501) staff       (20)      411 2023-06-13 16:45:49.000000 hcs-cli-0.1.38/NOTICE
--rw-r--r--   0 nanw       (501) staff       (20)     2516 2023-07-05 19:54:20.781269 hcs-cli-0.1.38/PKG-INFO
--rw-r--r--   0 nanw       (501) staff       (20)     1642 2023-06-24 01:22:59.000000 hcs-cli-0.1.38/README.md
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-05 19:54:20.495953 hcs-cli-0.1.38/doc/
--rw-r--r--   0 nanw       (501) staff       (20)     5950 2023-06-15 17:50:47.000000 hcs-cli-0.1.38/doc/dev-setup.md
--rw-r--r--   0 nanw       (501) staff       (20)      763 2023-06-13 17:49:20.000000 hcs-cli-0.1.38/doc/get-csp-user-api-token.md
--rw-r--r--   0 nanw       (501) staff       (20)     6394 2023-07-03 19:03:00.000000 hcs-cli-0.1.38/doc/hcs-cli-cheatsheet.md
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-05 19:54:20.506507 hcs-cli-0.1.38/hcs_cli.egg-info/
--rw-r--r--   0 nanw       (501) staff       (20)     2516 2023-07-05 19:54:20.000000 hcs-cli-0.1.38/hcs_cli.egg-info/PKG-INFO
--rw-r--r--   0 nanw       (501) staff       (20)     5934 2023-07-05 19:54:20.000000 hcs-cli-0.1.38/hcs_cli.egg-info/SOURCES.txt
--rw-r--r--   0 nanw       (501) staff       (20)        1 2023-07-05 19:54:20.000000 hcs-cli-0.1.38/hcs_cli.egg-info/dependency_links.txt
--rw-r--r--   0 nanw       (501) staff       (20)       43 2023-07-05 19:54:20.000000 hcs-cli-0.1.38/hcs_cli.egg-info/entry_points.txt
--rw-r--r--   0 nanw       (501) staff       (20)      127 2023-07-05 19:54:20.000000 hcs-cli-0.1.38/hcs_cli.egg-info/requires.txt
--rw-r--r--   0 nanw       (501) staff       (20)       11 2023-07-05 19:54:20.000000 hcs-cli-0.1.38/hcs_cli.egg-info/top_level.txt
--rw-r--r--   0 nanw       (501) staff       (20)       92 2023-04-24 20:24:05.000000 hcs-cli-0.1.38/mypy.ini
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-05 19:54:20.414223 hcs-cli-0.1.38/payload/
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-05 19:54:20.507834 hcs-cli-0.1.38/payload/lcm/
--rw-r--r--   0 nanw       (501) staff       (20)      752 2023-04-24 20:24:05.000000 hcs-cli-0.1.38/payload/lcm/zero.json
--rw-r--r--   0 nanw       (501) staff       (20)     1187 2023-06-13 19:56:09.000000 hcs-cli-0.1.38/pyproject.toml
--rw-r--r--   0 nanw       (501) staff       (20)      194 2023-04-24 20:24:05.000000 hcs-cli-0.1.38/requirements-dev.txt
--rw-r--r--   0 nanw       (501) staff       (20)      127 2023-04-24 20:24:05.000000 hcs-cli-0.1.38/requirements.txt
--rw-r--r--   0 nanw       (501) staff       (20)       38 2023-07-05 19:54:20.782328 hcs-cli-0.1.38/setup.cfg
--rw-r--r--   0 nanw       (501) staff       (20)     1154 2023-07-05 19:52:44.000000 hcs-cli-0.1.38/setup.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-05 19:54:20.511258 hcs-cli-0.1.38/tests/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-24 20:24:05.000000 hcs-cli-0.1.38/tests/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)      599 2023-06-13 19:40:36.000000 hcs-cli-0.1.38/tests/conftest.py
--rw-r--r--   0 nanw       (501) staff       (20)     3364 2023-07-05 16:02:01.000000 hcs-cli-0.1.38/tests/test_utils.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-05 19:54:20.512481 hcs-cli-0.1.38/tests/vhcs/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-24 20:24:05.000000 hcs-cli-0.1.38/tests/vhcs/__init__.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-05 19:54:20.513715 hcs-cli-0.1.38/tests/vhcs/cli/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-24 20:24:05.000000 hcs-cli-0.1.38/tests/vhcs/cli/__init__.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-05 19:54:20.518674 hcs-cli-0.1.38/tests/vhcs/cli/cmds/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-24 20:24:05.000000 hcs-cli-0.1.38/tests/vhcs/cli/cmds/__init__.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-05 19:54:20.521103 hcs-cli-0.1.38/tests/vhcs/cli/cmds/pki/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-24 20:24:05.000000 hcs-cli-0.1.38/tests/vhcs/cli/cmds/pki/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)      599 2023-06-13 19:40:36.000000 hcs-cli-0.1.38/tests/vhcs/cli/cmds/pki/get_root_ca.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-05 19:54:20.523214 hcs-cli-0.1.38/tests/vhcs/cli/cmds/plan/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-07-05 15:13:25.000000 hcs-cli-0.1.38/tests/vhcs/cli/cmds/plan/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)     6151 2023-07-05 19:50:01.000000 hcs-cli-0.1.38/tests/vhcs/cli/cmds/plan/test_plan.py
--rw-r--r--   0 nanw       (501) staff       (20)     1943 2023-06-13 19:40:36.000000 hcs-cli-0.1.38/tests/vhcs/cli/cmds/test_context.py
--rw-r--r--   0 nanw       (501) staff       (20)      918 2023-07-03 19:18:10.000000 hcs-cli-0.1.38/tests/vhcs/cli/cmds/test_login.py
--rw-r--r--   0 nanw       (501) staff       (20)     1151 2023-07-05 08:29:47.000000 hcs-cli-0.1.38/tests/vhcs/cli/cmds/test_profile.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-05 19:54:20.525810 hcs-cli-0.1.38/vhcs/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 21:25:27.000000 hcs-cli-0.1.38/vhcs/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)      687 2023-06-13 19:40:36.000000 hcs-cli-0.1.38/vhcs/__main__.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-05 19:54:20.529077 hcs-cli-0.1.38/vhcs/cli/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 02:05:21.000000 hcs-cli-0.1.38/vhcs/cli/__init__.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-05 19:54:20.533515 hcs-cli-0.1.38/vhcs/cli/cmds/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 02:05:21.000000 hcs-cli-0.1.38/vhcs/cli/cmds/__init__.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-05 19:54:20.535415 hcs-cli-0.1.38/vhcs/cli/cmds/admin/
--rw-r--r--   0 nanw       (501) staff       (20)      633 2023-06-13 19:40:36.000000 hcs-cli-0.1.38/vhcs/cli/cmds/admin/__init__.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-05 19:54:20.537901 hcs-cli-0.1.38/vhcs/cli/cmds/admin/azure-infra/
--rw-r--r--   0 nanw       (501) staff       (20)     1069 2023-06-27 20:44:31.000000 hcs-cli-0.1.38/vhcs/cli/cmds/admin/azure-infra/main.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-05 19:54:20.541517 hcs-cli-0.1.38/vhcs/cli/cmds/admin/edge/
--rw-r--r--   0 nanw       (501) staff       (20)      628 2023-06-13 19:40:36.000000 hcs-cli-0.1.38/vhcs/cli/cmds/admin/edge/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)      941 2023-06-13 19:40:36.000000 hcs-cli-0.1.38/vhcs/cli/cmds/admin/edge/get.py
--rw-r--r--   0 nanw       (501) staff       (20)      599 2023-06-13 19:40:36.000000 hcs-cli-0.1.38/vhcs/cli/cmds/admin/edge/list.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-05 19:54:20.543208 hcs-cli-0.1.38/vhcs/cli/cmds/admin/provider/
--rw-r--r--   0 nanw       (501) staff       (20)     1136 2023-06-15 22:34:38.000000 hcs-cli-0.1.38/vhcs/cli/cmds/admin/provider/list.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-05 19:54:20.549108 hcs-cli-0.1.38/vhcs/cli/cmds/admin/template/
--rw-r--r--   0 nanw       (501) staff       (20)      628 2023-06-13 19:40:36.000000 hcs-cli-0.1.38/vhcs/cli/cmds/admin/template/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)      949 2023-06-13 19:40:36.000000 hcs-cli-0.1.38/vhcs/cli/cmds/admin/template/get.py
--rw-r--r--   0 nanw       (501) staff       (20)     1841 2023-06-23 17:01:30.000000 hcs-cli-0.1.38/vhcs/cli/cmds/admin/template/list.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-05 19:54:20.552165 hcs-cli-0.1.38/vhcs/cli/cmds/daas/
--rw-r--r--   0 nanw       (501) staff       (20)      642 2023-06-15 22:15:00.000000 hcs-cli-0.1.38/vhcs/cli/cmds/daas/__init__.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-05 19:54:20.560114 hcs-cli-0.1.38/vhcs/cli/cmds/daas/infra/
--rw-r--r--   0 nanw       (501) staff       (20)      648 2023-06-21 17:56:47.000000 hcs-cli-0.1.38/vhcs/cli/cmds/daas/infra/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)     1041 2023-06-30 16:52:44.000000 hcs-cli-0.1.38/vhcs/cli/cmds/daas/infra/basic.py
--rw-r--r--   0 nanw       (501) staff       (20)     2335 2023-07-05 08:38:57.000000 hcs-cli-0.1.38/vhcs/cli/cmds/daas/infra/plan.py
--rw-r--r--   0 nanw       (501) staff       (20)      745 2023-06-21 18:14:23.000000 hcs-cli-0.1.38/vhcs/cli/cmds/daas/infra/validate.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-05 19:54:20.570082 hcs-cli-0.1.38/vhcs/cli/cmds/daas/tenant/
--rw-r--r--   0 nanw       (501) staff       (20)      633 2023-06-21 17:36:22.000000 hcs-cli-0.1.38/vhcs/cli/cmds/daas/tenant/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)      963 2023-06-30 16:57:41.000000 hcs-cli-0.1.38/vhcs/cli/cmds/daas/tenant/basic.py
--rw-r--r--   0 nanw       (501) staff       (20)     1022 2023-07-05 16:13:46.000000 hcs-cli-0.1.38/vhcs/cli/cmds/daas/tenant/deploy.py
--rw-r--r--   0 nanw       (501) staff       (20)     1378 2023-07-05 16:11:32.000000 hcs-cli-0.1.38/vhcs/cli/cmds/daas/tenant/destroy.py
--rw-r--r--   0 nanw       (501) staff       (20)     4991 2023-07-05 18:15:55.000000 hcs-cli-0.1.38/vhcs/cli/cmds/daas/tenant/plan.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-05 19:54:20.574805 hcs-cli-0.1.38/vhcs/cli/cmds/ims/
--rw-r--r--   0 nanw       (501) staff       (20)      633 2023-06-27 19:52:41.000000 hcs-cli-0.1.38/vhcs/cli/cmds/ims/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)      915 2023-06-27 19:56:58.000000 hcs-cli-0.1.38/vhcs/cli/cmds/ims/list.py
--rw-r--r--   0 nanw       (501) staff       (20)     1033 2023-06-27 20:14:16.000000 hcs-cli-0.1.38/vhcs/cli/cmds/ims/list_copies.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-05 19:54:20.576174 hcs-cli-0.1.38/vhcs/cli/cmds/lcm/
--rw-r--r--   0 nanw       (501) staff       (20)      631 2023-06-27 19:52:37.000000 hcs-cli-0.1.38/vhcs/cli/cmds/lcm/__init__.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-05 19:54:20.583545 hcs-cli-0.1.38/vhcs/cli/cmds/lcm/provider/
--rw-r--r--   0 nanw       (501) staff       (20)      628 2023-06-13 19:40:36.000000 hcs-cli-0.1.38/vhcs/cli/cmds/lcm/provider/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)      801 2023-06-23 02:35:21.000000 hcs-cli-0.1.38/vhcs/cli/cmds/lcm/provider/delete.py
--rw-r--r--   0 nanw       (501) staff       (20)      792 2023-06-23 02:35:30.000000 hcs-cli-0.1.38/vhcs/cli/cmds/lcm/provider/get.py
--rw-r--r--   0 nanw       (501) staff       (20)      987 2023-06-23 02:35:40.000000 hcs-cli-0.1.38/vhcs/cli/cmds/lcm/provider/list.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-05 19:54:20.591905 hcs-cli-0.1.38/vhcs/cli/cmds/lcm/template/
--rw-r--r--   0 nanw       (501) staff       (20)      628 2023-06-13 19:40:36.000000 hcs-cli-0.1.38/vhcs/cli/cmds/lcm/template/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)     1857 2023-06-23 02:36:50.000000 hcs-cli-0.1.38/vhcs/cli/cmds/lcm/template/create.py
--rw-r--r--   0 nanw       (501) staff       (20)     1079 2023-06-23 02:36:58.000000 hcs-cli-0.1.38/vhcs/cli/cmds/lcm/template/delete.py
--rw-r--r--   0 nanw       (501) staff       (20)      840 2023-06-23 02:37:07.000000 hcs-cli-0.1.38/vhcs/cli/cmds/lcm/template/get.py
--rw-r--r--   0 nanw       (501) staff       (20)     1588 2023-06-23 02:37:18.000000 hcs-cli-0.1.38/vhcs/cli/cmds/lcm/template/list.py
--rw-r--r--   0 nanw       (501) staff       (20)     2256 2023-06-23 02:37:44.000000 hcs-cli-0.1.38/vhcs/cli/cmds/lcm/template/wait.py
--rw-r--r--   0 nanw       (501) staff       (20)     6631 2023-07-05 07:47:22.000000 hcs-cli-0.1.38/vhcs/cli/cmds/login.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-05 19:54:20.436269 hcs-cli-0.1.38/vhcs/cli/cmds/org/
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-05 19:54:20.595288 hcs-cli-0.1.38/vhcs/cli/cmds/org/datacenter/
--rw-r--r--   0 nanw       (501) staff       (20)      848 2023-06-30 15:40:06.000000 hcs-cli-0.1.38/vhcs/cli/cmds/org/datacenter/get.py
--rw-r--r--   0 nanw       (501) staff       (20)      997 2023-06-30 15:40:15.000000 hcs-cli-0.1.38/vhcs/cli/cmds/org/datacenter/list.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-05 19:54:20.597993 hcs-cli-0.1.38/vhcs/cli/cmds/org/detail/
--rw-r--r--   0 nanw       (501) staff       (20)      906 2023-06-30 15:40:19.000000 hcs-cli-0.1.38/vhcs/cli/cmds/org/detail/get.py
--rw-r--r--   0 nanw       (501) staff       (20)     1201 2023-06-30 15:40:25.000000 hcs-cli-0.1.38/vhcs/cli/cmds/org/detail/list.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-05 19:54:20.610113 hcs-cli-0.1.38/vhcs/cli/cmds/pki/
--rw-r--r--   0 nanw       (501) staff       (20)      631 2023-06-13 19:45:45.000000 hcs-cli-0.1.38/vhcs/cli/cmds/pki/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)     1155 2023-06-30 15:38:40.000000 hcs-cli-0.1.38/vhcs/cli/cmds/pki/delete_org_cert.py
--rw-r--r--   0 nanw       (501) staff       (20)      906 2023-06-30 15:38:40.000000 hcs-cli-0.1.38/vhcs/cli/cmds/pki/get_org_cert.py
--rw-r--r--   0 nanw       (501) staff       (20)      775 2023-06-30 15:38:40.000000 hcs-cli-0.1.38/vhcs/cli/cmds/pki/get_root_ca.py
--rw-r--r--   0 nanw       (501) staff       (20)     1804 2023-06-30 15:38:40.000000 hcs-cli-0.1.38/vhcs/cli/cmds/pki/sign_resource_cert.py
--rw-r--r--   0 nanw       (501) staff       (20)      726 2023-06-30 15:38:40.000000 hcs-cli-0.1.38/vhcs/cli/cmds/pki/test.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-05 19:54:20.618647 hcs-cli-0.1.38/vhcs/cli/cmds/plan/
--rw-r--r--   0 nanw       (501) staff       (20)      665 2023-06-28 17:52:44.000000 hcs-cli-0.1.38/vhcs/cli/cmds/plan/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)     1745 2023-07-05 16:15:40.000000 hcs-cli-0.1.38/vhcs/cli/cmds/plan/deploy.py
--rw-r--r--   0 nanw       (501) staff       (20)     1328 2023-07-05 16:15:58.000000 hcs-cli-0.1.38/vhcs/cli/cmds/plan/destroy.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-05 19:54:20.630898 hcs-cli-0.1.38/vhcs/cli/cmds/profile/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 02:05:21.000000 hcs-cli-0.1.38/vhcs/cli/cmds/profile/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)     1765 2023-07-05 06:16:00.000000 hcs-cli-0.1.38/vhcs/cli/cmds/profile/init.py
--rw-r--r--   0 nanw       (501) staff       (20)      932 2023-06-13 19:40:36.000000 hcs-cli-0.1.38/vhcs/cli/cmds/upgrade.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-05 19:54:20.638632 hcs-cli-0.1.38/vhcs/cli/cmds/vmhub/
--rw-r--r--   0 nanw       (501) staff       (20)      633 2023-06-13 19:40:36.000000 hcs-cli-0.1.38/vhcs/cli/cmds/vmhub/__init__.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-05 19:54:20.648793 hcs-cli-0.1.38/vhcs/cli/cmds/vmhub/otp/
--rw-r--r--   0 nanw       (501) staff       (20)      643 2023-06-29 21:49:43.000000 hcs-cli-0.1.38/vhcs/cli/cmds/vmhub/otp/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)     1234 2023-06-29 21:49:20.000000 hcs-cli-0.1.38/vhcs/cli/cmds/vmhub/otp/redeem.py
--rw-r--r--   0 nanw       (501) staff       (20)     1143 2023-06-29 21:49:25.000000 hcs-cli-0.1.38/vhcs/cli/cmds/vmhub/otp/request.py
--rwxr-xr-x   0 nanw       (501) staff       (20)     2865 2023-06-23 02:40:39.000000 hcs-cli-0.1.38/vhcs/cli/main.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-05 19:54:20.653495 hcs-cli-0.1.38/vhcs/common/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 02:05:21.000000 hcs-cli-0.1.38/vhcs/common/__init__.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-05 19:54:20.679432 hcs-cli-0.1.38/vhcs/common/ctxp/
--rw-r--r--   0 nanw       (501) staff       (20)     1538 2023-07-03 20:20:16.000000 hcs-cli-0.1.38/vhcs/common/ctxp/README.md
--rw-r--r--   0 nanw       (501) staff       (20)      790 2023-07-03 20:45:37.000000 hcs-cli-0.1.38/vhcs/common/ctxp/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)     1155 2023-07-03 21:18:13.000000 hcs-cli-0.1.38/vhcs/common/ctxp/_init.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-05 19:54:20.682613 hcs-cli-0.1.38/vhcs/common/ctxp/built_in_cmds/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 02:05:21.000000 hcs-cli-0.1.38/vhcs/common/ctxp/built_in_cmds/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)     2421 2023-06-21 17:26:56.000000 hcs-cli-0.1.38/vhcs/common/ctxp/built_in_cmds/context.py
--rw-r--r--   0 nanw       (501) staff       (20)     3977 2023-07-05 08:26:35.000000 hcs-cli-0.1.38/vhcs/common/ctxp/built_in_cmds/profile.py
--rw-r--r--   0 nanw       (501) staff       (20)     5129 2023-07-05 06:22:51.000000 hcs-cli-0.1.38/vhcs/common/ctxp/cli_processor.py
--rw-r--r--   0 nanw       (501) staff       (20)      936 2023-07-03 21:17:12.000000 hcs-cli-0.1.38/vhcs/common/ctxp/config.py
--rw-r--r--   0 nanw       (501) staff       (20)     1205 2023-07-03 21:08:50.000000 hcs-cli-0.1.38/vhcs/common/ctxp/context.py
--rw-r--r--   0 nanw       (501) staff       (20)     6467 2023-06-23 00:26:19.000000 hcs-cli-0.1.38/vhcs/common/ctxp/fstore.py
--rw-r--r--   0 nanw       (501) staff       (20)     1200 2023-06-13 19:40:36.000000 hcs-cli-0.1.38/vhcs/common/ctxp/init.py
--rw-r--r--   0 nanw       (501) staff       (20)     2776 2023-06-22 22:58:23.000000 hcs-cli-0.1.38/vhcs/common/ctxp/jsondot.py
--rw-r--r--   0 nanw       (501) staff       (20)     5163 2023-07-05 08:33:15.000000 hcs-cli-0.1.38/vhcs/common/ctxp/profile.py
--rw-r--r--   0 nanw       (501) staff       (20)     1565 2023-07-05 06:52:28.000000 hcs-cli-0.1.38/vhcs/common/ctxp/profile_store.py
--rw-r--r--   0 nanw       (501) staff       (20)     1604 2023-07-03 22:06:25.000000 hcs-cli-0.1.38/vhcs/common/ctxp/state.py
--rw-r--r--   0 nanw       (501) staff       (20)     6258 2023-07-05 06:26:16.000000 hcs-cli-0.1.38/vhcs/common/ctxp/util.py
--rw-r--r--   0 nanw       (501) staff       (20)     3256 2023-06-13 19:40:36.000000 hcs-cli-0.1.38/vhcs/common/ctxp/var_template.py
--rw-r--r--   0 nanw       (501) staff       (20)     2259 2023-07-05 18:05:17.000000 hcs-cli-0.1.38/vhcs/common/duration.py
--rw-r--r--   0 nanw       (501) staff       (20)     4846 2023-06-13 19:40:36.000000 hcs-cli-0.1.38/vhcs/common/logger.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-05 19:54:20.692644 hcs-cli-0.1.38/vhcs/common/sglib/
--rw-r--r--   0 nanw       (501) staff       (20)      654 2023-06-13 19:40:36.000000 hcs-cli-0.1.38/vhcs/common/sglib/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)     4494 2023-07-05 08:39:50.000000 hcs-cli-0.1.38/vhcs/common/sglib/auth.py
--rw-r--r--   0 nanw       (501) staff       (20)     8079 2023-07-05 07:42:49.000000 hcs-cli-0.1.38/vhcs/common/sglib/csp.py
--rw-r--r--   0 nanw       (501) staff       (20)     4823 2023-07-05 08:20:04.000000 hcs-cli-0.1.38/vhcs/common/sglib/ez_client.py
--rw-r--r--   0 nanw       (501) staff       (20)     1013 2023-07-05 08:10:55.000000 hcs-cli-0.1.38/vhcs/common/sglib/hcs_client.py
--rw-r--r--   0 nanw       (501) staff       (20)     8243 2023-07-05 08:11:32.000000 hcs-cli-0.1.38/vhcs/common/sglib/login_support.py
--rw-r--r--   0 nanw       (501) staff       (20)     1307 2023-07-05 07:59:02.000000 hcs-cli-0.1.38/vhcs/common/sglib/util.py
--rw-r--r--   0 nanw       (501) staff       (20)     7955 2023-07-05 06:01:37.000000 hcs-cli-0.1.38/vhcs/common/util.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-05 19:54:20.695320 hcs-cli-0.1.38/vhcs/config/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 02:05:21.000000 hcs-cli-0.1.38/vhcs/config/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)     7771 2023-07-03 22:19:24.000000 hcs-cli-0.1.38/vhcs/config/hcs-deployments.yaml
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-05 19:54:20.701296 hcs-cli-0.1.38/vhcs/plan/
--rw-r--r--   0 nanw       (501) staff       (20)       67 2023-07-05 08:55:37.000000 hcs-cli-0.1.38/vhcs/plan/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)     8453 2023-07-05 19:47:30.000000 hcs-cli-0.1.38/vhcs/plan/core.py
--rw-r--r--   0 nanw       (501) staff       (20)     3864 2023-07-05 15:51:06.000000 hcs-cli-0.1.38/vhcs/plan/dag.py
--rw-r--r--   0 nanw       (501) staff       (20)     4229 2023-06-30 00:23:11.000000 hcs-cli-0.1.38/vhcs/plan/helper.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-05 19:54:20.702456 hcs-cli-0.1.38/vhcs/plan/provider/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-06-28 17:25:18.000000 hcs-cli-0.1.38/vhcs/plan/provider/__init__.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-05 19:54:20.709208 hcs-cli-0.1.38/vhcs/plan/provider/azure/
--rw-r--r--   0 nanw       (501) staff       (20)       29 2023-06-30 00:51:51.000000 hcs-cli-0.1.38/vhcs/plan/provider/azure/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)     3071 2023-06-30 01:10:54.000000 hcs-cli-0.1.38/vhcs/plan/provider/azure/_az_facade.py
--rw-r--r--   0 nanw       (501) staff       (20)      575 2023-06-30 00:26:03.000000 hcs-cli-0.1.38/vhcs/plan/provider/azure/_prepare.py
--rw-r--r--   0 nanw       (501) staff       (20)     1114 2023-06-30 01:27:22.000000 hcs-cli-0.1.38/vhcs/plan/provider/azure/nsg.py
--rw-r--r--   0 nanw       (501) staff       (20)      917 2023-06-29 23:12:33.000000 hcs-cli-0.1.38/vhcs/plan/provider/azure/resource_group.py
--rw-r--r--   0 nanw       (501) staff       (20)     1169 2023-06-30 01:28:00.000000 hcs-cli-0.1.38/vhcs/plan/provider/azure/subnet.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-05 19:54:20.712458 hcs-cli-0.1.38/vhcs/plan/provider/dev/
--rw-r--r--   0 nanw       (501) staff       (20)       29 2023-07-05 15:12:02.000000 hcs-cli-0.1.38/vhcs/plan/provider/dev/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)       33 2023-07-05 15:12:02.000000 hcs-cli-0.1.38/vhcs/plan/provider/dev/_prepare.py
--rw-r--r--   0 nanw       (501) staff       (20)     1074 2023-07-05 18:09:41.000000 hcs-cli-0.1.38/vhcs/plan/provider/dev/dummy.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-05 19:54:20.718696 hcs-cli-0.1.38/vhcs/plan/provider/hcs/
--rw-r--r--   0 nanw       (501) staff       (20)       29 2023-06-29 23:41:13.000000 hcs-cli-0.1.38/vhcs/plan/provider/hcs/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)       33 2023-06-29 23:41:19.000000 hcs-cli-0.1.38/vhcs/plan/provider/hcs/_prepare.py
--rw-r--r--   0 nanw       (501) staff       (20)      705 2023-06-30 00:56:23.000000 hcs-cli-0.1.38/vhcs/plan/provider/hcs/entitlement.py
--rw-r--r--   0 nanw       (501) staff       (20)      705 2023-06-30 00:56:27.000000 hcs-cli-0.1.38/vhcs/plan/provider/hcs/launch_item.py
--rw-r--r--   0 nanw       (501) staff       (20)      705 2023-06-30 00:56:29.000000 hcs-cli-0.1.38/vhcs/plan/provider/hcs/pool_group.py
--rw-r--r--   0 nanw       (501) staff       (20)      714 2023-06-30 00:56:32.000000 hcs-cli-0.1.38/vhcs/plan/provider/hcs/pool_template.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-05 19:54:20.723214 hcs-cli-0.1.38/vhcs/plan/provider/runtime/
--rw-r--r--   0 nanw       (501) staff       (20)       29 2023-06-30 00:29:55.000000 hcs-cli-0.1.38/vhcs/plan/provider/runtime/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)       84 2023-06-30 00:30:09.000000 hcs-cli-0.1.38/vhcs/plan/provider/runtime/_prepare.py
--rw-r--r--   0 nanw       (501) staff       (20)     1919 2023-07-05 08:57:56.000000 hcs-cli-0.1.38/vhcs/plan/provider/runtime/daas_tenant_calculation.py
--rw-r--r--   0 nanw       (501) staff       (20)     1919 2023-07-05 15:10:43.000000 hcs-cli-0.1.38/vhcs/plan/provider/runtime/dummy.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-05 19:54:20.725606 hcs-cli-0.1.38/vhcs/service/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-24 20:24:05.000000 hcs-cli-0.1.38/vhcs/service/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)     1586 2023-06-13 19:40:36.000000 hcs-cli-0.1.38/vhcs/service/_util.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-05 19:54:20.733192 hcs-cli-0.1.38/vhcs/service/admin/
--rw-r--r--   0 nanw       (501) staff       (20)       59 2023-06-27 20:41:57.000000 hcs-cli-0.1.38/vhcs/service/admin/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)     1184 2023-06-27 20:24:06.000000 hcs-cli-0.1.38/vhcs/service/admin/azure_infra.py
--rw-r--r--   0 nanw       (501) staff       (20)      940 2023-06-21 23:40:00.000000 hcs-cli-0.1.38/vhcs/service/admin/edge.py
--rw-r--r--   0 nanw       (501) staff       (20)     1265 2023-06-23 01:29:22.000000 hcs-cli-0.1.38/vhcs/service/admin/helper.py
--rw-r--r--   0 nanw       (501) staff       (20)     1103 2023-06-27 19:44:57.000000 hcs-cli-0.1.38/vhcs/service/admin/provider.py
--rw-r--r--   0 nanw       (501) staff       (20)     1455 2023-06-23 02:28:44.000000 hcs-cli-0.1.38/vhcs/service/admin/template.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-05 19:54:20.736285 hcs-cli-0.1.38/vhcs/service/auth/
--rw-r--r--   0 nanw       (501) staff       (20)       19 2023-06-22 18:49:46.000000 hcs-cli-0.1.38/vhcs/service/auth/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)      851 2023-06-22 18:45:24.000000 hcs-cli-0.1.38/vhcs/service/auth/admin.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-05 19:54:20.740730 hcs-cli-0.1.38/vhcs/service/ims_catalog/
--rw-r--r--   0 nanw       (501) staff       (20)       42 2023-06-27 19:54:19.000000 hcs-cli-0.1.38/vhcs/service/ims_catalog/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)     1218 2023-06-27 20:17:07.000000 hcs-cli-0.1.38/vhcs/service/ims_catalog/helper.py
--rw-r--r--   0 nanw       (501) staff       (20)      915 2023-06-22 15:43:13.000000 hcs-cli-0.1.38/vhcs/service/ims_catalog/image_copies.py
--rw-r--r--   0 nanw       (501) staff       (20)      909 2023-06-22 01:03:55.000000 hcs-cli-0.1.38/vhcs/service/ims_catalog/images.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-05 19:54:20.744015 hcs-cli-0.1.38/vhcs/service/lcm/
--rw-r--r--   0 nanw       (501) staff       (20)       32 2023-06-22 18:49:27.000000 hcs-cli-0.1.38/vhcs/service/lcm/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)     1437 2023-06-22 18:48:08.000000 hcs-cli-0.1.38/vhcs/service/lcm/provider.py
--rw-r--r--   0 nanw       (501) staff       (20)     2770 2023-06-22 18:47:45.000000 hcs-cli-0.1.38/vhcs/service/lcm/template.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-05 19:54:20.747280 hcs-cli-0.1.38/vhcs/service/org_service/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-06-30 15:38:56.000000 hcs-cli-0.1.38/vhcs/service/org_service/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)     1083 2023-06-30 15:37:59.000000 hcs-cli-0.1.38/vhcs/service/org_service/datacenter.py
--rw-r--r--   0 nanw       (501) staff       (20)     1040 2023-06-30 15:37:42.000000 hcs-cli-0.1.38/vhcs/service/org_service/details.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-05 19:54:20.749660 hcs-cli-0.1.38/vhcs/service/pki/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-06-30 15:38:50.000000 hcs-cli-0.1.38/vhcs/service/pki/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)     1211 2023-06-30 15:38:16.000000 hcs-cli-0.1.38/vhcs/service/pki/certificate.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-05 19:54:20.751766 hcs-cli-0.1.38/vhcs/service/portal/
--rw-r--r--   0 nanw       (501) staff       (20)       19 2023-06-28 15:59:32.000000 hcs-cli-0.1.38/vhcs/service/portal/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)      879 2023-06-28 16:01:23.000000 hcs-cli-0.1.38/vhcs/service/portal/pools.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-05 19:54:20.754103 hcs-cli-0.1.38/vhcs/service/vmhub/
--rw-r--r--   0 nanw       (501) staff       (20)       17 2023-07-03 19:03:42.000000 hcs-cli-0.1.38/vhcs/service/vmhub/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)     1406 2023-06-29 21:48:05.000000 hcs-cli-0.1.38/vhcs/service/vmhub/otp.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-05 19:54:20.756887 hcs-cli-0.1.38/vhcs/support/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-06-30 15:35:24.000000 hcs-cli-0.1.38/vhcs/support/__init__.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-05 19:54:20.767938 hcs-cli-0.1.38/vhcs/support/daas/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-06-21 23:10:31.000000 hcs-cli-0.1.38/vhcs/support/daas/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)     8430 2023-07-05 16:09:13.000000 hcs-cli-0.1.38/vhcs/support/daas/deployer.py
--rw-r--r--   0 nanw       (501) staff       (20)     4100 2023-07-05 16:09:49.000000 hcs-cli-0.1.38/vhcs/support/daas/destroyer.py
--rw-r--r--   0 nanw       (501) staff       (20)     1731 2023-06-30 16:55:29.000000 hcs-cli-0.1.38/vhcs/support/daas/helper.py
--rw-r--r--   0 nanw       (501) staff       (20)     1813 2023-06-22 21:16:24.000000 hcs-cli-0.1.38/vhcs/support/daas/infra.py
--rw-r--r--   0 nanw       (501) staff       (20)      242 2023-06-30 18:59:23.000000 hcs-cli-0.1.38/vhcs/support/daas/template.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-05 19:54:20.461000 hcs-cli-0.1.38/vhcs/support/daas/templates/
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-05 19:54:20.773304 hcs-cli-0.1.38/vhcs/support/daas/templates/v1/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-06-30 18:29:22.000000 hcs-cli-0.1.38/vhcs/support/daas/templates/v1/infra.blueprint.yml
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-06-30 18:27:18.000000 hcs-cli-0.1.38/vhcs/support/daas/templates/v1/infra.vars.yml
--rw-r--r--   0 nanw       (501) staff       (20)     1556 2023-07-05 18:16:30.000000 hcs-cli-0.1.38/vhcs/support/daas/templates/v1/tenant.blueprint.yml
--rw-r--r--   0 nanw       (501) staff       (20)      240 2023-07-05 18:16:48.000000 hcs-cli-0.1.38/vhcs/support/daas/templates/v1/tenant.vars.yml
--rw-r--r--   0 nanw       (501) staff       (20)     1979 2023-06-22 21:16:18.000000 hcs-cli-0.1.38/vhcs/support/daas/tenant.py
--rw-r--r--   0 nanw       (501) staff       (20)     2621 2023-07-05 07:42:08.000000 hcs-cli-0.1.38/vhcs/support/profile.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-05 19:54:20.780091 hcs-cli-0.1.38/vhcs/util/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 02:05:21.000000 hcs-cli-0.1.38/vhcs/util/__init__.py
--rwxr-xr-x   0 nanw       (501) staff       (20)     2535 2023-06-13 19:40:36.000000 hcs-cli-0.1.38/vhcs/util/check_license.py
--rw-r--r--   0 nanw       (501) staff       (20)     2759 2023-06-13 19:40:36.000000 hcs-cli-0.1.38/vhcs/util/duration.py
--rw-r--r--   0 nanw       (501) staff       (20)     5288 2023-06-13 19:40:36.000000 hcs-cli-0.1.38/vhcs/util/pki_util.py
--rw-r--r--   0 nanw       (501) staff       (20)     1819 2023-06-22 01:50:10.000000 hcs-cli-0.1.38/vhcs/util/query_util.py
--rw-r--r--   0 nanw       (501) staff       (20)     1725 2023-06-13 19:40:36.000000 hcs-cli-0.1.38/vhcs/util/versions.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-05 19:55:45.844931 hcs-cli-0.1.39/
+-rw-r--r--   0 nanw       (501) staff       (20)     2824 2023-06-21 18:44:48.000000 hcs-cli-0.1.39/.gitignore
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-05 19:55:45.595653 hcs-cli-0.1.39/.vscode/
+-rw-r--r--   0 nanw       (501) staff       (20)     2564 2023-07-05 08:21:14.000000 hcs-cli-0.1.39/.vscode/launch.json
+-rw-r--r--   0 nanw       (501) staff       (20)       49 2023-06-30 00:59:55.000000 hcs-cli-0.1.39/.vscode/settings.json
+-rw-r--r--   0 nanw       (501) staff       (20)       98 2023-06-13 19:57:56.000000 hcs-cli-0.1.39/CHANGELOG.md
+-rw-r--r--   0 nanw       (501) staff       (20)     5258 2023-06-13 16:45:49.000000 hcs-cli-0.1.39/CODE_OF_CONDUCT.md
+-rw-r--r--   0 nanw       (501) staff       (20)     2706 2023-06-13 18:53:18.000000 hcs-cli-0.1.39/CONTRIBUTING_CLA.md
+-rw-r--r--   0 nanw       (501) staff       (20)     6095 2023-04-25 23:13:27.000000 hcs-cli-0.1.39/GOVERNANCE.md
+-rw-r--r--   0 nanw       (501) staff       (20)    10449 2023-06-13 16:45:49.000000 hcs-cli-0.1.39/LICENSE
+-rw-r--r--   0 nanw       (501) staff       (20)      854 2023-07-03 19:19:46.000000 hcs-cli-0.1.39/Makefile
+-rw-r--r--   0 nanw       (501) staff       (20)      411 2023-06-13 16:45:49.000000 hcs-cli-0.1.39/NOTICE
+-rw-r--r--   0 nanw       (501) staff       (20)     2516 2023-07-05 19:55:45.844075 hcs-cli-0.1.39/PKG-INFO
+-rw-r--r--   0 nanw       (501) staff       (20)     1642 2023-06-24 01:22:59.000000 hcs-cli-0.1.39/README.md
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-05 19:55:45.600866 hcs-cli-0.1.39/doc/
+-rw-r--r--   0 nanw       (501) staff       (20)     5950 2023-06-15 17:50:47.000000 hcs-cli-0.1.39/doc/dev-setup.md
+-rw-r--r--   0 nanw       (501) staff       (20)      763 2023-06-13 17:49:20.000000 hcs-cli-0.1.39/doc/get-csp-user-api-token.md
+-rw-r--r--   0 nanw       (501) staff       (20)     6394 2023-07-03 19:03:00.000000 hcs-cli-0.1.39/doc/hcs-cli-cheatsheet.md
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-05 19:55:45.607914 hcs-cli-0.1.39/hcs_cli.egg-info/
+-rw-r--r--   0 nanw       (501) staff       (20)     2516 2023-07-05 19:55:45.000000 hcs-cli-0.1.39/hcs_cli.egg-info/PKG-INFO
+-rw-r--r--   0 nanw       (501) staff       (20)     5934 2023-07-05 19:55:45.000000 hcs-cli-0.1.39/hcs_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 nanw       (501) staff       (20)        1 2023-07-05 19:55:45.000000 hcs-cli-0.1.39/hcs_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 nanw       (501) staff       (20)       43 2023-07-05 19:55:45.000000 hcs-cli-0.1.39/hcs_cli.egg-info/entry_points.txt
+-rw-r--r--   0 nanw       (501) staff       (20)      136 2023-07-05 19:55:45.000000 hcs-cli-0.1.39/hcs_cli.egg-info/requires.txt
+-rw-r--r--   0 nanw       (501) staff       (20)       11 2023-07-05 19:55:45.000000 hcs-cli-0.1.39/hcs_cli.egg-info/top_level.txt
+-rw-r--r--   0 nanw       (501) staff       (20)       92 2023-04-24 20:24:05.000000 hcs-cli-0.1.39/mypy.ini
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-05 19:55:45.536355 hcs-cli-0.1.39/payload/
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-05 19:55:45.609095 hcs-cli-0.1.39/payload/lcm/
+-rw-r--r--   0 nanw       (501) staff       (20)      752 2023-04-24 20:24:05.000000 hcs-cli-0.1.39/payload/lcm/zero.json
+-rw-r--r--   0 nanw       (501) staff       (20)     1187 2023-06-13 19:56:09.000000 hcs-cli-0.1.39/pyproject.toml
+-rw-r--r--   0 nanw       (501) staff       (20)      194 2023-04-24 20:24:05.000000 hcs-cli-0.1.39/requirements-dev.txt
+-rw-r--r--   0 nanw       (501) staff       (20)      136 2023-07-05 19:55:05.000000 hcs-cli-0.1.39/requirements.txt
+-rw-r--r--   0 nanw       (501) staff       (20)       38 2023-07-05 19:55:45.845117 hcs-cli-0.1.39/setup.cfg
+-rw-r--r--   0 nanw       (501) staff       (20)     1154 2023-07-05 19:55:41.000000 hcs-cli-0.1.39/setup.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-05 19:55:45.612228 hcs-cli-0.1.39/tests/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-24 20:24:05.000000 hcs-cli-0.1.39/tests/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)      599 2023-06-13 19:40:36.000000 hcs-cli-0.1.39/tests/conftest.py
+-rw-r--r--   0 nanw       (501) staff       (20)     3364 2023-07-05 16:02:01.000000 hcs-cli-0.1.39/tests/test_utils.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-05 19:55:45.613511 hcs-cli-0.1.39/tests/vhcs/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-24 20:24:05.000000 hcs-cli-0.1.39/tests/vhcs/__init__.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-05 19:55:45.614694 hcs-cli-0.1.39/tests/vhcs/cli/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-24 20:24:05.000000 hcs-cli-0.1.39/tests/vhcs/cli/__init__.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-05 19:55:45.620228 hcs-cli-0.1.39/tests/vhcs/cli/cmds/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-24 20:24:05.000000 hcs-cli-0.1.39/tests/vhcs/cli/cmds/__init__.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-05 19:55:45.623650 hcs-cli-0.1.39/tests/vhcs/cli/cmds/pki/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-24 20:24:05.000000 hcs-cli-0.1.39/tests/vhcs/cli/cmds/pki/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)      599 2023-06-13 19:40:36.000000 hcs-cli-0.1.39/tests/vhcs/cli/cmds/pki/get_root_ca.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-05 19:55:45.625939 hcs-cli-0.1.39/tests/vhcs/cli/cmds/plan/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-07-05 15:13:25.000000 hcs-cli-0.1.39/tests/vhcs/cli/cmds/plan/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     6151 2023-07-05 19:50:01.000000 hcs-cli-0.1.39/tests/vhcs/cli/cmds/plan/test_plan.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1943 2023-06-13 19:40:36.000000 hcs-cli-0.1.39/tests/vhcs/cli/cmds/test_context.py
+-rw-r--r--   0 nanw       (501) staff       (20)      918 2023-07-03 19:18:10.000000 hcs-cli-0.1.39/tests/vhcs/cli/cmds/test_login.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1151 2023-07-05 08:29:47.000000 hcs-cli-0.1.39/tests/vhcs/cli/cmds/test_profile.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-05 19:55:45.629672 hcs-cli-0.1.39/vhcs/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 21:25:27.000000 hcs-cli-0.1.39/vhcs/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)      687 2023-06-13 19:40:36.000000 hcs-cli-0.1.39/vhcs/__main__.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-05 19:55:45.632296 hcs-cli-0.1.39/vhcs/cli/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 02:05:21.000000 hcs-cli-0.1.39/vhcs/cli/__init__.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-05 19:55:45.636613 hcs-cli-0.1.39/vhcs/cli/cmds/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 02:05:21.000000 hcs-cli-0.1.39/vhcs/cli/cmds/__init__.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-05 19:55:45.637690 hcs-cli-0.1.39/vhcs/cli/cmds/admin/
+-rw-r--r--   0 nanw       (501) staff       (20)      633 2023-06-13 19:40:36.000000 hcs-cli-0.1.39/vhcs/cli/cmds/admin/__init__.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-05 19:55:45.638807 hcs-cli-0.1.39/vhcs/cli/cmds/admin/azure-infra/
+-rw-r--r--   0 nanw       (501) staff       (20)     1069 2023-06-27 20:44:31.000000 hcs-cli-0.1.39/vhcs/cli/cmds/admin/azure-infra/main.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-05 19:55:45.642246 hcs-cli-0.1.39/vhcs/cli/cmds/admin/edge/
+-rw-r--r--   0 nanw       (501) staff       (20)      628 2023-06-13 19:40:36.000000 hcs-cli-0.1.39/vhcs/cli/cmds/admin/edge/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)      941 2023-06-13 19:40:36.000000 hcs-cli-0.1.39/vhcs/cli/cmds/admin/edge/get.py
+-rw-r--r--   0 nanw       (501) staff       (20)      599 2023-06-13 19:40:36.000000 hcs-cli-0.1.39/vhcs/cli/cmds/admin/edge/list.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-05 19:55:45.643318 hcs-cli-0.1.39/vhcs/cli/cmds/admin/provider/
+-rw-r--r--   0 nanw       (501) staff       (20)     1136 2023-06-15 22:34:38.000000 hcs-cli-0.1.39/vhcs/cli/cmds/admin/provider/list.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-05 19:55:45.646619 hcs-cli-0.1.39/vhcs/cli/cmds/admin/template/
+-rw-r--r--   0 nanw       (501) staff       (20)      628 2023-06-13 19:40:36.000000 hcs-cli-0.1.39/vhcs/cli/cmds/admin/template/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)      949 2023-06-13 19:40:36.000000 hcs-cli-0.1.39/vhcs/cli/cmds/admin/template/get.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1841 2023-06-23 17:01:30.000000 hcs-cli-0.1.39/vhcs/cli/cmds/admin/template/list.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-05 19:55:45.647874 hcs-cli-0.1.39/vhcs/cli/cmds/daas/
+-rw-r--r--   0 nanw       (501) staff       (20)      642 2023-06-15 22:15:00.000000 hcs-cli-0.1.39/vhcs/cli/cmds/daas/__init__.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-05 19:55:45.655028 hcs-cli-0.1.39/vhcs/cli/cmds/daas/infra/
+-rw-r--r--   0 nanw       (501) staff       (20)      648 2023-06-21 17:56:47.000000 hcs-cli-0.1.39/vhcs/cli/cmds/daas/infra/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1041 2023-06-30 16:52:44.000000 hcs-cli-0.1.39/vhcs/cli/cmds/daas/infra/basic.py
+-rw-r--r--   0 nanw       (501) staff       (20)     2335 2023-07-05 08:38:57.000000 hcs-cli-0.1.39/vhcs/cli/cmds/daas/infra/plan.py
+-rw-r--r--   0 nanw       (501) staff       (20)      745 2023-06-21 18:14:23.000000 hcs-cli-0.1.39/vhcs/cli/cmds/daas/infra/validate.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-05 19:55:45.660823 hcs-cli-0.1.39/vhcs/cli/cmds/daas/tenant/
+-rw-r--r--   0 nanw       (501) staff       (20)      633 2023-06-21 17:36:22.000000 hcs-cli-0.1.39/vhcs/cli/cmds/daas/tenant/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)      963 2023-06-30 16:57:41.000000 hcs-cli-0.1.39/vhcs/cli/cmds/daas/tenant/basic.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1022 2023-07-05 16:13:46.000000 hcs-cli-0.1.39/vhcs/cli/cmds/daas/tenant/deploy.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1378 2023-07-05 16:11:32.000000 hcs-cli-0.1.39/vhcs/cli/cmds/daas/tenant/destroy.py
+-rw-r--r--   0 nanw       (501) staff       (20)     4991 2023-07-05 18:15:55.000000 hcs-cli-0.1.39/vhcs/cli/cmds/daas/tenant/plan.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-05 19:55:45.664423 hcs-cli-0.1.39/vhcs/cli/cmds/ims/
+-rw-r--r--   0 nanw       (501) staff       (20)      633 2023-06-27 19:52:41.000000 hcs-cli-0.1.39/vhcs/cli/cmds/ims/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)      915 2023-06-27 19:56:58.000000 hcs-cli-0.1.39/vhcs/cli/cmds/ims/list.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1033 2023-06-27 20:14:16.000000 hcs-cli-0.1.39/vhcs/cli/cmds/ims/list_copies.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-05 19:55:45.665645 hcs-cli-0.1.39/vhcs/cli/cmds/lcm/
+-rw-r--r--   0 nanw       (501) staff       (20)      631 2023-06-27 19:52:37.000000 hcs-cli-0.1.39/vhcs/cli/cmds/lcm/__init__.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-05 19:55:45.670575 hcs-cli-0.1.39/vhcs/cli/cmds/lcm/provider/
+-rw-r--r--   0 nanw       (501) staff       (20)      628 2023-06-13 19:40:36.000000 hcs-cli-0.1.39/vhcs/cli/cmds/lcm/provider/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)      801 2023-06-23 02:35:21.000000 hcs-cli-0.1.39/vhcs/cli/cmds/lcm/provider/delete.py
+-rw-r--r--   0 nanw       (501) staff       (20)      792 2023-06-23 02:35:30.000000 hcs-cli-0.1.39/vhcs/cli/cmds/lcm/provider/get.py
+-rw-r--r--   0 nanw       (501) staff       (20)      987 2023-06-23 02:35:40.000000 hcs-cli-0.1.39/vhcs/cli/cmds/lcm/provider/list.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-05 19:55:45.679381 hcs-cli-0.1.39/vhcs/cli/cmds/lcm/template/
+-rw-r--r--   0 nanw       (501) staff       (20)      628 2023-06-13 19:40:36.000000 hcs-cli-0.1.39/vhcs/cli/cmds/lcm/template/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1857 2023-06-23 02:36:50.000000 hcs-cli-0.1.39/vhcs/cli/cmds/lcm/template/create.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1079 2023-06-23 02:36:58.000000 hcs-cli-0.1.39/vhcs/cli/cmds/lcm/template/delete.py
+-rw-r--r--   0 nanw       (501) staff       (20)      840 2023-06-23 02:37:07.000000 hcs-cli-0.1.39/vhcs/cli/cmds/lcm/template/get.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1588 2023-06-23 02:37:18.000000 hcs-cli-0.1.39/vhcs/cli/cmds/lcm/template/list.py
+-rw-r--r--   0 nanw       (501) staff       (20)     2256 2023-06-23 02:37:44.000000 hcs-cli-0.1.39/vhcs/cli/cmds/lcm/template/wait.py
+-rw-r--r--   0 nanw       (501) staff       (20)     6631 2023-07-05 07:47:22.000000 hcs-cli-0.1.39/vhcs/cli/cmds/login.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-05 19:55:45.549958 hcs-cli-0.1.39/vhcs/cli/cmds/org/
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-05 19:55:45.682331 hcs-cli-0.1.39/vhcs/cli/cmds/org/datacenter/
+-rw-r--r--   0 nanw       (501) staff       (20)      848 2023-06-30 15:40:06.000000 hcs-cli-0.1.39/vhcs/cli/cmds/org/datacenter/get.py
+-rw-r--r--   0 nanw       (501) staff       (20)      997 2023-06-30 15:40:15.000000 hcs-cli-0.1.39/vhcs/cli/cmds/org/datacenter/list.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-05 19:55:45.686162 hcs-cli-0.1.39/vhcs/cli/cmds/org/detail/
+-rw-r--r--   0 nanw       (501) staff       (20)      906 2023-06-30 15:40:19.000000 hcs-cli-0.1.39/vhcs/cli/cmds/org/detail/get.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1201 2023-06-30 15:40:25.000000 hcs-cli-0.1.39/vhcs/cli/cmds/org/detail/list.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-05 19:55:45.694204 hcs-cli-0.1.39/vhcs/cli/cmds/pki/
+-rw-r--r--   0 nanw       (501) staff       (20)      631 2023-06-13 19:45:45.000000 hcs-cli-0.1.39/vhcs/cli/cmds/pki/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1155 2023-06-30 15:38:40.000000 hcs-cli-0.1.39/vhcs/cli/cmds/pki/delete_org_cert.py
+-rw-r--r--   0 nanw       (501) staff       (20)      906 2023-06-30 15:38:40.000000 hcs-cli-0.1.39/vhcs/cli/cmds/pki/get_org_cert.py
+-rw-r--r--   0 nanw       (501) staff       (20)      775 2023-06-30 15:38:40.000000 hcs-cli-0.1.39/vhcs/cli/cmds/pki/get_root_ca.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1804 2023-06-30 15:38:40.000000 hcs-cli-0.1.39/vhcs/cli/cmds/pki/sign_resource_cert.py
+-rw-r--r--   0 nanw       (501) staff       (20)      726 2023-06-30 15:38:40.000000 hcs-cli-0.1.39/vhcs/cli/cmds/pki/test.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-05 19:55:45.698048 hcs-cli-0.1.39/vhcs/cli/cmds/plan/
+-rw-r--r--   0 nanw       (501) staff       (20)      665 2023-06-28 17:52:44.000000 hcs-cli-0.1.39/vhcs/cli/cmds/plan/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1745 2023-07-05 16:15:40.000000 hcs-cli-0.1.39/vhcs/cli/cmds/plan/deploy.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1328 2023-07-05 16:15:58.000000 hcs-cli-0.1.39/vhcs/cli/cmds/plan/destroy.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-05 19:55:45.700772 hcs-cli-0.1.39/vhcs/cli/cmds/profile/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 02:05:21.000000 hcs-cli-0.1.39/vhcs/cli/cmds/profile/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1765 2023-07-05 06:16:00.000000 hcs-cli-0.1.39/vhcs/cli/cmds/profile/init.py
+-rw-r--r--   0 nanw       (501) staff       (20)      932 2023-06-13 19:40:36.000000 hcs-cli-0.1.39/vhcs/cli/cmds/upgrade.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-05 19:55:45.702381 hcs-cli-0.1.39/vhcs/cli/cmds/vmhub/
+-rw-r--r--   0 nanw       (501) staff       (20)      633 2023-06-13 19:40:36.000000 hcs-cli-0.1.39/vhcs/cli/cmds/vmhub/__init__.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-05 19:55:45.707056 hcs-cli-0.1.39/vhcs/cli/cmds/vmhub/otp/
+-rw-r--r--   0 nanw       (501) staff       (20)      643 2023-06-29 21:49:43.000000 hcs-cli-0.1.39/vhcs/cli/cmds/vmhub/otp/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1234 2023-06-29 21:49:20.000000 hcs-cli-0.1.39/vhcs/cli/cmds/vmhub/otp/redeem.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1143 2023-06-29 21:49:25.000000 hcs-cli-0.1.39/vhcs/cli/cmds/vmhub/otp/request.py
+-rwxr-xr-x   0 nanw       (501) staff       (20)     2865 2023-06-23 02:40:39.000000 hcs-cli-0.1.39/vhcs/cli/main.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-05 19:55:45.711620 hcs-cli-0.1.39/vhcs/common/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 02:05:21.000000 hcs-cli-0.1.39/vhcs/common/__init__.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-05 19:55:45.732246 hcs-cli-0.1.39/vhcs/common/ctxp/
+-rw-r--r--   0 nanw       (501) staff       (20)     1538 2023-07-03 20:20:16.000000 hcs-cli-0.1.39/vhcs/common/ctxp/README.md
+-rw-r--r--   0 nanw       (501) staff       (20)      790 2023-07-03 20:45:37.000000 hcs-cli-0.1.39/vhcs/common/ctxp/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1155 2023-07-03 21:18:13.000000 hcs-cli-0.1.39/vhcs/common/ctxp/_init.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-05 19:55:45.736089 hcs-cli-0.1.39/vhcs/common/ctxp/built_in_cmds/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 02:05:21.000000 hcs-cli-0.1.39/vhcs/common/ctxp/built_in_cmds/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     2421 2023-06-21 17:26:56.000000 hcs-cli-0.1.39/vhcs/common/ctxp/built_in_cmds/context.py
+-rw-r--r--   0 nanw       (501) staff       (20)     3977 2023-07-05 08:26:35.000000 hcs-cli-0.1.39/vhcs/common/ctxp/built_in_cmds/profile.py
+-rw-r--r--   0 nanw       (501) staff       (20)     5129 2023-07-05 06:22:51.000000 hcs-cli-0.1.39/vhcs/common/ctxp/cli_processor.py
+-rw-r--r--   0 nanw       (501) staff       (20)      936 2023-07-03 21:17:12.000000 hcs-cli-0.1.39/vhcs/common/ctxp/config.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1205 2023-07-03 21:08:50.000000 hcs-cli-0.1.39/vhcs/common/ctxp/context.py
+-rw-r--r--   0 nanw       (501) staff       (20)     6467 2023-06-23 00:26:19.000000 hcs-cli-0.1.39/vhcs/common/ctxp/fstore.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1200 2023-06-13 19:40:36.000000 hcs-cli-0.1.39/vhcs/common/ctxp/init.py
+-rw-r--r--   0 nanw       (501) staff       (20)     2776 2023-06-22 22:58:23.000000 hcs-cli-0.1.39/vhcs/common/ctxp/jsondot.py
+-rw-r--r--   0 nanw       (501) staff       (20)     5163 2023-07-05 08:33:15.000000 hcs-cli-0.1.39/vhcs/common/ctxp/profile.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1565 2023-07-05 06:52:28.000000 hcs-cli-0.1.39/vhcs/common/ctxp/profile_store.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1604 2023-07-03 22:06:25.000000 hcs-cli-0.1.39/vhcs/common/ctxp/state.py
+-rw-r--r--   0 nanw       (501) staff       (20)     6258 2023-07-05 06:26:16.000000 hcs-cli-0.1.39/vhcs/common/ctxp/util.py
+-rw-r--r--   0 nanw       (501) staff       (20)     3256 2023-06-13 19:40:36.000000 hcs-cli-0.1.39/vhcs/common/ctxp/var_template.py
+-rw-r--r--   0 nanw       (501) staff       (20)     2259 2023-07-05 18:05:17.000000 hcs-cli-0.1.39/vhcs/common/duration.py
+-rw-r--r--   0 nanw       (501) staff       (20)     4846 2023-06-13 19:40:36.000000 hcs-cli-0.1.39/vhcs/common/logger.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-05 19:55:45.746705 hcs-cli-0.1.39/vhcs/common/sglib/
+-rw-r--r--   0 nanw       (501) staff       (20)      654 2023-06-13 19:40:36.000000 hcs-cli-0.1.39/vhcs/common/sglib/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     4494 2023-07-05 08:39:50.000000 hcs-cli-0.1.39/vhcs/common/sglib/auth.py
+-rw-r--r--   0 nanw       (501) staff       (20)     8079 2023-07-05 07:42:49.000000 hcs-cli-0.1.39/vhcs/common/sglib/csp.py
+-rw-r--r--   0 nanw       (501) staff       (20)     4823 2023-07-05 08:20:04.000000 hcs-cli-0.1.39/vhcs/common/sglib/ez_client.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1013 2023-07-05 08:10:55.000000 hcs-cli-0.1.39/vhcs/common/sglib/hcs_client.py
+-rw-r--r--   0 nanw       (501) staff       (20)     8243 2023-07-05 08:11:32.000000 hcs-cli-0.1.39/vhcs/common/sglib/login_support.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1307 2023-07-05 07:59:02.000000 hcs-cli-0.1.39/vhcs/common/sglib/util.py
+-rw-r--r--   0 nanw       (501) staff       (20)     7955 2023-07-05 06:01:37.000000 hcs-cli-0.1.39/vhcs/common/util.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-05 19:55:45.750176 hcs-cli-0.1.39/vhcs/config/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 02:05:21.000000 hcs-cli-0.1.39/vhcs/config/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     7771 2023-07-03 22:19:24.000000 hcs-cli-0.1.39/vhcs/config/hcs-deployments.yaml
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-05 19:55:45.759543 hcs-cli-0.1.39/vhcs/plan/
+-rw-r--r--   0 nanw       (501) staff       (20)       67 2023-07-05 08:55:37.000000 hcs-cli-0.1.39/vhcs/plan/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     8453 2023-07-05 19:47:30.000000 hcs-cli-0.1.39/vhcs/plan/core.py
+-rw-r--r--   0 nanw       (501) staff       (20)     3864 2023-07-05 15:51:06.000000 hcs-cli-0.1.39/vhcs/plan/dag.py
+-rw-r--r--   0 nanw       (501) staff       (20)     4229 2023-06-30 00:23:11.000000 hcs-cli-0.1.39/vhcs/plan/helper.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-05 19:55:45.760882 hcs-cli-0.1.39/vhcs/plan/provider/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-06-28 17:25:18.000000 hcs-cli-0.1.39/vhcs/plan/provider/__init__.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-05 19:55:45.768315 hcs-cli-0.1.39/vhcs/plan/provider/azure/
+-rw-r--r--   0 nanw       (501) staff       (20)       29 2023-06-30 00:51:51.000000 hcs-cli-0.1.39/vhcs/plan/provider/azure/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     3071 2023-06-30 01:10:54.000000 hcs-cli-0.1.39/vhcs/plan/provider/azure/_az_facade.py
+-rw-r--r--   0 nanw       (501) staff       (20)      575 2023-06-30 00:26:03.000000 hcs-cli-0.1.39/vhcs/plan/provider/azure/_prepare.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1114 2023-06-30 01:27:22.000000 hcs-cli-0.1.39/vhcs/plan/provider/azure/nsg.py
+-rw-r--r--   0 nanw       (501) staff       (20)      917 2023-06-29 23:12:33.000000 hcs-cli-0.1.39/vhcs/plan/provider/azure/resource_group.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1169 2023-06-30 01:28:00.000000 hcs-cli-0.1.39/vhcs/plan/provider/azure/subnet.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-05 19:55:45.771819 hcs-cli-0.1.39/vhcs/plan/provider/dev/
+-rw-r--r--   0 nanw       (501) staff       (20)       29 2023-07-05 15:12:02.000000 hcs-cli-0.1.39/vhcs/plan/provider/dev/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)       33 2023-07-05 15:12:02.000000 hcs-cli-0.1.39/vhcs/plan/provider/dev/_prepare.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1074 2023-07-05 18:09:41.000000 hcs-cli-0.1.39/vhcs/plan/provider/dev/dummy.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-05 19:55:45.779410 hcs-cli-0.1.39/vhcs/plan/provider/hcs/
+-rw-r--r--   0 nanw       (501) staff       (20)       29 2023-06-29 23:41:13.000000 hcs-cli-0.1.39/vhcs/plan/provider/hcs/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)       33 2023-06-29 23:41:19.000000 hcs-cli-0.1.39/vhcs/plan/provider/hcs/_prepare.py
+-rw-r--r--   0 nanw       (501) staff       (20)      705 2023-06-30 00:56:23.000000 hcs-cli-0.1.39/vhcs/plan/provider/hcs/entitlement.py
+-rw-r--r--   0 nanw       (501) staff       (20)      705 2023-06-30 00:56:27.000000 hcs-cli-0.1.39/vhcs/plan/provider/hcs/launch_item.py
+-rw-r--r--   0 nanw       (501) staff       (20)      705 2023-06-30 00:56:29.000000 hcs-cli-0.1.39/vhcs/plan/provider/hcs/pool_group.py
+-rw-r--r--   0 nanw       (501) staff       (20)      714 2023-06-30 00:56:32.000000 hcs-cli-0.1.39/vhcs/plan/provider/hcs/pool_template.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-05 19:55:45.785010 hcs-cli-0.1.39/vhcs/plan/provider/runtime/
+-rw-r--r--   0 nanw       (501) staff       (20)       29 2023-06-30 00:29:55.000000 hcs-cli-0.1.39/vhcs/plan/provider/runtime/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)       84 2023-06-30 00:30:09.000000 hcs-cli-0.1.39/vhcs/plan/provider/runtime/_prepare.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1919 2023-07-05 08:57:56.000000 hcs-cli-0.1.39/vhcs/plan/provider/runtime/daas_tenant_calculation.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1919 2023-07-05 15:10:43.000000 hcs-cli-0.1.39/vhcs/plan/provider/runtime/dummy.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-05 19:55:45.788689 hcs-cli-0.1.39/vhcs/service/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-24 20:24:05.000000 hcs-cli-0.1.39/vhcs/service/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1586 2023-06-13 19:40:36.000000 hcs-cli-0.1.39/vhcs/service/_util.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-05 19:55:45.796045 hcs-cli-0.1.39/vhcs/service/admin/
+-rw-r--r--   0 nanw       (501) staff       (20)       59 2023-06-27 20:41:57.000000 hcs-cli-0.1.39/vhcs/service/admin/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1184 2023-06-27 20:24:06.000000 hcs-cli-0.1.39/vhcs/service/admin/azure_infra.py
+-rw-r--r--   0 nanw       (501) staff       (20)      940 2023-06-21 23:40:00.000000 hcs-cli-0.1.39/vhcs/service/admin/edge.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1265 2023-06-23 01:29:22.000000 hcs-cli-0.1.39/vhcs/service/admin/helper.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1103 2023-06-27 19:44:57.000000 hcs-cli-0.1.39/vhcs/service/admin/provider.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1455 2023-06-23 02:28:44.000000 hcs-cli-0.1.39/vhcs/service/admin/template.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-05 19:55:45.798252 hcs-cli-0.1.39/vhcs/service/auth/
+-rw-r--r--   0 nanw       (501) staff       (20)       19 2023-06-22 18:49:46.000000 hcs-cli-0.1.39/vhcs/service/auth/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)      851 2023-06-22 18:45:24.000000 hcs-cli-0.1.39/vhcs/service/auth/admin.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-05 19:55:45.802604 hcs-cli-0.1.39/vhcs/service/ims_catalog/
+-rw-r--r--   0 nanw       (501) staff       (20)       42 2023-06-27 19:54:19.000000 hcs-cli-0.1.39/vhcs/service/ims_catalog/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1218 2023-06-27 20:17:07.000000 hcs-cli-0.1.39/vhcs/service/ims_catalog/helper.py
+-rw-r--r--   0 nanw       (501) staff       (20)      915 2023-06-22 15:43:13.000000 hcs-cli-0.1.39/vhcs/service/ims_catalog/image_copies.py
+-rw-r--r--   0 nanw       (501) staff       (20)      909 2023-06-22 01:03:55.000000 hcs-cli-0.1.39/vhcs/service/ims_catalog/images.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-05 19:55:45.805901 hcs-cli-0.1.39/vhcs/service/lcm/
+-rw-r--r--   0 nanw       (501) staff       (20)       32 2023-06-22 18:49:27.000000 hcs-cli-0.1.39/vhcs/service/lcm/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1437 2023-06-22 18:48:08.000000 hcs-cli-0.1.39/vhcs/service/lcm/provider.py
+-rw-r--r--   0 nanw       (501) staff       (20)     2770 2023-06-22 18:47:45.000000 hcs-cli-0.1.39/vhcs/service/lcm/template.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-05 19:55:45.810166 hcs-cli-0.1.39/vhcs/service/org_service/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-06-30 15:38:56.000000 hcs-cli-0.1.39/vhcs/service/org_service/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1083 2023-06-30 15:37:59.000000 hcs-cli-0.1.39/vhcs/service/org_service/datacenter.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1040 2023-06-30 15:37:42.000000 hcs-cli-0.1.39/vhcs/service/org_service/details.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-05 19:55:45.812566 hcs-cli-0.1.39/vhcs/service/pki/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-06-30 15:38:50.000000 hcs-cli-0.1.39/vhcs/service/pki/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1211 2023-06-30 15:38:16.000000 hcs-cli-0.1.39/vhcs/service/pki/certificate.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-05 19:55:45.815107 hcs-cli-0.1.39/vhcs/service/portal/
+-rw-r--r--   0 nanw       (501) staff       (20)       19 2023-06-28 15:59:32.000000 hcs-cli-0.1.39/vhcs/service/portal/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)      879 2023-06-28 16:01:23.000000 hcs-cli-0.1.39/vhcs/service/portal/pools.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-05 19:55:45.817638 hcs-cli-0.1.39/vhcs/service/vmhub/
+-rw-r--r--   0 nanw       (501) staff       (20)       17 2023-07-03 19:03:42.000000 hcs-cli-0.1.39/vhcs/service/vmhub/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1406 2023-06-29 21:48:05.000000 hcs-cli-0.1.39/vhcs/service/vmhub/otp.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-05 19:55:45.821144 hcs-cli-0.1.39/vhcs/support/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-06-30 15:35:24.000000 hcs-cli-0.1.39/vhcs/support/__init__.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-05 19:55:45.831392 hcs-cli-0.1.39/vhcs/support/daas/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-06-21 23:10:31.000000 hcs-cli-0.1.39/vhcs/support/daas/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     8430 2023-07-05 16:09:13.000000 hcs-cli-0.1.39/vhcs/support/daas/deployer.py
+-rw-r--r--   0 nanw       (501) staff       (20)     4100 2023-07-05 16:09:49.000000 hcs-cli-0.1.39/vhcs/support/daas/destroyer.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1731 2023-06-30 16:55:29.000000 hcs-cli-0.1.39/vhcs/support/daas/helper.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1813 2023-06-22 21:16:24.000000 hcs-cli-0.1.39/vhcs/support/daas/infra.py
+-rw-r--r--   0 nanw       (501) staff       (20)      242 2023-06-30 18:59:23.000000 hcs-cli-0.1.39/vhcs/support/daas/template.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-05 19:55:45.573301 hcs-cli-0.1.39/vhcs/support/daas/templates/
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-05 19:55:45.836554 hcs-cli-0.1.39/vhcs/support/daas/templates/v1/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-06-30 18:29:22.000000 hcs-cli-0.1.39/vhcs/support/daas/templates/v1/infra.blueprint.yml
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-06-30 18:27:18.000000 hcs-cli-0.1.39/vhcs/support/daas/templates/v1/infra.vars.yml
+-rw-r--r--   0 nanw       (501) staff       (20)     1556 2023-07-05 18:16:30.000000 hcs-cli-0.1.39/vhcs/support/daas/templates/v1/tenant.blueprint.yml
+-rw-r--r--   0 nanw       (501) staff       (20)      240 2023-07-05 18:16:48.000000 hcs-cli-0.1.39/vhcs/support/daas/templates/v1/tenant.vars.yml
+-rw-r--r--   0 nanw       (501) staff       (20)     1979 2023-06-22 21:16:18.000000 hcs-cli-0.1.39/vhcs/support/daas/tenant.py
+-rw-r--r--   0 nanw       (501) staff       (20)     2621 2023-07-05 07:42:08.000000 hcs-cli-0.1.39/vhcs/support/profile.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-05 19:55:45.842762 hcs-cli-0.1.39/vhcs/util/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 02:05:21.000000 hcs-cli-0.1.39/vhcs/util/__init__.py
+-rwxr-xr-x   0 nanw       (501) staff       (20)     2535 2023-06-13 19:40:36.000000 hcs-cli-0.1.39/vhcs/util/check_license.py
+-rw-r--r--   0 nanw       (501) staff       (20)     2759 2023-06-13 19:40:36.000000 hcs-cli-0.1.39/vhcs/util/duration.py
+-rw-r--r--   0 nanw       (501) staff       (20)     5288 2023-06-13 19:40:36.000000 hcs-cli-0.1.39/vhcs/util/pki_util.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1819 2023-06-22 01:50:10.000000 hcs-cli-0.1.39/vhcs/util/query_util.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1725 2023-06-13 19:40:36.000000 hcs-cli-0.1.39/vhcs/util/versions.py
```

### Comparing `hcs-cli-0.1.38/.gitignore` & `hcs-cli-0.1.39/.gitignore`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.38/.vscode/launch.json` & `hcs-cli-0.1.39/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.38/CODE_OF_CONDUCT.md` & `hcs-cli-0.1.39/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.38/CONTRIBUTING_CLA.md` & `hcs-cli-0.1.39/CONTRIBUTING_CLA.md`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.38/GOVERNANCE.md` & `hcs-cli-0.1.39/GOVERNANCE.md`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.38/LICENSE` & `hcs-cli-0.1.39/LICENSE`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.38/Makefile` & `hcs-cli-0.1.39/Makefile`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.38/PKG-INFO` & `hcs-cli-0.1.39/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hcs-cli
-Version: 0.1.38
+Version: 0.1.39
 Summary: Horizon Cloud Service CLI
 Author-email: Nanw1103 <nanw1103@gmail.com>
 Project-URL: Homepage, https://github.com/vmware/horizon-cloud-service-cli
 Project-URL: Bug Tracker, https://github.com/vmware/horizon-cloud-service-cli/issues
 Project-URL: documentation, https://readthedocs.org
 Project-URL: repository, https://github.com/vmware/horizon-cloud-service-cli
 Project-URL: changelog, https://github.com/vmware/horizon-cloud-service-cli/blob/main/CHANGELOG.md
```

### Comparing `hcs-cli-0.1.38/README.md` & `hcs-cli-0.1.39/README.md`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.38/doc/dev-setup.md` & `hcs-cli-0.1.39/doc/dev-setup.md`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.38/doc/get-csp-user-api-token.md` & `hcs-cli-0.1.39/doc/get-csp-user-api-token.md`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.38/doc/hcs-cli-cheatsheet.md` & `hcs-cli-0.1.39/doc/hcs-cli-cheatsheet.md`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.38/hcs_cli.egg-info/PKG-INFO` & `hcs-cli-0.1.39/hcs_cli.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hcs-cli
-Version: 0.1.38
+Version: 0.1.39
 Summary: Horizon Cloud Service CLI
 Author-email: Nanw1103 <nanw1103@gmail.com>
 Project-URL: Homepage, https://github.com/vmware/horizon-cloud-service-cli
 Project-URL: Bug Tracker, https://github.com/vmware/horizon-cloud-service-cli/issues
 Project-URL: documentation, https://readthedocs.org
 Project-URL: repository, https://github.com/vmware/horizon-cloud-service-cli
 Project-URL: changelog, https://github.com/vmware/horizon-cloud-service-cli/blob/main/CHANGELOG.md
```

### Comparing `hcs-cli-0.1.38/hcs_cli.egg-info/SOURCES.txt` & `hcs-cli-0.1.39/hcs_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.38/payload/lcm/zero.json` & `hcs-cli-0.1.39/payload/lcm/zero.json`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.38/pyproject.toml` & `hcs-cli-0.1.39/pyproject.toml`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.38/setup.py` & `hcs-cli-0.1.39/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 from setuptools_scm import get_version
 import os
 
 with open("requirements.txt") as f:
     requirements = f.read().splitlines()
 
-VERSION = "0.1.38"
+VERSION = "0.1.39"
 
 
 def get_version():
     version = VERSION
     local_version = os.environ.get("SCM_REV")
     if local_version:
         version += "+" + local_version
```

### Comparing `hcs-cli-0.1.38/tests/conftest.py` & `hcs-cli-0.1.39/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.38/tests/test_utils.py` & `hcs-cli-0.1.39/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.38/tests/vhcs/cli/cmds/pki/get_root_ca.py` & `hcs-cli-0.1.39/tests/vhcs/cli/cmds/pki/get_root_ca.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.38/tests/vhcs/cli/cmds/plan/test_plan.py` & `hcs-cli-0.1.39/tests/vhcs/cli/cmds/plan/test_plan.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.38/tests/vhcs/cli/cmds/test_context.py` & `hcs-cli-0.1.39/tests/vhcs/cli/cmds/test_context.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.38/tests/vhcs/cli/cmds/test_login.py` & `hcs-cli-0.1.39/tests/vhcs/cli/cmds/test_login.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.38/tests/vhcs/cli/cmds/test_profile.py` & `hcs-cli-0.1.39/tests/vhcs/cli/cmds/test_profile.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.38/vhcs/__main__.py` & `hcs-cli-0.1.39/vhcs/__main__.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.38/vhcs/cli/cmds/admin/__init__.py` & `hcs-cli-0.1.39/vhcs/cli/cmds/admin/__init__.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.38/vhcs/cli/cmds/admin/azure-infra/main.py` & `hcs-cli-0.1.39/vhcs/cli/cmds/admin/azure-infra/main.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.38/vhcs/cli/cmds/admin/edge/__init__.py` & `hcs-cli-0.1.39/vhcs/cli/cmds/admin/edge/__init__.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.38/vhcs/cli/cmds/admin/edge/get.py` & `hcs-cli-0.1.39/vhcs/cli/cmds/admin/edge/get.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.38/vhcs/cli/cmds/admin/edge/list.py` & `hcs-cli-0.1.39/vhcs/cli/cmds/admin/edge/list.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.38/vhcs/cli/cmds/admin/provider/list.py` & `hcs-cli-0.1.39/vhcs/cli/cmds/admin/provider/list.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.38/vhcs/cli/cmds/admin/template/__init__.py` & `hcs-cli-0.1.39/vhcs/cli/cmds/admin/template/__init__.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.38/vhcs/cli/cmds/admin/template/get.py` & `hcs-cli-0.1.39/vhcs/cli/cmds/admin/template/get.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.38/vhcs/cli/cmds/admin/template/list.py` & `hcs-cli-0.1.39/vhcs/cli/cmds/admin/template/list.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.38/vhcs/cli/cmds/daas/__init__.py` & `hcs-cli-0.1.39/vhcs/cli/cmds/daas/__init__.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.38/vhcs/cli/cmds/daas/infra/__init__.py` & `hcs-cli-0.1.39/vhcs/cli/cmds/daas/infra/__init__.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.38/vhcs/cli/cmds/daas/infra/basic.py` & `hcs-cli-0.1.39/vhcs/cli/cmds/daas/infra/basic.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.38/vhcs/cli/cmds/daas/infra/plan.py` & `hcs-cli-0.1.39/vhcs/cli/cmds/daas/infra/plan.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.38/vhcs/cli/cmds/daas/infra/validate.py` & `hcs-cli-0.1.39/vhcs/cli/cmds/daas/infra/validate.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.38/vhcs/cli/cmds/daas/tenant/__init__.py` & `hcs-cli-0.1.39/vhcs/cli/cmds/daas/tenant/__init__.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.38/vhcs/cli/cmds/daas/tenant/basic.py` & `hcs-cli-0.1.39/vhcs/cli/cmds/daas/tenant/basic.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.38/vhcs/cli/cmds/daas/tenant/deploy.py` & `hcs-cli-0.1.39/vhcs/cli/cmds/daas/tenant/deploy.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.38/vhcs/cli/cmds/daas/tenant/destroy.py` & `hcs-cli-0.1.39/vhcs/cli/cmds/daas/tenant/destroy.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.38/vhcs/cli/cmds/daas/tenant/plan.py` & `hcs-cli-0.1.39/vhcs/cli/cmds/daas/tenant/plan.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.38/vhcs/cli/cmds/ims/__init__.py` & `hcs-cli-0.1.39/vhcs/cli/cmds/ims/__init__.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.38/vhcs/cli/cmds/ims/list.py` & `hcs-cli-0.1.39/vhcs/cli/cmds/ims/list.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.38/vhcs/cli/cmds/ims/list_copies.py` & `hcs-cli-0.1.39/vhcs/cli/cmds/ims/list_copies.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.38/vhcs/cli/cmds/lcm/__init__.py` & `hcs-cli-0.1.39/vhcs/cli/cmds/lcm/__init__.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.38/vhcs/cli/cmds/lcm/provider/__init__.py` & `hcs-cli-0.1.39/vhcs/cli/cmds/lcm/provider/__init__.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.38/vhcs/cli/cmds/lcm/provider/delete.py` & `hcs-cli-0.1.39/vhcs/cli/cmds/lcm/provider/delete.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.38/vhcs/cli/cmds/lcm/provider/get.py` & `hcs-cli-0.1.39/vhcs/cli/cmds/lcm/provider/get.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.38/vhcs/cli/cmds/lcm/provider/list.py` & `hcs-cli-0.1.39/vhcs/cli/cmds/lcm/provider/list.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.38/vhcs/cli/cmds/lcm/template/__init__.py` & `hcs-cli-0.1.39/vhcs/cli/cmds/lcm/template/__init__.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.38/vhcs/cli/cmds/lcm/template/create.py` & `hcs-cli-0.1.39/vhcs/cli/cmds/lcm/template/create.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.38/vhcs/cli/cmds/lcm/template/delete.py` & `hcs-cli-0.1.39/vhcs/cli/cmds/lcm/template/delete.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.38/vhcs/cli/cmds/lcm/template/get.py` & `hcs-cli-0.1.39/vhcs/cli/cmds/lcm/template/get.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.38/vhcs/cli/cmds/lcm/template/list.py` & `hcs-cli-0.1.39/vhcs/cli/cmds/lcm/template/list.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.38/vhcs/cli/cmds/lcm/template/wait.py` & `hcs-cli-0.1.39/vhcs/cli/cmds/lcm/template/wait.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.38/vhcs/cli/cmds/login.py` & `hcs-cli-0.1.39/vhcs/cli/cmds/login.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.38/vhcs/cli/cmds/org/datacenter/get.py` & `hcs-cli-0.1.39/vhcs/cli/cmds/org/datacenter/get.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.38/vhcs/cli/cmds/org/datacenter/list.py` & `hcs-cli-0.1.39/vhcs/cli/cmds/org/datacenter/list.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.38/vhcs/cli/cmds/org/detail/get.py` & `hcs-cli-0.1.39/vhcs/cli/cmds/org/detail/get.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.38/vhcs/cli/cmds/org/detail/list.py` & `hcs-cli-0.1.39/vhcs/cli/cmds/org/detail/list.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.38/vhcs/cli/cmds/pki/__init__.py` & `hcs-cli-0.1.39/vhcs/cli/cmds/pki/__init__.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.38/vhcs/cli/cmds/pki/delete_org_cert.py` & `hcs-cli-0.1.39/vhcs/cli/cmds/pki/delete_org_cert.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.38/vhcs/cli/cmds/pki/get_org_cert.py` & `hcs-cli-0.1.39/vhcs/cli/cmds/pki/get_org_cert.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.38/vhcs/cli/cmds/pki/get_root_ca.py` & `hcs-cli-0.1.39/vhcs/cli/cmds/pki/get_root_ca.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.38/vhcs/cli/cmds/pki/sign_resource_cert.py` & `hcs-cli-0.1.39/vhcs/cli/cmds/pki/sign_resource_cert.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.38/vhcs/cli/cmds/pki/test.py` & `hcs-cli-0.1.39/vhcs/cli/cmds/pki/test.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.38/vhcs/cli/cmds/plan/__init__.py` & `hcs-cli-0.1.39/vhcs/cli/cmds/plan/__init__.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.38/vhcs/cli/cmds/plan/deploy.py` & `hcs-cli-0.1.39/vhcs/cli/cmds/plan/deploy.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.38/vhcs/cli/cmds/plan/destroy.py` & `hcs-cli-0.1.39/vhcs/cli/cmds/plan/destroy.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.38/vhcs/cli/cmds/profile/init.py` & `hcs-cli-0.1.39/vhcs/cli/cmds/profile/init.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.38/vhcs/cli/cmds/upgrade.py` & `hcs-cli-0.1.39/vhcs/cli/cmds/upgrade.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.38/vhcs/cli/cmds/vmhub/__init__.py` & `hcs-cli-0.1.39/vhcs/cli/cmds/vmhub/__init__.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.38/vhcs/cli/cmds/vmhub/otp/__init__.py` & `hcs-cli-0.1.39/vhcs/cli/cmds/vmhub/otp/__init__.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.38/vhcs/cli/cmds/vmhub/otp/redeem.py` & `hcs-cli-0.1.39/vhcs/cli/cmds/vmhub/otp/redeem.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.38/vhcs/cli/cmds/vmhub/otp/request.py` & `hcs-cli-0.1.39/vhcs/cli/cmds/vmhub/otp/request.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.38/vhcs/cli/main.py` & `hcs-cli-0.1.39/vhcs/cli/main.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.38/vhcs/common/ctxp/README.md` & `hcs-cli-0.1.39/vhcs/common/ctxp/README.md`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.38/vhcs/common/ctxp/__init__.py` & `hcs-cli-0.1.39/vhcs/common/ctxp/__init__.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.38/vhcs/common/ctxp/_init.py` & `hcs-cli-0.1.39/vhcs/common/ctxp/_init.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.38/vhcs/common/ctxp/built_in_cmds/context.py` & `hcs-cli-0.1.39/vhcs/common/ctxp/built_in_cmds/context.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.38/vhcs/common/ctxp/built_in_cmds/profile.py` & `hcs-cli-0.1.39/vhcs/common/ctxp/built_in_cmds/profile.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.38/vhcs/common/ctxp/cli_processor.py` & `hcs-cli-0.1.39/vhcs/common/ctxp/cli_processor.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.38/vhcs/common/ctxp/config.py` & `hcs-cli-0.1.39/vhcs/common/ctxp/config.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.38/vhcs/common/ctxp/context.py` & `hcs-cli-0.1.39/vhcs/common/ctxp/context.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.38/vhcs/common/ctxp/fstore.py` & `hcs-cli-0.1.39/vhcs/common/ctxp/fstore.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.38/vhcs/common/ctxp/init.py` & `hcs-cli-0.1.39/vhcs/common/ctxp/init.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.38/vhcs/common/ctxp/jsondot.py` & `hcs-cli-0.1.39/vhcs/common/ctxp/jsondot.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.38/vhcs/common/ctxp/profile.py` & `hcs-cli-0.1.39/vhcs/common/ctxp/profile.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.38/vhcs/common/ctxp/profile_store.py` & `hcs-cli-0.1.39/vhcs/common/ctxp/profile_store.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.38/vhcs/common/ctxp/state.py` & `hcs-cli-0.1.39/vhcs/common/ctxp/state.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.38/vhcs/common/ctxp/util.py` & `hcs-cli-0.1.39/vhcs/common/ctxp/util.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.38/vhcs/common/ctxp/var_template.py` & `hcs-cli-0.1.39/vhcs/common/ctxp/var_template.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.38/vhcs/common/duration.py` & `hcs-cli-0.1.39/vhcs/common/duration.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.38/vhcs/common/logger.py` & `hcs-cli-0.1.39/vhcs/common/logger.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.38/vhcs/common/sglib/__init__.py` & `hcs-cli-0.1.39/vhcs/common/sglib/__init__.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.38/vhcs/common/sglib/auth.py` & `hcs-cli-0.1.39/vhcs/common/sglib/auth.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.38/vhcs/common/sglib/csp.py` & `hcs-cli-0.1.39/vhcs/common/sglib/csp.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.38/vhcs/common/sglib/ez_client.py` & `hcs-cli-0.1.39/vhcs/common/sglib/ez_client.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.38/vhcs/common/sglib/hcs_client.py` & `hcs-cli-0.1.39/vhcs/common/sglib/hcs_client.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.38/vhcs/common/sglib/login_support.py` & `hcs-cli-0.1.39/vhcs/common/sglib/login_support.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.38/vhcs/common/sglib/util.py` & `hcs-cli-0.1.39/vhcs/common/sglib/util.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.38/vhcs/common/util.py` & `hcs-cli-0.1.39/vhcs/common/util.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.38/vhcs/config/hcs-deployments.yaml` & `hcs-cli-0.1.39/vhcs/config/hcs-deployments.yaml`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.38/vhcs/plan/core.py` & `hcs-cli-0.1.39/vhcs/plan/core.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.38/vhcs/plan/dag.py` & `hcs-cli-0.1.39/vhcs/plan/dag.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.38/vhcs/plan/helper.py` & `hcs-cli-0.1.39/vhcs/plan/helper.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.38/vhcs/plan/provider/azure/_az_facade.py` & `hcs-cli-0.1.39/vhcs/plan/provider/azure/_az_facade.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.38/vhcs/plan/provider/azure/_prepare.py` & `hcs-cli-0.1.39/vhcs/plan/provider/azure/_prepare.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.38/vhcs/plan/provider/azure/nsg.py` & `hcs-cli-0.1.39/vhcs/plan/provider/azure/nsg.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.38/vhcs/plan/provider/azure/resource_group.py` & `hcs-cli-0.1.39/vhcs/plan/provider/azure/resource_group.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.38/vhcs/plan/provider/azure/subnet.py` & `hcs-cli-0.1.39/vhcs/plan/provider/azure/subnet.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.38/vhcs/plan/provider/dev/dummy.py` & `hcs-cli-0.1.39/vhcs/plan/provider/dev/dummy.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.38/vhcs/plan/provider/hcs/entitlement.py` & `hcs-cli-0.1.39/vhcs/plan/provider/hcs/entitlement.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.38/vhcs/plan/provider/hcs/launch_item.py` & `hcs-cli-0.1.39/vhcs/plan/provider/hcs/launch_item.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.38/vhcs/plan/provider/hcs/pool_group.py` & `hcs-cli-0.1.39/vhcs/plan/provider/hcs/pool_group.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.38/vhcs/plan/provider/hcs/pool_template.py` & `hcs-cli-0.1.39/vhcs/plan/provider/hcs/pool_template.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.38/vhcs/plan/provider/runtime/daas_tenant_calculation.py` & `hcs-cli-0.1.39/vhcs/plan/provider/runtime/daas_tenant_calculation.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.38/vhcs/plan/provider/runtime/dummy.py` & `hcs-cli-0.1.39/vhcs/plan/provider/runtime/dummy.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.38/vhcs/service/_util.py` & `hcs-cli-0.1.39/vhcs/service/_util.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.38/vhcs/service/admin/azure_infra.py` & `hcs-cli-0.1.39/vhcs/service/admin/azure_infra.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.38/vhcs/service/admin/edge.py` & `hcs-cli-0.1.39/vhcs/service/admin/edge.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.38/vhcs/service/admin/helper.py` & `hcs-cli-0.1.39/vhcs/service/admin/helper.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.38/vhcs/service/admin/provider.py` & `hcs-cli-0.1.39/vhcs/service/admin/provider.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.38/vhcs/service/admin/template.py` & `hcs-cli-0.1.39/vhcs/service/admin/template.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.38/vhcs/service/auth/admin.py` & `hcs-cli-0.1.39/vhcs/service/auth/admin.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.38/vhcs/service/ims_catalog/helper.py` & `hcs-cli-0.1.39/vhcs/service/ims_catalog/helper.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.38/vhcs/service/ims_catalog/image_copies.py` & `hcs-cli-0.1.39/vhcs/service/ims_catalog/image_copies.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.38/vhcs/service/ims_catalog/images.py` & `hcs-cli-0.1.39/vhcs/service/ims_catalog/images.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.38/vhcs/service/lcm/provider.py` & `hcs-cli-0.1.39/vhcs/service/lcm/provider.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.38/vhcs/service/lcm/template.py` & `hcs-cli-0.1.39/vhcs/service/lcm/template.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.38/vhcs/service/org_service/datacenter.py` & `hcs-cli-0.1.39/vhcs/service/org_service/datacenter.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.38/vhcs/service/org_service/details.py` & `hcs-cli-0.1.39/vhcs/service/org_service/details.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.38/vhcs/service/pki/certificate.py` & `hcs-cli-0.1.39/vhcs/service/pki/certificate.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.38/vhcs/service/portal/pools.py` & `hcs-cli-0.1.39/vhcs/service/portal/pools.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.38/vhcs/service/vmhub/otp.py` & `hcs-cli-0.1.39/vhcs/service/vmhub/otp.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.38/vhcs/support/daas/deployer.py` & `hcs-cli-0.1.39/vhcs/support/daas/deployer.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.38/vhcs/support/daas/destroyer.py` & `hcs-cli-0.1.39/vhcs/support/daas/destroyer.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.38/vhcs/support/daas/helper.py` & `hcs-cli-0.1.39/vhcs/support/daas/helper.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.38/vhcs/support/daas/infra.py` & `hcs-cli-0.1.39/vhcs/support/daas/infra.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.38/vhcs/support/daas/templates/v1/tenant.blueprint.yml` & `hcs-cli-0.1.39/vhcs/support/daas/templates/v1/tenant.blueprint.yml`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.38/vhcs/support/daas/tenant.py` & `hcs-cli-0.1.39/vhcs/support/daas/tenant.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.38/vhcs/support/profile.py` & `hcs-cli-0.1.39/vhcs/support/profile.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.38/vhcs/util/check_license.py` & `hcs-cli-0.1.39/vhcs/util/check_license.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.38/vhcs/util/duration.py` & `hcs-cli-0.1.39/vhcs/util/duration.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.38/vhcs/util/pki_util.py` & `hcs-cli-0.1.39/vhcs/util/pki_util.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.38/vhcs/util/query_util.py` & `hcs-cli-0.1.39/vhcs/util/query_util.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.38/vhcs/util/versions.py` & `hcs-cli-0.1.39/vhcs/util/versions.py`

 * *Files identical despite different names*

