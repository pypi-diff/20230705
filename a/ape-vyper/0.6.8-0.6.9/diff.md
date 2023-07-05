# Comparing `tmp/ape-vyper-0.6.8.tar.gz` & `tmp/ape-vyper-0.6.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ape-vyper-0.6.8.tar", last modified: Tue Jun 13 16:43:43 2023, max compression
+gzip compressed data, was "ape-vyper-0.6.9.tar", last modified: Wed Jul  5 19:16:34 2023, max compression
```

## Comparing `ape-vyper-0.6.8.tar` & `ape-vyper-0.6.9.tar`

### file list

```diff
@@ -1,70 +1,83 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:43:43.700535 ape-vyper-0.6.8/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:43:43.696535 ape-vyper-0.6.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:43:43.696535 ape-vyper-0.6.8/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      703 2023-06-13 16:42:24.000000 ape-vyper-0.6.8/.github/ISSUE_TEMPLATE/bug.md
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-06-13 16:42:24.000000 ape-vyper-0.6.8/.github/ISSUE_TEMPLATE/feature.md
--rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-06-13 16:42:24.000000 ape-vyper-0.6.8/.github/ISSUE_TEMPLATE/work-item.md
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-06-13 16:42:24.000000 ape-vyper-0.6.8/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (123)      651 2023-06-13 16:42:24.000000 ape-vyper-0.6.8/.github/release-drafter.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:43:43.696535 ape-vyper-0.6.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      686 2023-06-13 16:42:24.000000 ape-vyper-0.6.8/.github/workflows/commitlint.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-06-13 16:42:24.000000 ape-vyper-0.6.8/.github/workflows/draft.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      616 2023-06-13 16:42:24.000000 ape-vyper-0.6.8/.github/workflows/prtitle.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-06-13 16:42:24.000000 ape-vyper-0.6.8/.github/workflows/publish.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3410 2023-06-13 16:42:24.000000 ape-vyper-0.6.8/.github/workflows/test.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-06-13 16:42:24.000000 ape-vyper-0.6.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-13 16:42:24.000000 ape-vyper-0.6.8/.mdformat.toml
--rw-r--r--   0 runner    (1001) docker     (123)      796 2023-06-13 16:42:24.000000 ape-vyper-0.6.8/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-06-13 16:42:24.000000 ape-vyper-0.6.8/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    11342 2023-06-13 16:42:24.000000 ape-vyper-0.6.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2818 2023-06-13 16:43:43.700535 ape-vyper-0.6.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1861 2023-06-13 16:42:24.000000 ape-vyper-0.6.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:43:43.696535 ape-vyper-0.6.8/ape_vyper/
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-06-13 16:42:24.000000 ape-vyper-0.6.8/ape_vyper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    30501 2023-06-13 16:42:24.000000 ape-vyper-0.6.8/ape_vyper/compiler.py
--rw-r--r--   0 runner    (1001) docker     (123)     4300 2023-06-13 16:42:24.000000 ape-vyper-0.6.8/ape_vyper/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-13 16:43:43.000000 ape-vyper-0.6.8/ape_vyper/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:43:43.696535 ape-vyper-0.6.8/ape_vyper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2818 2023-06-13 16:43:43.000000 ape-vyper-0.6.8/ape_vyper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-06-13 16:43:43.000000 ape-vyper-0.6.8/ape_vyper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 16:43:43.000000 ape-vyper-0.6.8/ape_vyper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 16:43:43.000000 ape-vyper-0.6.8/ape_vyper.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      616 2023-06-13 16:43:43.000000 ape-vyper-0.6.8/ape_vyper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-13 16:43:43.000000 ape-vyper-0.6.8/ape_vyper.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      952 2023-06-13 16:42:24.000000 ape-vyper-0.6.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-13 16:43:43.704535 ape-vyper-0.6.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3116 2023-06-13 16:42:24.000000 ape-vyper-0.6.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:43:43.700535 ape-vyper-0.6.8/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:43:43.692535 ape-vyper-0.6.8/tests/ExampleDependency/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:43:43.700535 ape-vyper-0.6.8/tests/ExampleDependency/contracts/
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-13 16:42:24.000000 ape-vyper-0.6.8/tests/ExampleDependency/contracts/Dependency.vy
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 16:42:24.000000 ape-vyper-0.6.8/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-06-13 16:42:24.000000 ape-vyper-0.6.8/tests/ape-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     4105 2023-06-13 16:42:24.000000 ape-vyper-0.6.8/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:43:43.692535 ape-vyper-0.6.8/tests/contracts/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:43:43.700535 ape-vyper-0.6.8/tests/contracts/failing_contracts/
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-06-13 16:42:24.000000 ape-vyper-0.6.8/tests/contracts/failing_contracts/contract_undeclared_variable.vy
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-13 16:42:24.000000 ape-vyper-0.6.8/tests/contracts/failing_contracts/contract_unknown_pragma.vy
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:43:43.700535 ape-vyper-0.6.8/tests/contracts/passing_contracts/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:43:43.700535 ape-vyper-0.6.8/tests/contracts/passing_contracts/DirectoryWithExtension.vy/
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-06-13 16:42:24.000000 ape-vyper-0.6.8/tests/contracts/passing_contracts/DirectoryWithExtension.vy/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     3088 2023-06-13 16:42:24.000000 ape-vyper-0.6.8/tests/contracts/passing_contracts/contract.vy
--rw-r--r--   0 runner    (1001) docker     (123)     3088 2023-06-13 16:42:24.000000 ape-vyper-0.6.8/tests/contracts/passing_contracts/contract_37.vy
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-13 16:42:24.000000 ape-vyper-0.6.8/tests/contracts/passing_contracts/contract_no_pragma.vy
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-06-13 16:42:24.000000 ape-vyper-0.6.8/tests/contracts/passing_contracts/contract_with_dev_messages.vy
--rw-r--r--   0 runner    (1001) docker     (123)     5231 2023-06-13 16:42:24.000000 ape-vyper-0.6.8/tests/contracts/passing_contracts/erc20.vy
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:43:43.700535 ape-vyper-0.6.8/tests/contracts/passing_contracts/interfaces/
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-13 16:42:24.000000 ape-vyper-0.6.8/tests/contracts/passing_contracts/interfaces/IFace.vy
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-13 16:42:24.000000 ape-vyper-0.6.8/tests/contracts/passing_contracts/interfaces/IFace2.vy
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-06-13 16:42:24.000000 ape-vyper-0.6.8/tests/contracts/passing_contracts/interfaces/IRegistry_037.vy
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-06-13 16:42:24.000000 ape-vyper-0.6.8/tests/contracts/passing_contracts/interfaces/IRegistry_039.vy
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-13 16:42:24.000000 ape-vyper-0.6.8/tests/contracts/passing_contracts/non_payable_default.vy
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-13 16:42:24.000000 ape-vyper-0.6.8/tests/contracts/passing_contracts/older_version.vy
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-13 16:42:24.000000 ape-vyper-0.6.8/tests/contracts/passing_contracts/payable_default.vy
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-06-13 16:42:24.000000 ape-vyper-0.6.8/tests/contracts/passing_contracts/registry_037.vy
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-06-13 16:42:24.000000 ape-vyper-0.6.8/tests/contracts/passing_contracts/registry_039.vy
--rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-06-13 16:42:24.000000 ape-vyper-0.6.8/tests/contracts/passing_contracts/traceback_contract_037.vy
--rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-06-13 16:42:24.000000 ape-vyper-0.6.8/tests/contracts/passing_contracts/traceback_contract_039.vy
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-06-13 16:42:24.000000 ape-vyper-0.6.8/tests/contracts/passing_contracts/use_iface.vy
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-06-13 16:42:24.000000 ape-vyper-0.6.8/tests/contracts/passing_contracts/use_iface2.vy
--rw-r--r--   0 runner    (1001) docker     (123)    15085 2023-06-13 16:42:24.000000 ape-vyper-0.6.8/tests/test_compiler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 19:16:34.091809 ape-vyper-0.6.9/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 19:16:34.083809 ape-vyper-0.6.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 19:16:34.087809 ape-vyper-0.6.9/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2023-07-05 19:15:28.000000 ape-vyper-0.6.9/.github/ISSUE_TEMPLATE/bug.md
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-07-05 19:15:28.000000 ape-vyper-0.6.9/.github/ISSUE_TEMPLATE/feature.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-07-05 19:15:28.000000 ape-vyper-0.6.9/.github/ISSUE_TEMPLATE/work-item.md
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-07-05 19:15:28.000000 ape-vyper-0.6.9/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-07-05 19:15:28.000000 ape-vyper-0.6.9/.github/release-drafter.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 19:16:34.087809 ape-vyper-0.6.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-07-05 19:15:28.000000 ape-vyper-0.6.9/.github/workflows/commitlint.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-07-05 19:15:28.000000 ape-vyper-0.6.9/.github/workflows/draft.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-07-05 19:15:28.000000 ape-vyper-0.6.9/.github/workflows/prtitle.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-07-05 19:15:28.000000 ape-vyper-0.6.9/.github/workflows/publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3828 2023-07-05 19:15:28.000000 ape-vyper-0.6.9/.github/workflows/test.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-07-05 19:15:28.000000 ape-vyper-0.6.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-05 19:15:28.000000 ape-vyper-0.6.9/.mdformat.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      796 2023-07-05 19:15:28.000000 ape-vyper-0.6.9/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-07-05 19:15:28.000000 ape-vyper-0.6.9/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11342 2023-07-05 19:15:28.000000 ape-vyper-0.6.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2818 2023-07-05 19:16:34.091809 ape-vyper-0.6.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1861 2023-07-05 19:15:28.000000 ape-vyper-0.6.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 19:16:34.087809 ape-vyper-0.6.9/ape_vyper/
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-07-05 19:15:28.000000 ape-vyper-0.6.9/ape_vyper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40238 2023-07-05 19:15:28.000000 ape-vyper-0.6.9/ape_vyper/compiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4300 2023-07-05 19:15:28.000000 ape-vyper-0.6.9/ape_vyper/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-05 19:16:33.000000 ape-vyper-0.6.9/ape_vyper/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 19:16:34.087809 ape-vyper-0.6.9/ape_vyper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2818 2023-07-05 19:16:33.000000 ape-vyper-0.6.9/ape_vyper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2468 2023-07-05 19:16:34.000000 ape-vyper-0.6.9/ape_vyper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 19:16:33.000000 ape-vyper-0.6.9/ape_vyper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 19:16:33.000000 ape-vyper-0.6.9/ape_vyper.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-07-05 19:16:33.000000 ape-vyper-0.6.9/ape_vyper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-05 19:16:33.000000 ape-vyper-0.6.9/ape_vyper.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      877 2023-07-05 19:15:28.000000 ape-vyper-0.6.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-05 19:16:34.091809 ape-vyper-0.6.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3116 2023-07-05 19:15:28.000000 ape-vyper-0.6.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 19:16:34.087809 ape-vyper-0.6.9/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 19:16:34.083809 ape-vyper-0.6.9/tests/ExampleDependency/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 19:16:34.087809 ape-vyper-0.6.9/tests/ExampleDependency/contracts/
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-05 19:15:28.000000 ape-vyper-0.6.9/tests/ExampleDependency/contracts/Dependency.vy
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 19:15:28.000000 ape-vyper-0.6.9/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-07-05 19:15:28.000000 ape-vyper-0.6.9/tests/ape-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     4190 2023-07-05 19:15:28.000000 ape-vyper-0.6.9/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 19:16:34.083809 ape-vyper-0.6.9/tests/contracts/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 19:16:34.087809 ape-vyper-0.6.9/tests/contracts/failing_contracts/
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-07-05 19:15:28.000000 ape-vyper-0.6.9/tests/contracts/failing_contracts/contract_undeclared_variable.vy
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-05 19:15:28.000000 ape-vyper-0.6.9/tests/contracts/failing_contracts/contract_unknown_pragma.vy
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 19:16:34.087809 ape-vyper-0.6.9/tests/contracts/passing_contracts/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 19:16:34.087809 ape-vyper-0.6.9/tests/contracts/passing_contracts/DirectoryWithExtension.vy/
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-07-05 19:15:28.000000 ape-vyper-0.6.9/tests/contracts/passing_contracts/DirectoryWithExtension.vy/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3088 2023-07-05 19:15:28.000000 ape-vyper-0.6.9/tests/contracts/passing_contracts/contract.vy
+-rw-r--r--   0 runner    (1001) docker     (123)     3088 2023-07-05 19:15:28.000000 ape-vyper-0.6.9/tests/contracts/passing_contracts/contract_037.vy
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-05 19:15:28.000000 ape-vyper-0.6.9/tests/contracts/passing_contracts/contract_no_pragma.vy
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-07-05 19:15:28.000000 ape-vyper-0.6.9/tests/contracts/passing_contracts/contract_with_dev_messages.vy
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 19:15:28.000000 ape-vyper-0.6.9/tests/contracts/passing_contracts/empty.vy
+-rw-r--r--   0 runner    (1001) docker     (123)     5231 2023-07-05 19:15:28.000000 ape-vyper-0.6.9/tests/contracts/passing_contracts/erc20.vy
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 19:16:34.091809 ape-vyper-0.6.9/tests/contracts/passing_contracts/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-05 19:15:28.000000 ape-vyper-0.6.9/tests/contracts/passing_contracts/interfaces/IFace.vy
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-05 19:15:28.000000 ape-vyper-0.6.9/tests/contracts/passing_contracts/interfaces/IFace2.vy
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-07-05 19:15:28.000000 ape-vyper-0.6.9/tests/contracts/passing_contracts/interfaces/IRegistry_037.vy
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-07-05 19:15:28.000000 ape-vyper-0.6.9/tests/contracts/passing_contracts/interfaces/IRegistry_039.vy
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-07-05 19:15:28.000000 ape-vyper-0.6.9/tests/contracts/passing_contracts/non_payable_default.vy
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-05 19:15:28.000000 ape-vyper-0.6.9/tests/contracts/passing_contracts/older_version.vy
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-05 19:15:28.000000 ape-vyper-0.6.9/tests/contracts/passing_contracts/payable_default.vy
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-07-05 19:15:28.000000 ape-vyper-0.6.9/tests/contracts/passing_contracts/registry_037.vy
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-07-05 19:15:28.000000 ape-vyper-0.6.9/tests/contracts/passing_contracts/registry_039.vy
+-rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-07-05 19:15:28.000000 ape-vyper-0.6.9/tests/contracts/passing_contracts/traceback_contract_037.vy
+-rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-07-05 19:15:28.000000 ape-vyper-0.6.9/tests/contracts/passing_contracts/traceback_contract_039.vy
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-07-05 19:15:28.000000 ape-vyper-0.6.9/tests/contracts/passing_contracts/use_iface.vy
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-07-05 19:15:28.000000 ape-vyper-0.6.9/tests/contracts/passing_contracts/use_iface2.vy
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 19:16:34.083809 ape-vyper-0.6.9/tests/projects/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 19:16:34.091809 ape-vyper-0.6.9/tests/projects/coverage_project/
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-07-05 19:15:28.000000 ape-vyper-0.6.9/tests/projects/coverage_project/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-07-05 19:15:28.000000 ape-vyper-0.6.9/tests/projects/coverage_project/ape-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 19:16:34.091809 ape-vyper-0.6.9/tests/projects/coverage_project/contracts/
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-07-05 19:15:28.000000 ape-vyper-0.6.9/tests/projects/coverage_project/contracts/coverage_test.vy
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-07-05 19:15:28.000000 ape-vyper-0.6.9/tests/projects/coverage_project/contracts/exclude_part_of_contract.vy
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-05 19:15:28.000000 ape-vyper-0.6.9/tests/projects/coverage_project/contracts/exclude_whole_contract.vy
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 19:16:34.091809 ape-vyper-0.6.9/tests/projects/coverage_project/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-07-05 19:15:28.000000 ape-vyper-0.6.9/tests/projects/coverage_project/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2057 2023-07-05 19:15:28.000000 ape-vyper-0.6.9/tests/projects/coverage_project/tests/test_coverage.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16189 2023-07-05 19:15:28.000000 ape-vyper-0.6.9/tests/test_compiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5678 2023-07-05 19:15:28.000000 ape-vyper-0.6.9/tests/test_coverage.py
```

### Comparing `ape-vyper-0.6.8/.github/ISSUE_TEMPLATE/bug.md` & `ape-vyper-0.6.9/.github/ISSUE_TEMPLATE/bug.md`

 * *Files identical despite different names*

### Comparing `ape-vyper-0.6.8/.github/ISSUE_TEMPLATE/feature.md` & `ape-vyper-0.6.9/.github/ISSUE_TEMPLATE/feature.md`

 * *Files identical despite different names*

### Comparing `ape-vyper-0.6.8/.github/ISSUE_TEMPLATE/work-item.md` & `ape-vyper-0.6.9/.github/ISSUE_TEMPLATE/work-item.md`

 * *Files identical despite different names*

### Comparing `ape-vyper-0.6.8/.github/release-drafter.yml` & `ape-vyper-0.6.9/.github/release-drafter.yml`

 * *Files identical despite different names*

### Comparing `ape-vyper-0.6.8/.github/workflows/commitlint.yaml` & `ape-vyper-0.6.9/.github/workflows/commitlint.yaml`

 * *Files identical despite different names*

### Comparing `ape-vyper-0.6.8/.github/workflows/prtitle.yaml` & `ape-vyper-0.6.9/.github/workflows/prtitle.yaml`

 * *Files identical despite different names*

### Comparing `ape-vyper-0.6.8/.github/workflows/publish.yaml` & `ape-vyper-0.6.9/.github/workflows/publish.yaml`

 * *Files identical despite different names*

### Comparing `ape-vyper-0.6.8/.github/workflows/test.yaml` & `ape-vyper-0.6.9/.github/workflows/test.yaml`

 * *Files 15% similar despite different names*

```diff
@@ -104,15 +104,27 @@
 
         - name: Install Dependencies
           run: |
             python -m pip install --upgrade pip
             pip install .[test]
 
         - name: Run Tests
