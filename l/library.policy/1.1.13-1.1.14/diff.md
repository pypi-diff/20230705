# Comparing `tmp/library.policy-1.1.13.tar.gz` & `tmp/library.policy-1.1.14.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/library.policy-1.1.13.tar", last modified: Mon Feb 28 11:52:15 2022, max compression
+gzip compressed data, was "library.policy-1.1.14.tar", last modified: Wed Jul  5 10:53:10 2023, max compression
```

## Comparing `library.policy-1.1.13.tar` & `library.policy-1.1.14.tar`

### file list

```diff
@@ -1,75 +1,74 @@
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2022-02-28 11:52:15.000000 library.policy-1.1.13/
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2022-02-28 11:52:15.000000 library.policy-1.1.13/docs/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)       63 2022-02-28 11:52:14.000000 library.policy-1.1.13/docs/index.rst
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)       39 2022-02-28 11:52:14.000000 library.policy-1.1.13/requirements.txt
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      297 2022-02-28 11:52:14.000000 library.policy-1.1.13/DEVELOP.rst
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     6863 2022-02-28 11:52:15.000000 library.policy-1.1.13/PKG-INFO
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      112 2022-02-28 11:52:14.000000 library.policy-1.1.13/CONTRIBUTORS.rst
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1413 2022-02-28 11:52:14.000000 library.policy-1.1.13/README.rst
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)    18092 2022-02-28 11:52:14.000000 library.policy-1.1.13/LICENSE.GPL
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2655 2022-02-28 11:52:14.000000 library.policy-1.1.13/CHANGES.rst
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      154 2022-02-28 11:52:14.000000 library.policy-1.1.13/MANIFEST.in
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2500 2022-02-28 11:52:14.000000 library.policy-1.1.13/setup.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      660 2022-02-28 11:52:14.000000 library.policy-1.1.13/LICENSE.rst
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      280 2022-02-28 11:52:15.000000 library.policy-1.1.13/setup.cfg
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2022-02-28 11:52:15.000000 library.policy-1.1.13/src/
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2022-02-28 11:52:15.000000 library.policy-1.1.13/src/library.policy.egg-info/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        8 2022-02-28 11:52:14.000000 library.policy-1.1.13/src/library.policy.egg-info/top_level.txt
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     6863 2022-02-28 11:52:14.000000 library.policy-1.1.13/src/library.policy.egg-info/PKG-INFO
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        1 2022-02-28 11:52:14.000000 library.policy-1.1.13/src/library.policy.egg-info/dependency_links.txt
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      546 2022-02-28 11:52:14.000000 library.policy-1.1.13/src/library.policy.egg-info/requires.txt
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        8 2022-02-28 11:52:14.000000 library.policy-1.1.13/src/library.policy.egg-info/namespace_packages.txt
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1922 2022-02-28 11:52:14.000000 library.policy-1.1.13/src/library.policy.egg-info/SOURCES.txt
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        1 2022-02-28 11:52:14.000000 library.policy-1.1.13/src/library.policy.egg-info/not-zip-safe
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        5 2022-02-28 11:52:14.000000 library.policy-1.1.13/src/library.policy.egg-info/entry_points.txt
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2022-02-28 11:52:15.000000 library.policy-1.1.13/src/library/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)       80 2022-02-28 11:52:14.000000 library.policy-1.1.13/src/library/__init__.py
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2022-02-28 11:52:15.000000 library.policy-1.1.13/src/library/policy/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1430 2022-02-28 11:52:14.000000 library.policy-1.1.13/src/library/policy/testing.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      263 2022-02-28 11:52:14.000000 library.policy-1.1.13/src/library/policy/interfaces.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     4264 2022-02-28 11:52:14.000000 library.policy-1.1.13/src/library/policy/setuphandlers.py
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2022-02-28 11:52:15.000000 library.policy-1.1.13/src/library/policy/tests/
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2022-02-28 11:52:15.000000 library.policy-1.1.13/src/library/policy/tests/robot/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1987 2022-02-28 11:52:14.000000 library.policy-1.1.13/src/library/policy/tests/robot/test_example.robot
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2022-02-28 11:52:14.000000 library.policy-1.1.13/src/library/policy/tests/__init__.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2013 2022-02-28 11:52:14.000000 library.policy-1.1.13/src/library/policy/tests/test_setup.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      872 2022-02-28 11:52:14.000000 library.policy-1.1.13/src/library/policy/tests/test_robot.py
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2022-02-28 11:52:15.000000 library.policy-1.1.13/src/library/policy/faceted/
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2022-02-28 11:52:15.000000 library.policy-1.1.13/src/library/policy/faceted/templates/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     5120 2022-02-28 11:52:14.000000 library.policy-1.1.13/src/library/policy/faceted/templates/explorer.pt
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2022-02-28 11:52:15.000000 library.policy-1.1.13/src/library/policy/faceted/config/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     4844 2022-02-28 11:52:14.000000 library.policy-1.1.13/src/library/policy/faceted/config/explorer.xml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2022-02-28 11:52:14.000000 library.policy-1.1.13/src/library/policy/faceted/__init__.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2025 2022-02-28 11:52:14.000000 library.policy-1.1.13/src/library/policy/faceted/explorer.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      433 2022-02-28 11:52:14.000000 library.policy-1.1.13/src/library/policy/faceted/configure.zcml
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2022-02-28 11:52:15.000000 library.policy-1.1.13/src/library/policy/profiles/
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2022-02-28 11:52:15.000000 library.policy-1.1.13/src/library/policy/profiles/uninstall/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      124 2022-02-28 11:52:14.000000 library.policy-1.1.13/src/library/policy/profiles/uninstall/browserlayer.xml
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2022-02-28 11:52:15.000000 library.policy-1.1.13/src/library/policy/profiles/default/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      713 2022-02-28 11:52:14.000000 library.policy-1.1.13/src/library/policy/profiles/default/registry.xml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      105 2022-02-28 11:52:14.000000 library.policy-1.1.13/src/library/policy/profiles/default/catalog.xml
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2022-02-28 11:52:15.000000 library.policy-1.1.13/src/library/policy/profiles/default/types/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2626 2022-02-28 11:52:14.000000 library.policy-1.1.13/src/library/policy/profiles/default/types/Document.xml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2644 2022-02-28 11:52:14.000000 library.policy-1.1.13/src/library/policy/profiles/default/types/Folder.xml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      280 2022-02-28 11:52:14.000000 library.policy-1.1.13/src/library/policy/profiles/default/types.xml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1074 2022-02-28 11:52:14.000000 library.policy-1.1.13/src/library/policy/profiles/default/metadata.xml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      118 2022-02-28 11:52:14.000000 library.policy-1.1.13/src/library/policy/profiles/default/rolemap.xml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      168 2022-02-28 11:52:14.000000 library.policy-1.1.13/src/library/policy/profiles/default/browserlayer.xml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      624 2022-02-28 11:52:14.000000 library.policy-1.1.13/src/library/policy/upgrades.zcml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      666 2022-02-28 11:52:14.000000 library.policy-1.1.13/src/library/policy/upgrades.py
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2022-02-28 11:52:15.000000 library.policy-1.1.13/src/library/policy/locales/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1409 2022-02-28 11:52:14.000000 library.policy-1.1.13/src/library/policy/locales/library.policy.pot
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2022-02-28 11:52:15.000000 library.policy-1.1.13/src/library/policy/locales/fr/
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2022-02-28 11:52:15.000000 library.policy-1.1.13/src/library/policy/locales/fr/LC_MESSAGES/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1327 2022-02-28 11:52:14.000000 library.policy-1.1.13/src/library/policy/locales/fr/LC_MESSAGES/library.policy.po
--rwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)      479 2022-02-28 11:52:14.000000 library.policy-1.1.13/src/library/policy/locales/update.sh
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      260 2022-02-28 11:52:14.000000 library.policy-1.1.13/src/library/policy/permissions.zcml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      131 2022-02-28 11:52:14.000000 library.policy-1.1.13/src/library/policy/__init__.py
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2022-02-28 11:52:15.000000 library.policy-1.1.13/src/library/policy/browser/
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2022-02-28 11:52:15.000000 library.policy-1.1.13/src/library/policy/browser/static/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2022-02-28 11:52:14.000000 library.policy-1.1.13/src/library/policy/browser/static/.gitkeep
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2022-02-28 11:52:15.000000 library.policy-1.1.13/src/library/policy/browser/overrides/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2022-02-28 11:52:14.000000 library.policy-1.1.13/src/library/policy/browser/overrides/.gitkeep
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2022-02-28 11:52:14.000000 library.policy-1.1.13/src/library/policy/browser/__init__.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      574 2022-02-28 11:52:14.000000 library.policy-1.1.13/src/library/policy/browser/configure.zcml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2168 2022-02-28 11:52:14.000000 library.policy-1.1.13/src/library/policy/configure.zcml
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-07-05 10:53:10.347841 library.policy-1.1.14/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2791 2023-07-05 10:53:09.000000 library.policy-1.1.14/CHANGES.rst
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      112 2023-07-05 10:53:09.000000 library.policy-1.1.14/CONTRIBUTORS.rst
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      297 2023-07-05 10:53:09.000000 library.policy-1.1.14/DEVELOP.rst
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)    18092 2023-07-05 10:53:09.000000 library.policy-1.1.14/LICENSE.GPL
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      660 2023-07-05 10:53:09.000000 library.policy-1.1.14/LICENSE.rst
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      154 2023-07-05 10:53:09.000000 library.policy-1.1.14/MANIFEST.in
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     5449 2023-07-05 10:53:10.347841 library.policy-1.1.14/PKG-INFO
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1778 2023-07-05 10:53:09.000000 library.policy-1.1.14/README.rst
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-07-05 10:53:10.343841 library.policy-1.1.14/docs/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)       63 2023-07-05 10:53:09.000000 library.policy-1.1.14/docs/index.rst
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)       58 2023-07-05 10:53:09.000000 library.policy-1.1.14/requirements.txt
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      280 2023-07-05 10:53:10.347841 library.policy-1.1.14/setup.cfg
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2522 2023-07-05 10:53:09.000000 library.policy-1.1.14/setup.py
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-07-05 10:53:10.339841 library.policy-1.1.14/src/
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-07-05 10:53:10.343841 library.policy-1.1.14/src/library/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)       80 2023-07-05 10:53:09.000000 library.policy-1.1.14/src/library/__init__.py
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-07-05 10:53:10.343841 library.policy-1.1.14/src/library/policy/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      131 2023-07-05 10:53:09.000000 library.policy-1.1.14/src/library/policy/__init__.py
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-07-05 10:53:10.343841 library.policy-1.1.14/src/library/policy/browser/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2023-07-05 10:53:09.000000 library.policy-1.1.14/src/library/policy/browser/__init__.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      574 2023-07-05 10:53:09.000000 library.policy-1.1.14/src/library/policy/browser/configure.zcml
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-07-05 10:53:10.343841 library.policy-1.1.14/src/library/policy/browser/overrides/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2023-07-05 10:53:09.000000 library.policy-1.1.14/src/library/policy/browser/overrides/.gitkeep
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-07-05 10:53:10.343841 library.policy-1.1.14/src/library/policy/browser/static/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2023-07-05 10:53:09.000000 library.policy-1.1.14/src/library/policy/browser/static/.gitkeep
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2203 2023-07-05 10:53:09.000000 library.policy-1.1.14/src/library/policy/configure.zcml
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-07-05 10:53:10.347841 library.policy-1.1.14/src/library/policy/faceted/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2023-07-05 10:53:09.000000 library.policy-1.1.14/src/library/policy/faceted/__init__.py
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-07-05 10:53:10.347841 library.policy-1.1.14/src/library/policy/faceted/config/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     4808 2023-07-05 10:53:09.000000 library.policy-1.1.14/src/library/policy/faceted/config/explorer.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      433 2023-07-05 10:53:09.000000 library.policy-1.1.14/src/library/policy/faceted/configure.zcml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2025 2023-07-05 10:53:09.000000 library.policy-1.1.14/src/library/policy/faceted/explorer.py
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-07-05 10:53:10.347841 library.policy-1.1.14/src/library/policy/faceted/templates/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     5120 2023-07-05 10:53:09.000000 library.policy-1.1.14/src/library/policy/faceted/templates/explorer.pt
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      263 2023-07-05 10:53:09.000000 library.policy-1.1.14/src/library/policy/interfaces.py
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-07-05 10:53:10.347841 library.policy-1.1.14/src/library/policy/locales/
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-07-05 10:53:10.339841 library.policy-1.1.14/src/library/policy/locales/fr/
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-07-05 10:53:10.347841 library.policy-1.1.14/src/library/policy/locales/fr/LC_MESSAGES/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1327 2023-07-05 10:53:09.000000 library.policy-1.1.14/src/library/policy/locales/fr/LC_MESSAGES/library.policy.po
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1409 2023-07-05 10:53:09.000000 library.policy-1.1.14/src/library/policy/locales/library.policy.pot
+-rwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)      479 2023-07-05 10:53:09.000000 library.policy-1.1.14/src/library/policy/locales/update.sh
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      260 2023-07-05 10:53:09.000000 library.policy-1.1.14/src/library/policy/permissions.zcml
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-07-05 10:53:10.343841 library.policy-1.1.14/src/library/policy/profiles/
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-07-05 10:53:10.347841 library.policy-1.1.14/src/library/policy/profiles/default/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      168 2023-07-05 10:53:09.000000 library.policy-1.1.14/src/library/policy/profiles/default/browserlayer.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      105 2023-07-05 10:53:09.000000 library.policy-1.1.14/src/library/policy/profiles/default/catalog.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1074 2023-07-05 10:53:09.000000 library.policy-1.1.14/src/library/policy/profiles/default/metadata.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      713 2023-07-05 10:53:09.000000 library.policy-1.1.14/src/library/policy/profiles/default/registry.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      118 2023-07-05 10:53:09.000000 library.policy-1.1.14/src/library/policy/profiles/default/rolemap.xml
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-07-05 10:53:10.347841 library.policy-1.1.14/src/library/policy/profiles/default/types/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2626 2023-07-05 10:53:09.000000 library.policy-1.1.14/src/library/policy/profiles/default/types/Document.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2644 2023-07-05 10:53:09.000000 library.policy-1.1.14/src/library/policy/profiles/default/types/Folder.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      280 2023-07-05 10:53:09.000000 library.policy-1.1.14/src/library/policy/profiles/default/types.xml
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-07-05 10:53:10.347841 library.policy-1.1.14/src/library/policy/profiles/uninstall/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      124 2023-07-05 10:53:09.000000 library.policy-1.1.14/src/library/policy/profiles/uninstall/browserlayer.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     4263 2023-07-05 10:53:09.000000 library.policy-1.1.14/src/library/policy/setuphandlers.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1429 2023-07-05 10:53:09.000000 library.policy-1.1.14/src/library/policy/testing.py
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-07-05 10:53:10.347841 library.policy-1.1.14/src/library/policy/tests/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2023-07-05 10:53:09.000000 library.policy-1.1.14/src/library/policy/tests/__init__.py
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-07-05 10:53:10.347841 library.policy-1.1.14/src/library/policy/tests/robot/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1987 2023-07-05 10:53:09.000000 library.policy-1.1.14/src/library/policy/tests/robot/test_example.robot
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      922 2023-07-05 10:53:09.000000 library.policy-1.1.14/src/library/policy/tests/test_robot.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2012 2023-07-05 10:53:09.000000 library.policy-1.1.14/src/library/policy/tests/test_setup.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1374 2023-07-05 10:53:09.000000 library.policy-1.1.14/src/library/policy/upgrades.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      865 2023-07-05 10:53:09.000000 library.policy-1.1.14/src/library/policy/upgrades.zcml
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-07-05 10:53:10.343841 library.policy-1.1.14/src/library.policy.egg-info/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     5449 2023-07-05 10:53:10.000000 library.policy-1.1.14/src/library.policy.egg-info/PKG-INFO
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1877 2023-07-05 10:53:10.000000 library.policy-1.1.14/src/library.policy.egg-info/SOURCES.txt
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        1 2023-07-05 10:53:10.000000 library.policy-1.1.14/src/library.policy.egg-info/dependency_links.txt
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        8 2023-07-05 10:53:10.000000 library.policy-1.1.14/src/library.policy.egg-info/namespace_packages.txt
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        1 2023-07-05 10:53:10.000000 library.policy-1.1.14/src/library.policy.egg-info/not-zip-safe
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      557 2023-07-05 10:53:10.000000 library.policy-1.1.14/src/library.policy.egg-info/requires.txt
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        8 2023-07-05 10:53:10.000000 library.policy-1.1.14/src/library.policy.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `library.policy-1.1.13/README.rst` & `library.policy-1.1.14/README.rst`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,19 @@
 .. This README is meant for consumption by humans and pypi. Pypi can render rst files so please do not use Sphinx features.
    If you want to learn more about writing documentation, please check out: http://docs.plone.org/about/documentation_styleguide.html
    This text does not appear on pypi or github. It is a comment.
 
