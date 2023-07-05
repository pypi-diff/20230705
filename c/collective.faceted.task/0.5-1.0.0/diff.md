# Comparing `tmp/collective.faceted.task-0.5.tar.gz` & `tmp/collective.faceted.task-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/collective.faceted.task-0.5.tar", last modified: Thu Apr  6 15:08:03 2023, max compression
+gzip compressed data, was "dist/collective.faceted.task-1.0.0.tar", last modified: Wed Jul  5 07:14:49 2023, max compression
```

## Comparing `collective.faceted.task-0.5.tar` & `collective.faceted.task-1.0.0.tar`

### file list

```diff
@@ -1,87 +1,89 @@
-drwxrwxr-x   0 fngaha    (1000) fngaha    (1000)        0 2023-04-06 15:08:03.000000 collective.faceted.task-0.5/
-drwxrwxr-x   0 fngaha    (1000) fngaha    (1000)        0 2023-04-06 15:08:03.000000 collective.faceted.task-0.5/docs/
--rw-rw-r--   0 fngaha    (1000) fngaha    (1000)        0 2023-04-06 15:08:03.000000 collective.faceted.task-0.5/docs/LICENSE.rst
--rw-rw-r--   0 fngaha    (1000) fngaha    (1000)    18092 2023-04-06 15:08:03.000000 collective.faceted.task-0.5/docs/LICENSE.GPL
--rw-rw-r--   0 fngaha    (1000) fngaha    (1000)      172 2023-04-06 15:08:03.000000 collective.faceted.task-0.5/travis.cfg
-drwxrwxr-x   0 fngaha    (1000) fngaha    (1000)        0 2023-04-06 15:08:03.000000 collective.faceted.task-0.5/src/
-drwxrwxr-x   0 fngaha    (1000) fngaha    (1000)        0 2023-04-06 15:08:03.000000 collective.faceted.task-0.5/src/collective.faceted.task.egg-info/
--rw-rw-r--   0 fngaha    (1000) fngaha    (1000)      126 2023-04-06 15:08:03.000000 collective.faceted.task-0.5/src/collective.faceted.task.egg-info/requires.txt
--rw-rw-r--   0 fngaha    (1000) fngaha    (1000)     1467 2023-04-06 15:08:03.000000 collective.faceted.task-0.5/src/collective.faceted.task.egg-info/PKG-INFO
--rw-rw-r--   0 fngaha    (1000) fngaha    (1000)        1 2023-04-06 15:08:03.000000 collective.faceted.task-0.5/src/collective.faceted.task.egg-info/not-zip-safe
--rw-rw-r--   0 fngaha    (1000) fngaha    (1000)       30 2023-04-06 15:08:03.000000 collective.faceted.task-0.5/src/collective.faceted.task.egg-info/namespace_packages.txt
--rw-rw-r--   0 fngaha    (1000) fngaha    (1000)        1 2023-04-06 15:08:03.000000 collective.faceted.task-0.5/src/collective.faceted.task.egg-info/dependency_links.txt
--rw-rw-r--   0 fngaha    (1000) fngaha    (1000)       11 2023-04-06 15:08:03.000000 collective.faceted.task-0.5/src/collective.faceted.task.egg-info/top_level.txt
--rw-rw-r--   0 fngaha    (1000) fngaha    (1000)       53 2023-04-06 15:08:03.000000 collective.faceted.task-0.5/src/collective.faceted.task.egg-info/entry_points.txt
--rw-rw-r--   0 fngaha    (1000) fngaha    (1000)     2902 2023-04-06 15:08:03.000000 collective.faceted.task-0.5/src/collective.faceted.task.egg-info/SOURCES.txt
-drwxrwxr-x   0 fngaha    (1000) fngaha    (1000)        0 2023-04-06 15:08:03.000000 collective.faceted.task-0.5/src/collective/
-drwxrwxr-x   0 fngaha    (1000) fngaha    (1000)        0 2023-04-06 15:08:03.000000 collective.faceted.task-0.5/src/collective/faceted/
-drwxrwxr-x   0 fngaha    (1000) fngaha    (1000)        0 2023-04-06 15:08:03.000000 collective.faceted.task-0.5/src/collective/faceted/task/
-drwxrwxr-x   0 fngaha    (1000) fngaha    (1000)        0 2023-04-06 15:08:03.000000 collective.faceted.task-0.5/src/collective/faceted/task/tests/
--rw-rw-r--   0 fngaha    (1000) fngaha    (1000)      633 2023-04-06 15:08:03.000000 collective.faceted.task-0.5/src/collective/faceted/task/tests/test_robot.py
-drwxrwxr-x   0 fngaha    (1000) fngaha    (1000)        0 2023-04-06 15:08:03.000000 collective.faceted.task-0.5/src/collective/faceted/task/tests/robot/
--rw-rw-r--   0 fngaha    (1000) fngaha    (1000)        0 2023-04-06 15:08:03.000000 collective.faceted.task-0.5/src/collective/faceted/task/tests/robot/.gitkeep
--rw-rw-r--   0 fngaha    (1000) fngaha    (1000)        0 2023-04-06 15:08:03.000000 collective.faceted.task-0.5/src/collective/faceted/task/tests/__init__.py
--rw-rw-r--   0 fngaha    (1000) fngaha    (1000)     1257 2023-04-06 15:08:03.000000 collective.faceted.task-0.5/src/collective/faceted/task/tests/test_setup.py
--rw-rw-r--   0 fngaha    (1000) fngaha    (1000)      715 2023-04-06 15:08:03.000000 collective.faceted.task-0.5/src/collective/faceted/task/interfaces.py
-drwxrwxr-x   0 fngaha    (1000) fngaha    (1000)        0 2023-04-06 15:08:03.000000 collective.faceted.task-0.5/src/collective/faceted/task/locales/
--rwxrwxr-x   0 fngaha    (1000) fngaha    (1000)      530 2023-04-06 15:08:03.000000 collective.faceted.task-0.5/src/collective/faceted/task/locales/update.sh
--rw-rw-r--   0 fngaha    (1000) fngaha    (1000)     1365 2023-04-06 15:08:03.000000 collective.faceted.task-0.5/src/collective/faceted/task/locales/collective.faceted.task.pot
-drwxrwxr-x   0 fngaha    (1000) fngaha    (1000)        0 2023-04-06 15:08:03.000000 collective.faceted.task-0.5/src/collective/faceted/task/locales/fr/
-drwxrwxr-x   0 fngaha    (1000) fngaha    (1000)        0 2023-04-06 15:08:03.000000 collective.faceted.task-0.5/src/collective/faceted/task/locales/fr/LC_MESSAGES/
--rw-rw-r--   0 fngaha    (1000) fngaha    (1000)     1118 2023-04-06 15:08:03.000000 collective.faceted.task-0.5/src/collective/faceted/task/locales/fr/LC_MESSAGES/eea.po
--rw-rw-r--   0 fngaha    (1000) fngaha    (1000)     1256 2023-04-06 15:08:03.000000 collective.faceted.task-0.5/src/collective/faceted/task/locales/fr/LC_MESSAGES/collective.faceted.task.po
--rw-rw-r--   0 fngaha    (1000) fngaha    (1000)      971 2023-04-06 15:08:03.000000 collective.faceted.task-0.5/src/collective/faceted/task/locales/eea.pot
--rw-rw-r--   0 fngaha    (1000) fngaha    (1000)     1448 2023-04-06 15:08:03.000000 collective.faceted.task-0.5/src/collective/faceted/task/configure.zcml
--rw-rw-r--   0 fngaha    (1000) fngaha    (1000)     1319 2023-04-06 15:08:03.000000 collective.faceted.task-0.5/src/collective/faceted/task/setuphandlers.py
-drwxrwxr-x   0 fngaha    (1000) fngaha    (1000)        0 2023-04-06 15:08:03.000000 collective.faceted.task-0.5/src/collective/faceted/task/events/
--rw-rw-r--   0 fngaha    (1000) fngaha    (1000)      902 2023-04-06 15:08:03.000000 collective.faceted.task-0.5/src/collective/faceted/task/events/task_events.py
--rw-rw-r--   0 fngaha    (1000) fngaha    (1000)      436 2023-04-06 15:08:03.000000 collective.faceted.task-0.5/src/collective/faceted/task/events/configure.zcml
--rw-rw-r--   0 fngaha    (1000) fngaha    (1000)        0 2023-04-06 15:08:03.000000 collective.faceted.task-0.5/src/collective/faceted/task/events/__init__.py
--rw-rw-r--   0 fngaha    (1000) fngaha    (1000)     2528 2023-04-06 15:08:03.000000 collective.faceted.task-0.5/src/collective/faceted/task/testing.py
--rw-rw-r--   0 fngaha    (1000) fngaha    (1000)      604 2023-04-06 15:08:03.000000 collective.faceted.task-0.5/src/collective/faceted/task/adapters.py
--rw-rw-r--   0 fngaha    (1000) fngaha    (1000)     3263 2023-04-06 15:08:03.000000 collective.faceted.task-0.5/src/collective/faceted/task/faceted_task_config.xml
--rw-rw-r--   0 fngaha    (1000) fngaha    (1000)      623 2023-04-06 15:08:03.000000 collective.faceted.task-0.5/src/collective/faceted/task/faceted_task_config.py
-drwxrwxr-x   0 fngaha    (1000) fngaha    (1000)        0 2023-04-06 15:08:03.000000 collective.faceted.task-0.5/src/collective/faceted/task/browser/
--rw-rw-r--   0 fngaha    (1000) fngaha    (1000)     2231 2023-04-06 15:08:03.000000 collective.faceted.task-0.5/src/collective/faceted/task/browser/list_tasks.py
--rw-rw-r--   0 fngaha    (1000) fngaha    (1000)     3792 2023-04-06 15:08:03.000000 collective.faceted.task-0.5/src/collective/faceted/task/browser/configure.zcml
--rw-rw-r--   0 fngaha    (1000) fngaha    (1000)     1176 2023-04-06 15:08:03.000000 collective.faceted.task-0.5/src/collective/faceted/task/browser/table.py
--rw-rw-r--   0 fngaha    (1000) fngaha    (1000)      627 2023-04-06 15:08:03.000000 collective.faceted.task-0.5/src/collective/faceted/task/browser/task_table_view.py
--rw-rw-r--   0 fngaha    (1000) fngaha    (1000)     1277 2023-04-06 15:08:03.000000 collective.faceted.task-0.5/src/collective/faceted/task/browser/task_view.py
--rw-rw-r--   0 fngaha    (1000) fngaha    (1000)        0 2023-04-06 15:08:03.000000 collective.faceted.task-0.5/src/collective/faceted/task/browser/__init__.py
--rw-rw-r--   0 fngaha    (1000) fngaha    (1000)     1241 2023-04-06 15:08:03.000000 collective.faceted.task-0.5/src/collective/faceted/task/browser/config_view.py
-drwxrwxr-x   0 fngaha    (1000) fngaha    (1000)        0 2023-04-06 15:08:03.000000 collective.faceted.task-0.5/src/collective/faceted/task/browser/templates/
--rw-rw-r--   0 fngaha    (1000) fngaha    (1000)     1811 2023-04-06 15:08:03.000000 collective.faceted.task-0.5/src/collective/faceted/task/browser/templates/facetedtask_view.pt
--rw-rw-r--   0 fngaha    (1000) fngaha    (1000)      602 2023-04-06 15:08:03.000000 collective.faceted.task-0.5/src/collective/faceted/task/browser/templates/config_view.pt
--rw-rw-r--   0 fngaha    (1000) fngaha    (1000)      169 2023-04-06 15:08:03.000000 collective.faceted.task-0.5/src/collective/faceted/task/browser/faceted_view.py
-drwxrwxr-x   0 fngaha    (1000) fngaha    (1000)        0 2023-04-06 15:08:03.000000 collective.faceted.task-0.5/src/collective/faceted/task/browser/static/
--rw-rw-r--   0 fngaha    (1000) fngaha    (1000)        0 2023-04-06 15:08:03.000000 collective.faceted.task-0.5/src/collective/faceted/task/browser/static/.gitkeep
--rw-rw-r--   0 fngaha    (1000) fngaha    (1000)       40 2023-04-06 15:08:03.000000 collective.faceted.task-0.5/src/collective/faceted/task/browser/static/faceted_task.css
-drwxrwxr-x   0 fngaha    (1000) fngaha    (1000)        0 2023-04-06 15:08:03.000000 collective.faceted.task-0.5/src/collective/faceted/task/profiles/
-drwxrwxr-x   0 fngaha    (1000) fngaha    (1000)        0 2023-04-06 15:08:03.000000 collective.faceted.task-0.5/src/collective/faceted/task/profiles/default/
--rw-rw-r--   0 fngaha    (1000) fngaha    (1000)      169 2023-04-06 15:08:03.000000 collective.faceted.task-0.5/src/collective/faceted/task/profiles/default/browserlayer.xml
--rw-rw-r--   0 fngaha    (1000) fngaha    (1000)      860 2023-04-06 15:08:03.000000 collective.faceted.task-0.5/src/collective/faceted/task/profiles/default/actions.xml
--rw-rw-r--   0 fngaha    (1000) fngaha    (1000)      665 2023-04-06 15:08:03.000000 collective.faceted.task-0.5/src/collective/faceted/task/profiles/default/jsregistry.xml
--rw-rw-r--   0 fngaha    (1000) fngaha    (1000)      514 2023-04-06 15:08:03.000000 collective.faceted.task-0.5/src/collective/faceted/task/profiles/default/cssregistry.xml
--rw-rw-r--   0 fngaha    (1000) fngaha    (1000)        0 2023-04-06 15:08:03.000000 collective.faceted.task-0.5/src/collective/faceted/task/profiles/default/collectivefacetedtask_marker.txt
--rw-rw-r--   0 fngaha    (1000) fngaha    (1000)      373 2023-04-06 15:08:03.000000 collective.faceted.task-0.5/src/collective/faceted/task/profiles/default/metadata.xml
-drwxrwxr-x   0 fngaha    (1000) fngaha    (1000)        0 2023-04-06 15:08:03.000000 collective.faceted.task-0.5/src/collective/faceted/task/profiles/base/
--rw-rw-r--   0 fngaha    (1000) fngaha    (1000)      258 2023-04-06 15:08:03.000000 collective.faceted.task-0.5/src/collective/faceted/task/profiles/base/componentregistry.xml
--rw-rw-r--   0 fngaha    (1000) fngaha    (1000)      103 2023-04-06 15:08:03.000000 collective.faceted.task-0.5/src/collective/faceted/task/profiles/base/metadata.xml
-drwxrwxr-x   0 fngaha    (1000) fngaha    (1000)        0 2023-04-06 15:08:03.000000 collective.faceted.task-0.5/src/collective/faceted/task/profiles/testing/
--rw-rw-r--   0 fngaha    (1000) fngaha    (1000)      172 2023-04-06 15:08:03.000000 collective.faceted.task-0.5/src/collective/faceted/task/profiles/testing/metadata.xml
--rw-rw-r--   0 fngaha    (1000) fngaha    (1000)      227 2023-04-06 15:08:03.000000 collective.faceted.task-0.5/src/collective/faceted/task/__init__.py
--rw-rw-r--   0 fngaha    (1000) fngaha    (1000)      532 2023-04-06 15:08:03.000000 collective.faceted.task-0.5/src/collective/faceted/task/testing.zcml
--rw-rw-r--   0 fngaha    (1000) fngaha    (1000)      455 2023-04-06 15:08:03.000000 collective.faceted.task-0.5/src/collective/faceted/task/overrides.zcml
--rw-rw-r--   0 fngaha    (1000) fngaha    (1000)      244 2023-04-06 15:08:03.000000 collective.faceted.task-0.5/src/collective/faceted/__init__.py
--rw-rw-r--   0 fngaha    (1000) fngaha    (1000)      244 2023-04-06 15:08:03.000000 collective.faceted.task-0.5/src/collective/__init__.py
--rw-rw-r--   0 fngaha    (1000) fngaha    (1000)     1467 2023-04-06 15:08:03.000000 collective.faceted.task-0.5/PKG-INFO
--rw-rw-r--   0 fngaha    (1000) fngaha    (1000)       38 2023-04-06 15:08:03.000000 collective.faceted.task-0.5/setup.cfg
--rw-rw-r--   0 fngaha    (1000) fngaha    (1000)     1464 2023-04-06 15:08:03.000000 collective.faceted.task-0.5/setup.py
--rw-rw-r--   0 fngaha    (1000) fngaha    (1000)     5686 2023-04-06 15:08:03.000000 collective.faceted.task-0.5/bootstrap.py
--rw-rw-r--   0 fngaha    (1000) fngaha    (1000)     7458 2023-04-06 15:08:03.000000 collective.faceted.task-0.5/bootstrap-buildout.py
--rw-rw-r--   0 fngaha    (1000) fngaha    (1000)       40 2023-04-06 15:08:03.000000 collective.faceted.task-0.5/CONTRIBUTORS.rst
--rw-rw-r--   0 fngaha    (1000) fngaha    (1000)      188 2023-04-06 15:08:03.000000 collective.faceted.task-0.5/MANIFEST.in
--rw-rw-r--   0 fngaha    (1000) fngaha    (1000)      422 2023-04-06 15:08:03.000000 collective.faceted.task-0.5/CHANGES.rst
--rw-rw-r--   0 fngaha    (1000) fngaha    (1000)      174 2023-04-06 15:08:03.000000 collective.faceted.task-0.5/README.rst
--rw-rw-r--   0 fngaha    (1000) fngaha    (1000)       48 2023-04-06 15:08:03.000000 collective.faceted.task-0.5/buildout.cfg
--rw-rw-r--   0 fngaha    (1000) fngaha    (1000)       76 2023-04-06 15:08:03.000000 collective.faceted.task-0.5/.coveragerc
+drwxr-xr-x   0 mpeeters   (501) staff       (20)        0 2023-07-05 07:14:49.000000 collective.faceted.task-1.0.0/
+-rw-r--r--   0 mpeeters   (501) staff       (20)       76 2023-07-05 07:14:48.000000 collective.faceted.task-1.0.0/.coveragerc
+-rw-r--r--   0 mpeeters   (501) staff       (20)      461 2023-07-05 07:14:48.000000 collective.faceted.task-1.0.0/CHANGES.rst
+-rw-r--r--   0 mpeeters   (501) staff       (20)       75 2023-07-05 07:14:48.000000 collective.faceted.task-1.0.0/CONTRIBUTORS.rst
+-rw-r--r--   0 mpeeters   (501) staff       (20)      186 2023-07-05 07:14:48.000000 collective.faceted.task-1.0.0/MANIFEST.in
+-rw-r--r--   0 mpeeters   (501) staff       (20)     1688 2023-07-05 07:14:49.000000 collective.faceted.task-1.0.0/PKG-INFO
+-rw-r--r--   0 mpeeters   (501) staff       (20)       72 2023-07-05 07:14:48.000000 collective.faceted.task-1.0.0/README.rst
+-rw-r--r--   0 mpeeters   (501) staff       (20)     7458 2023-07-05 07:14:48.000000 collective.faceted.task-1.0.0/bootstrap-buildout.py
+-rw-r--r--   0 mpeeters   (501) staff       (20)     5686 2023-07-05 07:14:48.000000 collective.faceted.task-1.0.0/bootstrap.py
+-rw-r--r--   0 mpeeters   (501) staff       (20)       48 2023-07-05 07:14:48.000000 collective.faceted.task-1.0.0/buildout.cfg
+drwxr-xr-x   0 mpeeters   (501) staff       (20)        0 2023-07-05 07:14:49.000000 collective.faceted.task-1.0.0/docs/
+-rw-r--r--   0 mpeeters   (501) staff       (20)    18092 2023-07-05 07:14:48.000000 collective.faceted.task-1.0.0/docs/LICENSE.GPL
+-rw-r--r--   0 mpeeters   (501) staff       (20)        0 2023-07-05 07:14:48.000000 collective.faceted.task-1.0.0/docs/LICENSE.rst
+-rw-r--r--   0 mpeeters   (501) staff       (20)       38 2023-07-05 07:14:49.000000 collective.faceted.task-1.0.0/setup.cfg
+-rw-r--r--   0 mpeeters   (501) staff       (20)     1695 2023-07-05 07:14:48.000000 collective.faceted.task-1.0.0/setup.py
+drwxr-xr-x   0 mpeeters   (501) staff       (20)        0 2023-07-05 07:14:49.000000 collective.faceted.task-1.0.0/src/
+drwxr-xr-x   0 mpeeters   (501) staff       (20)        0 2023-07-05 07:14:49.000000 collective.faceted.task-1.0.0/src/collective/
+-rw-r--r--   0 mpeeters   (501) staff       (20)      244 2023-07-05 07:14:48.000000 collective.faceted.task-1.0.0/src/collective/__init__.py
+drwxr-xr-x   0 mpeeters   (501) staff       (20)        0 2023-07-05 07:14:49.000000 collective.faceted.task-1.0.0/src/collective/faceted/
+-rw-r--r--   0 mpeeters   (501) staff       (20)      244 2023-07-05 07:14:48.000000 collective.faceted.task-1.0.0/src/collective/faceted/__init__.py
+drwxr-xr-x   0 mpeeters   (501) staff       (20)        0 2023-07-05 07:14:49.000000 collective.faceted.task-1.0.0/src/collective/faceted/task/
+-rw-r--r--   0 mpeeters   (501) staff       (20)      227 2023-07-05 07:14:48.000000 collective.faceted.task-1.0.0/src/collective/faceted/task/__init__.py
+-rw-r--r--   0 mpeeters   (501) staff       (20)      604 2023-07-05 07:14:48.000000 collective.faceted.task-1.0.0/src/collective/faceted/task/adapters.py
+drwxr-xr-x   0 mpeeters   (501) staff       (20)        0 2023-07-05 07:14:49.000000 collective.faceted.task-1.0.0/src/collective/faceted/task/browser/
+-rw-r--r--   0 mpeeters   (501) staff       (20)        0 2023-07-05 07:14:48.000000 collective.faceted.task-1.0.0/src/collective/faceted/task/browser/__init__.py
+-rw-r--r--   0 mpeeters   (501) staff       (20)     1241 2023-07-05 07:14:48.000000 collective.faceted.task-1.0.0/src/collective/faceted/task/browser/config_view.py
+-rw-r--r--   0 mpeeters   (501) staff       (20)     3792 2023-07-05 07:14:48.000000 collective.faceted.task-1.0.0/src/collective/faceted/task/browser/configure.zcml
+-rw-r--r--   0 mpeeters   (501) staff       (20)      169 2023-07-05 07:14:48.000000 collective.faceted.task-1.0.0/src/collective/faceted/task/browser/faceted_view.py
+-rw-r--r--   0 mpeeters   (501) staff       (20)     2231 2023-07-05 07:14:48.000000 collective.faceted.task-1.0.0/src/collective/faceted/task/browser/list_tasks.py
+drwxr-xr-x   0 mpeeters   (501) staff       (20)        0 2023-07-05 07:14:49.000000 collective.faceted.task-1.0.0/src/collective/faceted/task/browser/static/
+-rw-r--r--   0 mpeeters   (501) staff       (20)        0 2023-07-05 07:14:48.000000 collective.faceted.task-1.0.0/src/collective/faceted/task/browser/static/.gitkeep
+-rw-r--r--   0 mpeeters   (501) staff       (20)       40 2023-07-05 07:14:48.000000 collective.faceted.task-1.0.0/src/collective/faceted/task/browser/static/faceted_task.css
+-rw-r--r--   0 mpeeters   (501) staff       (20)     1196 2023-07-05 07:14:48.000000 collective.faceted.task-1.0.0/src/collective/faceted/task/browser/table.py
+-rw-r--r--   0 mpeeters   (501) staff       (20)      627 2023-07-05 07:14:48.000000 collective.faceted.task-1.0.0/src/collective/faceted/task/browser/task_table_view.py
+-rw-r--r--   0 mpeeters   (501) staff       (20)     1277 2023-07-05 07:14:48.000000 collective.faceted.task-1.0.0/src/collective/faceted/task/browser/task_view.py
+drwxr-xr-x   0 mpeeters   (501) staff       (20)        0 2023-07-05 07:14:49.000000 collective.faceted.task-1.0.0/src/collective/faceted/task/browser/templates/
+-rw-r--r--   0 mpeeters   (501) staff       (20)      602 2023-07-05 07:14:48.000000 collective.faceted.task-1.0.0/src/collective/faceted/task/browser/templates/config_view.pt
+-rw-r--r--   0 mpeeters   (501) staff       (20)     1811 2023-07-05 07:14:48.000000 collective.faceted.task-1.0.0/src/collective/faceted/task/browser/templates/facetedtask_view.pt
+-rw-r--r--   0 mpeeters   (501) staff       (20)     1448 2023-07-05 07:14:48.000000 collective.faceted.task-1.0.0/src/collective/faceted/task/configure.zcml
+drwxr-xr-x   0 mpeeters   (501) staff       (20)        0 2023-07-05 07:14:49.000000 collective.faceted.task-1.0.0/src/collective/faceted/task/events/
+-rw-r--r--   0 mpeeters   (501) staff       (20)        0 2023-07-05 07:14:48.000000 collective.faceted.task-1.0.0/src/collective/faceted/task/events/__init__.py
+-rw-r--r--   0 mpeeters   (501) staff       (20)      436 2023-07-05 07:14:48.000000 collective.faceted.task-1.0.0/src/collective/faceted/task/events/configure.zcml
+-rw-r--r--   0 mpeeters   (501) staff       (20)      902 2023-07-05 07:14:48.000000 collective.faceted.task-1.0.0/src/collective/faceted/task/events/task_events.py
+-rw-r--r--   0 mpeeters   (501) staff       (20)      623 2023-07-05 07:14:48.000000 collective.faceted.task-1.0.0/src/collective/faceted/task/faceted_task_config.py
+-rw-r--r--   0 mpeeters   (501) staff       (20)     3263 2023-07-05 07:14:48.000000 collective.faceted.task-1.0.0/src/collective/faceted/task/faceted_task_config.xml
+-rw-r--r--   0 mpeeters   (501) staff       (20)      715 2023-07-05 07:14:48.000000 collective.faceted.task-1.0.0/src/collective/faceted/task/interfaces.py
+drwxr-xr-x   0 mpeeters   (501) staff       (20)        0 2023-07-05 07:14:49.000000 collective.faceted.task-1.0.0/src/collective/faceted/task/locales/
+-rw-r--r--   0 mpeeters   (501) staff       (20)     1365 2023-07-05 07:14:48.000000 collective.faceted.task-1.0.0/src/collective/faceted/task/locales/collective.faceted.task.pot
+-rw-r--r--   0 mpeeters   (501) staff       (20)      971 2023-07-05 07:14:48.000000 collective.faceted.task-1.0.0/src/collective/faceted/task/locales/eea.pot
+drwxr-xr-x   0 mpeeters   (501) staff       (20)        0 2023-07-05 07:14:49.000000 collective.faceted.task-1.0.0/src/collective/faceted/task/locales/fr/
+drwxr-xr-x   0 mpeeters   (501) staff       (20)        0 2023-07-05 07:14:49.000000 collective.faceted.task-1.0.0/src/collective/faceted/task/locales/fr/LC_MESSAGES/
+-rw-r--r--   0 mpeeters   (501) staff       (20)      553 2023-07-05 07:14:48.000000 collective.faceted.task-1.0.0/src/collective/faceted/task/locales/fr/LC_MESSAGES/collective.faceted.task.mo
+-rw-r--r--   0 mpeeters   (501) staff       (20)     1256 2023-07-05 07:14:48.000000 collective.faceted.task-1.0.0/src/collective/faceted/task/locales/fr/LC_MESSAGES/collective.faceted.task.po
+-rw-r--r--   0 mpeeters   (501) staff       (20)      638 2023-07-05 07:14:48.000000 collective.faceted.task-1.0.0/src/collective/faceted/task/locales/fr/LC_MESSAGES/eea.mo
+-rw-r--r--   0 mpeeters   (501) staff       (20)     1118 2023-07-05 07:14:48.000000 collective.faceted.task-1.0.0/src/collective/faceted/task/locales/fr/LC_MESSAGES/eea.po
+-rwxr-xr-x   0 mpeeters   (501) staff       (20)      530 2023-07-05 07:14:48.000000 collective.faceted.task-1.0.0/src/collective/faceted/task/locales/update.sh
+-rw-r--r--   0 mpeeters   (501) staff       (20)      455 2023-07-05 07:14:48.000000 collective.faceted.task-1.0.0/src/collective/faceted/task/overrides.zcml
+drwxr-xr-x   0 mpeeters   (501) staff       (20)        0 2023-07-05 07:14:49.000000 collective.faceted.task-1.0.0/src/collective/faceted/task/profiles/
+drwxr-xr-x   0 mpeeters   (501) staff       (20)        0 2023-07-05 07:14:49.000000 collective.faceted.task-1.0.0/src/collective/faceted/task/profiles/base/
+-rw-r--r--   0 mpeeters   (501) staff       (20)      258 2023-07-05 07:14:48.000000 collective.faceted.task-1.0.0/src/collective/faceted/task/profiles/base/componentregistry.xml
+-rw-r--r--   0 mpeeters   (501) staff       (20)      103 2023-07-05 07:14:48.000000 collective.faceted.task-1.0.0/src/collective/faceted/task/profiles/base/metadata.xml
+drwxr-xr-x   0 mpeeters   (501) staff       (20)        0 2023-07-05 07:14:49.000000 collective.faceted.task-1.0.0/src/collective/faceted/task/profiles/default/
+-rw-r--r--   0 mpeeters   (501) staff       (20)      860 2023-07-05 07:14:48.000000 collective.faceted.task-1.0.0/src/collective/faceted/task/profiles/default/actions.xml
+-rw-r--r--   0 mpeeters   (501) staff       (20)      169 2023-07-05 07:14:48.000000 collective.faceted.task-1.0.0/src/collective/faceted/task/profiles/default/browserlayer.xml
+-rw-r--r--   0 mpeeters   (501) staff       (20)        0 2023-07-05 07:14:48.000000 collective.faceted.task-1.0.0/src/collective/faceted/task/profiles/default/collectivefacetedtask_marker.txt
+-rw-r--r--   0 mpeeters   (501) staff       (20)      514 2023-07-05 07:14:48.000000 collective.faceted.task-1.0.0/src/collective/faceted/task/profiles/default/cssregistry.xml
+-rw-r--r--   0 mpeeters   (501) staff       (20)      665 2023-07-05 07:14:48.000000 collective.faceted.task-1.0.0/src/collective/faceted/task/profiles/default/jsregistry.xml
+-rw-r--r--   0 mpeeters   (501) staff       (20)      373 2023-07-05 07:14:48.000000 collective.faceted.task-1.0.0/src/collective/faceted/task/profiles/default/metadata.xml
+drwxr-xr-x   0 mpeeters   (501) staff       (20)        0 2023-07-05 07:14:49.000000 collective.faceted.task-1.0.0/src/collective/faceted/task/profiles/testing/
+-rw-r--r--   0 mpeeters   (501) staff       (20)      172 2023-07-05 07:14:48.000000 collective.faceted.task-1.0.0/src/collective/faceted/task/profiles/testing/metadata.xml
+-rw-r--r--   0 mpeeters   (501) staff       (20)     1319 2023-07-05 07:14:48.000000 collective.faceted.task-1.0.0/src/collective/faceted/task/setuphandlers.py
+-rw-r--r--   0 mpeeters   (501) staff       (20)     2528 2023-07-05 07:14:48.000000 collective.faceted.task-1.0.0/src/collective/faceted/task/testing.py
+-rw-r--r--   0 mpeeters   (501) staff       (20)      532 2023-07-05 07:14:48.000000 collective.faceted.task-1.0.0/src/collective/faceted/task/testing.zcml
+drwxr-xr-x   0 mpeeters   (501) staff       (20)        0 2023-07-05 07:14:49.000000 collective.faceted.task-1.0.0/src/collective/faceted/task/tests/
+-rw-r--r--   0 mpeeters   (501) staff       (20)        0 2023-07-05 07:14:48.000000 collective.faceted.task-1.0.0/src/collective/faceted/task/tests/__init__.py
+drwxr-xr-x   0 mpeeters   (501) staff       (20)        0 2023-07-05 07:14:49.000000 collective.faceted.task-1.0.0/src/collective/faceted/task/tests/robot/
+-rw-r--r--   0 mpeeters   (501) staff       (20)        0 2023-07-05 07:14:48.000000 collective.faceted.task-1.0.0/src/collective/faceted/task/tests/robot/.gitkeep
+-rw-r--r--   0 mpeeters   (501) staff       (20)      633 2023-07-05 07:14:48.000000 collective.faceted.task-1.0.0/src/collective/faceted/task/tests/test_robot.py
+-rw-r--r--   0 mpeeters   (501) staff       (20)     1257 2023-07-05 07:14:48.000000 collective.faceted.task-1.0.0/src/collective/faceted/task/tests/test_setup.py
+drwxr-xr-x   0 mpeeters   (501) staff       (20)        0 2023-07-05 07:14:49.000000 collective.faceted.task-1.0.0/src/collective.faceted.task.egg-info/
+-rw-r--r--   0 mpeeters   (501) staff       (20)     1688 2023-07-05 07:14:49.000000 collective.faceted.task-1.0.0/src/collective.faceted.task.egg-info/PKG-INFO
+-rw-r--r--   0 mpeeters   (501) staff       (20)     3038 2023-07-05 07:14:49.000000 collective.faceted.task-1.0.0/src/collective.faceted.task.egg-info/SOURCES.txt
+-rw-r--r--   0 mpeeters   (501) staff       (20)        1 2023-07-05 07:14:49.000000 collective.faceted.task-1.0.0/src/collective.faceted.task.egg-info/dependency_links.txt
+-rw-r--r--   0 mpeeters   (501) staff       (20)       53 2023-07-05 07:14:49.000000 collective.faceted.task-1.0.0/src/collective.faceted.task.egg-info/entry_points.txt
+-rw-r--r--   0 mpeeters   (501) staff       (20)       30 2023-07-05 07:14:49.000000 collective.faceted.task-1.0.0/src/collective.faceted.task.egg-info/namespace_packages.txt
+-rw-r--r--   0 mpeeters   (501) staff       (20)        1 2023-07-05 07:14:49.000000 collective.faceted.task-1.0.0/src/collective.faceted.task.egg-info/not-zip-safe
+-rw-r--r--   0 mpeeters   (501) staff       (20)      126 2023-07-05 07:14:49.000000 collective.faceted.task-1.0.0/src/collective.faceted.task.egg-info/requires.txt
+-rw-r--r--   0 mpeeters   (501) staff       (20)       11 2023-07-05 07:14:49.000000 collective.faceted.task-1.0.0/src/collective.faceted.task.egg-info/top_level.txt
+-rw-r--r--   0 mpeeters   (501) staff       (20)      172 2023-07-05 07:14:48.000000 collective.faceted.task-1.0.0/travis.cfg
```

### Comparing `collective.faceted.task-0.5/docs/LICENSE.GPL` & `collective.faceted.task-1.0.0/docs/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `collective.faceted.task-0.5/src/collective.faceted.task.egg-info/PKG-INFO` & `collective.faceted.task-1.0.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,57 +1,68 @@
 Metadata-Version: 2.1
 Name: collective.faceted.task
-Version: 0.5
-Summary: UNKNOWN
+Version: 1.0.0
+Summary: Faceted tools and view for tasks
 Home-page: http://pypi.python.org/pypi/collective.faceted.task
 Author: Franck NGAHA
 Author-email: franck.o.ngaha@gmail.com
 License: GPL V2
-Description: ==========================================================================
+Description: =======================
         collective.faceted.task
-        ==========================================================================
+        =======================
         
+        Contributors
+        ============
         
-        - Franck NGAHA, franck.o.ngaha@gmail.com
+        - Franck NGAHA (iMio)
+        - Simon Delcourt (iMio)
+        - Martin Peeters (Affinitic)
         
         Changelog
         =========
         
         
-        0.5 (2023-04-06)
-        ----------------
+        1.0.0 (2023-07-05)
+        ------------------
+        
+        - Do not escape z3c.table column title
+          [sdelcourt, mpeeters]
         
-        - add translations
-          [MagDhyIm]
         
         0.4 (2018-06-05)
         ----------------
         
         - Add base profile to fix installation dependencies.
           [mpeeters]
         
+        
         0.3 (2017-01-10)
         ----------------
         
         - remove task link from header_path column.
           [sdelcourt]
         
+        
         0.2 (2016-06-22)
         ----------------
         
         - Nothing changed yet.
         
+        
         0.1 (2016-06-22)
         ----------------
         
         - Initial release.
           [sdelcourt, fngaha]
         
         
+        
 Keywords: Python Zope Plone
 Platform: UNKNOWN
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Plone
 Classifier: Framework :: Plone :: 4.3
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2.7
+Classifier: Operating System :: OS Independent
+Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Provides-Extra: test
```