-          run: pytest -m "not fuzzing" -n 0 -s --cov
+          run: |
+            pytest tests/test_compiler.py -m "not fuzzing" -n 0 -s \
+              --cov=ape_vyper \
+              --cov-branch \
+              --cov-report term \
+              --cov-report html \
+              --cov-report xml
+
+        # Since --cov does not play nicely with --coverage (low-level tracer issues),
+        #  we have to run the tests separately.
+        - name: Run Contract Coverage Tests
+          run: pytest tests/test_coverage.py
+
 
 # NOTE: uncomment this block after you've marked tests with @pytest.mark.fuzzing
 #    fuzzing:
 #        runs-on: ubuntu-latest
 #
 #        strategy:
 #            fail-fast: true
```

### Comparing `ape-vyper-0.6.8/.gitignore` & `ape-vyper-0.6.9/.gitignore`

 * *Files identical despite different names*

### Comparing `ape-vyper-0.6.8/.pre-commit-config.yaml` & `ape-vyper-0.6.9/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `ape-vyper-0.6.8/CONTRIBUTING.md` & `ape-vyper-0.6.9/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `ape-vyper-0.6.8/LICENSE` & `ape-vyper-0.6.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ape-vyper-0.6.8/PKG-INFO` & `ape-vyper-0.6.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ape-vyper
-Version: 0.6.8
+Version: 0.6.9
 Summary: Plugin for Ape Ethereum Framework for compiling Vyper contracts
 Home-page: https://github.com/ApeWorX/ape-vyper
 Author: ApeWorX Ltd.
 Author-email: admin@apeworx.io
 License: Apache-2.0
 Keywords: ethereum
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `ape-vyper-0.6.8/README.md` & `ape-vyper-0.6.9/README.md`

 * *Files identical despite different names*

