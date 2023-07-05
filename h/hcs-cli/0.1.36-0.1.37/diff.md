# Comparing `tmp/hcs-cli-0.1.36.tar.gz` & `tmp/hcs-cli-0.1.37.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hcs-cli-0.1.36.tar", last modified: Tue Jun 13 19:58:39 2023, max compression
+gzip compressed data, was "hcs-cli-0.1.37.tar", last modified: Wed Jul  5 08:34:56 2023, max compression
```

## Comparing `hcs-cli-0.1.36.tar` & `hcs-cli-0.1.37.tar`

### file list

```diff
@@ -1,151 +1,252 @@
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-06-13 19:58:39.564299 hcs-cli-0.1.36/
--rw-r--r--   0 nanw       (501) staff       (20)     2820 2023-01-11 22:10:27.000000 hcs-cli-0.1.36/.gitignore
--rw-r--r--   0 nanw       (501) staff       (20)       98 2023-06-13 19:57:56.000000 hcs-cli-0.1.36/CHANGELOG.md
--rw-r--r--   0 nanw       (501) staff       (20)     5258 2023-06-13 16:45:49.000000 hcs-cli-0.1.36/CODE_OF_CONDUCT.md
--rw-r--r--   0 nanw       (501) staff       (20)     2706 2023-06-13 18:53:18.000000 hcs-cli-0.1.36/CONTRIBUTING_CLA.md
--rw-r--r--   0 nanw       (501) staff       (20)     6095 2023-04-25 23:13:27.000000 hcs-cli-0.1.36/GOVERNANCE.md
--rw-r--r--   0 nanw       (501) staff       (20)    10449 2023-06-13 16:45:49.000000 hcs-cli-0.1.36/LICENSE
--rw-r--r--   0 nanw       (501) staff       (20)      851 2023-04-24 20:31:20.000000 hcs-cli-0.1.36/Makefile
--rw-r--r--   0 nanw       (501) staff       (20)      411 2023-06-13 16:45:49.000000 hcs-cli-0.1.36/NOTICE
--rw-r--r--   0 nanw       (501) staff       (20)     2375 2023-06-13 19:58:39.563914 hcs-cli-0.1.36/PKG-INFO
--rw-r--r--   0 nanw       (501) staff       (20)     1501 2023-06-13 18:55:03.000000 hcs-cli-0.1.36/README.md
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-06-13 19:58:39.471273 hcs-cli-0.1.36/doc/
--rw-r--r--   0 nanw       (501) staff       (20)     5685 2023-06-13 19:47:35.000000 hcs-cli-0.1.36/doc/dev-setup.md
--rw-r--r--   0 nanw       (501) staff       (20)      763 2023-06-13 17:49:20.000000 hcs-cli-0.1.36/doc/get-csp-user-api-token.md
--rw-r--r--   0 nanw       (501) staff       (20)     5700 2023-06-13 18:48:47.000000 hcs-cli-0.1.36/doc/hcs-cli-cheatsheet.md
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-06-13 19:58:39.475237 hcs-cli-0.1.36/hcs_cli.egg-info/
--rw-r--r--   0 nanw       (501) staff       (20)     2375 2023-06-13 19:58:39.000000 hcs-cli-0.1.36/hcs_cli.egg-info/PKG-INFO
--rw-r--r--   0 nanw       (501) staff       (20)     3207 2023-06-13 19:58:39.000000 hcs-cli-0.1.36/hcs_cli.egg-info/SOURCES.txt
--rw-r--r--   0 nanw       (501) staff       (20)        1 2023-06-13 19:58:39.000000 hcs-cli-0.1.36/hcs_cli.egg-info/dependency_links.txt
--rw-r--r--   0 nanw       (501) staff       (20)       43 2023-06-13 19:58:39.000000 hcs-cli-0.1.36/hcs_cli.egg-info/entry_points.txt
--rw-r--r--   0 nanw       (501) staff       (20)      127 2023-06-13 19:58:39.000000 hcs-cli-0.1.36/hcs_cli.egg-info/requires.txt
--rw-r--r--   0 nanw       (501) staff       (20)       11 2023-06-13 19:58:39.000000 hcs-cli-0.1.36/hcs_cli.egg-info/top_level.txt
--rw-r--r--   0 nanw       (501) staff       (20)       92 2023-04-24 20:24:05.000000 hcs-cli-0.1.36/mypy.ini
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-06-13 19:58:39.440331 hcs-cli-0.1.36/payload/
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-06-13 19:58:39.475964 hcs-cli-0.1.36/payload/lcm/
--rw-r--r--   0 nanw       (501) staff       (20)      752 2023-04-24 20:24:05.000000 hcs-cli-0.1.36/payload/lcm/zero.json
--rw-r--r--   0 nanw       (501) staff       (20)     1187 2023-06-13 19:56:09.000000 hcs-cli-0.1.36/pyproject.toml
--rw-r--r--   0 nanw       (501) staff       (20)      194 2023-04-24 20:24:05.000000 hcs-cli-0.1.36/requirements-dev.txt
--rw-r--r--   0 nanw       (501) staff       (20)      127 2023-04-24 20:24:05.000000 hcs-cli-0.1.36/requirements.txt
--rw-r--r--   0 nanw       (501) staff       (20)       38 2023-06-13 19:58:39.564418 hcs-cli-0.1.36/setup.cfg
--rw-r--r--   0 nanw       (501) staff       (20)     1145 2023-06-13 19:57:53.000000 hcs-cli-0.1.36/setup.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-06-13 19:58:39.477856 hcs-cli-0.1.36/tests/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-24 20:24:05.000000 hcs-cli-0.1.36/tests/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)      599 2023-06-13 19:40:36.000000 hcs-cli-0.1.36/tests/conftest.py
--rw-r--r--   0 nanw       (501) staff       (20)     3025 2023-06-13 19:40:36.000000 hcs-cli-0.1.36/tests/test_utils.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-06-13 19:58:39.478796 hcs-cli-0.1.36/tests/vhcs/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-24 20:24:05.000000 hcs-cli-0.1.36/tests/vhcs/__init__.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-06-13 19:58:39.479469 hcs-cli-0.1.36/tests/vhcs/cli/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-24 20:24:05.000000 hcs-cli-0.1.36/tests/vhcs/cli/__init__.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-06-13 19:58:39.482548 hcs-cli-0.1.36/tests/vhcs/cli/cmds/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-24 20:24:05.000000 hcs-cli-0.1.36/tests/vhcs/cli/cmds/__init__.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-06-13 19:58:39.484238 hcs-cli-0.1.36/tests/vhcs/cli/cmds/pki/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-24 20:24:05.000000 hcs-cli-0.1.36/tests/vhcs/cli/cmds/pki/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)      599 2023-06-13 19:40:36.000000 hcs-cli-0.1.36/tests/vhcs/cli/cmds/pki/get_root_ca.py
--rw-r--r--   0 nanw       (501) staff       (20)      890 2023-06-13 19:40:36.000000 hcs-cli-0.1.36/tests/vhcs/cli/cmds/test_auth.py
--rw-r--r--   0 nanw       (501) staff       (20)     1943 2023-06-13 19:40:36.000000 hcs-cli-0.1.36/tests/vhcs/cli/cmds/test_context.py
--rw-r--r--   0 nanw       (501) staff       (20)     1151 2023-06-13 19:40:36.000000 hcs-cli-0.1.36/tests/vhcs/cli/cmds/test_profile.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-06-13 19:58:39.486056 hcs-cli-0.1.36/vhcs/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 21:25:27.000000 hcs-cli-0.1.36/vhcs/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)      687 2023-06-13 19:40:36.000000 hcs-cli-0.1.36/vhcs/__main__.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-06-13 19:58:39.487842 hcs-cli-0.1.36/vhcs/cli/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 02:05:21.000000 hcs-cli-0.1.36/vhcs/cli/__init__.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-06-13 19:58:39.491122 hcs-cli-0.1.36/vhcs/cli/cmds/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 02:05:21.000000 hcs-cli-0.1.36/vhcs/cli/cmds/__init__.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-06-13 19:58:39.491964 hcs-cli-0.1.36/vhcs/cli/cmds/admin/
--rw-r--r--   0 nanw       (501) staff       (20)      633 2023-06-13 19:40:36.000000 hcs-cli-0.1.36/vhcs/cli/cmds/admin/__init__.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-06-13 19:58:39.494915 hcs-cli-0.1.36/vhcs/cli/cmds/admin/edge/
--rw-r--r--   0 nanw       (501) staff       (20)      628 2023-06-13 19:40:36.000000 hcs-cli-0.1.36/vhcs/cli/cmds/admin/edge/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)      941 2023-06-13 19:40:36.000000 hcs-cli-0.1.36/vhcs/cli/cmds/admin/edge/get.py
--rw-r--r--   0 nanw       (501) staff       (20)      599 2023-06-13 19:40:36.000000 hcs-cli-0.1.36/vhcs/cli/cmds/admin/edge/list.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-06-13 19:58:39.498417 hcs-cli-0.1.36/vhcs/cli/cmds/admin/template/
--rw-r--r--   0 nanw       (501) staff       (20)      628 2023-06-13 19:40:36.000000 hcs-cli-0.1.36/vhcs/cli/cmds/admin/template/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)      949 2023-06-13 19:40:36.000000 hcs-cli-0.1.36/vhcs/cli/cmds/admin/template/get.py
--rw-r--r--   0 nanw       (501) staff       (20)     1835 2023-06-13 19:40:36.000000 hcs-cli-0.1.36/vhcs/cli/cmds/admin/template/list.py
--rw-r--r--   0 nanw       (501) staff       (20)      975 2023-06-13 19:40:36.000000 hcs-cli-0.1.36/vhcs/cli/cmds/auth.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-06-13 19:58:39.500528 hcs-cli-0.1.36/vhcs/cli/cmds/lcm/
--rw-r--r--   0 nanw       (501) staff       (20)      631 2023-06-13 19:40:36.000000 hcs-cli-0.1.36/vhcs/cli/cmds/lcm/__init__.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-06-13 19:58:39.505405 hcs-cli-0.1.36/vhcs/cli/cmds/lcm/provider/
--rw-r--r--   0 nanw       (501) staff       (20)      628 2023-06-13 19:40:36.000000 hcs-cli-0.1.36/vhcs/cli/cmds/lcm/provider/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)      796 2023-06-13 19:40:36.000000 hcs-cli-0.1.36/vhcs/cli/cmds/lcm/provider/delete.py
--rw-r--r--   0 nanw       (501) staff       (20)      787 2023-06-13 19:40:36.000000 hcs-cli-0.1.36/vhcs/cli/cmds/lcm/provider/get.py
--rw-r--r--   0 nanw       (501) staff       (20)      982 2023-06-13 19:40:36.000000 hcs-cli-0.1.36/vhcs/cli/cmds/lcm/provider/list.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-06-13 19:58:39.512018 hcs-cli-0.1.36/vhcs/cli/cmds/lcm/template/
--rw-r--r--   0 nanw       (501) staff       (20)      628 2023-06-13 19:40:36.000000 hcs-cli-0.1.36/vhcs/cli/cmds/lcm/template/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)     1857 2023-06-13 19:40:36.000000 hcs-cli-0.1.36/vhcs/cli/cmds/lcm/template/create.py
--rw-r--r--   0 nanw       (501) staff       (20)     1074 2023-06-13 19:40:36.000000 hcs-cli-0.1.36/vhcs/cli/cmds/lcm/template/delete.py
--rw-r--r--   0 nanw       (501) staff       (20)      835 2023-06-13 19:40:36.000000 hcs-cli-0.1.36/vhcs/cli/cmds/lcm/template/get.py
--rw-r--r--   0 nanw       (501) staff       (20)     1575 2023-06-13 19:40:36.000000 hcs-cli-0.1.36/vhcs/cli/cmds/lcm/template/list.py
--rw-r--r--   0 nanw       (501) staff       (20)     2256 2023-06-13 19:40:36.000000 hcs-cli-0.1.36/vhcs/cli/cmds/lcm/template/wait.py
--rw-r--r--   0 nanw       (501) staff       (20)      706 2023-06-13 19:40:36.000000 hcs-cli-0.1.36/vhcs/cli/cmds/lcm/test.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-06-13 19:58:39.447635 hcs-cli-0.1.36/vhcs/cli/cmds/org/
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-06-13 19:58:39.513741 hcs-cli-0.1.36/vhcs/cli/cmds/org/datacenter/
--rw-r--r--   0 nanw       (501) staff       (20)      849 2023-06-13 19:40:36.000000 hcs-cli-0.1.36/vhcs/cli/cmds/org/datacenter/get.py
--rw-r--r--   0 nanw       (501) staff       (20)     1010 2023-06-13 19:40:36.000000 hcs-cli-0.1.36/vhcs/cli/cmds/org/datacenter/list.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-06-13 19:58:39.515612 hcs-cli-0.1.36/vhcs/cli/cmds/org/detail/
--rw-r--r--   0 nanw       (501) staff       (20)      910 2023-06-13 19:40:36.000000 hcs-cli-0.1.36/vhcs/cli/cmds/org/detail/get.py
--rw-r--r--   0 nanw       (501) staff       (20)     1205 2023-06-13 19:40:36.000000 hcs-cli-0.1.36/vhcs/cli/cmds/org/detail/list.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-06-13 19:58:39.521738 hcs-cli-0.1.36/vhcs/cli/cmds/pki/
--rw-r--r--   0 nanw       (501) staff       (20)      631 2023-06-13 19:45:45.000000 hcs-cli-0.1.36/vhcs/cli/cmds/pki/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)     1135 2023-06-13 19:40:36.000000 hcs-cli-0.1.36/vhcs/cli/cmds/pki/delete_org_cert.py
--rw-r--r--   0 nanw       (501) staff       (20)      886 2023-06-13 19:40:36.000000 hcs-cli-0.1.36/vhcs/cli/cmds/pki/get_org_cert.py
--rw-r--r--   0 nanw       (501) staff       (20)      755 2023-06-13 19:40:36.000000 hcs-cli-0.1.36/vhcs/cli/cmds/pki/get_root_ca.py
--rw-r--r--   0 nanw       (501) staff       (20)     1784 2023-06-13 19:40:36.000000 hcs-cli-0.1.36/vhcs/cli/cmds/pki/sign_resource_cert.py
--rw-r--r--   0 nanw       (501) staff       (20)      706 2023-06-13 19:40:36.000000 hcs-cli-0.1.36/vhcs/cli/cmds/pki/test.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-06-13 19:58:39.523400 hcs-cli-0.1.36/vhcs/cli/cmds/profile/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 02:05:21.000000 hcs-cli-0.1.36/vhcs/cli/cmds/profile/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)     4323 2023-06-13 19:41:20.000000 hcs-cli-0.1.36/vhcs/cli/cmds/profile/init.py
--rw-r--r--   0 nanw       (501) staff       (20)      771 2023-06-13 19:40:36.000000 hcs-cli-0.1.36/vhcs/cli/cmds/test.py
--rw-r--r--   0 nanw       (501) staff       (20)      932 2023-06-13 19:40:36.000000 hcs-cli-0.1.36/vhcs/cli/cmds/upgrade.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-06-13 19:58:39.526704 hcs-cli-0.1.36/vhcs/cli/cmds/vmhub/
--rw-r--r--   0 nanw       (501) staff       (20)      633 2023-06-13 19:40:36.000000 hcs-cli-0.1.36/vhcs/cli/cmds/vmhub/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)     1238 2023-06-13 19:40:36.000000 hcs-cli-0.1.36/vhcs/cli/cmds/vmhub/redeem-otp.py
--rw-r--r--   0 nanw       (501) staff       (20)     1147 2023-06-13 19:40:36.000000 hcs-cli-0.1.36/vhcs/cli/cmds/vmhub/request-otp.py
--rw-r--r--   0 nanw       (501) staff       (20)      710 2023-06-13 19:40:36.000000 hcs-cli-0.1.36/vhcs/cli/cmds/vmhub/test.py
--rwxr-xr-x   0 nanw       (501) staff       (20)     2865 2023-06-13 19:40:36.000000 hcs-cli-0.1.36/vhcs/cli/main.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-06-13 19:58:39.528155 hcs-cli-0.1.36/vhcs/common/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 02:05:21.000000 hcs-cli-0.1.36/vhcs/common/__init__.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-06-13 19:58:39.538231 hcs-cli-0.1.36/vhcs/common/ctxp/
--rw-r--r--   0 nanw       (501) staff       (20)     1839 2023-04-06 02:05:21.000000 hcs-cli-0.1.36/vhcs/common/ctxp/README.md
--rw-r--r--   0 nanw       (501) staff       (20)      707 2023-06-13 19:40:36.000000 hcs-cli-0.1.36/vhcs/common/ctxp/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)     1211 2023-06-13 19:40:36.000000 hcs-cli-0.1.36/vhcs/common/ctxp/_init.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-06-13 19:58:39.540463 hcs-cli-0.1.36/vhcs/common/ctxp/built_in_cmds/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 02:05:21.000000 hcs-cli-0.1.36/vhcs/common/ctxp/built_in_cmds/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)     1965 2023-06-13 19:40:36.000000 hcs-cli-0.1.36/vhcs/common/ctxp/built_in_cmds/context.py
--rw-r--r--   0 nanw       (501) staff       (20)     2341 2023-06-13 19:40:36.000000 hcs-cli-0.1.36/vhcs/common/ctxp/built_in_cmds/profile.py
--rw-r--r--   0 nanw       (501) staff       (20)     4741 2023-06-13 19:40:36.000000 hcs-cli-0.1.36/vhcs/common/ctxp/cli_processor.py
--rw-r--r--   0 nanw       (501) staff       (20)      937 2023-06-13 19:40:36.000000 hcs-cli-0.1.36/vhcs/common/ctxp/config.py
--rw-r--r--   0 nanw       (501) staff       (20)     2256 2023-06-13 19:40:36.000000 hcs-cli-0.1.36/vhcs/common/ctxp/context.py
--rw-r--r--   0 nanw       (501) staff       (20)     6348 2023-06-13 19:40:36.000000 hcs-cli-0.1.36/vhcs/common/ctxp/fstore.py
--rw-r--r--   0 nanw       (501) staff       (20)     1200 2023-06-13 19:40:36.000000 hcs-cli-0.1.36/vhcs/common/ctxp/init.py
--rw-r--r--   0 nanw       (501) staff       (20)     2762 2023-06-13 19:40:36.000000 hcs-cli-0.1.36/vhcs/common/ctxp/jsondot.py
--rw-r--r--   0 nanw       (501) staff       (20)     4574 2023-06-13 19:40:36.000000 hcs-cli-0.1.36/vhcs/common/ctxp/profile.py
--rw-r--r--   0 nanw       (501) staff       (20)     1499 2023-06-13 19:40:36.000000 hcs-cli-0.1.36/vhcs/common/ctxp/state.py
--rw-r--r--   0 nanw       (501) staff       (20)     2780 2023-06-13 19:40:36.000000 hcs-cli-0.1.36/vhcs/common/ctxp/util.py
--rw-r--r--   0 nanw       (501) staff       (20)     3256 2023-06-13 19:40:36.000000 hcs-cli-0.1.36/vhcs/common/ctxp/var_template.py
--rw-r--r--   0 nanw       (501) staff       (20)     4846 2023-06-13 19:40:36.000000 hcs-cli-0.1.36/vhcs/common/logger.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-06-13 19:58:39.545318 hcs-cli-0.1.36/vhcs/common/sglib/
--rw-r--r--   0 nanw       (501) staff       (20)      654 2023-06-13 19:40:36.000000 hcs-cli-0.1.36/vhcs/common/sglib/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)     3104 2023-06-13 19:40:36.000000 hcs-cli-0.1.36/vhcs/common/sglib/auth.py
--rw-r--r--   0 nanw       (501) staff       (20)     4201 2023-06-13 19:40:36.000000 hcs-cli-0.1.36/vhcs/common/sglib/csp.py
--rw-r--r--   0 nanw       (501) staff       (20)     4470 2023-06-13 19:40:36.000000 hcs-cli-0.1.36/vhcs/common/sglib/ez_client.py
--rw-r--r--   0 nanw       (501) staff       (20)     1149 2023-06-13 19:40:36.000000 hcs-cli-0.1.36/vhcs/common/sglib/hcs_client.py
--rw-r--r--   0 nanw       (501) staff       (20)      970 2023-06-13 19:40:36.000000 hcs-cli-0.1.36/vhcs/common/sglib/util.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-06-13 19:58:39.547906 hcs-cli-0.1.36/vhcs/config/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 02:05:21.000000 hcs-cli-0.1.36/vhcs/config/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)     7771 2023-04-24 20:24:09.000000 hcs-cli-0.1.36/vhcs/config/hcs-deployments.yaml
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-06-13 19:58:39.558641 hcs-cli-0.1.36/vhcs/service/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-24 20:24:05.000000 hcs-cli-0.1.36/vhcs/service/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)     1586 2023-06-13 19:40:36.000000 hcs-cli-0.1.36/vhcs/service/_util.py
--rw-r--r--   0 nanw       (501) staff       (20)     1423 2023-06-13 19:40:36.000000 hcs-cli-0.1.36/vhcs/service/admin.py
--rw-r--r--   0 nanw       (501) staff       (20)     3817 2023-06-13 19:40:36.000000 hcs-cli-0.1.36/vhcs/service/lcm.py
--rw-r--r--   0 nanw       (501) staff       (20)     1595 2023-06-13 19:40:36.000000 hcs-cli-0.1.36/vhcs/service/org_service.py
--rw-r--r--   0 nanw       (501) staff       (20)     1210 2023-06-13 19:40:36.000000 hcs-cli-0.1.36/vhcs/service/pki.py
--rw-r--r--   0 nanw       (501) staff       (20)     1529 2023-06-13 19:40:36.000000 hcs-cli-0.1.36/vhcs/service/vmhub.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-06-13 19:58:39.563222 hcs-cli-0.1.36/vhcs/util/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 02:05:21.000000 hcs-cli-0.1.36/vhcs/util/__init__.py
--rwxr-xr-x   0 nanw       (501) staff       (20)     2535 2023-06-13 19:40:36.000000 hcs-cli-0.1.36/vhcs/util/check_license.py
--rw-r--r--   0 nanw       (501) staff       (20)     2759 2023-06-13 19:40:36.000000 hcs-cli-0.1.36/vhcs/util/duration.py
--rw-r--r--   0 nanw       (501) staff       (20)     5288 2023-06-13 19:40:36.000000 hcs-cli-0.1.36/vhcs/util/pki_util.py
--rw-r--r--   0 nanw       (501) staff       (20)     1760 2023-06-13 19:40:36.000000 hcs-cli-0.1.36/vhcs/util/query_util.py
--rw-r--r--   0 nanw       (501) staff       (20)     1725 2023-06-13 19:40:36.000000 hcs-cli-0.1.36/vhcs/util/versions.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-05 08:34:56.502875 hcs-cli-0.1.37/
+-rw-r--r--   0 nanw       (501) staff       (20)     2824 2023-06-21 18:44:48.000000 hcs-cli-0.1.37/.gitignore
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-05 08:34:56.154247 hcs-cli-0.1.37/.vscode/
+-rw-r--r--   0 nanw       (501) staff       (20)     2564 2023-07-05 08:21:14.000000 hcs-cli-0.1.37/.vscode/launch.json
+-rw-r--r--   0 nanw       (501) staff       (20)       49 2023-06-30 00:59:55.000000 hcs-cli-0.1.37/.vscode/settings.json
+-rw-r--r--   0 nanw       (501) staff       (20)       98 2023-06-13 19:57:56.000000 hcs-cli-0.1.37/CHANGELOG.md
+-rw-r--r--   0 nanw       (501) staff       (20)     5258 2023-06-13 16:45:49.000000 hcs-cli-0.1.37/CODE_OF_CONDUCT.md
+-rw-r--r--   0 nanw       (501) staff       (20)     2706 2023-06-13 18:53:18.000000 hcs-cli-0.1.37/CONTRIBUTING_CLA.md
+-rw-r--r--   0 nanw       (501) staff       (20)     6095 2023-04-25 23:13:27.000000 hcs-cli-0.1.37/GOVERNANCE.md
+-rw-r--r--   0 nanw       (501) staff       (20)    10449 2023-06-13 16:45:49.000000 hcs-cli-0.1.37/LICENSE
+-rw-r--r--   0 nanw       (501) staff       (20)      854 2023-07-03 19:19:46.000000 hcs-cli-0.1.37/Makefile
+-rw-r--r--   0 nanw       (501) staff       (20)      411 2023-06-13 16:45:49.000000 hcs-cli-0.1.37/NOTICE
+-rw-r--r--   0 nanw       (501) staff       (20)     2516 2023-07-05 08:34:56.501983 hcs-cli-0.1.37/PKG-INFO
+-rw-r--r--   0 nanw       (501) staff       (20)     1642 2023-06-24 01:22:59.000000 hcs-cli-0.1.37/README.md
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-05 08:34:56.160513 hcs-cli-0.1.37/doc/
+-rw-r--r--   0 nanw       (501) staff       (20)     5950 2023-06-15 17:50:47.000000 hcs-cli-0.1.37/doc/dev-setup.md
+-rw-r--r--   0 nanw       (501) staff       (20)      763 2023-06-13 17:49:20.000000 hcs-cli-0.1.37/doc/get-csp-user-api-token.md
+-rw-r--r--   0 nanw       (501) staff       (20)     6394 2023-07-03 19:03:00.000000 hcs-cli-0.1.37/doc/hcs-cli-cheatsheet.md
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-05 08:34:56.167648 hcs-cli-0.1.37/hcs_cli.egg-info/
+-rw-r--r--   0 nanw       (501) staff       (20)     2516 2023-07-05 08:34:55.000000 hcs-cli-0.1.37/hcs_cli.egg-info/PKG-INFO
+-rw-r--r--   0 nanw       (501) staff       (20)     5747 2023-07-05 08:34:55.000000 hcs-cli-0.1.37/hcs_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 nanw       (501) staff       (20)        1 2023-07-05 08:34:55.000000 hcs-cli-0.1.37/hcs_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 nanw       (501) staff       (20)       43 2023-07-05 08:34:55.000000 hcs-cli-0.1.37/hcs_cli.egg-info/entry_points.txt
+-rw-r--r--   0 nanw       (501) staff       (20)      127 2023-07-05 08:34:55.000000 hcs-cli-0.1.37/hcs_cli.egg-info/requires.txt
+-rw-r--r--   0 nanw       (501) staff       (20)       11 2023-07-05 08:34:55.000000 hcs-cli-0.1.37/hcs_cli.egg-info/top_level.txt
+-rw-r--r--   0 nanw       (501) staff       (20)       92 2023-04-24 20:24:05.000000 hcs-cli-0.1.37/mypy.ini
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-05 08:34:56.093395 hcs-cli-0.1.37/payload/
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-05 08:34:56.169141 hcs-cli-0.1.37/payload/lcm/
+-rw-r--r--   0 nanw       (501) staff       (20)      752 2023-04-24 20:24:05.000000 hcs-cli-0.1.37/payload/lcm/zero.json
+-rw-r--r--   0 nanw       (501) staff       (20)     1187 2023-06-13 19:56:09.000000 hcs-cli-0.1.37/pyproject.toml
+-rw-r--r--   0 nanw       (501) staff       (20)      194 2023-04-24 20:24:05.000000 hcs-cli-0.1.37/requirements-dev.txt
+-rw-r--r--   0 nanw       (501) staff       (20)      127 2023-04-24 20:24:05.000000 hcs-cli-0.1.37/requirements.txt
+-rw-r--r--   0 nanw       (501) staff       (20)       38 2023-07-05 08:34:56.503242 hcs-cli-0.1.37/setup.cfg
+-rw-r--r--   0 nanw       (501) staff       (20)     1154 2023-07-05 08:34:12.000000 hcs-cli-0.1.37/setup.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-05 08:34:56.172484 hcs-cli-0.1.37/tests/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-24 20:24:05.000000 hcs-cli-0.1.37/tests/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)      599 2023-06-13 19:40:36.000000 hcs-cli-0.1.37/tests/conftest.py
+-rw-r--r--   0 nanw       (501) staff       (20)     3025 2023-06-13 19:40:36.000000 hcs-cli-0.1.37/tests/test_utils.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-05 08:34:56.173906 hcs-cli-0.1.37/tests/vhcs/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-24 20:24:05.000000 hcs-cli-0.1.37/tests/vhcs/__init__.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-05 08:34:56.174954 hcs-cli-0.1.37/tests/vhcs/cli/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-24 20:24:05.000000 hcs-cli-0.1.37/tests/vhcs/cli/__init__.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-05 08:34:56.179027 hcs-cli-0.1.37/tests/vhcs/cli/cmds/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-24 20:24:05.000000 hcs-cli-0.1.37/tests/vhcs/cli/cmds/__init__.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-05 08:34:56.181316 hcs-cli-0.1.37/tests/vhcs/cli/cmds/pki/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-24 20:24:05.000000 hcs-cli-0.1.37/tests/vhcs/cli/cmds/pki/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)      599 2023-06-13 19:40:36.000000 hcs-cli-0.1.37/tests/vhcs/cli/cmds/pki/get_root_ca.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1943 2023-06-13 19:40:36.000000 hcs-cli-0.1.37/tests/vhcs/cli/cmds/test_context.py
+-rw-r--r--   0 nanw       (501) staff       (20)      918 2023-07-03 19:18:10.000000 hcs-cli-0.1.37/tests/vhcs/cli/cmds/test_login.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1151 2023-07-05 08:29:47.000000 hcs-cli-0.1.37/tests/vhcs/cli/cmds/test_profile.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-05 08:34:56.183300 hcs-cli-0.1.37/vhcs/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 21:25:27.000000 hcs-cli-0.1.37/vhcs/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)      687 2023-06-13 19:40:36.000000 hcs-cli-0.1.37/vhcs/__main__.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-05 08:34:56.188083 hcs-cli-0.1.37/vhcs/cli/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 02:05:21.000000 hcs-cli-0.1.37/vhcs/cli/__init__.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-05 08:34:56.192000 hcs-cli-0.1.37/vhcs/cli/cmds/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 02:05:21.000000 hcs-cli-0.1.37/vhcs/cli/cmds/__init__.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-05 08:34:56.193018 hcs-cli-0.1.37/vhcs/cli/cmds/admin/
+-rw-r--r--   0 nanw       (501) staff       (20)      633 2023-06-13 19:40:36.000000 hcs-cli-0.1.37/vhcs/cli/cmds/admin/__init__.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-05 08:34:56.193951 hcs-cli-0.1.37/vhcs/cli/cmds/admin/azure-infra/
+-rw-r--r--   0 nanw       (501) staff       (20)     1069 2023-06-27 20:44:31.000000 hcs-cli-0.1.37/vhcs/cli/cmds/admin/azure-infra/main.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-05 08:34:56.197133 hcs-cli-0.1.37/vhcs/cli/cmds/admin/edge/
+-rw-r--r--   0 nanw       (501) staff       (20)      628 2023-06-13 19:40:36.000000 hcs-cli-0.1.37/vhcs/cli/cmds/admin/edge/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)      941 2023-06-13 19:40:36.000000 hcs-cli-0.1.37/vhcs/cli/cmds/admin/edge/get.py
+-rw-r--r--   0 nanw       (501) staff       (20)      599 2023-06-13 19:40:36.000000 hcs-cli-0.1.37/vhcs/cli/cmds/admin/edge/list.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-05 08:34:56.198234 hcs-cli-0.1.37/vhcs/cli/cmds/admin/provider/
+-rw-r--r--   0 nanw       (501) staff       (20)     1136 2023-06-15 22:34:38.000000 hcs-cli-0.1.37/vhcs/cli/cmds/admin/provider/list.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-05 08:34:56.204213 hcs-cli-0.1.37/vhcs/cli/cmds/admin/template/
+-rw-r--r--   0 nanw       (501) staff       (20)      628 2023-06-13 19:40:36.000000 hcs-cli-0.1.37/vhcs/cli/cmds/admin/template/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)      949 2023-06-13 19:40:36.000000 hcs-cli-0.1.37/vhcs/cli/cmds/admin/template/get.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1841 2023-06-23 17:01:30.000000 hcs-cli-0.1.37/vhcs/cli/cmds/admin/template/list.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-05 08:34:56.205484 hcs-cli-0.1.37/vhcs/cli/cmds/daas/
+-rw-r--r--   0 nanw       (501) staff       (20)      642 2023-06-15 22:15:00.000000 hcs-cli-0.1.37/vhcs/cli/cmds/daas/__init__.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-05 08:34:56.211588 hcs-cli-0.1.37/vhcs/cli/cmds/daas/infra/
+-rw-r--r--   0 nanw       (501) staff       (20)      648 2023-06-21 17:56:47.000000 hcs-cli-0.1.37/vhcs/cli/cmds/daas/infra/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1041 2023-06-30 16:52:44.000000 hcs-cli-0.1.37/vhcs/cli/cmds/daas/infra/basic.py
+-rw-r--r--   0 nanw       (501) staff       (20)     2336 2023-06-30 16:50:10.000000 hcs-cli-0.1.37/vhcs/cli/cmds/daas/infra/plan.py
+-rw-r--r--   0 nanw       (501) staff       (20)      745 2023-06-21 18:14:23.000000 hcs-cli-0.1.37/vhcs/cli/cmds/daas/infra/validate.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-05 08:34:56.217460 hcs-cli-0.1.37/vhcs/cli/cmds/daas/tenant/
+-rw-r--r--   0 nanw       (501) staff       (20)      633 2023-06-21 17:36:22.000000 hcs-cli-0.1.37/vhcs/cli/cmds/daas/tenant/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)      963 2023-06-30 16:57:41.000000 hcs-cli-0.1.37/vhcs/cli/cmds/daas/tenant/basic.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1062 2023-06-30 16:42:16.000000 hcs-cli-0.1.37/vhcs/cli/cmds/daas/tenant/deploy.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1366 2023-06-30 16:42:22.000000 hcs-cli-0.1.37/vhcs/cli/cmds/daas/tenant/destroy.py
+-rw-r--r--   0 nanw       (501) staff       (20)     4964 2023-07-01 03:22:23.000000 hcs-cli-0.1.37/vhcs/cli/cmds/daas/tenant/plan.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-05 08:34:56.223271 hcs-cli-0.1.37/vhcs/cli/cmds/ims/
+-rw-r--r--   0 nanw       (501) staff       (20)      633 2023-06-27 19:52:41.000000 hcs-cli-0.1.37/vhcs/cli/cmds/ims/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)      915 2023-06-27 19:56:58.000000 hcs-cli-0.1.37/vhcs/cli/cmds/ims/list.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1033 2023-06-27 20:14:16.000000 hcs-cli-0.1.37/vhcs/cli/cmds/ims/list_copies.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-05 08:34:56.224287 hcs-cli-0.1.37/vhcs/cli/cmds/lcm/
+-rw-r--r--   0 nanw       (501) staff       (20)      631 2023-06-27 19:52:37.000000 hcs-cli-0.1.37/vhcs/cli/cmds/lcm/__init__.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-05 08:34:56.228075 hcs-cli-0.1.37/vhcs/cli/cmds/lcm/provider/
+-rw-r--r--   0 nanw       (501) staff       (20)      628 2023-06-13 19:40:36.000000 hcs-cli-0.1.37/vhcs/cli/cmds/lcm/provider/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)      801 2023-06-23 02:35:21.000000 hcs-cli-0.1.37/vhcs/cli/cmds/lcm/provider/delete.py
+-rw-r--r--   0 nanw       (501) staff       (20)      792 2023-06-23 02:35:30.000000 hcs-cli-0.1.37/vhcs/cli/cmds/lcm/provider/get.py
+-rw-r--r--   0 nanw       (501) staff       (20)      987 2023-06-23 02:35:40.000000 hcs-cli-0.1.37/vhcs/cli/cmds/lcm/provider/list.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-05 08:34:56.234026 hcs-cli-0.1.37/vhcs/cli/cmds/lcm/template/
+-rw-r--r--   0 nanw       (501) staff       (20)      628 2023-06-13 19:40:36.000000 hcs-cli-0.1.37/vhcs/cli/cmds/lcm/template/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1857 2023-06-23 02:36:50.000000 hcs-cli-0.1.37/vhcs/cli/cmds/lcm/template/create.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1079 2023-06-23 02:36:58.000000 hcs-cli-0.1.37/vhcs/cli/cmds/lcm/template/delete.py
+-rw-r--r--   0 nanw       (501) staff       (20)      840 2023-06-23 02:37:07.000000 hcs-cli-0.1.37/vhcs/cli/cmds/lcm/template/get.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1588 2023-06-23 02:37:18.000000 hcs-cli-0.1.37/vhcs/cli/cmds/lcm/template/list.py
+-rw-r--r--   0 nanw       (501) staff       (20)     2256 2023-06-23 02:37:44.000000 hcs-cli-0.1.37/vhcs/cli/cmds/lcm/template/wait.py
+-rw-r--r--   0 nanw       (501) staff       (20)     6631 2023-07-05 07:47:22.000000 hcs-cli-0.1.37/vhcs/cli/cmds/login.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-05 08:34:56.113582 hcs-cli-0.1.37/vhcs/cli/cmds/org/
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-05 08:34:56.235587 hcs-cli-0.1.37/vhcs/cli/cmds/org/datacenter/
+-rw-r--r--   0 nanw       (501) staff       (20)      848 2023-06-30 15:40:06.000000 hcs-cli-0.1.37/vhcs/cli/cmds/org/datacenter/get.py
+-rw-r--r--   0 nanw       (501) staff       (20)      997 2023-06-30 15:40:15.000000 hcs-cli-0.1.37/vhcs/cli/cmds/org/datacenter/list.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-05 08:34:56.236982 hcs-cli-0.1.37/vhcs/cli/cmds/org/detail/
+-rw-r--r--   0 nanw       (501) staff       (20)      906 2023-06-30 15:40:19.000000 hcs-cli-0.1.37/vhcs/cli/cmds/org/detail/get.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1201 2023-06-30 15:40:25.000000 hcs-cli-0.1.37/vhcs/cli/cmds/org/detail/list.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-05 08:34:56.241029 hcs-cli-0.1.37/vhcs/cli/cmds/pki/
+-rw-r--r--   0 nanw       (501) staff       (20)      631 2023-06-13 19:45:45.000000 hcs-cli-0.1.37/vhcs/cli/cmds/pki/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1155 2023-06-30 15:38:40.000000 hcs-cli-0.1.37/vhcs/cli/cmds/pki/delete_org_cert.py
+-rw-r--r--   0 nanw       (501) staff       (20)      906 2023-06-30 15:38:40.000000 hcs-cli-0.1.37/vhcs/cli/cmds/pki/get_org_cert.py
+-rw-r--r--   0 nanw       (501) staff       (20)      775 2023-06-30 15:38:40.000000 hcs-cli-0.1.37/vhcs/cli/cmds/pki/get_root_ca.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1804 2023-06-30 15:38:40.000000 hcs-cli-0.1.37/vhcs/cli/cmds/pki/sign_resource_cert.py
+-rw-r--r--   0 nanw       (501) staff       (20)      726 2023-06-30 15:38:40.000000 hcs-cli-0.1.37/vhcs/cli/cmds/pki/test.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-05 08:34:56.243225 hcs-cli-0.1.37/vhcs/cli/cmds/plan/
+-rw-r--r--   0 nanw       (501) staff       (20)      665 2023-06-28 17:52:44.000000 hcs-cli-0.1.37/vhcs/cli/cmds/plan/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1895 2023-07-01 03:32:43.000000 hcs-cli-0.1.37/vhcs/cli/cmds/plan/deploy.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1675 2023-06-29 21:56:28.000000 hcs-cli-0.1.37/vhcs/cli/cmds/plan/destroy.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-05 08:34:56.244841 hcs-cli-0.1.37/vhcs/cli/cmds/profile/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 02:05:21.000000 hcs-cli-0.1.37/vhcs/cli/cmds/profile/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1765 2023-07-05 06:16:00.000000 hcs-cli-0.1.37/vhcs/cli/cmds/profile/init.py
+-rw-r--r--   0 nanw       (501) staff       (20)      932 2023-06-13 19:40:36.000000 hcs-cli-0.1.37/vhcs/cli/cmds/upgrade.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-05 08:34:56.246281 hcs-cli-0.1.37/vhcs/cli/cmds/vmhub/
+-rw-r--r--   0 nanw       (501) staff       (20)      633 2023-06-13 19:40:36.000000 hcs-cli-0.1.37/vhcs/cli/cmds/vmhub/__init__.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-05 08:34:56.251984 hcs-cli-0.1.37/vhcs/cli/cmds/vmhub/otp/
+-rw-r--r--   0 nanw       (501) staff       (20)      643 2023-06-29 21:49:43.000000 hcs-cli-0.1.37/vhcs/cli/cmds/vmhub/otp/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1234 2023-06-29 21:49:20.000000 hcs-cli-0.1.37/vhcs/cli/cmds/vmhub/otp/redeem.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1143 2023-06-29 21:49:25.000000 hcs-cli-0.1.37/vhcs/cli/cmds/vmhub/otp/request.py
+-rwxr-xr-x   0 nanw       (501) staff       (20)     2865 2023-06-23 02:40:39.000000 hcs-cli-0.1.37/vhcs/cli/main.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-05 08:34:56.263395 hcs-cli-0.1.37/vhcs/common/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 02:05:21.000000 hcs-cli-0.1.37/vhcs/common/__init__.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-05 08:34:56.292198 hcs-cli-0.1.37/vhcs/common/ctxp/
+-rw-r--r--   0 nanw       (501) staff       (20)     1538 2023-07-03 20:20:16.000000 hcs-cli-0.1.37/vhcs/common/ctxp/README.md
+-rw-r--r--   0 nanw       (501) staff       (20)      790 2023-07-03 20:45:37.000000 hcs-cli-0.1.37/vhcs/common/ctxp/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1155 2023-07-03 21:18:13.000000 hcs-cli-0.1.37/vhcs/common/ctxp/_init.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-05 08:34:56.297086 hcs-cli-0.1.37/vhcs/common/ctxp/built_in_cmds/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 02:05:21.000000 hcs-cli-0.1.37/vhcs/common/ctxp/built_in_cmds/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     2421 2023-06-21 17:26:56.000000 hcs-cli-0.1.37/vhcs/common/ctxp/built_in_cmds/context.py
+-rw-r--r--   0 nanw       (501) staff       (20)     3977 2023-07-05 08:26:35.000000 hcs-cli-0.1.37/vhcs/common/ctxp/built_in_cmds/profile.py
+-rw-r--r--   0 nanw       (501) staff       (20)     5129 2023-07-05 06:22:51.000000 hcs-cli-0.1.37/vhcs/common/ctxp/cli_processor.py
+-rw-r--r--   0 nanw       (501) staff       (20)      936 2023-07-03 21:17:12.000000 hcs-cli-0.1.37/vhcs/common/ctxp/config.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1205 2023-07-03 21:08:50.000000 hcs-cli-0.1.37/vhcs/common/ctxp/context.py
+-rw-r--r--   0 nanw       (501) staff       (20)     6467 2023-06-23 00:26:19.000000 hcs-cli-0.1.37/vhcs/common/ctxp/fstore.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1200 2023-06-13 19:40:36.000000 hcs-cli-0.1.37/vhcs/common/ctxp/init.py
+-rw-r--r--   0 nanw       (501) staff       (20)     2776 2023-06-22 22:58:23.000000 hcs-cli-0.1.37/vhcs/common/ctxp/jsondot.py
+-rw-r--r--   0 nanw       (501) staff       (20)     5163 2023-07-05 08:33:15.000000 hcs-cli-0.1.37/vhcs/common/ctxp/profile.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1565 2023-07-05 06:52:28.000000 hcs-cli-0.1.37/vhcs/common/ctxp/profile_store.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1604 2023-07-03 22:06:25.000000 hcs-cli-0.1.37/vhcs/common/ctxp/state.py
+-rw-r--r--   0 nanw       (501) staff       (20)     6258 2023-07-05 06:26:16.000000 hcs-cli-0.1.37/vhcs/common/ctxp/util.py
+-rw-r--r--   0 nanw       (501) staff       (20)     3256 2023-06-13 19:40:36.000000 hcs-cli-0.1.37/vhcs/common/ctxp/var_template.py
+-rw-r--r--   0 nanw       (501) staff       (20)     4846 2023-06-13 19:40:36.000000 hcs-cli-0.1.37/vhcs/common/logger.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-05 08:34:56.323694 hcs-cli-0.1.37/vhcs/common/sglib/
+-rw-r--r--   0 nanw       (501) staff       (20)      654 2023-06-13 19:40:36.000000 hcs-cli-0.1.37/vhcs/common/sglib/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     4493 2023-07-05 08:06:23.000000 hcs-cli-0.1.37/vhcs/common/sglib/auth.py
+-rw-r--r--   0 nanw       (501) staff       (20)     8079 2023-07-05 07:42:49.000000 hcs-cli-0.1.37/vhcs/common/sglib/csp.py
+-rw-r--r--   0 nanw       (501) staff       (20)     4823 2023-07-05 08:20:04.000000 hcs-cli-0.1.37/vhcs/common/sglib/ez_client.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1013 2023-07-05 08:10:55.000000 hcs-cli-0.1.37/vhcs/common/sglib/hcs_client.py
+-rw-r--r--   0 nanw       (501) staff       (20)     8243 2023-07-05 08:11:32.000000 hcs-cli-0.1.37/vhcs/common/sglib/login_support.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1307 2023-07-05 07:59:02.000000 hcs-cli-0.1.37/vhcs/common/sglib/util.py
+-rw-r--r--   0 nanw       (501) staff       (20)     7955 2023-07-05 06:01:37.000000 hcs-cli-0.1.37/vhcs/common/util.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-05 08:34:56.331936 hcs-cli-0.1.37/vhcs/config/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 02:05:21.000000 hcs-cli-0.1.37/vhcs/config/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     7771 2023-07-03 22:19:24.000000 hcs-cli-0.1.37/vhcs/config/hcs-deployments.yaml
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-05 08:34:56.341812 hcs-cli-0.1.37/vhcs/plan/
+-rw-r--r--   0 nanw       (501) staff       (20)       64 2023-06-29 18:59:28.000000 hcs-cli-0.1.37/vhcs/plan/__init__.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-05 08:34:56.351359 hcs-cli-0.1.37/vhcs/plan/engine/
+-rw-r--r--   0 nanw       (501) staff       (20)       67 2023-06-29 18:57:52.000000 hcs-cli-0.1.37/vhcs/plan/engine/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     6874 2023-07-01 03:33:39.000000 hcs-cli-0.1.37/vhcs/plan/engine/core.py
+-rw-r--r--   0 nanw       (501) staff       (20)     3759 2023-07-01 03:38:16.000000 hcs-cli-0.1.37/vhcs/plan/engine/dag.py
+-rw-r--r--   0 nanw       (501) staff       (20)     4229 2023-06-30 00:23:11.000000 hcs-cli-0.1.37/vhcs/plan/engine/helper.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-05 08:34:56.354765 hcs-cli-0.1.37/vhcs/plan/provider/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-06-28 17:25:18.000000 hcs-cli-0.1.37/vhcs/plan/provider/__init__.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-05 08:34:56.365568 hcs-cli-0.1.37/vhcs/plan/provider/azure/
+-rw-r--r--   0 nanw       (501) staff       (20)       29 2023-06-30 00:51:51.000000 hcs-cli-0.1.37/vhcs/plan/provider/azure/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     3071 2023-06-30 01:10:54.000000 hcs-cli-0.1.37/vhcs/plan/provider/azure/_az_facade.py
+-rw-r--r--   0 nanw       (501) staff       (20)      575 2023-06-30 00:26:03.000000 hcs-cli-0.1.37/vhcs/plan/provider/azure/_prepare.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1114 2023-06-30 01:27:22.000000 hcs-cli-0.1.37/vhcs/plan/provider/azure/nsg.py
+-rw-r--r--   0 nanw       (501) staff       (20)      917 2023-06-29 23:12:33.000000 hcs-cli-0.1.37/vhcs/plan/provider/azure/resource_group.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1169 2023-06-30 01:28:00.000000 hcs-cli-0.1.37/vhcs/plan/provider/azure/subnet.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-05 08:34:56.388621 hcs-cli-0.1.37/vhcs/plan/provider/hcs/
+-rw-r--r--   0 nanw       (501) staff       (20)       29 2023-06-29 23:41:13.000000 hcs-cli-0.1.37/vhcs/plan/provider/hcs/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)       33 2023-06-29 23:41:19.000000 hcs-cli-0.1.37/vhcs/plan/provider/hcs/_prepare.py
+-rw-r--r--   0 nanw       (501) staff       (20)      705 2023-06-30 00:56:23.000000 hcs-cli-0.1.37/vhcs/plan/provider/hcs/entitlement.py
+-rw-r--r--   0 nanw       (501) staff       (20)      705 2023-06-30 00:56:27.000000 hcs-cli-0.1.37/vhcs/plan/provider/hcs/launch_item.py
+-rw-r--r--   0 nanw       (501) staff       (20)      705 2023-06-30 00:56:29.000000 hcs-cli-0.1.37/vhcs/plan/provider/hcs/pool_group.py
+-rw-r--r--   0 nanw       (501) staff       (20)      714 2023-06-30 00:56:32.000000 hcs-cli-0.1.37/vhcs/plan/provider/hcs/pool_template.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-05 08:34:56.396376 hcs-cli-0.1.37/vhcs/plan/provider/runtime/
+-rw-r--r--   0 nanw       (501) staff       (20)       29 2023-06-30 00:29:55.000000 hcs-cli-0.1.37/vhcs/plan/provider/runtime/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)       84 2023-06-30 00:30:09.000000 hcs-cli-0.1.37/vhcs/plan/provider/runtime/_prepare.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1926 2023-06-30 21:31:40.000000 hcs-cli-0.1.37/vhcs/plan/provider/runtime/daas_tenant_calculation.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-05 08:34:56.402343 hcs-cli-0.1.37/vhcs/service/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-24 20:24:05.000000 hcs-cli-0.1.37/vhcs/service/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1586 2023-06-13 19:40:36.000000 hcs-cli-0.1.37/vhcs/service/_util.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-05 08:34:56.417136 hcs-cli-0.1.37/vhcs/service/admin/
+-rw-r--r--   0 nanw       (501) staff       (20)       59 2023-06-27 20:41:57.000000 hcs-cli-0.1.37/vhcs/service/admin/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1184 2023-06-27 20:24:06.000000 hcs-cli-0.1.37/vhcs/service/admin/azure_infra.py
+-rw-r--r--   0 nanw       (501) staff       (20)      940 2023-06-21 23:40:00.000000 hcs-cli-0.1.37/vhcs/service/admin/edge.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1265 2023-06-23 01:29:22.000000 hcs-cli-0.1.37/vhcs/service/admin/helper.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1103 2023-06-27 19:44:57.000000 hcs-cli-0.1.37/vhcs/service/admin/provider.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1455 2023-06-23 02:28:44.000000 hcs-cli-0.1.37/vhcs/service/admin/template.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-05 08:34:56.421155 hcs-cli-0.1.37/vhcs/service/auth/
+-rw-r--r--   0 nanw       (501) staff       (20)       19 2023-06-22 18:49:46.000000 hcs-cli-0.1.37/vhcs/service/auth/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)      851 2023-06-22 18:45:24.000000 hcs-cli-0.1.37/vhcs/service/auth/admin.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-05 08:34:56.434957 hcs-cli-0.1.37/vhcs/service/ims_catalog/
+-rw-r--r--   0 nanw       (501) staff       (20)       42 2023-06-27 19:54:19.000000 hcs-cli-0.1.37/vhcs/service/ims_catalog/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1218 2023-06-27 20:17:07.000000 hcs-cli-0.1.37/vhcs/service/ims_catalog/helper.py
+-rw-r--r--   0 nanw       (501) staff       (20)      915 2023-06-22 15:43:13.000000 hcs-cli-0.1.37/vhcs/service/ims_catalog/image_copies.py
+-rw-r--r--   0 nanw       (501) staff       (20)      909 2023-06-22 01:03:55.000000 hcs-cli-0.1.37/vhcs/service/ims_catalog/images.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-05 08:34:56.445776 hcs-cli-0.1.37/vhcs/service/lcm/
+-rw-r--r--   0 nanw       (501) staff       (20)       32 2023-06-22 18:49:27.000000 hcs-cli-0.1.37/vhcs/service/lcm/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1437 2023-06-22 18:48:08.000000 hcs-cli-0.1.37/vhcs/service/lcm/provider.py
+-rw-r--r--   0 nanw       (501) staff       (20)     2770 2023-06-22 18:47:45.000000 hcs-cli-0.1.37/vhcs/service/lcm/template.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-05 08:34:56.454570 hcs-cli-0.1.37/vhcs/service/org_service/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-06-30 15:38:56.000000 hcs-cli-0.1.37/vhcs/service/org_service/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1083 2023-06-30 15:37:59.000000 hcs-cli-0.1.37/vhcs/service/org_service/datacenter.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1040 2023-06-30 15:37:42.000000 hcs-cli-0.1.37/vhcs/service/org_service/details.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-05 08:34:56.458874 hcs-cli-0.1.37/vhcs/service/pki/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-06-30 15:38:50.000000 hcs-cli-0.1.37/vhcs/service/pki/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1211 2023-06-30 15:38:16.000000 hcs-cli-0.1.37/vhcs/service/pki/certificate.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-05 08:34:56.462628 hcs-cli-0.1.37/vhcs/service/portal/
+-rw-r--r--   0 nanw       (501) staff       (20)       19 2023-06-28 15:59:32.000000 hcs-cli-0.1.37/vhcs/service/portal/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)      879 2023-06-28 16:01:23.000000 hcs-cli-0.1.37/vhcs/service/portal/pools.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-05 08:34:56.465512 hcs-cli-0.1.37/vhcs/service/vmhub/
+-rw-r--r--   0 nanw       (501) staff       (20)       17 2023-07-03 19:03:42.000000 hcs-cli-0.1.37/vhcs/service/vmhub/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1406 2023-06-29 21:48:05.000000 hcs-cli-0.1.37/vhcs/service/vmhub/otp.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-05 08:34:56.472392 hcs-cli-0.1.37/vhcs/support/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-06-30 15:35:24.000000 hcs-cli-0.1.37/vhcs/support/__init__.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-05 08:34:56.483939 hcs-cli-0.1.37/vhcs/support/daas/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-06-21 23:10:31.000000 hcs-cli-0.1.37/vhcs/support/daas/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     8418 2023-06-30 16:58:38.000000 hcs-cli-0.1.37/vhcs/support/daas/deployer.py
+-rw-r--r--   0 nanw       (501) staff       (20)     4092 2023-06-30 16:57:21.000000 hcs-cli-0.1.37/vhcs/support/daas/destroyer.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1731 2023-06-30 16:55:29.000000 hcs-cli-0.1.37/vhcs/support/daas/helper.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1813 2023-06-22 21:16:24.000000 hcs-cli-0.1.37/vhcs/support/daas/infra.py
+-rw-r--r--   0 nanw       (501) staff       (20)      242 2023-06-30 18:59:23.000000 hcs-cli-0.1.37/vhcs/support/daas/template.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-05 08:34:56.133001 hcs-cli-0.1.37/vhcs/support/daas/templates/
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-05 08:34:56.491083 hcs-cli-0.1.37/vhcs/support/daas/templates/v1/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-06-30 18:29:22.000000 hcs-cli-0.1.37/vhcs/support/daas/templates/v1/infra.blueprint.yml
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-06-30 18:27:18.000000 hcs-cli-0.1.37/vhcs/support/daas/templates/v1/infra.vars.yml
+-rw-r--r--   0 nanw       (501) staff       (20)     1554 2023-07-03 23:45:01.000000 hcs-cli-0.1.37/vhcs/support/daas/templates/v1/tenant.blueprint.yml
+-rw-r--r--   0 nanw       (501) staff       (20)      238 2023-06-30 18:32:37.000000 hcs-cli-0.1.37/vhcs/support/daas/templates/v1/tenant.vars.yml
+-rw-r--r--   0 nanw       (501) staff       (20)     1979 2023-06-22 21:16:18.000000 hcs-cli-0.1.37/vhcs/support/daas/tenant.py
+-rw-r--r--   0 nanw       (501) staff       (20)     2621 2023-07-05 07:42:08.000000 hcs-cli-0.1.37/vhcs/support/profile.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-05 08:34:56.500171 hcs-cli-0.1.37/vhcs/util/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 02:05:21.000000 hcs-cli-0.1.37/vhcs/util/__init__.py
+-rwxr-xr-x   0 nanw       (501) staff       (20)     2535 2023-06-13 19:40:36.000000 hcs-cli-0.1.37/vhcs/util/check_license.py
+-rw-r--r--   0 nanw       (501) staff       (20)     2759 2023-06-13 19:40:36.000000 hcs-cli-0.1.37/vhcs/util/duration.py
+-rw-r--r--   0 nanw       (501) staff       (20)     5288 2023-06-13 19:40:36.000000 hcs-cli-0.1.37/vhcs/util/pki_util.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1819 2023-06-22 01:50:10.000000 hcs-cli-0.1.37/vhcs/util/query_util.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1725 2023-06-13 19:40:36.000000 hcs-cli-0.1.37/vhcs/util/versions.py
```

### Comparing `hcs-cli-0.1.36/.gitignore` & `hcs-cli-0.1.37/.gitignore`

 * *Files 0% similar despite different names*

```diff
@@ -156,7 +156,8 @@
 state/
 *.log
 *.exe
 .DS_Store
 *.bak
 t.py
 logs/*.log
+lab/
```

### Comparing `hcs-cli-0.1.36/CODE_OF_CONDUCT.md` & `hcs-cli-0.1.37/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.36/CONTRIBUTING_CLA.md` & `hcs-cli-0.1.37/CONTRIBUTING_CLA.md`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.36/GOVERNANCE.md` & `hcs-cli-0.1.37/GOVERNANCE.md`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.36/LICENSE` & `hcs-cli-0.1.37/LICENSE`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.36/Makefile` & `hcs-cli-0.1.37/Makefile`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 	export SCM_REV=$(shell git rev-parse --short HEAD); \
 	pip3 install -e .
 
 dev: clean uninstall lint build devinstall
 
 SHELL := /bin/bash
 test:
-	python3 -m unittest discover ./tests
+	python3 -m unittest discover -v ./tests
 
 testinstall:
 	docker run --rm python /bin/bash -c "pip3 install hcs-cli && hcs profile"
 
 publish:
 	twine upload --repository hcs-cli dist/*
```

### Comparing `hcs-cli-0.1.36/PKG-INFO` & `hcs-cli-0.1.37/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hcs-cli
-Version: 0.1.36
+Version: 0.1.37
 Summary: Horizon Cloud Service CLI
 Author-email: Nanw1103 <nanw1103@gmail.com>
 Project-URL: Homepage, https://github.com/vmware/horizon-cloud-service-cli
 Project-URL: Bug Tracker, https://github.com/vmware/horizon-cloud-service-cli/issues
 Project-URL: documentation, https://readthedocs.org
 Project-URL: repository, https://github.com/vmware/horizon-cloud-service-cli
 Project-URL: changelog, https://github.com/vmware/horizon-cloud-service-cli/blob/main/CHANGELOG.md
@@ -16,14 +16,16 @@
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: NOTICE
 
 # horizon-cloud-service-cli
 
+[![License](https://img.shields.io/badge/License-Apache%202.0-blue)](https://github.com/vmware-labs/compliance-dashboard-for-kubernetes/blob/main/LICENSE)
+
 ## Overview
 Command line toolbox for [VMware Horizon Cloud Service (HCS) Next-Gen](https://www.vmware.com/products/horizon-cloud.html). It provides human-friendly operations based on HCS REST API.
 
 ## Try it out
 
 
 ### Prerequisites
@@ -60,14 +62,14 @@
 * [Development Setup](doc/dev-setup.md)
 
 * Based on [Context Programming](https://github.com/nanw1103/context-programming)
 
   
 ## Contributing
 
-The horizon-cloud-service-cli project team welcomes contributions from the community. Before you start working with horizon-cloud-service-cli, please read and sign our [Contributor License Agreement CLA](CONTRIBUTING_CLA.md). If you wish to contribute code and you have not signed our contributor license agreement (CLA), our bot will prompt you to do so when you open a Pull Request. For any questions about the CLA process, please refer to our [FAQ]([https://cla.vmware.com/faq](https://cla.vmware.com/faq)).
+The horizon-cloud-service-cli project team welcomes contributions from the community. Before you start working with horizon-cloud-service-cli, please read and sign our Contributor License Agreement [CLA](https://cla.vmware.com/cla/1/preview). If you wish to contribute code and you have not signed our CLA, our bot will prompt you to do so when you open a Pull Request. For any questions about the CLA process, please refer to our [FAQ]([https://cla.vmware.com/faq](https://cla.vmware.com/faq)).
 
 ## License
 
 Apache 2.0
```

### Comparing `hcs-cli-0.1.36/doc/dev-setup.md` & `hcs-cli-0.1.37/doc/dev-setup.md`

 * *Files 5% similar despite different names*

```diff
@@ -158,21 +158,31 @@
 @click.argument("id", type=str, required=True)
 def get(id: str):
     """Get template by ID"""
     return lcm.template.get(id)
 ```
 
 #### Return error with non-zero return code
-If a failure case is encountered, the CLI should return a non-zero return code per convention. The second return value, if exists and is integer, will be used as return value:
+If a failure case is encountered, the CLI should return a non-zero return code per convention. The second return value, if exists and is integer, will be used as return value.
+In such error scenario, the output will be printed to STDERR, instead of STDOUT.
 ```python
 @click.command()
-def myFunc():
-    """This is command help doc"""
+def demoerror():
+    """Demo error return"""
     my_shell_return_code = 123
-    return my_date_to_print, my_shell_return_code
+    return "something wrong", my_shell_return_code
+```
+
+Or alternatively:
+```python
+import vhcs.common.ctxp as ctxp
+@click.command()
+def demoerror():
+    """Demo error return"""
+  return ctxp.error("Only set or get should be specified.")
 ```
 
 By default, if an exception is thrown from a command function, it is considered as error and the CLI will have a non-zero return code.
 
 ### Customize Output
 
 #### Customize Output Format
```

### Comparing `hcs-cli-0.1.36/doc/get-csp-user-api-token.md` & `hcs-cli-0.1.37/doc/get-csp-user-api-token.md`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.36/doc/hcs-cli-cheatsheet.md` & `hcs-cli-0.1.37/doc/hcs-cli-cheatsheet.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,34 +1,41 @@
-# hcs-cli Command Cheatsheet
+# hcs-cli Cheatsheet
 
 ## Utility Commands
 
 ### Profile Commands
 * Profile is a configuration for the target HCS environment you want to access, with the API token or client ID/credential for authentication.
 * HCS CLI has the "profile" subcommand to manage multiple profiles.
 * All HCS CLI commands works with the "current" profile, which can be changed via the profile subcommand.
 * Profiles are nothing but files in ~/.hcs/profiles. You may also edit the files directly.
 
 | Example                                | Purpose                                |
 |----------------------------------------|----------------------------------------|
 | hcs profile init	                     | Initialize a default profile. |
-| hcs profile init --name \<name\>   | Initialize a profile with a custom name. | 
+| hcs profile init --name \<name\>       | Initialize a profile with a custom name. | 
 | hcs profile list	                     | List existing profiles. |
-| hcs profile get	                     | Get content of the current profile. |
-| hcs profile get \<name\>	         | Get a profile by name. |
-| hcs profile use \<name\>	         | Switch to a profile. |
-| hcs profile file \<name\>         | Show the file path of a profile by name. So you can edit the file directly. |
-| hcs profile delete \<name\>        | Delete a profile. |
+| hcs profile get \[name\]	             | Get the current profile, or a specific profile by name. |
+| hcs profile use \<name\>	             | Switch to a profile. |
+| hcs profile delete \<name\>            | Delete a profile. |
+| vi $(hcs profile file)                 | Edit the current profile file directly. |
+| hcs profile file \[name\]              | Show the file path of a profile, current or by name. So you can use the file directly. |
 
-### Auth Commands
+### Login Commands
+
+The login command works with the current profile and will update the current profile. If no token is specified, a browser will be launched to login interactively.
 
 | Example                                | Purpose                                |
 |----------------------------------------|----------------------------------------|
-| hcs auth                               | Get the bearer token that can be used for REST API. |
-| hcs auth --details                     | Get auth token details. |
+| hcs login                              | Interactive login with browser. |
+| hcs login -di                          | Get authentication details. |
+| hcs login --api-token <your-csp-api-token> | Programmatically login with API token. |
+| hcs login --refresh-token <your-csp-api-token> | Programmatically login with OAuth2 refresh token. |
+| hcs login --client-id <client-id> --client-secret <client-secret> | Programmatically login with OAuth client id/secret. |
+| hcs login --bearer <bearer-token> | Programmatically login with bearer token. |
+
 
 ### Context Commands
 * Context is a state store backed by disk files. Context is associated with a profile. Different profiles have different contexts. Context is for supporting automation. E.g. the authentication state is cached using context.
 * Context is similar to the environment variable, and context template utility is like the envsubst command. The difference is, context is persisted and can be reused.
 * Context is internally used to support some complex subcommands which has orchestration and has the need to support break-and-resume.
 
 | Example                                | Purpose                                |
@@ -59,15 +66,16 @@
 | hcs admin edge get \<id\> | Get a specific edge by ID. |
 | hcs admin template list --template-search "providerLocation $eq westus2" | List templates by query. | 
 | hcs admin template get \<id\> | Get a template by ID. |
 
 ### VmHub
 | Example                                | Purpose                                |
 |----------------------------------------|----------------------------------------|
-|                                        |                                        |
+| hcs vmhub otp request                  |                                        |
+| hcs vmhub otp redeem                   |                                        |
 
 
 ### PKI
 | Example                                | Purpose                                |
 |----------------------------------------|----------------------------------------|
 | hcs pki sign-resource-cert my-res1     | Request a resource certificate. |
 | hcs pki get-root-ca                    | Get root CA configured for the target environment. |
```

### Comparing `hcs-cli-0.1.36/hcs_cli.egg-info/PKG-INFO` & `hcs-cli-0.1.37/hcs_cli.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hcs-cli
-Version: 0.1.36
+Version: 0.1.37
 Summary: Horizon Cloud Service CLI
 Author-email: Nanw1103 <nanw1103@gmail.com>
 Project-URL: Homepage, https://github.com/vmware/horizon-cloud-service-cli
 Project-URL: Bug Tracker, https://github.com/vmware/horizon-cloud-service-cli/issues
 Project-URL: documentation, https://readthedocs.org
 Project-URL: repository, https://github.com/vmware/horizon-cloud-service-cli
 Project-URL: changelog, https://github.com/vmware/horizon-cloud-service-cli/blob/main/CHANGELOG.md
@@ -16,14 +16,16 @@
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: NOTICE
 
 # horizon-cloud-service-cli
 
+[![License](https://img.shields.io/badge/License-Apache%202.0-blue)](https://github.com/vmware-labs/compliance-dashboard-for-kubernetes/blob/main/LICENSE)
+
 ## Overview
 Command line toolbox for [VMware Horizon Cloud Service (HCS) Next-Gen](https://www.vmware.com/products/horizon-cloud.html). It provides human-friendly operations based on HCS REST API.
 
 ## Try it out
 
 
 ### Prerequisites
@@ -60,14 +62,14 @@
 * [Development Setup](doc/dev-setup.md)
 
 * Based on [Context Programming](https://github.com/nanw1103/context-programming)
 
   
 ## Contributing
 
-The horizon-cloud-service-cli project team welcomes contributions from the community. Before you start working with horizon-cloud-service-cli, please read and sign our [Contributor License Agreement CLA](CONTRIBUTING_CLA.md). If you wish to contribute code and you have not signed our contributor license agreement (CLA), our bot will prompt you to do so when you open a Pull Request. For any questions about the CLA process, please refer to our [FAQ]([https://cla.vmware.com/faq](https://cla.vmware.com/faq)).
+The horizon-cloud-service-cli project team welcomes contributions from the community. Before you start working with horizon-cloud-service-cli, please read and sign our Contributor License Agreement [CLA](https://cla.vmware.com/cla/1/preview). If you wish to contribute code and you have not signed our CLA, our bot will prompt you to do so when you open a Pull Request. For any questions about the CLA process, please refer to our [FAQ]([https://cla.vmware.com/faq](https://cla.vmware.com/faq)).
 
 ## License
 
 Apache 2.0
```

### Comparing `hcs-cli-0.1.36/payload/lcm/zero.json` & `hcs-cli-0.1.37/payload/lcm/zero.json`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.36/pyproject.toml` & `hcs-cli-0.1.37/pyproject.toml`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.36/setup.py` & `hcs-cli-0.1.37/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 from setuptools_scm import get_version
 import os
 
 with open("requirements.txt") as f:
     requirements = f.read().splitlines()
 
-VERSION = "0.1.36"
+VERSION = "0.1.37"
 
 
 def get_version():
     version = VERSION
     local_version = os.environ.get("SCM_REV")
     if local_version:
         version += "+" + local_version
@@ -33,11 +33,11 @@
 
 
 setup(
     version=get_version(),
     packages=find_packages(),
     install_requires=requirements,
     package_data={
-        "": ["*.yaml"],
+        "": ["*.yaml", "*.yml"],
     },
     include_package_data=True,
 )
```

### Comparing `hcs-cli-0.1.36/tests/conftest.py` & `hcs-cli-0.1.37/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.36/tests/test_utils.py` & `hcs-cli-0.1.37/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.36/tests/vhcs/cli/cmds/pki/get_root_ca.py` & `hcs-cli-0.1.37/tests/vhcs/cli/cmds/pki/get_root_ca.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.36/tests/vhcs/cli/cmds/test_auth.py` & `hcs-cli-0.1.37/tests/vhcs/cli/cmds/test_login.py`

 * *Files 13% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 import unittest
 from test_utils import CliTest
 
 
 class TestAuth(CliTest):
     def test_not_initialized(self):
-        self.verify("hcs auth", "", 1, False)
+        self.verify("hcs login --api-token x", "", 1, False)
 
     def test_details(self):
-        self.verify("hcs auth --details", "", 1, False)
+        self.verify("hcs login --details --info-only", "", 1, False)
 
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `hcs-cli-0.1.36/tests/vhcs/cli/cmds/test_context.py` & `hcs-cli-0.1.37/tests/vhcs/cli/cmds/test_context.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.36/tests/vhcs/cli/cmds/test_profile.py` & `hcs-cli-0.1.37/tests/vhcs/cli/cmds/test_profile.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.36/vhcs/__main__.py` & `hcs-cli-0.1.37/vhcs/__main__.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.36/vhcs/cli/cmds/admin/__init__.py` & `hcs-cli-0.1.37/vhcs/cli/cmds/admin/__init__.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.36/vhcs/cli/cmds/admin/edge/__init__.py` & `hcs-cli-0.1.37/vhcs/cli/cmds/admin/edge/__init__.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.36/vhcs/cli/cmds/admin/edge/get.py` & `hcs-cli-0.1.37/vhcs/cli/cmds/admin/edge/get.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.36/vhcs/cli/cmds/admin/edge/list.py` & `hcs-cli-0.1.37/vhcs/cli/cmds/admin/edge/list.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.36/vhcs/cli/cmds/admin/template/__init__.py` & `hcs-cli-0.1.37/vhcs/cli/cmds/admin/template/__init__.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.36/vhcs/cli/cmds/admin/template/get.py` & `hcs-cli-0.1.37/vhcs/cli/cmds/admin/template/get.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.36/vhcs/cli/cmds/admin/template/list.py` & `hcs-cli-0.1.37/vhcs/cli/cmds/admin/template/list.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,15 +37,15 @@
     help="Ascending/Descending. Format is property,{asc|desc} and default is ascending",
 )
 def list(
     limit: int, org: str, brokerable_only: bool, expanded: bool, reported_search: str, template_search: str, sort: str
 ):
     """List templates"""
     return admin.template.list(
-        limit,
+        limit=limit,
         org_id=get_org_id(org),
         borkerable_only=brokerable_only,
         expanded=expanded,
         reported_search=reported_search,
         template_search=template_search,
         sort=sort,
     )
```

### Comparing `hcs-cli-0.1.36/vhcs/cli/cmds/auth.py` & `hcs-cli-0.1.37/vhcs/cli/cmds/ims/list.py`

 * *Files 17% similar despite different names*

```diff
@@ -10,20 +10,19 @@
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 import click
-import vhcs.common.sglib as sglib
+from vhcs.service import ims_catalog
+from vhcs.common.sglib.util import option_org_id, get_org_id
 
 
 @click.command()
-@click.option("--details/--no-details", default=False)
-@click.option("--refresh/--no-refresh", default=False)
-def auth(details: bool, refresh: bool):
-    """Print the API auth token."""
-    data = sglib.auth.login(force_refresh=refresh)
-    if details:
-        return data
-    else:
-        return data.token
+@click.option("--limit", "-l", type=int, required=False, default=20)
+@option_org_id
+def list(**kwargs):
+    """List images"""
+    return ims_catalog.images.list(
+        **kwargs
+    )
```

### Comparing `hcs-cli-0.1.36/vhcs/cli/cmds/lcm/__init__.py` & `hcs-cli-0.1.37/vhcs/cli/cmds/lcm/__init__.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.36/vhcs/cli/cmds/lcm/provider/__init__.py` & `hcs-cli-0.1.37/vhcs/cli/cmds/lcm/provider/__init__.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.36/vhcs/cli/cmds/lcm/provider/delete.py` & `hcs-cli-0.1.37/vhcs/cli/cmds/lcm/provider/delete.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 import click
-from vhcs.service import lcm
+from vhcs.service.lcm import provider
 
 
 @click.command()
 @click.argument("id", type=str, required=True)
 def delete(id: str):
     """Delete provider by ID"""
-    return lcm.provider.delete(id)
+    return provider.delete(id)
```

### Comparing `hcs-cli-0.1.36/vhcs/cli/cmds/lcm/provider/get.py` & `hcs-cli-0.1.37/vhcs/cli/cmds/lcm/provider/get.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 import click
-from vhcs.service import lcm
+from vhcs.service.lcm import provider
 
 
 @click.command()
 @click.argument("id", type=str, required=True)
 def get(id: str):
     """Get provider by ID"""
-    return lcm.provider.get(id)
+    return provider.get(id)
```

### Comparing `hcs-cli-0.1.36/vhcs/cli/cmds/lcm/provider/list.py` & `hcs-cli-0.1.37/vhcs/cli/cmds/lcm/provider/list.py`

 * *Files 16% similar despite different names*

```diff
@@ -10,18 +10,18 @@
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 import click
-from vhcs.service import lcm
+from vhcs.service.lcm import provider
 from vhcs.common.sglib.util import option_org_id, get_org_id
 
 
 @click.command()
 @option_org_id
 @click.option("--type", "-t", type=str, required=False, help="Optionally, specify cloud provider type.")
 def list(org: str, type: str):
     """List providers"""
     org_id = get_org_id(org)
-    return lcm.provider.list(org_id=org_id, type=type)
+    return provider.list(org_id=org_id, type=type)
```

### Comparing `hcs-cli-0.1.36/vhcs/cli/cmds/lcm/template/__init__.py` & `hcs-cli-0.1.37/vhcs/cli/cmds/lcm/template/__init__.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.36/vhcs/cli/cmds/lcm/template/create.py` & `hcs-cli-0.1.37/vhcs/cli/cmds/lcm/template/create.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.36/vhcs/cli/cmds/lcm/template/delete.py` & `hcs-cli-0.1.37/vhcs/cli/cmds/lcm/template/delete.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,21 +10,21 @@
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 import click
-from vhcs.service import lcm
+from vhcs.service.lcm import template
 from vhcs.common.sglib.util import option_org_id, get_org_id
 
 
 @click.command()
 @click.argument("id", type=str, required=True)
 @option_org_id
 @click.option(
     "--force/--safe", default=True, help="In 'force' mode, the template deletion will continue and ignore any error."
 )
 def delete(id: str, org: str, force: bool):
     """Delete template by ID"""
     org_id = get_org_id(org)
-    return lcm.template.delete(id, org_id, force)
+    return template.delete(id, org_id, force)
```

### Comparing `hcs-cli-0.1.36/vhcs/cli/cmds/lcm/template/get.py` & `hcs-cli-0.1.37/vhcs/cli/cmds/org/datacenter/get.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,18 +10,18 @@
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 import click
-from vhcs.service import lcm
+from vhcs.service.org_service import datacenter
 
 
 @click.command()
 @click.argument("id", type=str, required=True)
 def get(id: str):
-    """Get template by ID"""
-    ret = lcm.template.get(id)
+    """Get datacenter"""
+    ret = datacenter.get(id)
     if ret:
         return ret
     return ret, 1
```

### Comparing `hcs-cli-0.1.36/vhcs/cli/cmds/lcm/template/list.py` & `hcs-cli-0.1.37/vhcs/cli/cmds/lcm/template/list.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 import click
-from vhcs.service import lcm
+from vhcs.service.lcm import template
 from vhcs.common.sglib.util import option_org_id, get_org_id
 from vhcs.common.ctxp.util import option_id_only
 
 
 @click.command("list")
 @click.option(
     "--limit", "-l", type=int, required=False, default=20, help="Optionally, specify the number of records to return."
@@ -26,17 +26,17 @@
 @option_org_id
 @option_id_only
 @click.option("--type", "-t", type=str, required=False, help="Optionally, specify cloud provider type.")
 @click.option("--name", "-n", type=str, required=False, help="Optionally, specify name pattern to find.")
 def list_templates(limit: int, org: str, id_only: bool, type: str, name: str):
     """List templates"""
     if org == "all":
-        ret = lcm.template.list(limit, name=name, type=type)
+        ret = template.list(limit=limit, name=name, type=type)
     else:
-        ret = lcm.template.list(limit, org_id=get_org_id(org), name=name, type=type)
+        ret = template.list(limit=limit, org_id=get_org_id(org), name=name, type=type)
 
     if id_only:
 
         def _get_id_only(t):
             return t.get("id")
 
         return list(map(_get_id_only, ret))
```

### Comparing `hcs-cli-0.1.36/vhcs/cli/cmds/lcm/template/wait.py` & `hcs-cli-0.1.37/vhcs/cli/cmds/lcm/template/wait.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.36/vhcs/cli/cmds/lcm/test.py` & `hcs-cli-0.1.37/vhcs/cli/cmds/daas/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -9,14 +9,8 @@
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
-import click
-from vhcs.service import lcm
-
-
-@click.command(hidden=True)
-def test():
-    return lcm.test()
+help = "Desktop-as-a-Service Operations."
```

### Comparing `hcs-cli-0.1.36/vhcs/cli/cmds/org/datacenter/get.py` & `hcs-cli-0.1.37/vhcs/cli/cmds/org/detail/get.py`

 * *Files 14% similar despite different names*

```diff
@@ -10,18 +10,20 @@
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 import click
-from vhcs.service import org_service
+from vhcs.service.org_service import details
+from vhcs.common.sglib.util import option_org_id, get_org_id
 
 
 @click.command()
-@click.argument("id", type=str, required=True)
-def get(id: str):
-    """Get datacenter"""
-    ret = org_service.datacenter.get(id)
+@option_org_id
+def get(org: str):
+    """Get org details"""
+    org_id = get_org_id(org)
+    ret = details.get(org_id)
     if ret:
         return ret
     return ret, 1
```

### Comparing `hcs-cli-0.1.36/vhcs/cli/cmds/org/datacenter/list.py` & `hcs-cli-0.1.37/vhcs/cli/cmds/org/datacenter/list.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,23 +10,23 @@
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 import click
-from vhcs.service import org_service
+from vhcs.service.org_service import datacenter
 from vhcs.common.sglib.util import option_org_id, get_org_id
 
 
 @click.command("list")
 @option_org_id
 def list_datacenters(org: str):
     """List all datacenters"""
 
     if org == "" or org == "all":
-        ret = org_service.datacenter.list()
+        ret = datacenter.list()
     else:
         org_id = get_org_id(org)
-        return org_service.datacenter.find_by_org(org_id)
+        return datacenter.find_by_org(org_id)
 
     return ret
```

### Comparing `hcs-cli-0.1.36/vhcs/cli/cmds/org/detail/get.py` & `hcs-cli-0.1.37/vhcs/cli/cmds/pki/get_org_cert.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,20 +10,17 @@
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 import click
-from vhcs.service import org_service
+from vhcs.service.pki import certificate
 from vhcs.common.sglib.util import option_org_id, get_org_id
 
 
 @click.command()
 @option_org_id
-def get(org: str):
-    """Get org details"""
+def get_org_cert(org: str):
+    """Get the signing certificate of a specific org"""
     org_id = get_org_id(org)
-    ret = org_service.details.get(org_id)
-    if ret:
-        return ret
-    return ret, 1
+    return certificate.get_org_cert(org_id)
```

### Comparing `hcs-cli-0.1.36/vhcs/cli/cmds/org/detail/list.py` & `hcs-cli-0.1.37/vhcs/cli/cmds/org/detail/list.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 import click
-from vhcs.service import org_service
+from vhcs.service.org_service import details
 
 
 @click.command("list")
 @click.option(
     "--limit", "-l", type=int, required=False, default=20, help="Optionally, specify the number of records to return."
 )
 @click.option(
@@ -26,9 +26,9 @@
     "-s",
     type=str,
     required=False,
     help="Specify the REST-search string. E.g. 'orgId $eq 21eb79bc-f737-479f-b790-7753da55f363 AND orgName $like VMW'. Note, in bash/sh/zsh, use single quote.",
 )
 def list_org_details(limit: int, search: str):
     """List all org details"""
-    ret = org_service.details.list(limit=limit, search=search)
+    ret = details.list(limit=limit, search=search)
     return ret
```

### Comparing `hcs-cli-0.1.36/vhcs/cli/cmds/pki/__init__.py` & `hcs-cli-0.1.37/vhcs/cli/cmds/pki/__init__.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.36/vhcs/cli/cmds/pki/delete_org_cert.py` & `hcs-cli-0.1.37/vhcs/cli/cmds/pki/delete_org_cert.py`

 * *Files 14% similar despite different names*

```diff
@@ -11,21 +11,21 @@
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 import click
 from vhcs.common.ctxp import panic
-from vhcs.service import pki
+from vhcs.service.pki import certificate
 from vhcs.common.sglib.util import option_org_id, get_org_id
 
 
 @click.command()
 @option_org_id
 @click.option("--confirm/--no-confirm", default=False)
 def delete_org_cert(org: str, confirm: bool):
     """Delete the signing certificate of a specific org"""
 
     if not confirm:
         panic('Delete an org certificate will impact some service. Specify "--confirm" to perform the deletion.')
     org_id = get_org_id(org)
-    return pki.delete_org_cert(org_id)
+    return certificate.delete_org_cert(org_id)
```

### Comparing `hcs-cli-0.1.36/vhcs/cli/cmds/pki/get_org_cert.py` & `hcs-cli-0.1.37/vhcs/plan/provider/hcs/entitlement.py`

 * *Files 21% similar despite different names*

```diff
@@ -9,18 +9,12 @@
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
-import click
-from vhcs.service import pki
-from vhcs.common.sglib.util import option_org_id, get_org_id
+def deploy(data: dict) -> dict:
+    return {}
 
-
-@click.command()
-@option_org_id
-def get_org_cert(org: str):
-    """Get the signing certificate of a specific org"""
-    org_id = get_org_id(org)
-    return pki.get_org_cert(org_id)
+def destroy(data: dict, prev: dict) -> dict:
+    return {}
```

### Comparing `hcs-cli-0.1.36/vhcs/cli/cmds/pki/get_root_ca.py` & `hcs-cli-0.1.37/vhcs/cli/cmds/daas/infra/validate.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 import click
-from vhcs.service import pki
+import vhcs.common.ctxp as ctxp
 
+_config_name = "daas-infra"
 
 @click.command()
-def get_root_ca():
-    """Get the certificate of the root CA."""
-    return pki.get_root_ca()
+def validate():
+    """Validate the infra config"""
+
```

### Comparing `hcs-cli-0.1.36/vhcs/cli/cmds/pki/sign_resource_cert.py` & `hcs-cli-0.1.37/vhcs/cli/cmds/pki/sign_resource_cert.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 import click
 from vhcs.common.ctxp import profile
-from vhcs.service import pki
+from vhcs.service.pki import certificate
 from vhcs.util import pki_util
 from vhcs.common.sglib.util import option_org_id, get_org_id
 
 
 def _write_file(file_path: str, text: str):
     with open(file_path, "w") as file:
         file.write(text)
@@ -35,15 +35,15 @@
     help="Private key length",
 )
 @option_org_id
 def sign_resource_cert(resource_name: str, key_length: int, org: str):
     """Get the certificate for a specific resource"""
     org_id = get_org_id(org)
     csr_pem, private_key_pem = pki_util.generate_CSR(resource_name, key_length=key_length)
-    ret = pki.sign_resource_cert(org_id, csr_pem)
+    ret = certificate.sign_resource_cert(org_id, csr_pem)
 
     long_name = f"{profile.name()}-{org_id}-{resource_name}"
     key_file = resource_name + ".key"
     print("Private key (generated by CLI): " + key_file)
     _write_file(key_file, private_key_pem)
 
     client_cert_chain_file = long_name + ".crt"
```

### Comparing `hcs-cli-0.1.36/vhcs/cli/cmds/pki/test.py` & `hcs-cli-0.1.37/vhcs/cli/cmds/pki/get_root_ca.py`

 * *Files 18% similar despite different names*

```diff
@@ -10,13 +10,14 @@
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 import click
-from vhcs.service import pki
+from vhcs.service.pki import certificate
 
 
-@click.command(hidden=True)
-def test():
-    return pki.test()
+@click.command()
+def get_root_ca():
+    """Get the certificate of the root CA."""
+    return certificate.get_root_ca()
```

### Comparing `hcs-cli-0.1.36/vhcs/cli/cmds/test.py` & `hcs-cli-0.1.37/vhcs/cli/cmds/pki/test.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,15 +10,13 @@
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 import click
-
-from vhcs.common.ctxp.util import option_field
+from vhcs.service.pki import certificate
 
 
 @click.command(hidden=True)
-@click.argument("id", type=str, required=True)
-def test(id: str):
-    print(id)
+def test():
+    return certificate.test()
```

### Comparing `hcs-cli-0.1.36/vhcs/cli/cmds/upgrade.py` & `hcs-cli-0.1.37/vhcs/cli/cmds/upgrade.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.36/vhcs/cli/cmds/vmhub/__init__.py` & `hcs-cli-0.1.37/vhcs/cli/cmds/vmhub/__init__.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.36/vhcs/cli/cmds/vmhub/redeem-otp.py` & `hcs-cli-0.1.37/vhcs/cli/cmds/vmhub/otp/redeem.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,30 +10,30 @@
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 import click
-from vhcs.service import vmhub
+from vhcs.service.vmhub import otp
 from vhcs.util import pki_util
 
 
 @click.command()
 @click.option(
     "--region",
     type=str,
     default=None,
     required=False,
     help="Specify region name",
 )
 @click.argument("resource-name", type=str, required=True)
 @click.argument("otp", type=str, required=True)
-def redeem_otp(region: str, resource_name: str, otp: str):
+def redeem(region: str, resource_name: str, otp: str):
     """Redeem OTP with CSR, receive resource cert."""
 
-    vmhub.use_region(region)
+    otp.use_region(region)
     csr_pem, private_key_pem = pki_util.generate_CSR(resource_name)
 
-    ret = vmhub.redeem_otp(resource_name, otp, csr_pem)
+    ret = otp.redeem_otp(resource_name, otp, csr_pem)
     ret.private_key = private_key_pem
     return ret
```

### Comparing `hcs-cli-0.1.36/vhcs/cli/cmds/vmhub/request-otp.py` & `hcs-cli-0.1.37/vhcs/cli/cmds/vmhub/otp/request.py`

 * *Files 11% similar despite different names*

```diff
@@ -11,25 +11,25 @@
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 import click
 from vhcs.common.sglib.util import option_org_id, get_org_id
-from vhcs.service import vmhub
+from vhcs.service.vmhub import otp
 
 
 @click.command()
 @option_org_id
 @click.option(
     "--region",
     type=str,
     default=None,
     required=False,
     help="Specify region name",
 )
 @click.argument("resource-name", type=str, required=True)
-def request_otp(org: str, region: str, resource_name: str):
+def request(org: str, region: str, resource_name: str):
     """Request an one-time password for a specific resource"""
     org_id = get_org_id(org)
-    vmhub.use_region(region)
-    return vmhub.request_otp(org_id, resource_name)
+    otp.use_region(region)
+    return otp.request_otp(org_id, resource_name)
```

### Comparing `hcs-cli-0.1.36/vhcs/cli/cmds/vmhub/test.py` & `hcs-cli-0.1.37/vhcs/common/sglib/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,14 +9,9 @@
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
-import click
-from vhcs.service import vmhub
-
-
-@click.command(hidden=True)
-def test():
-    return vmhub.test()
+from . import auth
+from .hcs_client import hcs_client
```

### Comparing `hcs-cli-0.1.36/vhcs/cli/main.py` & `hcs-cli-0.1.37/vhcs/cli/main.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.36/vhcs/common/ctxp/README.md` & `hcs-cli-0.1.37/vhcs/common/ctxp/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,68 +1,58 @@
 
 
 This is an implementation of [Context Programming](https://github.com/nanw1103/context-programming), for CLI program.
 
-It has the following configuration data structure, to support multiple CLIs, and multiple profiles per CLI.
+This implementation has the following configuration data structure, to support:
+- Multiple command line tools in the same OS.
+- Multiple profiles per tool.
+- Context (and other context-like collections) per profile.
 
 ```
 <repo-path>
     <cli-name-1>
-        profile
-            default
-            <profile-name-11>.yml
-            <profile-name-12>.yml
-            ...
-        context
-            <profile-name-11>
+        .state      # CLI specific global runtime state
+        <profile-name-11>
+            profile.yml
+            context
                 <application-specific-data-111>.yml
                 <application-specific-data-112>.yml
-                ...
-            <profile-name-12>
-                <application-specific-data-121>.yml
-                <application-specific-data-122>.yml
-                ...
-            ...
+            <other profile store 1>
+                <file11>
+            <other profile store 2>
+                <file21>
+                <file22>
+        <profile-name-12>.yml
+        ...
     <cli-name-2>
-        profile
-            default
-            <profile-name-21>.yml
-            <profile-name-22>.yml
-            ...
-        context
-            <profile-name-21>
-                <application-specific-data-211>.yml
-                <application-specific-data-212>.yml
-                ...
-            <profile-name-22>
-                <application-specific-data-221>.yml
-                <application-specific-data-222>.yml
-                ...
-            ...
+        ... # The same structure as cli-name-1
     ...
 ```
 
-The efault repo-path is: <user-home-dir>/<cli-name>
+The default repo-path is: <user-home-dir>/<cli-name>
 Take two different CLI programs _helloctl_ and _kittyctl_ as examples. Each of them may have multiple environments. By default the structure will be:
 
 ```
 ~
     helloctl
-        profile
-            default
-            my-hello-env1.yml
-            my-hello-env2.yml
-        context
-            my-hello-env1
-                my-data1.yml
-                my-data2.yml
-            my-hello-env2
-                my-data1.yml
+        .state
+        default
+            profile.yml
+            context
+                my-data11.yml
+                my-data12.yml
+        my-hello-env1
+            profile.yml
+            context
+                my-data21.yml
+        my-hello-env2
+            profile.yml
+            context <empty>
     kittyctl
-        profile
-            default
-            my-kitty-env.yml
-        context
-            my-kitty-env
+        .state
+        default
+            profile.yml
+        my-kitty-env
+            context
                 my-data1.yml
 ```
```

### Comparing `hcs-cli-0.1.36/vhcs/common/ctxp/__init__.py` & `hcs-cli-0.1.37/vhcs/common/ctxp/config.py`

 * *Files 19% similar despite different names*

```diff
@@ -9,10 +9,24 @@
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
-from ._init import init
-from .util import panic, CtxpException
-from . import profile, config, var_template
+from .jsondot import dotdict
+from .fstore import fstore
+
+_store_impl: fstore = None
+
+
+def init(config_path: str) -> None:
+    global _store_impl
+    _store_impl = fstore(config_path)
+
+
+def get(name: str, reload: bool = False) -> dotdict:
+    return _store_impl.get(name, reload)
+
+
+def list() -> list[str]:
+    return _store_impl.keys()
```

### Comparing `hcs-cli-0.1.36/vhcs/common/ctxp/_init.py` & `hcs-cli-0.1.37/vhcs/common/ctxp/_init.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,13 +28,12 @@
     cli_name: str,
     main_cli: click.Group,
     commands_dir: str = "./cmds",
     store_path: str = user_home,
     config_path="./config",
 ):
     real_store_path = path.join(store_path, "." + cli_name)
-    profile_path = path.join(real_store_path, "profile")
-    profile.init(profile_path)
-    state._init(real_store_path, ".state")
-    config._init(config_path)
+    state.init(real_store_path, ".state")
+    profile.init(real_store_path)
+    config.init(config_path)
 
     return cli_processor.init(main_cli, commands_dir)
```

### Comparing `hcs-cli-0.1.36/vhcs/common/ctxp/built_in_cmds/context.py` & `hcs-cli-0.1.37/vhcs/common/ctxp/built_in_cmds/context.py`

 * *Files 20% similar despite different names*

```diff
@@ -10,60 +10,77 @@
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 import click
+import os
+import subprocess
 import vhcs.common.ctxp as ctxp
-
+import vhcs.common.ctxp.util as util
 
 @click.group(cls=ctxp.cli_processor.LazyGroup)
 def context():
-    """Commands for context, for the current profile."""
+    """Commands for context. Each profile has its own context. The commands work for the current profile."""
 
 
 @context.command()
 def list():
-    """List all context item names, for the current profile."""
+    """List all context item names."""
     return ctxp.context.list()
 
 
 @context.command()
 @click.argument("name")
 @click.argument("key", required=False)
 def get(name: str, key: str):
-    """Get data of a specific context object, for the current profile."""
+    """Get data of a specific context object."""
     data = ctxp.context.get(name)
 
     if key is None:
         return data
     if data is None:
         return None
     return data.get(key)
 
 
 @context.command()
 @click.argument("name")
 @click.argument("key_value")  #'key value pair, example: k1=v1'
 def set(name: str, key_value: str):
-    """Set a context object by name, for the current profile."""
+    """Set a context object by name."""
     parts = key_value.split("=")
     if len(parts) != 2:
         ctxp.panic("Invalid KEY_VALUE format. Valid example: key1=value1")
     k, v = parts
     data = ctxp.context.get(name, default={})
     data[k] = v
     ctxp.context.set(name, data)
 
 
 @context.command()
 @click.argument("name")
 def delete(name: str):
-    """Delete a context object by name, for the current profile."""
+    """Delete a context object by name."""
     ctxp.context.delete(name)
 
 
 @context.command()
 def clear():
-    """Delete all context objects, for the current profile."""
+    """Delete all context objects."""
     ctxp.context.clear()
+
+@context.command()
+@click.argument("name", type=str, required = True)
+def file(name: str):
+    """Get the file path of the specific context object."""
+    return _get_file(name)
+
+def _get_file(name: str) -> str:
+    return ctxp.context._store()._get_path(name)
+
+@context.command()
+@click.argument("name", type=str, required = True)
+def edit(name : str):
+    """Launch platform-specific editor to edit a context file."""
+    util.launch_text_editor(_get_file(name))
```

### Comparing `hcs-cli-0.1.36/vhcs/common/ctxp/built_in_cmds/profile.py` & `hcs-cli-0.1.37/vhcs/common/ctxp/built_in_cmds/profile.py`

 * *Files 27% similar despite different names*

```diff
@@ -12,71 +12,101 @@
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 import click
 import sys
 import json
-import vhcs.common.ctxp as ctxp
+import questionary
+from vhcs.common.ctxp import util, panic, profile, cli_processor
 
 
-@click.group(cls=ctxp.cli_processor.LazyGroup)
-def profile():
+@click.group(name='profile', cls=cli_processor.LazyGroup)
+def profile_cmd_group():
     """Commands for profile."""
 
 
-@profile.command()
+@profile_cmd_group.command()
 def list():
     """List all profile names."""
-    return ctxp.profile.list()
+    return profile.names()
 
 
-@profile.command()
-@click.argument("name")
+@profile_cmd_group.command()
+@click.argument("name", required=False)
 def use(name: str):
-    """Switch to a specific profile."""
-    success = ctxp.profile.use(name) != None
-
-    if not success:
-        ctxp.panic("No such profile: " + name)
-
+    """Switch to a specific profile. If no name specified, launch interactive list to choose profile."""
+    
+    if name:
+        if profile.use(name) == None:
+            panic("No such profile: " + name)
+    else:
+        current = profile.name()
+        choices = profile.names()
+        if not choices:
+            panic('No profile available.')
+
+        ret = questionary.select("Select profile", choices, default=current, show_selected=True).ask()
+        if ret:
+            if profile.use(ret) == None:
+                panic("No such profile: " + name)
+        else:
+            # aborted
+            return "", 1
+    
+@profile_cmd_group.command()
+@click.argument("from-name", required=True)
+@click.argument("to-name", required=True)
+def copy(from_name: str, to_name: str):
+    """Copy profile."""
+    
+    data = profile.get(from_name)
+    if not data:
+        panic("No such profile: " + from_name)
+    if profile.exists(to_name):
+        panic("Profile already exists: " + to_name)
+    profile.create(to_name, data, True)
 
-@profile.command()
+@profile_cmd_group.command()
 @click.argument("name", required=False)
 def get(name: str):
     """Get content of a specific profile."""
     if name:
-        data = ctxp.profile.get(name)
+        data = profile.get(name)
+        if data == None:
+            panic(
+                "Profile not found. Use 'hcs profile list' to show available profiles, or 'hcs profile init' to create one."
+            )
     else:
-        data = ctxp.profile.current()
+        data = profile.current()
+        if data == None:
+            panic(
+                "Default profile not set. Use 'hcs profile list' to show available profiles, 'hcs profile user <name>' to switch to a profile, or 'hcs profile init' to create one."
+            )
 
-    if data == None:
-        ctxp.panic(
-            "Profile not set. Use 'hcs profile use <profile-name>' to choose one, or 'hcs profile init' to create."
-        )
     return data
 
 
-@profile.command()
+@profile_cmd_group.command()
 @click.argument("name")
 def delete(name: str):
     """Delete a profile by name."""
-    ctxp.profile.delete(name)
+    profile.delete(name)
 
 
-@profile.command()
+@profile_cmd_group.command()
 @click.argument("name", required=False)
 def file(name: str):
     """Show file location of a profile by name."""
     if not name:
-        name = ctxp.profile.name()
-    return ctxp.profile.file(name)
+        name = profile.name()
+    return profile.file(name)
 
 
-@profile.command()
+@profile_cmd_group.command()
 @click.argument("name", type=str)
 @click.option(
     "--file",
     "-f",
     type=click.File("rt"),
     default=sys.stdin,
     help="Specify the template file name. If not specified, STDIN will be used.",
@@ -84,10 +114,25 @@
 def create(name: str, file):
     """Create a profile from file or STDIN."""
     with file:
         text = file.read()
     try:
         data = json.loads(text)
     except Exception as e:
-        ctxp.panic(f"Invalid json {e}")
+        panic(f"Invalid json {e}")
+
+    profile.create(name, data)
 
-    return ctxp.profile.create(name, data)
+@profile_cmd_group.command()
+def name():
+    """Get current profile name."""
+    return profile.name()
+
+@profile_cmd_group.command()
+@click.argument("name", type=str, required = False)
+def edit(name : str):
+    """Launch platform-specific editor to edit the profile file."""
+
+    if not name:
+        name = profile.name()
+    file_name = profile.file(name)
+    util.launch_text_editor(file_name)
```

### Comparing `hcs-cli-0.1.36/vhcs/common/ctxp/cli_processor.py` & `hcs-cli-0.1.37/vhcs/common/ctxp/cli_processor.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 import yaml
 from click.core import Group
 import os.path as path
 import os
 import importlib
 import importlib.util
 from pathlib import Path
-from .util import print_output
+from .util import print_output, print_error, validate_error_return
 
 _eager_loading = os.environ.get("_CTXP_EAGER_LOAD")
 if _eager_loading:
     print("_CTXP_EAGER_LOAD:", _eager_loading, file=sys.stderr)
 
 
 class LazyGroup(click.Group):
@@ -68,19 +68,28 @@
 
     subgroup = LazyGroup(name=name, help=help, mod_path=mod_path)
     current.add_command(subgroup)
     return subgroup
 
 
 def _read_group_meta(mod_path: Path) -> dict:
-    meta_file = mod_path.absolute().joinpath("meta.yaml")
-    if not meta_file.exists():
-        return {}
-    with open(meta_file, "r") as f:
-        return yaml.safe_load(f)
+    meta_file = mod_path.absolute().joinpath("__init__.py")
+    
+    ret = {
+        'help': None,
+        'hidden': False
+    }
+    if meta_file.exists():
+        # TODO
+        with open(meta_file, "r") as f:
+            lines = f.readlines()
+
+    return ret
+
+
 
 
 _excluded_names = ["__pycache__", "__init__.py", ".DS_Store"]
 
 
 def _add_subcommands(commands_dir: str, group: Group):
     for mod_path in Path(commands_dir).glob("*"):
@@ -119,26 +128,37 @@
 
     for foo in cli_methods:
         if isinstance(foo, click.core.Command):
             parent.add_command(foo)
 
 
 def _process_result(result, **kwargs):
-    if result is not None:
-        if isinstance(result, tuple):
-            data, return_code = result
-            if data is not None:
-                print_output(data, kwargs.get("output"), kwargs.get("field"))
-            if isinstance(return_code, int):
-                ctx = click.get_current_context()
-                ctx.exit(return_code)
+    if result is None:
+        return
+    if isinstance(result, tuple):
+        data, return_code = result
+
+        is_error = isinstance(data, Exception) or return_code != None
+        if is_error:
+            if return_code == None:
+                return_code = 1
+            validate_error_return(data, return_code)
+            if isinstance(data, Exception):
+                print_error(data)
             else:
-                raise Exception("Invalid command return code. Expect int, actual=" + str(type(return_code)))
-        else:
-            print_output(result, kwargs.get("output"), kwargs.get("field"))
+                print_output(data, kwargs.get("output"), kwargs.get("field"), file=sys.stderr)
+            ctx = click.get_current_context()
+            ctx.exit(return_code)
+        #else fall-through
+    elif isinstance(result, Exception):
+        print_error(result)
+        ctx = click.get_current_context()
+        ctx.exit(1)
+    else:
+        print_output(result, kwargs.get("output"), kwargs.get("field"))
 
 
 def init(main_cli: click.Group, commands_dir: str):
     _add_built_in_commands(main_cli)
     _add_subcommands(commands_dir, main_cli)
     main_cli.result_callback()(_process_result)
     return main_cli(obj={})
```

### Comparing `hcs-cli-0.1.36/vhcs/common/ctxp/config.py` & `hcs-cli-0.1.37/vhcs/cli/cmds/daas/tenant/destroy.py`

 * *Files 25% similar despite different names*

```diff
@@ -9,24 +9,29 @@
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
-from .jsondot import dotdict
-from .fstore import fstore
+import yaml
+import click
+from vhcs.support.daas import destroyer
+from vhcs.common.ctxp import context, panic
+
+@click.command()
+@click.option("--file", "-f", type=str, required=True)
+@click.option("--confirm/--no-confirm", "-c", type=bool, required=False, help="Confirm destroy of the tenant.")
+def destroy(file: str, confirm: bool):
+    """Delete a tenant"""
+
+    if not confirm:
+        panic("The destroy operation will delete all resources allocated for the tenant. Specify additional parameter '--confirm' to proceed.")
+
+    with open(file, "r") as file:
+        payload = file.read()
+    tenant_request = yaml.safe_load(payload)
+    tenant_id = tenant_request['tenantId']
 
-_store_impl: fstore = None
+    print('Destroying tenant:', tenant_id)
 
-
-def _init(config_path: str) -> None:
-    global _store_impl
-    _store_impl = fstore(config_path)
-
-
-def get(name: str, reload: bool = False) -> dotdict:
-    return _store_impl.get(name, reload)
-
-
-def list() -> list[str]:
-    return _store_impl.keys()
+    return destroyer.destroy(tenant_request)
```

### Comparing `hcs-cli-0.1.36/vhcs/common/ctxp/context.py` & `hcs-cli-0.1.37/vhcs/common/ctxp/profile_store.py`

 * *Files 17% similar despite different names*

```diff
@@ -9,74 +9,41 @@
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
+# Profile_store provides a utility method to create profile-scoped fstore
+
 import os
-from .jsondot import dotdict
 from . import profile
 from .fstore import fstore
 from .util import CtxpException
 
-
-_store_impl: fstore = None
-_plain_profile: dict = None
+_store_map: dict[str, fstore] = {}
 _active_profile_name: str = None
 
 
-def _store():
-    global _store_impl, _active_profile_name, _plain_profile, _variables
+def profile_store(store_name : str) -> fstore:
+    global _store_map, _active_profile_name
 
     profile_name = profile.name()
     if not profile_name:
         raise CtxpException("Profile not specified")
 
     if profile_name != _active_profile_name:
+        # profile changed
         _active_profile_name = profile_name
-        _store_impl = None
-
-    if _store_impl == None:
-        _store_impl = _context_store_from_profile_name(profile_name)
-        _plain_profile = None
-        _variables = None
-    return _store_impl
-
-
-def _context_store_from_profile_name(profile_name: str) -> fstore:
-    profile_path = profile.path()
-    if profile_path is None:
-        return fstore(store_path=None)  # RAM only. No file persist
-
-    profile_dir = os.path.dirname(profile.path())
-    repo_dir = os.path.dirname(profile_dir)
-    context_dir = os.path.join(repo_dir, "context", profile_name)
-    return fstore(context_dir)
-
-
-def list() -> list[str]:
-    return _store().keys()
-
-
-def get(name: str, reload: bool = False, default=None) -> dotdict:
-    return _store().get(key=name, reload=reload, default=default)
-
-
-def set(name: str, data: dict):
-    return _store().save(name, data)
-
-
-def delete(name: str):
-    return _store().delete(name)
-
+        _store_map = {}
 
-def clear():
-    return _store().clear()
+    ret = _store_map.get(store_name)
+    if ret == None:
+        ret = _store_from_profile_name(profile_name, store_name)
+        _store_map[store_name] = ret
+    return ret
 
 
-def destroy(profile_name: str):
-    if profile.name() == profile_name:
-        _store().destroy()
-    else:
-        store = _context_store_from_profile_name(profile_name)
-        store.destroy()
+def _store_from_profile_name(profile_name: str, store_name: str) -> fstore:
+    profile_path = profile.path(profile_name)
+    store_path = os.path.join(profile_path, store_name)
+    return fstore(store_path)
```

### Comparing `hcs-cli-0.1.36/vhcs/common/ctxp/fstore.py` & `hcs-cli-0.1.37/vhcs/common/ctxp/fstore.py`

 * *Files 2% similar despite different names*

```diff
@@ -114,15 +114,15 @@
             data = _load_file(file_path, format)
             if data != None:
                 self._cache[key] = data
         else:
             data = self._cache.get(key)
 
         if data is None and default is not None:
-            return default
+            return jsondot.dotify(default)
         return data
 
     def _get_path(self, key: str) -> str:
         if not self._path:
             return None
         return path.join(self._path, key)
 
@@ -164,21 +164,25 @@
                 os.remove(file_path)
 
     def keys(self) -> list[str]:
         if self._path:
             return [f for f in listdir(self._path) if path.isfile(path.join(self._path, f))]
         return list(self._cache.keys())
 
+    def values(self) -> Generator[Any, None, None]:
+        for k in self.keys():
+            yield self.get(k)
+
     def items(self) -> Generator[tuple[str, dict], None, None]:
-        for key in self.keys():
-            yield (key, self.get(key))
+        for k in self.keys():
+            yield (k, self.get(k))
 
     def clear(self) -> None:
-        for key in self.keys():
-            self.delete(key)
+        for k in self.keys():
+            self.delete(k)
 
     def destroy(self) -> None:
         self._cache.clear()
         if self._path:
             import shutil
 
             shutil.rmtree(self._path)
```

### Comparing `hcs-cli-0.1.36/vhcs/common/ctxp/init.py` & `hcs-cli-0.1.37/vhcs/common/ctxp/init.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.36/vhcs/common/ctxp/jsondot.py` & `hcs-cli-0.1.37/vhcs/common/ctxp/jsondot.py`

 * *Files 2% similar despite different names*

```diff
@@ -97,10 +97,10 @@
     dict = json.loads(text)
     return dotify(dict)
 
 
 def save(data: dict, file, format=True) -> None:
     with open(file, "w") as outfile:
         if format:
-            json.dump(data, outfile, indent="\t")
+            json.dump(data, outfile, indent="\t", default=vars)
         else:
             json.dump(data, outfile)
```

### Comparing `hcs-cli-0.1.36/vhcs/common/ctxp/state.py` & `hcs-cli-0.1.37/vhcs/common/ctxp/state.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,43 +9,44 @@
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
-from . import jsondot
+import pathlib
 from typing import Any
 import os
+from . import jsondot
 
-
-class state_file:
+class _StateFile:
     def __init__(self, file_path: str):
         self._path = file_path
         self._cache = None
-
+        pathlib.Path(os.path.dirname(file_path)).mkdir(parents=True, exist_ok=True)
+        
     def _data(self, reload: bool = False):
         if self._cache is None or reload:
             self._cache = jsondot.load(self._path, {})
         return self._cache
 
     def get(self, key: str, default: Any, reload: bool = False):
         return self._data(reload).get(key, default)
 
     def set(self, key: str, value: Any):
         self._data()[key] = value
         jsondot.save(self._cache, self._path)
 
 
-_file: state_file = None
+_file: _StateFile = None
 
 
-def _init(store_path: str, name: str):
+def init(store_path: str, name: str):
     global _file
-    _file = state_file(os.path.join(store_path, name))
+    _file = _StateFile(os.path.join(store_path, name))
 
 
 def get(key: str, default: Any, reload: bool = False):
     return _file.get(key=key, default=default, reload=reload)
 
 
 def set(key: str, value: Any):
```

### Comparing `hcs-cli-0.1.36/vhcs/common/ctxp/util.py` & `hcs-cli-0.1.37/vhcs/support/daas/tenant.py`

 * *Files 26% similar despite different names*

```diff
@@ -9,102 +9,69 @@
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
-import json
-import yaml
-import sys
-import click
-from typing import Any
-
-
-class CtxpException(Exception):
-    pass
-
-
-def print_output(data: Any, output: str = "json", fields: str = None):
-    if type(data) is str:
-        text = data
-    else:
-        _filter_fields(data, fields)
-
-        if output == "json":
-            text = json.dumps(data, indent=4)
-        elif output == "json-compact":
-            text = json.dumps(data)
-        elif output == "yaml":
-            import vhcs.common.ctxp as ctxp
-
-            text = yaml.dump(ctxp.jsondot.plain(data))
-        elif output == "text":
-            if isinstance(data, list):
-                text = ""
-                for i in data:
-                    line = i if type(i) is str else json.dumps(i)
-                    text += line + "\n"
-            elif isinstance(data, dict):
-                text = json.dumps(data, indent=4)
-            else:
-                text = json.dumps(data, indent=4)
-        else:
-            raise Exception(f"Unexpected output format: {output}")
-
-    print(text, end="")
-
-
-def _filter_fields(obj: Any, fields: str):
-    if not fields:
-        return obj
-    parts = fields.split(",")
-
-    def _filter_obj(o):
-        if not isinstance(o, dict):
-            return o
-        for k in list(o.keys()):
-            if k not in parts:
-                del o[k]
-        return o
-
-    if isinstance(obj, list):
-        return list(map(_filter_obj, obj))
-    return _filter_obj(obj)
-
-
-def panic(reason: Any = None, code: int = 1):
-    print(reason, file=sys.stderr)
-    sys.exit(code)
-
-
-option_verbose = click.option(
-    "-v",
-    "--verbose",
-    count=True,
-    default=0,
-    help="Print debug logs",
-)
-
-option_output = click.option(
-    "-o",
-    "--output",
-    type=click.Choice(["json", "json-compact", "yaml", "text"]),
-    default="json",
-    help="Specify output format",
-)
-
-option_field = click.option(
-    "-f",
-    "--field",
-    type=str,
-    required=False,
-    help="Specify fields to output",
-)
-
-option_id_only = click.option(
-    "--id-only/--full-object",
-    type=bool,
-    default=False,
-    required=False,
-    help="Output only the object, instead of the full data object",
-)
+from ulid import ULID
+import vhcs.common.ctxp as ctxp
+
+def _store() -> ctxp.fstore:
+    return ctxp.profile_store('daas-tenant')
+
+_config_template = {
+    "id": "",
+    "customerName": "",
+    "applicationId": "",
+    "applicationSecret": "",
+    "desktopName": "",
+    "groupName": "",
+    "markerId": "",
+    "orgId": "",
+    "providerInstanceId": "",
+    "streamId": "",
+    "templateType": "",
+    "userEmails": "",
+    "vmSkuName": ""
+}
+
+def _with_default(target : dict, default : dict) -> dict:
+    ret = dict(default)
+    if target:
+        ret.update(target)
+    return ret
+
+def list():
+    return _store().values()
+
+def names():
+    ret = []
+    for v in list():
+        ret.append(v['customerName'])
+    return ret
+
+def ids():
+    return _store().keys()
+
+def get(id: str):
+    return _store().get(id)
+
+def find_by_customer_name(customer_name: str):
+    for doc in list():
+        if doc['customerName'] == customer_name:
+            return doc
+
+def save(id: str, data: dict):
+    return _store().save(id, data)
+
+def delete(id: str):
+    return _store().delete(id)
+
+def create(customer_name: str):
+    data = find_by_customer_name(customer_name)
+    if data:
+        raise ctxp.CtxpException("A tenant with that name already exists.")
+    data = _with_default(data, _config_template)
+    data['id'] = str(ULID())
+    data['customerName'] = customer_name
+    return data
```

### Comparing `hcs-cli-0.1.36/vhcs/common/ctxp/var_template.py` & `hcs-cli-0.1.37/vhcs/common/ctxp/var_template.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.36/vhcs/common/logger.py` & `hcs-cli-0.1.37/vhcs/common/logger.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.36/vhcs/common/sglib/__init__.py` & `hcs-cli-0.1.37/vhcs/cli/cmds/daas/infra/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,9 +9,8 @@
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
-from . import auth
-from .hcs_client import hcs_client
+help = "DaaS shared infrastructure operations."
```

### Comparing `hcs-cli-0.1.36/vhcs/common/sglib/ez_client.py` & `hcs-cli-0.1.37/vhcs/common/sglib/ez_client.py`

 * *Files 9% similar despite different names*

```diff
@@ -9,28 +9,26 @@
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
+from authlib.integrations.httpx_client import OAuth2Client
 from http.client import HTTPResponse
 import httpx
 from typing import Callable
 import logging
 import json
 from vhcs.common.ctxp import jsondot
 
 log = logging.getLogger(__name__)
 
-log_http_details = False
-
 
 def _raise_on_4xx_5xx(response: httpx.Response):
-
     if not response.is_success:
         response.read()
         if len(response.text) > 0:
             text = _try_formatting_json(response.text)
             log.debug(text)
 
     response.raise_for_status()
@@ -81,70 +79,80 @@
         except:
             log.info("--- Fail parsing json. Dump content ---")
             log.info(resp.content)
             raise
     else:
         return None
 
+def _is_404(e: httpx.HTTPStatusError) -> bool:
+    return e.response.status_code == 404
 
 def on404ReturnNone(func):
     try:
         resp = func()
         return _parse_resp(resp)
     except httpx.HTTPStatusError as e:
         if e.response.status_code == 404:
             return None
         raise
 
 
 class EzClient:
-    def __init__(self, base_url: str, get_auth: Callable = None) -> None:
-        event_hooks = {"response": [_raise_on_4xx_5xx]}
-        event_hooks["request"] = [_log_request]
-        event_hooks["response"].insert(0, _log_response)
-
-        self._client = httpx.Client(base_url=base_url, timeout=30, event_hooks=event_hooks)
-        self._get_auth = get_auth
-
-    def login(self, force: bool = False):
-        header_name, header_value = self._get_auth(self, force)
-        self._client.headers[header_name] = header_value
+    def __init__(self, base_url: str, oauth_client: OAuth2Client) -> None:
+
+        #self._client = httpx.Client(base_url=base_url, timeout=30, event_hooks=event_hooks)
+        self._client = oauth_client
+        oauth_client.base_url = base_url
+        oauth_client.timeout = 30
+        request_hooks = oauth_client.event_hooks['request']
+        response_hooks = oauth_client.event_hooks['response']
+        if _log_request not in request_hooks:
+            request_hooks.append(_log_request)
+        if _log_response not in response_hooks:
+            response_hooks.append(_log_response)
+        if _raise_on_4xx_5xx not in response_hooks:
+            response_hooks.append(_raise_on_4xx_5xx)
 
     def post(self, url: str, json: dict = None, text: str = None, headers: dict = None):
-        self.login()
         if text:
             resp = self._client.post(url, content=text, headers=headers)
         else:
             resp = self._client.post(url, json=json)
         return _parse_resp(resp)
 
     def get(self, url: str, raise_on_404: bool = False):
-        self.login()
         try:
             resp = self._client.get(url)
             return _parse_resp(resp)
         except httpx.HTTPStatusError as e:
-            if e.response.status_code == 404 and raise_on_404:
-                raise e
+            if _is_404(e):
+                if raise_on_404:
+                    raise e
+                else:
+                    pass
+            else:
+                raise
 
     def patch(self, url: str, json: dict):
-        self.login()
         resp = self._client.patch(url, json=json)
         return _parse_resp(resp)
 
     def delete(self, url: str, raise_on_404: bool = False):
-        self.login()
         try:
             return self._client.delete(url)
         except httpx.HTTPStatusError as e:
-            if not raise_on_404 and e.response.status_code == 404:
-                return None
+            if _is_404(e):
+                if raise_on_404: 
+                    raise
+                else:
+                    pass
+            else:
+                raise
 
     def put(self, url: str, json: dict):
-        self.login()
         resp = self._client.put(url, json=json)
         return _parse_resp(resp)
 
     def close(self):
         self._client.close()
 
     def dump_response(self, response: HTTPResponse):
```

### Comparing `hcs-cli-0.1.36/vhcs/common/sglib/hcs_client.py` & `hcs-cli-0.1.37/vhcs/service/admin/provider.py`

 * *Files 24% similar despite different names*

```diff
@@ -9,27 +9,23 @@
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
-from vhcs.common.ctxp import context, profile
-from .ez_client import EzClient
-from . import auth as auth
+from .._util import hdc_service_client
+from vhcs.util.query_util import with_query, PageRequest
 
+_client = hdc_service_client("admin")
 
-def _get_auth(client: EzClient, force: bool):
-    auth_data = auth.login()
-    return "authorization", f"Bearer {auth_data.token}"
+def list(label: str, **kwargs):
+    def _get_page(query_string):
+        url = f"/v2/providers/{label}/instances?{query_string}"
+        return _client.get(url)
 
+    return PageRequest(_get_page, **kwargs).get()
 
-def hcs_client(url: str, login: bool = False) -> EzClient:
-    if not url:
-        url = profile.current().hcs.url
-    if url.endswith("/"):
-        url = url[:-1]
-    _client = EzClient(url, _get_auth)
-    if login:
-        _client.login()
-        context.set("orgId", auth.data().org.id)
-    return _client
+def get(label: str, id: str, **kwargs):
+    url = f"/v2/providers/{label}/instances/{id}"
+    url = with_query(url, **kwargs)
+    return _client.get(url)
```

### Comparing `hcs-cli-0.1.36/vhcs/common/sglib/util.py` & `hcs-cli-0.1.37/vhcs/plan/provider/hcs/pool_template.py`

 * *Files 18% similar despite different names*

```diff
@@ -9,26 +9,12 @@
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
-import click
+def deploy(data: dict) -> dict:
+    return {'id':'t1'}
 
-option_org_id = click.option(
-    "--org",
-    type=str,
-    default=None,
-    required=False,
-    help="Specify org ID. If not specified, org ID from the current auth token will be used.",
-)
-
-
-def get_org_id(org: str) -> str:
-    if org:
-        return org
-
-    from vhcs.common.sglib import auth
-
-    auth_info = auth.login()
-    return auth_info.org.id
+def destroy(data: dict, prev: dict) -> dict:
+    return {}
```

### Comparing `hcs-cli-0.1.36/vhcs/config/hcs-deployments.yaml` & `hcs-cli-0.1.37/vhcs/config/hcs-deployments.yaml`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.36/vhcs/service/_util.py` & `hcs-cli-0.1.37/vhcs/service/_util.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.36/vhcs/service/admin.py` & `hcs-cli-0.1.37/vhcs/service/org_service/details.py`

 * *Files 17% similar despite different names*

```diff
@@ -9,41 +9,23 @@
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
-from ._util import hdc_service_client
+from .._util import hdc_service_client
 from vhcs.util.query_util import with_query, PageRequest
 
-_client = hdc_service_client("admin")
+_client = hdc_service_client("org-service")
 
 
-class template:
-    @staticmethod
-    def get(id: str, **kwargs):
-        url = with_query(f"/v2/edge-deployments/{id}", **kwargs)
-        return _client.get(url)
-
-    @staticmethod
-    def list(limit: int = 10, **kwargs):
-        def _get_page(query_string):
-            url = "/v2/templates?" + query_string
-            return _client.get(url)
-
-        return PageRequest(_get_page, limit, **kwargs).get()
-
+def get(id: str, **kwargs):
+    url = with_query(f"/v1/org-details/{id}", **kwargs)
+    return _client.get(url)
 
-class edge:
-    @staticmethod
-    def get(id: str, **kwargs):
-        url = with_query(f"/v2/edge-deployments/{id}", **kwargs)
+def list(**kwargs):
+    def _get_page(query_string):
+        url = "/v1/org-details?" + query_string
         return _client.get(url)
 
-    @staticmethod
-    def list():
-        return _client.get("/v2/edge-deployments")
-
-
-def test():
-    print("test")
+    return PageRequest(_get_page, **kwargs).get()
```

### Comparing `hcs-cli-0.1.36/vhcs/service/lcm.py` & `hcs-cli-0.1.37/vhcs/service/lcm/template.py`

 * *Files 22% similar despite different names*

```diff
@@ -12,118 +12,83 @@
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 import time
 import json
 from typing import Any
-from ._util import hdc_service_client
+from .._util import hdc_service_client
 from vhcs.util.query_util import with_query, PageRequest
 
 _client = hdc_service_client("lcm")
 
 
-class template:
-    @staticmethod
-    def get(id: str, **kwargs: Any):
-        url = with_query(f"/v1/templates/{id}", **kwargs)
+def get(id: str, **kwargs: Any):
+    url = with_query(f"/v1/templates/{id}", **kwargs)
+    return _client.get(url)
+
+def list(name: str = None, **kwargs):
+    def _get_page(query_string):
+        url = "/v1/templates?" + query_string
         return _client.get(url)
 
-    @staticmethod
-    def list(limit: int = 20, name: str = None, **kwargs):
-        def _get_page(query_string):
-            url = "/v1/templates?" + query_string
-            return _client.get(url)
-
-        ret = PageRequest(_get_page, limit, **kwargs).get()
-        if name:
-            # filter_fn = lambda t : t.name.find(name) >= 0
-            def filter_fn(t):
-                return t.name.find(name) >= 0
-
-            ret = list(filter(filter_fn, ret))
-        return ret
-
-    @staticmethod
-    def delete(id: str, org_id: str, force: bool):
-        resp = _client.delete(f"/v1/templates/{id}?org_id={org_id}&force={force}")
-        return _convert_resp(resp)
-
-    @staticmethod
-    def create(template: dict):
-        url = "/v1/templates"
-        url += "/" + template["providerType"].lower()
-        return _client.post(url=url, json=template)
-
-    @staticmethod
-    def wait(
-        id: str,
-        expected_status: list,
-        timeout_seconds: int,
-        exclude_status: list = ["ERROR"],
-        interval_seconds: int = 10,
-    ):
-        start = int(time.time())
-        while True:
-            t = template.get(id)
-            if not t:
-                msg = f"Error waiting for template {id}. Not found."
-                raise Exception(msg)
-
-            status = t.status
-
-            if status in expected_status:
-                return t
-
-            if status in exclude_status:
-                msg = f"Error waiting for template {id}. Current status is {status}, which is not expected."
-                raise Exception(msg)
-
-            now = int(time.time())
-            elapsed = now - start
-
-            if elapsed > timeout_seconds:
-                msg = f"Timeout waiting for template {id}. Current: {status}, expect: {expected_status}"
-                raise Exception(msg)
-
-            delay = min(interval_seconds, timeout_seconds - elapsed)
-            time.sleep(delay)
-
-            print(f"Waiting for template {id}. Expected={exclude_status}, current={status}...")
-
-
-class provider:
-    @staticmethod
-    def get(id: str, **kwargs: Any):
-        url = with_query(f"/v1/providers/{id}", **kwargs)
-        return _client.get(url)
+    ret = PageRequest(_get_page, **kwargs).get()
+    if name:
+        # filter_fn = lambda t : t.name.find(name) >= 0
+        def filter_fn(t):
+            return t.name.find(name) >= 0
+
+        ret = list(filter(filter_fn, ret))
+    return ret
+
+def delete(id: str, org_id: str, force: bool):
+    resp = _client.delete(f"/v1/templates/{id}?org_id={org_id}&force={force}")
+    return _convert_resp(resp)
+
+def create(template: dict):
+    url = "/v1/templates"
+    url += "/" + template["providerType"].lower()
+    return _client.post(url=url, json=template)
+
+def wait(
+    id: str,
+    expected_status: list,
+    timeout_seconds: int,
+    exclude_status: list = ["ERROR"],
+    interval_seconds: int = 10,
+):
+    start = int(time.time())
+    while True:
+        t = get(id)
+        if not t:
+            msg = f"Error waiting for template {id}. Not found."
+            raise Exception(msg)
+
+        status = t.status
+
+        if status in expected_status:
+            return t
+
+        if status in exclude_status:
+            msg = f"Error waiting for template {id}. Current status is {status}, which is not expected."
+            raise Exception(msg)
+
+        now = int(time.time())
+        elapsed = now - start
+
+        if elapsed > timeout_seconds:
+            msg = f"Timeout waiting for template {id}. Current: {status}, expect: {expected_status}"
+            raise Exception(msg)
+
+        delay = min(interval_seconds, timeout_seconds - elapsed)
+        time.sleep(delay)
 
-    @staticmethod
-    def list(limit: int = 20, **kwargs):
-        def _get_page(query_string):
-            url = "/v1/providers?" + query_string
-            return _client.get(url)
-
-        return PageRequest(_get_page, limit, **kwargs).get()
-
-    @staticmethod
-    def delete(id: str):
-        resp = _client.delete(f"/v1/providers/{id}")
-        return _convert_resp(resp)
-
-    @staticmethod
-    def create(data: dict):
-        url = "/v1/providers/" + data["type"].lower()
-        return _client.post(url, json=data)
+        print(f"Waiting for template {id}. Expected={exclude_status}, current={status}...")
 
 
 def _convert_resp(resp):
     if resp:
         resp.read()
         try:
             json.loads(resp.text)
         except:
             return resp.text
-
-
-def test():
-    print("test")
```

### Comparing `hcs-cli-0.1.36/vhcs/service/org_service.py` & `hcs-cli-0.1.37/vhcs/service/org_service/datacenter.py`

 * *Files 24% similar despite different names*

```diff
@@ -9,43 +9,25 @@
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
-from ._util import hdc_service_client
+from .._util import hdc_service_client
 from vhcs.util.query_util import with_query, PageRequest
 
 _client = hdc_service_client("org-service")
 
 
-class datacenter:
-    @staticmethod
-    def get(id: str, **kwargs):
-        url = with_query(f"/v1/datacenters/{id}", **kwargs)
-        return _client.get(url)
-
-    @staticmethod
-    def list(**kwargs):
-        url = with_query(f"/v1/datacenters", **kwargs)
-        return _client.get(url)
-
-    @staticmethod
-    def find_by_org(orgId, **kwargs):
-        url = with_query(f"/v1/datacenters/orgs/{orgId}", **kwargs)
-        return _client.get(url)
-
-
-class details:
-    @staticmethod
-    def get(id: str, **kwargs):
-        url = with_query(f"/v1/org-details/{id}", **kwargs)
-        return _client.get(url)
-
-    @staticmethod
-    def list(limit: int = 10, **kwargs):
-        def _get_page(query_string):
-            url = "/v1/org-details?" + query_string
-            return _client.get(url)
+def get(id: str, **kwargs):
+    url = with_query(f"/v1/datacenters/{id}", **kwargs)
+    return _client.get(url)
+
+def list(**kwargs):
+    url = with_query(f"/v1/datacenters", **kwargs)
+    return _client.get(url)
+
+def find_by_org(orgId, **kwargs):
+    url = with_query(f"/v1/datacenters/orgs/{orgId}", **kwargs)
+    return _client.get(url)
 
-        return PageRequest(_get_page, limit, **kwargs).get()
```

### Comparing `hcs-cli-0.1.36/vhcs/service/pki.py` & `hcs-cli-0.1.37/vhcs/service/pki/certificate.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
-from ._util import hdc_service_client
+from .._util import hdc_service_client
 
 _client = hdc_service_client("pki")
 
 
 def test():
     print("TODO: test. Migrate that from pki-util here")
```

### Comparing `hcs-cli-0.1.36/vhcs/service/vmhub.py` & `hcs-cli-0.1.37/vhcs/service/vmhub/otp.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,42 +10,37 @@
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 import base64
-from ._util import regional_service_client
-from vhcs.common.ctxp import profile, panic
-from vhcs.common.sglib import hcs_client
+from .._util import regional_service_client
 
 _region_name = None
 
 
 def use_region(region_name: str):
     global _region_name
     _region_name = region_name
 
 
 def _client():
     return regional_service_client(_region_name, "vmhub")
 
 
-def request_otp(org_id: str, resource_name: str) -> str:
+def request(org_id: str, resource_name: str) -> str:
     mqtt_endpoint_request = {
         #'mqttEndpoint': '',
         "orgId": org_id,
         "vmId": resource_name,
     }
     ret = _client().post("/credentials/generate-otp", mqtt_endpoint_request)
     return ret
 
 
-def redeem_otp(resource_name: str, otp: str, csr: str):
+def redeem(resource_name: str, otp: str, csr: str):
     base64_encoded_csr = base64.b64encode(csr.encode("ascii")).decode("ascii")
 
     credentials_request = {"vmId": resource_name, "otp": otp, "clientCsr": base64_encoded_csr}
     return _client().post("/credentials", credentials_request)
 
-
-def test():
-    print("TODO")
```

### Comparing `hcs-cli-0.1.36/vhcs/util/check_license.py` & `hcs-cli-0.1.37/vhcs/util/check_license.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.36/vhcs/util/duration.py` & `hcs-cli-0.1.37/vhcs/util/duration.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.36/vhcs/util/pki_util.py` & `hcs-cli-0.1.37/vhcs/util/pki_util.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.36/vhcs/util/query_util.py` & `hcs-cli-0.1.37/vhcs/util/query_util.py`

 * *Files 14% similar despite different names*

```diff
@@ -30,16 +30,17 @@
     qs = urlencode(_remove_none(dict(kwargs)))
     if qs:
         url += "?" + qs
     return url
 
 
 class PageRequest:
-    def __init__(self, fn_get_page: Callable, limit: int, **kwargs):
-        self.limit = limit
+    def __init__(self, fn_get_page: Callable, **kwargs):
+        limit = kwargs.get('limit')
+        self.limit = int(limit) if limit else 10
         self.fn_get_page = fn_get_page
         self.query = _remove_none(dict(kwargs))
 
     def get(self) -> list:
         ret = []
         page_index = 0
 
@@ -47,14 +48,15 @@
             page_size = self.limit - len(ret)
             if page_size < 1:
                 break
             if page_size > 200:
                 page_size = 200
             self.query["size"] = page_size
             self.query["page"] = page_index
+            
             query_string = urlencode(self.query)
             page = self.fn_get_page(query_string)
             if not page or not page.content:
                 break
             ret += page.content
             page_index += 1
```

### Comparing `hcs-cli-0.1.36/vhcs/util/versions.py` & `hcs-cli-0.1.37/vhcs/util/versions.py`

 * *Files identical despite different names*