### Comparing `collective.faceted.task-0.5/src/collective.faceted.task.egg-info/SOURCES.txt` & `collective.faceted.task-1.0.0/src/collective.faceted.task.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -44,15 +44,17 @@
 src/collective/faceted/task/browser/templates/facetedtask_view.pt
 src/collective/faceted/task/events/__init__.py
 src/collective/faceted/task/events/configure.zcml
 src/collective/faceted/task/events/task_events.py
 src/collective/faceted/task/locales/collective.faceted.task.pot
 src/collective/faceted/task/locales/eea.pot
 src/collective/faceted/task/locales/update.sh
+src/collective/faceted/task/locales/fr/LC_MESSAGES/collective.faceted.task.mo
 src/collective/faceted/task/locales/fr/LC_MESSAGES/collective.faceted.task.po
+src/collective/faceted/task/locales/fr/LC_MESSAGES/eea.mo
 src/collective/faceted/task/locales/fr/LC_MESSAGES/eea.po
 src/collective/faceted/task/profiles/base/componentregistry.xml
 src/collective/faceted/task/profiles/base/metadata.xml
 src/collective/faceted/task/profiles/default/actions.xml
 src/collective/faceted/task/profiles/default/browserlayer.xml
 src/collective/faceted/task/profiles/default/collectivefacetedtask_marker.txt
 src/collective/faceted/task/profiles/default/cssregistry.xml