### Comparing `ape-vyper-0.6.8/ape_vyper/compiler.py` & `ape-vyper-0.6.9/ape_vyper/compiler.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 import os
 import re
 import shutil
+from fnmatch import fnmatch
 from pathlib import Path
 from typing import Any, Dict, Iterator, List, Optional, Set, Tuple, Union, cast
 
 import vvm  # type: ignore
 from ape.api import PluginConfig
 from ape.api.compiler import CompilerAPI
 from ape.exceptions import ContractLogicError
-from ape.types import ContractType, SourceTraceback, TraceFrame
+from ape.types import ContractSourceCoverage, ContractType, SourceTraceback, TraceFrame
 from ape.utils import cached_property, get_relative_path
 from eth_utils import is_0x_prefixed
 from ethpm_types import ASTNode, HexBytes, PackageManifest, PCMap, SourceMapItem
 from ethpm_types.ast import ASTClassification
 from ethpm_types.contract_type import SourceMap
-from ethpm_types.source import ContractSource, Function
+from ethpm_types.source import ContractSource, Function, SourceLocation
 from evm_trace.enums import CALL_OPCODES
 from semantic_version import NpmSpec, Version  # type: ignore
 from vvm.exceptions import VyperError  # type: ignore
 
 from ape_vyper.exceptions import (
     RUNTIME_ERROR_MAP,
     RuntimeErrorType,
@@ -274,15 +275,16 @@
 
                         # NOTE: Constructor is handled elsewhere.
                         if node.ast_type == "FunctionDef" and "__init__" not in content.get(
                             lineno, ""
                         ):
                             function_offsets.append((node.lineno, node.end_lineno))
 
-                    bytecode = output["evm"]["deployedBytecode"]
+                    evm = output["evm"]
+                    bytecode = evm["deployedBytecode"]
                     opcodes = bytecode["opcodes"].split(" ")
                     compressed_src_map = SourceMap(__root__=bytecode["sourceMap"])
                     src_map = list(compressed_src_map.parse())[1:]
 
                     if vyper_version < Version("0.3.8"):
                         pcmap = _get_legacy_pcmap(ast, src_map, opcodes)
                     else:
@@ -294,15 +296,15 @@
                         if match := re.search(DEV_MSG_PATTERN, line):
                             dev_messages[line_no] = match.group(1).strip()
 
                     contract_type = ContractType(
                         ast=ast,
                         contractName=name,
                         sourceId=source_id,
-                        deploymentBytecode={"bytecode": output["evm"]["bytecode"]["object"]},
+                        deploymentBytecode={"bytecode": evm["bytecode"]["object"]},
                         runtimeBytecode={"bytecode": bytecode["object"]},
                         abi=output["abi"],
                         sourcemap=compressed_src_map,
                         pcmap=pcmap,
                         userdoc=output["userdoc"],
                         devdoc=output["devdoc"],
                         dev_messages=dev_messages,
@@ -386,14 +388,183 @@
             if evm_version := data.get("evm_version"):
                 version_settings["evmVersion"] = evm_version
 
             settings[version] = version_settings
 
         return settings
 
+    def init_coverage_profile(
+        self, source_coverage: ContractSourceCoverage, contract_source: ContractSource
+    ):
+        exclusions = self.config_manager.get_config("test").coverage.exclude
+        contract_name = contract_source.contract_type.name or "__UnknownContract__"
+
+        # Check if excluding this contract.
+        for exclusion in exclusions:
+            if fnmatch(contract_name, exclusion.contract_name) and (
+                not exclusion.method_name or exclusion.method_name == "*"
+            ):
+                # Skip this whole source.
+                return
+
+        contract_coverage = source_coverage.include(contract_name)
+
+        def _exclude_fn(_name: str) -> bool:
+            for _exclusion in exclusions:
+                if fnmatch(contract_coverage.name, _exclusion.contract_name) and fnmatch(
+                    _name, _exclusion.method_name
+                ):
+                    # This function should be skipped.
+                    return True
+
+            return False
+
+        def _profile(_name: str, _full_name: str):
+            # Ensure function isn't excluded.
+            if _exclude_fn(_name):
+                return
+
+            _function_coverage = contract_coverage.include(_name, _full_name)
+            tag = str(item["dev"]) if item.get("dev") else None
+            _function_coverage.profile_statement(pc_int, location=location, tag=tag)
+
+        # Some statements are too difficult to know right away where they belong,
+        # such as statement related to kwarg-default auto-generated implicit lookups.
+        # function_name -> (pc, location)
+        pending_statements: Dict[str, List[Tuple[int, SourceLocation]]] = {}
+
+        for pc, item in contract_source.pcmap.__root__.items():
+            pc_int = int(pc)
+            if pc_int < 0:
+                continue
+
+            location: Optional[SourceLocation]
+            if item.get("location"):
+                location_list = item["location"]
+                if not isinstance(location_list, (list, tuple)):
+                    raise TypeError(f"Unexpected location type '{type(location_list)}'.")
+
+                # NOTE: Only doing 0 because mypy for some reason thinks it is optional.
+                location = (
+                    location_list[0] or 0,
+                    location_list[1] or 0,
+                    location_list[2] or 0,
+                    location_list[3] or 0,
+                )
+            else:
+                location = None
+
+            if location is not None and not isinstance(location, tuple):
+                # Only really for mypy.
+                raise TypeError(f"Received unexpected type for location '{location}'.")
+
+            if not location and not item.get("dev"):
+                # Not a statement we can measure.
+                continue
+
+            if location:
+                function = contract_source.lookup_function(location)
+                if not function:
+                    # Not sure if this happens.
+                    continue
+
+                matching_abis = [
+                    a for a in contract_source.contract_type.methods if a.name == function.name
+                ]
+                if len(matching_abis) > 1:
+                    # In Vyper, if there are multiple method ABIs with the same name,
+                    # that is evidence of the default key-word argument generated methods.
+
+                    is_part_of_signature = location[0] < function.offset
+                    if is_part_of_signature and location[0] != location[2]:
+                        # This likely is not a real statement, but not really sure what this is.
+                        continue
+
+                    # In Vyper, the ABI with the most inputs should be the one without extra steps.
+                    longest_abi = max(matching_abis, key=lambda x: len(x.inputs))
+                    if is_part_of_signature and longest_abi.name in pending_statements:
+                        pending_statements[longest_abi.name].append((pc_int, location))
+                    elif is_part_of_signature:
+                        pending_statements[longest_abi.name] = [(pc_int, location)]
+                    else:
+                        # Put actual source statements under the ABI with all parameters as inputs.
+                        _profile(longest_abi.name, longest_abi.selector)
+
+                elif len(matching_abis) == 1:
+                    _profile(function.name, matching_abis[0].selector)
+
+                elif len(matching_abis) == 0:
+                    # Is likely an internal method.
+                    _profile(function.name, function.full_name or function.name)
+
+            else:
+                _profile("__builtin__", "__builtin__")
+
+        if pending_statements:
+            # Handle auto-generated kwarg-default statements here.
+            # Sort each statement into buckets mapping to the method it belongs in.
+            for fn_name, pending_ls in pending_statements.items():
+                matching_abis = [
+                    m for m in contract_source.contract_type.methods if m.name == fn_name
+                ]
+                longest_abi = max(matching_abis, key=lambda x: len(x.inputs))
+                autogenerated_abis = [
+                    abi for abi in matching_abis if abi.selector != longest_abi.selector
+                ]
+                # Sort the autogenerated ABIs so we can loop through them in the correct order.
+                autogenerated_abis.sort(key=lambda a: len(a.inputs))
+                buckets: Dict[str, List[Tuple[int, SourceLocation]]] = {
+                    a.selector: [] for a in autogenerated_abis
+                }
+                selector_index = 0
+                selector = autogenerated_abis[0].selector
+                # Must loop through PCs from smallest to greatest for this to work.
+                pending_ls.sort()
+                jump_threshold = 10
+                for _pc, loc in pending_ls:
+                    if selector_index < len(autogenerated_abis):
+                        selector = autogenerated_abis[selector_index].selector
+
+                    if not buckets[selector]:
+                        # No need for bounds checking when the bucket is empty.
+                        buckets[selector].append((_pc, loc))
+                        continue
+
+                    last_pc = buckets[selector][-1][0]
+
+                    # Check if jumped.
+                    distance = _pc - last_pc
+                    if distance > jump_threshold:
+                        selector_index += 1
+                        if selector_index >= len(autogenerated_abis):
+                            break
+
+                        selector = autogenerated_abis[selector_index].selector
+                        buckets[selector].append((_pc, loc))
+                    else:
+                        buckets[selector].append((_pc, loc))
+
+                for full_name, statements in buckets.items():
+                    for _pc, location in statements:
+                        if _exclude_fn(fn_name):
+                            continue
+
+                        function_coverage = contract_coverage.include(fn_name, full_name)
+                        function_coverage.profile_statement(_pc, location=location)
+
+        # After handling all methods with locations, let's also add the auto-getters,
+        # which are not present in the source map.
+        for method in contract_source.contract_type.view_methods:
+            if method.selector not in [fn.full_name for fn in contract_coverage.functions]:
+                if _exclude_fn(method.name):
+                    return
+
+                # Auto-getter found. Profile function without statements.
+                contract_coverage.include(method.name, method.selector)
+
     def _get_compiler_arguments(self, version_map: Dict, base_path: Path) -> Dict[Version, Dict]:
         base_path = base_path or self.project_manager.contracts_folder
         arguments_map = {}
         for vyper_version, source_paths in version_map.items():
             bin_arg = self._get_vyper_bin(vyper_version)
             arguments_map[vyper_version] = {
                 "base_path": str(base_path),
@@ -414,30 +585,38 @@
             # Not available.
             return err
 
         if not dev_message:
             return err
 
         err_str = dev_message.replace("dev: ", "")
-
+        error_type = None
         if err_str in [m.value for m in RuntimeErrorType]:
             # Is a builtin compiler error.
-            runtime_error_type = RuntimeErrorType(err_str)
-            runtime_error_cls = RUNTIME_ERROR_MAP[runtime_error_type]
-            return runtime_error_cls(
-                contract_address=err.contract_address,
-                source_traceback=err.source_traceback,
-                trace=err.trace,
-                txn=err.txn,
-            )
+            error_type = RuntimeErrorType(err_str)
 
         else:
+            # Check names
+            for name, _type in [(m.name, m) for m in RuntimeErrorType]:
+                if err_str == name:
+                    error_type = _type
+                    break
+
+        if not error_type:
             # Not a builtin compiler error; cannot enrich.
             return err
 
+        runtime_error_cls = RUNTIME_ERROR_MAP[error_type]
+        return runtime_error_cls(
+            contract_address=err.contract_address,
+            source_traceback=err.source_traceback,
+            trace=err.trace,
+            txn=err.txn,
+        )
+
     def trace_source(
         self, contract_type: ContractType, trace: Iterator[TraceFrame], calldata: HexBytes
     ) -> SourceTraceback:
         source_contract_type = self.project_manager._create_contract_source(contract_type)
         if not source_contract_type:
             return SourceTraceback.parse_obj([])
 
@@ -445,14 +624,15 @@
 
     def _get_traceback(
         self, contract_src: ContractSource, trace: Iterator[TraceFrame], calldata: HexBytes
     ) -> SourceTraceback:
         traceback = SourceTraceback.parse_obj([])
         function = None
         last_pc = None
+        method_id = HexBytes(calldata[:4])
 
         for frame in trace:
             if frame.op in CALL_OPCODES:
                 called_contract, sub_calldata = self._create_contract_from_call(frame)
                 if called_contract:
                     ext = Path(called_contract.source_id).suffix
                     if not ext.endswith(".vy"):
@@ -482,98 +662,138 @@
             elif frame.op in _RETURN_OPCODES:
                 if frame.op in "RETURN" and function:
                     _extend_return(function, traceback, last_pc, contract_src.source_path)
 
                 # Completed!
                 return traceback
 
+            pcs_to_try_adding = set()
             if "PUSH" in frame.op and frame.pc in contract_src.pcmap:
                 # Check if next op is SSTORE to properly use AST from push op.
-                next_frame = next(trace, None)
+                next_frame: Optional[TraceFrame] = frame
+                loc = contract_src.pcmap[frame.pc]
+                pcs_to_try_adding.add(frame.pc)
+
+                while next_frame and "PUSH" in next_frame.op:
+                    next_frame = next(trace, None)
+                    if next_frame and "PUSH" in next_frame.op:
+                        pcs_to_try_adding.add(next_frame.pc)
+
                 is_non_payable_hit = False
                 if next_frame and next_frame.op == "SSTORE":
-                    push_location = tuple(contract_src.pcmap[frame.pc]["location"])  # type: ignore
+                    push_location = tuple(loc["location"])  # type: ignore
                     pcmap = PCMap.parse_obj({next_frame.pc: {"location": push_location}})
 
                 elif next_frame and next_frame.op in _RETURN_OPCODES:
                     if next_frame.op in "RETURN" and function:
                         _extend_return(function, traceback, last_pc, contract_src.source_path)
 
                     # Completed!
                     return traceback
 
                 else:
                     pcmap = contract_src.pcmap
-                    dev_val = str((pcmap[frame.pc].get("dev") or "")).replace("dev: ", "")
+                    dev_val = str((loc.get("dev") or "")).replace("dev: ", "")
                     is_non_payable_hit = dev_val == RuntimeErrorType.NONPAYABLE_CHECK.value
 
                 if not is_non_payable_hit and next_frame:
                     frame = next_frame
 
             else:
                 pcmap = contract_src.pcmap
 
-            if frame.pc not in pcmap:
+            pcs_to_try_adding.add(frame.pc)
+            pcs_to_try_adding = {pc for pc in pcs_to_try_adding if pc in pcmap}
+            if not pcs_to_try_adding:
                 continue
 
-            method_id = HexBytes(calldata[:4])
-            location = cast(Tuple[int, int, int, int], tuple(pcmap[frame.pc].get("location") or []))
-            dev_item = pcmap[frame.pc].get("dev", "")
-            dev = str(dev_item).replace("dev: ", "")
-            if not location and dev in [m.value for m in RuntimeErrorType]:
-                error_type = RuntimeErrorType(dev)
-                if error_type != RuntimeErrorType.NONPAYABLE_CHECK and traceback.last is not None:
-                    # If the error type is not the non-payable check,
-                    # it happened in the last method.
-                    name = traceback.last.closure.name
-
-                elif method_id in contract_src.contract_type.methods:
-                    # For non-payable checks, they should hit here.
-                    method_checked = contract_src.contract_type.methods[method_id]
-                    name = method_checked.name
-
-                else:
-                    # Not sure if possible to get here.
-                    name = error_type.name.lower()
-
-                # Empty source (is builtin)
-                traceback.add_builtin_jump(
-                    name, dev_item, self.name, pcs={frame.pc}, source_path=contract_src.source_path
+            pc_groups: List[List] = []
+            for pc in pcs_to_try_adding:
+                location = (
+                    cast(Tuple[int, int, int, int], tuple(pcmap[pc].get("location") or [])) or None
                 )
-                continue
+                dev_item = pcmap[pc].get("dev", "")
+                dev = str(dev_item).replace("dev: ", "")
+                done = False
+                for group in pc_groups:
+                    if group[0] != location:
+                        continue
+
+                    group[1].add(pc)
+                    group[2] = dev
+                    done = True
+                    break
+
+                if not done:
+                    # New group.
+                    pc_groups.append([location, {pc}, dev])
+
+            for location, pcs, dev in pc_groups:
+                if not location and dev in [m.value for m in RuntimeErrorType]:
+                    error_type = RuntimeErrorType(dev)
+                    if (
+                        error_type != RuntimeErrorType.NONPAYABLE_CHECK
+                        and traceback.last is not None
+                    ):
+                        # If the error type is not the non-payable check,
+                        # it happened in the last method.
+                        name = traceback.last.closure.name
+                        full_name = traceback.last.closure.full_name
+
+                    elif method_id in contract_src.contract_type.methods:
+                        # For non-payable checks, they should hit here.
+                        method_checked = contract_src.contract_type.methods[method_id]
+                        name = method_checked.name
+                        full_name = method_checked.selector
 
-            elif not location:
-                # Unknown.
-                continue
+                    else:
+                        # Not sure if possible to get here.
+                        name = error_type.name.lower()
+                        full_name = name
+
+                    # Empty source (is builtin)
+                    traceback.add_builtin_jump(
+                        name,
+                        f"dev: {dev}",
+                        self.name,
+                        full_name=full_name,
+                        pcs=pcs,
+                        source_path=contract_src.source_path,
+                    )
+                    continue
 
-            function = contract_src.lookup_function(location, method_id=method_id)
-            if not function:
-                continue
+                elif not location:
+                    # Unknown.
+                    continue
 
-            if (
-                not traceback.last
-                or traceback.last.closure.name != function.name
-                or not isinstance(traceback.last.closure, Function)
-            ):
-                depth = (
-                    frame.depth + 1
-                    if traceback.last and traceback.last.depth == frame.depth
-                    else frame.depth
-                )
-                traceback.add_jump(
-                    location,
-                    function,
-                    depth,
-                    pcs={frame.pc},
-                    source_path=contract_src.source_path,
-                )
-            else:
-                traceback.extend_last(location, pcs={frame.pc})
+                function = contract_src.lookup_function(location, method_id=method_id)
+                if not function:
+                    continue
+
+                if (
+                    not traceback.last
+                    or traceback.last.closure.full_name != function.full_name
+                    or not isinstance(traceback.last.closure, Function)
+                ):
+                    depth = (
+                        frame.depth + 1
+                        if traceback.last and traceback.last.depth == frame.depth
+                        else frame.depth
+                    )
+                    traceback.add_jump(
+                        location,
+                        function,
+                        depth,
+                        pcs=pcs,
+                        source_path=contract_src.source_path,
+                    )
+                else:
+                    traceback.extend_last(location, pcs=pcs)
 
-            last_pc = frame.pc
+                last_pc = max(pcs)
 
         # Never actually hits this return.
         # See `Completed!` comment above.
         return traceback
 
 
 def _safe_append(data: Dict, version: Union[Version, NpmSpec], paths: Union[Path, Set]):
@@ -595,14 +815,17 @@
     )
 
 
 def _get_pcmap(bytecode: Dict, src_map: List[SourceMapItem], opcodes: List[str]) -> PCMap:
     # Find the non payable value check.
     src_info = bytecode["sourceMapFull"]
     pc_data = {pc: {"location": ln} for pc, ln in src_info["pc_pos_map"].items()}
+    if not pc_data:
+        return PCMap.parse_obj({})
+
     non_payable_check = _find_non_payable_check(src_map, opcodes)
     if not non_payable_check:
         non_payable_check = min([int(x) for x in pc_data]) - 1
 
     pc_data[non_payable_check] = {"dev": _NON_PAYABLE_STR, "location": None}
 
     # Apply other errors.
```

### Comparing `ape-vyper-0.6.8/ape_vyper/exceptions.py` & `ape-vyper-0.6.9/ape_vyper/exceptions.py`

 * *Files identical despite different names*

### Comparing `ape-vyper-0.6.8/ape_vyper.egg-info/PKG-INFO` & `ape-vyper-0.6.9/ape_vyper.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ape-vyper
-Version: 0.6.8
+Version: 0.6.9
 Summary: Plugin for Ape Ethereum Framework for compiling Vyper contracts
 Home-page: https://github.com/ApeWorX/ape-vyper
 Author: ApeWorX Ltd.
 Author-email: admin@apeworx.io
 License: Apache-2.0
 Keywords: ethereum
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `ape-vyper-0.6.8/ape_vyper.egg-info/SOURCES.txt` & `ape-vyper-0.6.9/ape_vyper.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -27,29 +27,38 @@
 ape_vyper.egg-info/not-zip-safe
 ape_vyper.egg-info/requires.txt
 ape_vyper.egg-info/top_level.txt
 tests/__init__.py
 tests/ape-config.yaml
 tests/conftest.py
 tests/test_compiler.py
+tests/test_coverage.py
 tests/ExampleDependency/contracts/Dependency.vy
 tests/contracts/failing_contracts/contract_undeclared_variable.vy
 tests/contracts/failing_contracts/contract_unknown_pragma.vy
 tests/contracts/passing_contracts/contract.vy
-tests/contracts/passing_contracts/contract_37.vy
+tests/contracts/passing_contracts/contract_037.vy
 tests/contracts/passing_contracts/contract_no_pragma.vy
 tests/contracts/passing_contracts/contract_with_dev_messages.vy
+tests/contracts/passing_contracts/empty.vy
 tests/contracts/passing_contracts/erc20.vy
 tests/contracts/passing_contracts/non_payable_default.vy
 tests/contracts/passing_contracts/older_version.vy
 tests/contracts/passing_contracts/payable_default.vy
 tests/contracts/passing_contracts/registry_037.vy
 tests/contracts/passing_contracts/registry_039.vy
 tests/contracts/passing_contracts/traceback_contract_037.vy
 tests/contracts/passing_contracts/traceback_contract_039.vy
 tests/contracts/passing_contracts/use_iface.vy
 tests/contracts/passing_contracts/use_iface2.vy
 tests/contracts/passing_contracts/DirectoryWithExtension.vy/README.md
 tests/contracts/passing_contracts/interfaces/IFace.vy
 tests/contracts/passing_contracts/interfaces/IFace2.vy
 tests/contracts/passing_contracts/interfaces/IRegistry_037.vy
-tests/contracts/passing_contracts/interfaces/IRegistry_039.vy
+tests/contracts/passing_contracts/interfaces/IRegistry_039.vy
+tests/projects/coverage_project/README.md
+tests/projects/coverage_project/ape-config.yaml
+tests/projects/coverage_project/contracts/coverage_test.vy
+tests/projects/coverage_project/contracts/exclude_part_of_contract.vy
+tests/projects/coverage_project/contracts/exclude_whole_contract.vy
+tests/projects/coverage_project/tests/conftest.py
+tests/projects/coverage_project/tests/test_coverage.py
```

### Comparing `ape-vyper-0.6.8/ape_vyper.egg-info/requires.txt` & `ape-vyper-0.6.9/ape_vyper.egg-info/requires.txt`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-eth-ape<0.7,>=0.6.10
+eth-ape<0.7,>=0.6.12
 ethpm-types
 tqdm
 vvm<0.2,>=0.1.0
 
 [dev]
 pytest>=6.0
 pytest-mock
```

### Comparing `ape-vyper-0.6.8/setup.py` & `ape-vyper-0.6.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -54,15 +54,15 @@
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="ApeWorX Ltd.",
     author_email="admin@apeworx.io",
     url="https://github.com/ApeWorX/ape-vyper",
     include_package_data=True,
     install_requires=[
-        "eth-ape>=0.6.10,<0.7",
+        "eth-ape>=0.6.12,<0.7",
         "ethpm-types",  # Use same version as eth-ape
         "tqdm",  # Use same version as eth-ape
         "vvm>=0.1.0,<0.2",
     ],
     python_requires=">=3.8,<4",
     extras_require=extras_require,
     py_modules=["ape_vyper"],
```

### Comparing `ape-vyper-0.6.8/tests/conftest.py` & `ape-vyper-0.6.9/tests/conftest.py`

 * *Files 2% similar despite different names*

```diff
@@ -127,14 +127,19 @@
         ) as provider:
             yield provider
     else:
         yield ape.networks.provider
 
 
 @pytest.fixture
+def projects_path():
+    return Path(__file__).parent / "projects"
+
+
+@pytest.fixture
 def account():
     return ape.accounts.test_accounts[0]
 
 
 @pytest.fixture(params=("037", "039"))
 def traceback_contract(request, account, project, geth_provider):
     return _get_tb_contract(request.param, project, account)
```

### Comparing `ape-vyper-0.6.8/tests/contracts/passing_contracts/contract.vy` & `ape-vyper-0.6.9/tests/contracts/passing_contracts/contract.vy`

 * *Files identical despite different names*

### Comparing `ape-vyper-0.6.8/tests/contracts/passing_contracts/contract_37.vy` & `ape-vyper-0.6.9/tests/contracts/passing_contracts/contract_037.vy`

 * *Files identical despite different names*

### Comparing `ape-vyper-0.6.8/tests/contracts/passing_contracts/erc20.vy` & `ape-vyper-0.6.9/tests/contracts/passing_contracts/erc20.vy`

 * *Files identical despite different names*

### Comparing `ape-vyper-0.6.8/tests/contracts/passing_contracts/traceback_contract_037.vy` & `ape-vyper-0.6.9/tests/contracts/passing_contracts/traceback_contract_037.vy`

 * *Files 8% similar despite different names*

```diff
@@ -9,17 +9,19 @@
 @external
 def __init__(registry: IRegistry_037):
     self.registry = registry
 
 
 @external
 def addBalance(
-    num: uint256
+    num: uint256 = 123,
+    num2: uint256 = 321,
 ) -> uint256:
     assert num != self._balance
+    assert num != num2
     self.registry.register(msg.sender)
     self._balance = self._balance + self.addInterest(num)
 
     # Run some loops.
     for i in [1, 2, 3, 4, 5]:
         if i == num:
             break
```

### Comparing `ape-vyper-0.6.8/tests/contracts/passing_contracts/traceback_contract_039.vy` & `ape-vyper-0.6.9/tests/contracts/passing_contracts/traceback_contract_039.vy`

 * *Files 6% similar despite different names*

```diff
@@ -9,17 +9,19 @@
 @external
 def __init__(registry: IRegistry_039):
     self.registry = registry
 
 
 @external
 def addBalance(
-    num: uint256
+    num: uint256 = 123,
+    num2: uint256 = 321,
 ) -> uint256:
     assert num != self._balance
+    assert num != num2
     self.registry.register(msg.sender)
     self._balance = self._balance + self.addInterest(num)
 
     # Run some loops.
     for i in [1, 2, 3, 4, 5]:
         if i == num:
             break
```

### Comparing `ape-vyper-0.6.8/tests/test_compiler.py` & `ape-vyper-0.6.9/tests/test_compiler.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,31 +15,30 @@
     IntegerOverflowError,
     NonPayableError,
     VyperCompileError,
     VyperInstallError,
 )
 
 BASE_CONTRACTS_PATH = Path(__file__).parent / "contracts"
-PASSING_BASE = BASE_CONTRACTS_PATH / "passing_contracts"
 FAILING_BASE = BASE_CONTRACTS_PATH / "failing_contracts"
 
 # Currently, this is the only version specified from a pragma spec
 OLDER_VERSION_FROM_PRAGMA = Version("0.2.8")
 VERSION_37 = Version("0.3.7")
 
 # NOTE: This is really just about testing > 0.3.7.
 #  Should get switched as soon as a more stable version is released.
 VERSION_FROM_PRAGMA = Version("0.3.9")
 
 APE_VERSION = Version(get_distribution("eth-ape").version.split(".dev")[0].strip())
 
 
 @pytest.fixture
-def dev_revert_source():
-    return PASSING_BASE / "contract_with_dev_messages.vy"
+def dev_revert_source(project):
+    return project.contracts_folder / "contract_with_dev_messages.vy"
 
 
 def contract_test_cases(passing: bool) -> List[str]:
     """
     Returns test-case names for outputting nicely with pytest.
     """
     suffix = "passing_contracts" if passing else "failing_contracts"
@@ -59,23 +58,25 @@
     ),
     "contract_unknown_pragma": "",
 }
 
 
 def test_compile_project(project):
     contracts = project.load_contracts()