+.. image:: https://github.com/IMIO/library.policy/workflows/Tests/badge.svg
+    :target: https://github.com/IMIO/library.policy/actions?query=workflow%3ATests
+    :alt: CI Status
+
+.. image:: https://coveralls.io/repos/github/IMIO/library.policy/badge.svg?branch=master
+    :target: https://coveralls.io/github/IMIO/library.policy?branch=master
+    :alt: Coveralls
+
 ==============
 library.policy
 ==============
 
 Tell me what your product does
 
 Features
```

### Comparing `library.policy-1.1.13/LICENSE.GPL` & `library.policy-1.1.14/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `library.policy-1.1.13/CHANGES.rst` & `library.policy-1.1.14/CHANGES.rst`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,18 @@
 Changelog
 =========
 
 
+1.1.14 (2023-07-05)
+-------------------
+
+- Create upgrade step to reimport faceted "explorer" config (Fix select2 widgets)
+  [boulch]
+
+
 1.1.13 (2022-02-28)
 -------------------
 
 - Add collective.big.bang dependency
   [boulch]
```

### Comparing `library.policy-1.1.13/setup.py` & `library.policy-1.1.14/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,15 +12,15 @@
         open("CHANGES.rst").read(),
     ]
 )
 
 
 setup(
     name="library.policy",
-    version="1.1.13",
+    version="1.1.14",
     description="Policy for the installation of buildout.library",
     long_description=long_description,
     # Get more from https://pypi.python.org/pypi?%3Aaction=list_classifiers
     classifiers=[
         "Environment :: Web Environment",
         "Framework :: Plone",
         "Framework :: Plone :: 5.2",
@@ -44,14 +44,15 @@
     install_requires=[
         # -*- Extra requirements: -*-
         "plone.api>=1.8.4",
         "Products.GenericSetup>=1.8.2",
         "setuptools",
         "z3c.jbot",
         "eea.facetednavigation",
+        "eea.jquery",
         "collective.big.bang",
         "collective.faceted.map",
         "collective.faceted.taxonomywidget",
         "collective.taxonomy",
         "plone.app.imagecropping",
         "plone.app.mosaic",
         "library.core",
```

### Comparing `library.policy-1.1.13/LICENSE.rst` & `library.policy-1.1.14/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `library.policy-1.1.13/src/library.policy.egg-info/requires.txt` & `library.policy-1.1.14/src/library.policy.egg-info/requires.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 plone.api>=1.8.4
 Products.GenericSetup>=1.8.2
 setuptools
 z3c.jbot
 eea.facetednavigation
+eea.jquery
 collective.big.bang
 collective.faceted.map
 collective.faceted.taxonomywidget
 collective.taxonomy
 plone.app.imagecropping
 plone.app.mosaic
 library.core
```

### Comparing `library.policy-1.1.13/src/library.policy.egg-info/SOURCES.txt` & `library.policy-1.1.14/src/library.policy.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 setup.cfg
 setup.py
 docs/index.rst
 src/library/__init__.py
 src/library.policy.egg-info/PKG-INFO
 src/library.policy.egg-info/SOURCES.txt
 src/library.policy.egg-info/dependency_links.txt
-src/library.policy.egg-info/entry_points.txt
 src/library.policy.egg-info/namespace_packages.txt
 src/library.policy.egg-info/not-zip-safe
 src/library.policy.egg-info/requires.txt
 src/library.policy.egg-info/top_level.txt
 src/library/policy/__init__.py
 src/library/policy/configure.zcml
 src/library/policy/interfaces.py
```

### Comparing `library.policy-1.1.13/src/library/policy/testing.py` & `library.policy-1.1.14/src/library/policy/testing.py`

 * *Files 13% similar despite different names*

```diff
@@ -7,43 +7,42 @@
 from plone.app.testing import PloneSandboxLayer
 from plone.testing import z2
 
 import library.policy
 
 
 class LibraryPolicyLayer(PloneSandboxLayer):
-
     defaultBases = (PLONE_APP_CONTENTTYPES_FIXTURE,)
 
     def setUpZope(self, app, configurationContext):
         # Load any other ZCML that is required for your tests.
         # The z3c.autoinclude feature is disabled in the Plone fixture base
         # layer.
         self.loadZCML(package=library.policy)
 
     def setUpPloneSite(self, portal):
-        applyProfile(portal, 'library.policy:default')
+        applyProfile(portal, "library.policy:default")
 
 
 LIBRARY_POLICY_FIXTURE = LibraryPolicyLayer()
 
 
 LIBRARY_POLICY_INTEGRATION_TESTING = IntegrationTesting(
     bases=(LIBRARY_POLICY_FIXTURE,),
-    name='LibraryPolicyLayer:IntegrationTesting',
+    name="LibraryPolicyLayer:IntegrationTesting",
 )
 
 
 LIBRARY_POLICY_FUNCTIONAL_TESTING = FunctionalTesting(
     bases=(LIBRARY_POLICY_FIXTURE,),
-    name='LibraryPolicyLayer:FunctionalTesting',
+    name="LibraryPolicyLayer:FunctionalTesting",
 )
 
 
 LIBRARY_POLICY_ACCEPTANCE_TESTING = FunctionalTesting(
     bases=(
         LIBRARY_POLICY_FIXTURE,
         REMOTE_LIBRARY_BUNDLE_FIXTURE,
         z2.ZSERVER_FIXTURE,
     ),
-    name='LibraryPolicyLayer:AcceptanceTesting',
+    name="LibraryPolicyLayer:AcceptanceTesting",
 )
```

### Comparing `library.policy-1.1.13/src/library/policy/setuphandlers.py` & `library.policy-1.1.14/src/library/policy/setuphandlers.py`

 * *Files 4% similar despite different names*

```diff
@@ -88,15 +88,15 @@
     create_taxonomy_object(data_villages)
     create_taxonomy_object(data_periodes)
 
 
 def add_stucture(portal):
     # Folder professionals
     if "explorer" not in portal:
-        obj = create_content("Folder", _(u"explorer"), portal)
+        obj = create_content("Folder", _("explorer"), portal)
         _activate_dashboard_navigation(obj, True, "/faceted/config/explorer.xml")
         explorer_layout = FacetedLayout(obj)
         explorer_layout.update_layout(layout="faceted-explorer")
         _publish(obj)
 
 
 def create_taxonomy_object(data_tax):
```

### Comparing `library.policy-1.1.13/src/library/policy/tests/robot/test_example.robot` & `library.policy-1.1.14/src/library/policy/tests/robot/test_example.robot`

 * *Files identical despite different names*

### Comparing `library.policy-1.1.13/src/library/policy/tests/test_setup.py` & `library.policy-1.1.14/src/library/policy/tests/test_setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,14 @@
         from library.policy.interfaces import ILibraryPolicyLayer
         from plone.browserlayer import utils
 
         self.assertIn(ILibraryPolicyLayer, utils.registered_layers())
 
 
 class TestUninstall(unittest.TestCase):
-
     layer = LIBRARY_POLICY_INTEGRATION_TESTING
 
     def setUp(self):
         self.portal = self.layer["portal"]
         self.installer = get_installer(self.portal, self.layer["request"])
         roles_before = api.user.get_roles(TEST_USER_ID)
         setRoles(self.portal, TEST_USER_ID, ["Manager"])
```

### Comparing `library.policy-1.1.13/src/library/policy/tests/test_robot.py` & `library.policy-1.1.14/src/library/policy/tests/test_robot.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,22 +7,25 @@
 import robotsuite
 import unittest
 
 
 def test_suite():
     suite = unittest.TestSuite()
     current_dir = os.path.abspath(os.path.dirname(__file__))
-    robot_dir = os.path.join(current_dir, 'robot')
+    robot_dir = os.path.join(current_dir, "robot")
     robot_tests = [
-        os.path.join('robot', doc) for doc in os.listdir(robot_dir)
-        if doc.endswith('.robot') and doc.startswith('test_')
+        os.path.join("robot", doc)
+        for doc in os.listdir(robot_dir)
+        if doc.endswith(".robot") and doc.startswith("test_")
     ]
     for robot_test in robot_tests:
         robottestsuite = robotsuite.RobotTestSuite(robot_test)
         robottestsuite.level = ROBOT_TEST_LEVEL
-        suite.addTests([
-            layered(
-                robottestsuite,
-                layer=LIBRARY_POLICY_ACCEPTANCE_TESTING,
-            ),
-        ])
+        suite.addTests(
+            [
+                layered(
+                    robottestsuite,
+                    layer=LIBRARY_POLICY_ACCEPTANCE_TESTING,
+                ),
+            ]
+        )
     return suite
```

### Comparing `library.policy-1.1.13/src/library/policy/faceted/templates/explorer.pt` & `library.policy-1.1.14/src/library/policy/faceted/templates/explorer.pt`

 * *Files identical despite different names*

### Comparing `library.policy-1.1.13/src/library/policy/faceted/config/explorer.xml` & `library.policy-1.1.14/src/library/policy/faceted/config/explorer.xml`

 * *Files 4% similar despite different names*

#### Comparing `library.policy-1.1.13/src/library/policy/faceted/config/explorer.xml` & `library.policy-1.1.14/src/library/policy/faceted/config/explorer.xml`

```diff
@@ -1,72 +1,72 @@
 <?xml version="1.0" encoding="utf-8"?>
 <object name="explorer" meta_type="Dexterity Container">
   <criteria>
+    <criterion name="c8">
+      <property name="widget">text</property>
+      <property name="title">Chercher</property>
+      <property name="index">SearchableText</property>
+      <property name="onlyallelements">True</property>
+      <property name="wildcard">True</property>
+      <property name="position">center</property>
+      <property name="section">default</property>
+      <property name="hidden">False</property>
+    </criterion>
     <criterion name="c4">
-      <property name="widget">taxonomy_select2</property>
+      <property name="widget">select2</property>
       <property name="title">Dossiers</property>
       <property name="index">taxonomy_dossiers</property>
       <property name="vocabulary">collective.taxonomy.dossiers</property>
       <property name="position">center</property>
       <property name="section">default</property>
       <property name="hidden">False</property>
       <property name="count">True</property>
       <property name="sortcountable">False</property>
       <property name="hidezerocount">True</property>
       <property name="sortreversed">False</property>
     </criterion>
     <criterion name="c5">
-      <property name="widget">taxonomy_select2</property>
+      <property name="widget">select2</property>
       <property name="title">Types de patrimoines</property>
       <property name="index">taxonomy_patrimoine</property>
       <property name="vocabulary">collective.taxonomy.patrimoine</property>
       <property name="position">center</property>
       <property name="section">default</property>
       <property name="hidden">False</property>
       <property name="count">True</property>
       <property name="sortcountable">False</property>
       <property name="hidezerocount">True</property>
       <property name="sortreversed">False</property>
     </criterion>
     <criterion name="c6">
-      <property name="widget">taxonomy_select2</property>
+      <property name="widget">select2</property>
       <property name="title">Villages</property>
       <property name="index">taxonomy_villages</property>
       <property name="vocabulary">collective.taxonomy.villages</property>
       <property name="position">center</property>
       <property name="section">default</property>
       <property name="hidden">False</property>
       <property name="count">True</property>
       <property name="sortcountable">False</property>
       <property name="hidezerocount">True</property>
       <property name="sortreversed">False</property>
     </criterion>
     <criterion name="c7">
-      <property name="widget">taxonomy_select2</property>
+      <property name="widget">select2</property>
       <property name="title">périodes</property>
       <property name="index">taxonomy_periodes</property>
       <property name="vocabulary">collective.taxonomy.periodes</property>
       <property name="position">center</property>
       <property name="section">default</property>
       <property name="hidden">False</property>
       <property name="count">True</property>
       <property name="sortcountable">False</property>
       <property name="hidezerocount">True</property>
       <property name="sortreversed">False</property>
     </criterion>
-    <criterion name="c8">
-      <property name="widget">text</property>
-      <property name="title">Chercher</property>
-      <property name="index">SearchableText</property>
-      <property name="onlyallelements">True</property>
-      <property name="wildcard">True</property>
-      <property name="position">center</property>
-      <property name="section">default</property>
-      <property name="hidden">False</property>
-    </criterion>
     <criterion name="c3">
       <property name="widget">criteria</property>
       <property name="title">Current search</property>
       <property name="hidecriteriaenabled">False</property>
       <property name="position">center</property>
       <property name="section">default</property>
       <property name="hidden">False</property>
```

### Comparing `library.policy-1.1.13/src/library/policy/faceted/explorer.py` & `library.policy-1.1.14/src/library/policy/faceted/explorer.py`

 * *Files identical despite different names*

### Comparing `library.policy-1.1.13/src/library/policy/profiles/default/registry.xml` & `library.policy-1.1.14/src/library/policy/profiles/default/registry.xml`

 * *Files identical despite different names*

### Comparing `library.policy-1.1.13/src/library/policy/profiles/default/types/Document.xml` & `library.policy-1.1.14/src/library/policy/profiles/default/types/Document.xml`

 * *Files identical despite different names*

### Comparing `library.policy-1.1.13/src/library/policy/profiles/default/types/Folder.xml` & `library.policy-1.1.14/src/library/policy/profiles/default/types/Folder.xml`

 * *Files identical despite different names*

### Comparing `library.policy-1.1.13/src/library/policy/profiles/default/metadata.xml` & `library.policy-1.1.14/src/library/policy/profiles/default/metadata.xml`

 * *Files 1% similar despite different names*

#### Comparing `library.policy-1.1.13/src/library/policy/profiles/default/metadata.xml` & `library.policy-1.1.14/src/library/policy/profiles/default/metadata.xml`

```diff
@@ -1,10 +1,10 @@
 <?xml version="1.0" encoding="utf-8"?>
 <metadata>
-  <version>1002</version>
+  <version>1003</version>
   <dependencies>
     <dependency>profile-eea.facetednavigation:default</dependency>
     <dependency>profile-collective.behavior.banner:default</dependency>
     <dependency>profile-collective.behavior.gallery:default</dependency>
     <dependency>profile-collective.easyform:default</dependency>
     <dependency>profile-collective.preventactions:default</dependency>
     <dependency>profile-collective.taxonomy:default</dependency>
```

### Comparing `library.policy-1.1.13/src/library/policy/locales/library.policy.pot` & `library.policy-1.1.14/src/library/policy/locales/library.policy.pot`

 * *Files identical despite different names*

### Comparing `library.policy-1.1.13/src/library/policy/locales/fr/LC_MESSAGES/library.policy.po` & `library.policy-1.1.14/src/library/policy/locales/fr/LC_MESSAGES/library.policy.po`

 * *Files identical despite different names*

### Comparing `library.policy-1.1.13/src/library/policy/browser/configure.zcml` & `library.policy-1.1.14/src/library/policy/browser/configure.zcml`

 * *Files identical despite different names*

### Comparing `library.policy-1.1.13/src/library/policy/configure.zcml` & `library.policy-1.1.14/src/library/policy/configure.zcml`

 * *Files 1% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 
   <!--
     Be careful if you use general includeDependencies, it can have sideffects!
     Better import explicite packages or configurations ;)
   -->
   <!--<includeDependencies package="." />-->
   <include package="eea.facetednavigation" />
+  <include package="eea.jquery" />
   <include package="collective.big.bang" />
   <include package="collective.faceted.map" />
   <include package="collective.geolocationbehavior" />
   <include package="collective.faceted.taxonomywidget" />
   <include package="collective.taxonomy" />
   <include package="plone.app.imagecropping" />
   <include package="plone.app.mosaic" />
```