```

### Comparing `collective.faceted.task-0.5/src/collective/faceted/task/tests/test_robot.py` & `collective.faceted.task-1.0.0/src/collective/faceted/task/tests/test_robot.py`

 * *Files identical despite different names*

### Comparing `collective.faceted.task-0.5/src/collective/faceted/task/tests/test_setup.py` & `collective.faceted.task-1.0.0/src/collective/faceted/task/tests/test_setup.py`

 * *Files identical despite different names*

### Comparing `collective.faceted.task-0.5/src/collective/faceted/task/interfaces.py` & `collective.faceted.task-1.0.0/src/collective/faceted/task/interfaces.py`

 * *Files identical despite different names*

### Comparing `collective.faceted.task-0.5/src/collective/faceted/task/locales/update.sh` & `collective.faceted.task-1.0.0/src/collective/faceted/task/locales/update.sh`

 * *Files identical despite different names*

### Comparing `collective.faceted.task-0.5/src/collective/faceted/task/locales/collective.faceted.task.pot` & `collective.faceted.task-1.0.0/src/collective/faceted/task/locales/collective.faceted.task.pot`

 * *Files identical despite different names*

### Comparing `collective.faceted.task-0.5/src/collective/faceted/task/locales/fr/LC_MESSAGES/eea.po` & `collective.faceted.task-1.0.0/src/collective/faceted/task/locales/fr/LC_MESSAGES/eea.po`

 * *Files identical despite different names*

### Comparing `collective.faceted.task-0.5/src/collective/faceted/task/locales/fr/LC_MESSAGES/collective.faceted.task.po` & `collective.faceted.task-1.0.0/src/collective/faceted/task/locales/fr/LC_MESSAGES/collective.faceted.task.po`

 * *Files identical despite different names*

### Comparing `collective.faceted.task-0.5/src/collective/faceted/task/locales/eea.pot` & `collective.faceted.task-1.0.0/src/collective/faceted/task/locales/eea.pot`

 * *Files identical despite different names*

### Comparing `collective.faceted.task-0.5/src/collective/faceted/task/configure.zcml` & `collective.faceted.task-1.0.0/src/collective/faceted/task/configure.zcml`

 * *Files identical despite different names*

### Comparing `collective.faceted.task-0.5/src/collective/faceted/task/setuphandlers.py` & `collective.faceted.task-1.0.0/src/collective/faceted/task/setuphandlers.py`

 * *Files identical despite different names*

### Comparing `collective.faceted.task-0.5/src/collective/faceted/task/events/task_events.py` & `collective.faceted.task-1.0.0/src/collective/faceted/task/events/task_events.py`

 * *Files identical despite different names*

### Comparing `collective.faceted.task-0.5/src/collective/faceted/task/testing.py` & `collective.faceted.task-1.0.0/src/collective/faceted/task/testing.py`

 * *Files identical despite different names*

### Comparing `collective.faceted.task-0.5/src/collective/faceted/task/adapters.py` & `collective.faceted.task-1.0.0/src/collective/faceted/task/adapters.py`

 * *Files identical despite different names*

### Comparing `collective.faceted.task-0.5/src/collective/faceted/task/faceted_task_config.xml` & `collective.faceted.task-1.0.0/src/collective/faceted/task/faceted_task_config.xml`

 * *Files identical despite different names*

### Comparing `collective.faceted.task-0.5/src/collective/faceted/task/faceted_task_config.py` & `collective.faceted.task-1.0.0/src/collective/faceted/task/faceted_task_config.py`

 * *Files identical despite different names*

### Comparing `collective.faceted.task-0.5/src/collective/faceted/task/browser/list_tasks.py` & `collective.faceted.task-1.0.0/src/collective/faceted/task/browser/list_tasks.py`

 * *Files identical despite different names*

### Comparing `collective.faceted.task-0.5/src/collective/faceted/task/browser/configure.zcml` & `collective.faceted.task-1.0.0/src/collective/faceted/task/browser/configure.zcml`

 * *Files identical despite different names*

### Comparing `collective.faceted.task-0.5/src/collective/faceted/task/browser/table.py` & `collective.faceted.task-1.0.0/src/collective/faceted/task/browser/table.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,14 +25,16 @@
 
 
 class TitleColumn(BaseColumn):
     """
     Column that displays title.
     """
 