-    assert len(contracts) == len([p.name for p in PASSING_BASE.glob("*.vy") if p.is_file()])
+    assert len(contracts) == len(
+        [p.name for p in project.contracts_folder.glob("*.vy") if p.is_file()]
+    )
     assert contracts["contract"].source_id == "contract.vy"
     assert contracts["contract_no_pragma"].source_id == "contract_no_pragma.vy"
     assert contracts["older_version"].source_id == "older_version.vy"
 
 
 @pytest.mark.parametrize("contract_name", PASSING_CONTRACT_NAMES)
-def test_compile_individual_contracts(contract_name, compiler):
-    path = PASSING_BASE / contract_name
+def test_compile_individual_contracts(project, contract_name, compiler):
+    path = project.contracts_folder / contract_name
     assert compiler.compile([path])
 
 
 @pytest.mark.parametrize(
     "contract_name", [n for n in FAILING_CONTRACT_NAMES if n != "contract_unknown_pragma.vy"]
 )
 def test_compile_failures(contract_name, compiler):
@@ -104,21 +105,22 @@
             continue
 
         sources = ", ".join([p.name for p in actual[version]])
         fail_message = f"Unexpected version '{version}' with sources: {sources}"
         pytest.fail(fail_message)
 
     assert len(actual[OLDER_VERSION_FROM_PRAGMA]) == 1
-    assert len(actual[VERSION_FROM_PRAGMA]) == 8
+    assert len(actual[VERSION_FROM_PRAGMA]) == 9
     assert actual[OLDER_VERSION_FROM_PRAGMA] == {project.contracts_folder / "older_version.vy"}
 
     expected = (
         "contract.vy",
         "contract_no_pragma.vy",
         "contract_with_dev_messages.vy",
+        "empty.vy",
         "erc20.vy",
         "registry_039.vy",
         "traceback_contract_039.vy",
         "use_iface.vy",
         "use_iface2.vy",
     )
     names = [x.name for x in actual[VERSION_FROM_PRAGMA]]
@@ -151,31 +153,31 @@
     vyper_028 = [c for c in manifest.compilers if str(c.version) == str(OLDER_VERSION_FROM_PRAGMA)][
         0
     ]
 
     for compiler in (vyper_028, vyper_latest):
         assert compiler.name == "vyper"
 
-    assert len(vyper_latest.contractTypes) == 8
+    assert len(vyper_latest.contractTypes) == 9
     assert len(vyper_028.contractTypes) == 1
     assert "contract" in vyper_latest.contractTypes
     assert "older_version" in vyper_028.contractTypes
     for compiler in (vyper_latest, vyper_028):
         assert compiler.settings["evmVersion"] == "istanbul"
         assert compiler.settings["optimize"] is True
 
 