+    escape = False
+
     def renderCell(self, item):
         adaptedTask = TaskAdapter(item.getObject())
         title = adaptedTask.get_full_tree_title().decode('utf-8')
 
         path = title.split('/')
         head = path[-1]
         tail = u'/'.join(path[0:-1])
```

### Comparing `collective.faceted.task-0.5/src/collective/faceted/task/browser/task_table_view.py` & `collective.faceted.task-1.0.0/src/collective/faceted/task/browser/task_table_view.py`

 * *Files identical despite different names*

### Comparing `collective.faceted.task-0.5/src/collective/faceted/task/browser/task_view.py` & `collective.faceted.task-1.0.0/src/collective/faceted/task/browser/task_view.py`

 * *Files identical despite different names*

### Comparing `collective.faceted.task-0.5/src/collective/faceted/task/browser/config_view.py` & `collective.faceted.task-1.0.0/src/collective/faceted/task/browser/config_view.py`

 * *Files identical despite different names*

### Comparing `collective.faceted.task-0.5/src/collective/faceted/task/browser/templates/facetedtask_view.pt` & `collective.faceted.task-1.0.0/src/collective/faceted/task/browser/templates/facetedtask_view.pt`

 * *Files identical despite different names*

### Comparing `collective.faceted.task-0.5/src/collective/faceted/task/browser/templates/config_view.pt` & `collective.faceted.task-1.0.0/src/collective/faceted/task/browser/templates/config_view.pt`

 * *Files identical despite different names*

### Comparing `collective.faceted.task-0.5/src/collective/faceted/task/profiles/default/actions.xml` & `collective.faceted.task-1.0.0/src/collective/faceted/task/profiles/default/actions.xml`

 * *Files identical despite different names*

### Comparing `collective.faceted.task-0.5/src/collective/faceted/task/profiles/default/jsregistry.xml` & `collective.faceted.task-1.0.0/src/collective/faceted/task/profiles/default/jsregistry.xml`

 * *Files identical despite different names*

### Comparing `collective.faceted.task-0.5/src/collective/faceted/task/profiles/default/cssregistry.xml` & `collective.faceted.task-1.0.0/src/collective/faceted/task/profiles/default/cssregistry.xml`

 * *Files identical despite different names*

### Comparing `collective.faceted.task-0.5/src/collective/faceted/task/testing.zcml` & `collective.faceted.task-1.0.0/src/collective/faceted/task/testing.zcml`

 * *Files identical despite different names*

### Comparing `collective.faceted.task-0.5/PKG-INFO` & `collective.faceted.task-1.0.0/src/collective.faceted.task.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,57 +1,68 @@
 Metadata-Version: 2.1
 Name: collective.faceted.task
-Version: 0.5
-Summary: UNKNOWN
+Version: 1.0.0
+Summary: Faceted tools and view for tasks
 Home-page: http://pypi.python.org/pypi/collective.faceted.task
 Author: Franck NGAHA
 Author-email: franck.o.ngaha@gmail.com
 License: GPL V2
-Description: ==========================================================================
+Description: =======================
         collective.faceted.task
-        ==========================================================================
+        =======================
         
+        Contributors
+        ============
         
-        - Franck NGAHA, franck.o.ngaha@gmail.com
+        - Franck NGAHA (iMio)
+        - Simon Delcourt (iMio)
+        - Martin Peeters (Affinitic)
         
         Changelog
         =========
         
         
-        0.5 (2023-04-06)
-        ----------------
+        1.0.0 (2023-07-05)
+        ------------------
+        
+        - Do not escape z3c.table column title
+          [sdelcourt, mpeeters]
         
-        - add translations
-          [MagDhyIm]
         
         0.4 (2018-06-05)
         ----------------
         
         - Add base profile to fix installation dependencies.
           [mpeeters]
         
+        
         0.3 (2017-01-10)
         ----------------
         
         - remove task link from header_path column.
           [sdelcourt]
         
+        
         0.2 (2016-06-22)
         ----------------
         
         - Nothing changed yet.
         