-def test_compile_parse_dev_messages(compiler, dev_revert_source):
+def test_compile_parse_dev_messages(compiler, dev_revert_source, project):
     """
     Test parsing of dev messages in a contract. These follow the form of "#dev: ...".
 
     The compiler will output a map that maps dev messages to line numbers.
     See contract_with_dev_messages.vy for more information.
     """
-    result = compiler.compile([dev_revert_source], base_path=PASSING_BASE)
+    result = compiler.compile([dev_revert_source], base_path=project.contracts_folder)
 
     assert len(result) == 1
 
     contract = result[0]
 
     assert contract.dev_messages is not None
     assert len(contract.dev_messages) == 4
@@ -200,23 +202,23 @@
     assert set(actual["contract.vy"]) == {builtin_import}
     assert len(actual["use_iface.vy"]) == 3
     assert set(actual["use_iface.vy"]) == {local_import, local_from_import, dependency_import}
     assert len(actual["use_iface2.vy"]) == 1
     assert set(actual["use_iface2.vy"]) == {local_import}
 
 
-@pytest.mark.parametrize("src,vers", [("contract", "0.3.9"), ("contract_37", "0.3.7")])
+@pytest.mark.parametrize("src,vers", [("contract", "0.3.9"), ("contract_037", "0.3.7")])
 def test_pc_map(compiler, project, src, vers):
     """
     Ensure we de-compress the source map correctly by comparing to the results
     from `compile_src()` which includes the uncompressed source map data.
     """
 