+        
         0.1 (2016-06-22)
         ----------------
         
         - Initial release.
           [sdelcourt, fngaha]
         
         
+        
 Keywords: Python Zope Plone
 Platform: UNKNOWN
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Plone
 Classifier: Framework :: Plone :: 4.3
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2.7
+Classifier: Operating System :: OS Independent
+Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Provides-Extra: test
```

### Comparing `collective.faceted.task-0.5/setup.py` & `collective.faceted.task-1.0.0/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,33 +1,40 @@
 # -*- coding: utf-8 -*-
 """Installer for the collective.faceted.task package."""
 
 from setuptools import find_packages
 from setuptools import setup
 
 
-long_description = '\n\n'.join([
-    open('README.rst').read(),
-    open('CONTRIBUTORS.rst').read(),
-    open('CHANGES.rst').read(),
-])
+long_description = (
+    open('README.rst').read()
+    + '\n' +
+    'Contributors\n'
+    '============\n'
+    + '\n' +
+    open('CONTRIBUTORS.rst').read()
+    + '\n' +
+    open('CHANGES.rst').read()
+    + '\n')
 
 
 setup(
     name='collective.faceted.task',
-    version='0.5',
-    description="",
+    version='1.0.0',
+    description="Faceted tools and view for tasks",
     long_description=long_description,
     # Get more from http://pypi.python.org/pypi?%3Aaction=list_classifiers
     classifiers=[
         "Environment :: Web Environment",
         "Framework :: Plone",
         "Framework :: Plone :: 4.3",
         "Programming Language :: Python",
         "Programming Language :: Python :: 2.7",
+        "Operating System :: OS Independent",
+        "License :: OSI Approved :: GNU General Public License v2 (GPLv2)",
     ],
     keywords='Python Zope Plone',
     author='Franck NGAHA',
     author_email='franck.o.ngaha@gmail.com',
     url='http://pypi.python.org/pypi/collective.faceted.task',
     license='GPL V2',
     packages=find_packages('src', exclude=['ez_setup']),
```

### Comparing `collective.faceted.task-0.5/bootstrap.py` & `collective.faceted.task-1.0.0/bootstrap.py`

 * *Files identical despite different names*

### Comparing `collective.faceted.task-0.5/bootstrap-buildout.py` & `collective.faceted.task-1.0.0/bootstrap-buildout.py`

 * *Files identical despite different names*