-    path = PASSING_BASE / f"{src}.vy"
-    result = compiler.compile([path], base_path=PASSING_BASE)[0]
+    path = project.contracts_folder / f"{src}.vy"
+    result = compiler.compile([path], base_path=project.contracts_folder)[0]
     actual = result.pcmap.__root__
     code = path.read_text()
     compile_result = compile_source(code, vyper_version=vers, evm_version=compiler.evm_version)[
         "<stdin>"
     ]
     src_map = compile_result["source_map"]
     lines = code.splitlines()
@@ -324,47 +326,78 @@
 
 
 def test_enrich_error_non_payable_check(geth_provider, traceback_contract_037, account):
     with pytest.raises(NonPayableError):
         traceback_contract_037.addBalance(123, sender=account, value=1)
 
 
-@pytest.mark.skipif(APE_VERSION <= Version("0.6.10"), reason="Fallback invoked via new API")
 def test_enrich_error_fallback(geth_provider, traceback_contract_037, account):
     """
     Show that when attempting to call a contract's fallback method when there is
     no fallback defined results in a custom contract logic error.
     """
     with pytest.raises(FallbackNotDefinedError):
         traceback_contract_037(sender=account)
 
 
-def test_trace_source(account, geth_provider, project, traceback_contract):
+def test_enrich_error_handle_when_name(compiler, geth_provider):
     """
-    NOTE: Using 0.3.7 because 0.3.9 bugs and shows the wrong lines.
+    Sometimes, a provider may use the name of the enum instead of the value,
+    which we are still able to enrich.
     """
 
-    receipt = traceback_contract.addBalance(123, sender=account)
+    error = ContractLogicError("")
+    error.__dict__["dev_message"] = "dev: NONPAYABLE_CHECK"
+    new_error = compiler.enrich_error(error)
+    assert isinstance(new_error, NonPayableError)
+
+
+@pytest.mark.parametrize("arguments", [(), (123,), (123, 321)])
+def test_trace_source(account, geth_provider, project, traceback_contract, arguments):
+    receipt = traceback_contract.addBalance(*arguments, sender=account)
     actual = receipt.source_traceback
     base_folder = project.contracts_folder
     contract_name = traceback_contract.contract_type.name
     expected = rf"""
 Traceback (most recent call last)
   File {base_folder}/{contract_name}.vy, in addBalance
-       27     # Comments in the middle (is a test)
-       28
-       29     for i in [1, 2, 3, 4, 5]:
-       30         if i != num:
-       31             continue
-       32
-  -->  33     return self._balance
+       32         if i != num:
+       33             continue
+       34
+  -->  35     return self._balance
 """.strip()
     assert str(actual) == expected
 
 
+def test_trace_source_content_from_kwarg_default_parametrization(
+    account, geth_provider, project, traceback_contract
+):
+    """
+    This test is for verifying stuff around Vyper auto-generated methods from kwarg defaults.
+    Mostly, need to make sure the correct content is discoverable in the source traceback
+    so that coverage works properly.
+    """
+    no_args_tx = traceback_contract.addBalance(sender=account)
+    no_args_tb = no_args_tx.source_traceback
+
+    def check(name: str, tb):
+        items = [x.closure.full_name for x in tb if x.closure.full_name == name]
+        assert len(items) >= 1
+
+    check("addBalance()", no_args_tb)
+
+    single_arg_tx = traceback_contract.addBalance(442, sender=account)
+    single_arg_tb = single_arg_tx.source_traceback
+    check("addBalance(uint256)", single_arg_tb)
+
+    both_args_tx = traceback_contract.addBalance(4, 5, sender=account)
+    both_args_tb = both_args_tx.source_traceback
+    check("addBalance(uint256,uint256)", both_args_tb)
+
+
 def test_trace_err_source(account, geth_provider, project, traceback_contract):
     txn = traceback_contract.addBalance_f.as_transaction(123)
     try:
         account.call(txn)
     except ContractLogicError:
         pass
 
@@ -372,36 +405,33 @@
     actual = receipt.source_traceback
     base_folder = project.contracts_folder
     contract_name = traceback_contract.contract_type.name
     version_key = contract_name.split("traceback_contract_")[-1]
     expected = rf"""
 Traceback (most recent call last)
   File {base_folder}/{contract_name}.vy, in addBalance_f
-       44     # Run some loops.
-       45     for i in [1, 2, 3, 4, 5]:
-       46         if i == num:
-       47             break
-       48
-       49     # Fail in the middle (is test)
-       50     # Fails because was already set above.
-  -->  51     self.registry.register_f(msg.sender)
-       52
-       53     for i in [1, 2, 3, 4, 5]:
-       54         if i != num:
-       55             continue
+       48         if i == num:
+       49             break
+       50
+       51     # Fail in the middle (is test)
+       52     # Fails because was already set above.
+  -->  53     self.registry.register_f(msg.sender)
+       54
+       55     for i in [1, 2, 3, 4, 5]:
+       56         if i != num:
+       57             continue
 
   File {base_folder}/registry_{version_key}.vy, in register_f
        11 def register_f(addr: address):
   -->  12     assert self.addr != addr, "doubling."
        13     self.addr = addr
     """.strip()
     assert str(actual) == expected
 
 
-@pytest.mark.skipif(APE_VERSION <= Version("0.6.10"), reason="Fallback invoked via new API")
 def test_trace_source_default_method(geth_provider, account, project):
     """
     This test proves you get a working source-traceback from __default__ calls.
     """
     contract = project.non_payable_default.deploy(sender=account)
     receipt = contract(sender=account)
     src_tb = receipt.source_traceback
```

