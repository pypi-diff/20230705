# Comparing `tmp/invenio-drafts-resources-1.4.1.tar.gz` & `tmp/invenio-drafts-resources-1.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/invenio-drafts-resources-1.4.1.tar", last modified: Wed Jun  7 14:03:26 2023, max compression
+gzip compressed data, was "dist/invenio-drafts-resources-1.4.2.tar", last modified: Wed Jul  5 11:54:31 2023, max compression
```

## Comparing `invenio-drafts-resources-1.4.1.tar` & `invenio-drafts-resources-1.4.2.tar`

### file list

```diff
@@ -1,270 +1,326 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:03:25.000000 invenio-drafts-resources-1.4.1/
--rw-r--r--   0 runner    (1001) docker     (123)      667 2023-06-07 14:03:19.000000 invenio-drafts-resources-1.4.1/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-07 14:03:19.000000 invenio-drafts-resources-1.4.1/.git-blame-ignore-revs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:03:25.000000 invenio-drafts-resources-1.4.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:03:25.000000 invenio-drafts-resources-1.4.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-06-07 14:03:19.000000 invenio-drafts-resources-1.4.1/.github/workflows/i18n-pull.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2014 2023-06-07 14:03:19.000000 invenio-drafts-resources-1.4.1/.github/workflows/i18n-push.yml
--rw-r--r--   0 runner    (1001) docker     (123)      868 2023-06-07 14:03:19.000000 invenio-drafts-resources-1.4.1/.github/workflows/pypi-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3134 2023-06-07 14:03:19.000000 invenio-drafts-resources-1.4.1/.github/workflows/tests.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:03:25.000000 invenio-drafts-resources-1.4.1/.tx/
--rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-06-07 14:03:19.000000 invenio-drafts-resources-1.4.1/.tx/config
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-06-07 14:03:19.000000 invenio-drafts-resources-1.4.1/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-06-07 14:03:19.000000 invenio-drafts-resources-1.4.1/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3583 2023-06-07 14:03:19.000000 invenio-drafts-resources-1.4.1/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-06-07 14:03:19.000000 invenio-drafts-resources-1.4.1/INSTALL.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-06-07 14:03:19.000000 invenio-drafts-resources-1.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      886 2023-06-07 14:03:19.000000 invenio-drafts-resources-1.4.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4066 2023-06-07 14:03:25.000000 invenio-drafts-resources-1.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-06-07 14:03:19.000000 invenio-drafts-resources-1.4.1/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-06-07 14:03:19.000000 invenio-drafts-resources-1.4.1/babel.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:03:25.000000 invenio-drafts-resources-1.4.1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     7481 2023-06-07 14:03:19.000000 invenio-drafts-resources-1.4.1/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-06-07 14:03:19.000000 invenio-drafts-resources-1.4.1/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-06-07 14:03:19.000000 invenio-drafts-resources-1.4.1/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-06-07 14:03:19.000000 invenio-drafts-resources-1.4.1/docs/changes.rst
--rw-r--r--   0 runner    (1001) docker     (123)    10309 2023-06-07 14:03:19.000000 invenio-drafts-resources-1.4.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-06-07 14:03:19.000000 invenio-drafts-resources-1.4.1/docs/configuration.rst
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-06-07 14:03:19.000000 invenio-drafts-resources-1.4.1/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      819 2023-06-07 14:03:19.000000 invenio-drafts-resources-1.4.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-06-07 14:03:19.000000 invenio-drafts-resources-1.4.1/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-06-07 14:03:19.000000 invenio-drafts-resources-1.4.1/docs/license.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7017 2023-06-07 14:03:19.000000 invenio-drafts-resources-1.4.1/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-07 14:03:19.000000 invenio-drafts-resources-1.4.1/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-06-07 14:03:19.000000 invenio-drafts-resources-1.4.1/docs/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:03:25.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-06-07 14:03:19.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:03:25.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/records/
--rw-r--r--   0 runner    (1001) docker     (123)      687 2023-06-07 14:03:19.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/records/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9005 2023-06-07 14:03:19.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/records/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     4316 2023-06-07 14:03:19.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/records/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:03:25.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/records/systemfields/
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-06-07 14:03:19.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/records/systemfields/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4409 2023-06-07 14:03:19.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/records/systemfields/parent.py
--rw-r--r--   0 runner    (1001) docker     (123)     7618 2023-06-07 14:03:19.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/records/systemfields/versions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:03:25.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/resources/
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-06-07 14:03:19.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/resources/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:03:25.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/resources/records/
--rw-r--r--   0 runner    (1001) docker     (123)      442 2023-06-07 14:03:19.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/resources/records/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      605 2023-06-07 14:03:19.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/resources/records/args.py
--rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-06-07 14:03:19.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/resources/records/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-06-07 14:03:19.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/resources/records/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     7603 2023-06-07 14:03:19.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/resources/records/resource.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:03:25.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/services/
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-06-07 14:03:19.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/services/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:03:25.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/services/records/
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-06-07 14:03:19.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/services/records/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:03:25.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/services/records/components/
--rw-r--r--   0 runner    (1001) docker     (123)      645 2023-06-07 14:03:19.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/services/records/components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1362 2023-06-07 14:03:19.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/services/records/components/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     7832 2023-06-07 14:03:19.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/services/records/components/files.py
--rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-06-07 14:03:19.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/services/records/components/metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     1209 2023-06-07 14:03:19.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/services/records/components/pid.py
--rw-r--r--   0 runner    (1001) docker     (123)      591 2023-06-07 14:03:19.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/services/records/components/relations.py
--rw-r--r--   0 runner    (1001) docker     (123)     5055 2023-06-07 14:03:19.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/services/records/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      988 2023-06-07 14:03:19.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/services/records/permissions.py
--rw-r--r--   0 runner    (1001) docker     (123)      997 2023-06-07 14:03:19.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/services/records/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-06-07 14:03:19.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/services/records/search_params.py
--rw-r--r--   0 runner    (1001) docker     (123)    22127 2023-06-07 14:03:19.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/services/records/service.py
--rw-r--r--   0 runner    (1001) docker     (123)      789 2023-06-07 14:03:19.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/services/records/tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:03:25.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:03:25.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/af/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:03:25.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/af/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      527 2023-06-07 14:03:25.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/af/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-06-07 14:03:19.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/af/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:03:25.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/ar/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:03:25.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/ar/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-06-07 14:03:25.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/ar/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)     2870 2023-06-07 14:03:19.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/ar/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:03:25.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/bg/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:03:25.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/bg/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      527 2023-06-07 14:03:25.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/bg/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-06-07 14:03:19.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/bg/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:03:25.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/ca/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:03:25.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/ca/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-06-07 14:03:25.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/ca/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)     2283 2023-06-07 14:03:19.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/ca/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:03:25.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/cs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:03:25.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/cs/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      646 2023-06-07 14:03:25.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/cs/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)     2353 2023-06-07 14:03:19.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/cs/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:03:25.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/da/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:03:25.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/da/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      524 2023-06-07 14:03:25.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/da/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)     2150 2023-06-07 14:03:19.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/da/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:03:25.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/de/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:03:25.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/de/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-06-07 14:03:25.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/de/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)     2784 2023-06-07 14:03:19.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/de/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:03:25.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/el/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:03:25.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/el/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      523 2023-06-07 14:03:25.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/el/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)     2149 2023-06-07 14:03:19.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/el/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:03:25.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/es/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:03:25.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/es/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-06-07 14:03:25.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/es/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)     2670 2023-06-07 14:03:19.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/es/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:03:25.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/et/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:03:25.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/et/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-06-07 14:03:25.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/et/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)     2588 2023-06-07 14:03:19.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/et/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:03:25.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/et_EE/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:03:25.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/et_EE/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      542 2023-06-07 14:03:25.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/et_EE/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-06-07 14:03:19.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/et_EE/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:03:25.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/fa/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:03:25.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/fa/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      524 2023-06-07 14:03:25.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/fa/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)     2150 2023-06-07 14:03:19.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/fa/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:03:25.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/fr/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:03:25.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/fr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-06-07 14:03:25.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/fr/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)     2333 2023-06-07 14:03:19.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/fr/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:03:25.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/gl/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:03:25.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/gl/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-06-07 14:03:25.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/gl/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-06-07 14:03:19.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/gl/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:03:25.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/hr/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:03:25.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/hr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-06-07 14:03:25.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/hr/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)     2224 2023-06-07 14:03:19.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/hr/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:03:25.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/hu/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:03:25.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/hu/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-06-07 14:03:25.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/hu/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)     2598 2023-06-07 14:03:19.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/hu/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:03:25.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/it/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:03:25.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/it/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-06-07 14:03:25.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/it/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)     2323 2023-06-07 14:03:19.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/it/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:03:25.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/ja/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:03:25.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/ja/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-06-07 14:03:25.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/ja/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)     2145 2023-06-07 14:03:19.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/ja/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:03:25.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/ka/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:03:25.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/ka/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      524 2023-06-07 14:03:25.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/ka/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)     2150 2023-06-07 14:03:19.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/ka/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:03:25.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/lt/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:03:25.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/lt/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-06-07 14:03:25.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/lt/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)     2285 2023-06-07 14:03:19.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/lt/LC_MESSAGES/messages.po
--rw-r--r--   0 runner    (1001) docker     (123)     2087 2023-06-07 14:03:19.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/messages.pot
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:03:25.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/no/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:03:25.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/no/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      527 2023-06-07 14:03:25.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/no/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-06-07 14:03:19.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/no/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:03:25.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/pl/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:03:25.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/pl/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      670 2023-06-07 14:03:25.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/pl/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)     2296 2023-06-07 14:03:19.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/pl/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:03:25.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/pt/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:03:25.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/pt/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-06-07 14:03:25.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/pt/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-06-07 14:03:19.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/pt/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:03:25.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/ro/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:03:25.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/ro/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      567 2023-06-07 14:03:25.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/ro/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-06-07 14:03:19.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/ro/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:03:25.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/ru/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:03:25.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/ru/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      663 2023-06-07 14:03:25.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/ru/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)     2289 2023-06-07 14:03:19.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/ru/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:03:25.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/rw/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:03:25.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/rw/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-06-07 14:03:25.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/rw/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)     2155 2023-06-07 14:03:19.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/rw/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:03:25.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/sk/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:03:25.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/sk/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      643 2023-06-07 14:03:25.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/sk/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)     2350 2023-06-07 14:03:19.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/sk/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:03:25.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/sv/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:03:25.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/sv/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-06-07 14:03:25.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/sv/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)     2483 2023-06-07 14:03:19.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/sv/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:03:25.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/tr/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:03:25.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/tr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-06-07 14:03:25.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/tr/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)     2696 2023-06-07 14:03:19.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/tr/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:03:25.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/uk/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:03:25.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/uk/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-06-07 14:03:25.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/uk/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)     2375 2023-06-07 14:03:19.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/uk/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:03:25.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/zh_CN/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:03:25.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/zh_CN/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-06-07 14:03:25.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/zh_CN/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)     2470 2023-06-07 14:03:19.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/zh_CN/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:03:25.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/zh_TW/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:03:25.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/zh_TW/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      533 2023-06-07 14:03:25.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/zh_TW/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)     2159 2023-06-07 14:03:19.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/zh_TW/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:03:25.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4066 2023-06-07 14:03:25.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8234 2023-06-07 14:03:25.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 14:03:25.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-06-07 14:03:25.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 14:03:25.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-06-07 14:03:25.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-07 14:03:25.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-07 14:03:19.000000 invenio-drafts-resources-1.4.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-06-07 14:03:19.000000 invenio-drafts-resources-1.4.1/requirements-devel.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)     1853 2023-06-07 14:03:19.000000 invenio-drafts-resources-1.4.1/run-tests.sh
--rw-r--r--   0 runner    (1001) docker     (123)     2297 2023-06-07 14:03:25.000000 invenio-drafts-resources-1.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-06-07 14:03:19.000000 invenio-drafts-resources-1.4.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:03:25.000000 invenio-drafts-resources-1.4.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2438 2023-06-07 14:03:19.000000 invenio-drafts-resources-1.4.1/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:03:25.000000 invenio-drafts-resources-1.4.1/tests/mock_module/
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-06-07 14:03:19.000000 invenio-drafts-resources-1.4.1/tests/mock_module/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2619 2023-06-07 14:03:19.000000 invenio-drafts-resources-1.4.1/tests/mock_module/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:03:25.000000 invenio-drafts-resources-1.4.1/tests/mock_module/jsonschemas/
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-06-07 14:03:19.000000 invenio-drafts-resources-1.4.1/tests/mock_module/jsonschemas/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:03:25.000000 invenio-drafts-resources-1.4.1/tests/mock_module/jsonschemas/records/
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-06-07 14:03:19.000000 invenio-drafts-resources-1.4.1/tests/mock_module/jsonschemas/records/parent-v1.0.0.json
--rw-r--r--   0 runner    (1001) docker     (123)      342 2023-06-07 14:03:19.000000 invenio-drafts-resources-1.4.1/tests/mock_module/jsonschemas/records/record-v1.0.0.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:03:25.000000 invenio-drafts-resources-1.4.1/tests/mock_module/mappings/
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-06-07 14:03:19.000000 invenio-drafts-resources-1.4.1/tests/mock_module/mappings/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:03:25.000000 invenio-drafts-resources-1.4.1/tests/mock_module/mappings/os-v1/
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-06-07 14:03:19.000000 invenio-drafts-resources-1.4.1/tests/mock_module/mappings/os-v1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:03:25.000000 invenio-drafts-resources-1.4.1/tests/mock_module/mappings/os-v1/draftsresources/
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-06-07 14:03:19.000000 invenio-drafts-resources-1.4.1/tests/mock_module/mappings/os-v1/draftsresources/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:03:25.000000 invenio-drafts-resources-1.4.1/tests/mock_module/mappings/os-v1/draftsresources/drafts/
--rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-06-07 14:03:19.000000 invenio-drafts-resources-1.4.1/tests/mock_module/mappings/os-v1/draftsresources/drafts/draft-v1.0.0.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:03:25.000000 invenio-drafts-resources-1.4.1/tests/mock_module/mappings/os-v1/draftsresources/records/
--rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-06-07 14:03:19.000000 invenio-drafts-resources-1.4.1/tests/mock_module/mappings/os-v1/draftsresources/records/record-v1.0.0.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:03:25.000000 invenio-drafts-resources-1.4.1/tests/mock_module/mappings/os-v2/
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-06-07 14:03:19.000000 invenio-drafts-resources-1.4.1/tests/mock_module/mappings/os-v2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:03:25.000000 invenio-drafts-resources-1.4.1/tests/mock_module/mappings/os-v2/draftsresources/
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-06-07 14:03:19.000000 invenio-drafts-resources-1.4.1/tests/mock_module/mappings/os-v2/draftsresources/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:03:25.000000 invenio-drafts-resources-1.4.1/tests/mock_module/mappings/os-v2/draftsresources/drafts/
--rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-06-07 14:03:19.000000 invenio-drafts-resources-1.4.1/tests/mock_module/mappings/os-v2/draftsresources/drafts/draft-v1.0.0.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:03:25.000000 invenio-drafts-resources-1.4.1/tests/mock_module/mappings/os-v2/draftsresources/records/
--rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-06-07 14:03:19.000000 invenio-drafts-resources-1.4.1/tests/mock_module/mappings/os-v2/draftsresources/records/record-v1.0.0.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:03:25.000000 invenio-drafts-resources-1.4.1/tests/mock_module/mappings/v7/
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-06-07 14:03:19.000000 invenio-drafts-resources-1.4.1/tests/mock_module/mappings/v7/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:03:25.000000 invenio-drafts-resources-1.4.1/tests/mock_module/mappings/v7/draftsresources/
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-06-07 14:03:19.000000 invenio-drafts-resources-1.4.1/tests/mock_module/mappings/v7/draftsresources/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:03:25.000000 invenio-drafts-resources-1.4.1/tests/mock_module/mappings/v7/draftsresources/drafts/
--rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-06-07 14:03:19.000000 invenio-drafts-resources-1.4.1/tests/mock_module/mappings/v7/draftsresources/drafts/draft-v1.0.0.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:03:25.000000 invenio-drafts-resources-1.4.1/tests/mock_module/mappings/v7/draftsresources/records/
--rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-06-07 14:03:19.000000 invenio-drafts-resources-1.4.1/tests/mock_module/mappings/v7/draftsresources/records/record-v1.0.0.json
--rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-06-07 14:03:19.000000 invenio-drafts-resources-1.4.1/tests/mock_module/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-06-07 14:03:19.000000 invenio-drafts-resources-1.4.1/tests/mock_module/permissions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-06-07 14:03:19.000000 invenio-drafts-resources-1.4.1/tests/mock_module/resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2252 2023-06-07 14:03:19.000000 invenio-drafts-resources-1.4.1/tests/mock_module/schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)     2043 2023-06-07 14:03:19.000000 invenio-drafts-resources-1.4.1/tests/mock_module/service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:03:25.000000 invenio-drafts-resources-1.4.1/tests/records/
--rw-r--r--   0 runner    (1001) docker     (123)      787 2023-06-07 14:03:19.000000 invenio-drafts-resources-1.4.1/tests/records/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    11614 2023-06-07 14:03:19.000000 invenio-drafts-resources-1.4.1/tests/records/test_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:03:25.000000 invenio-drafts-resources-1.4.1/tests/resources/
--rw-r--r--   0 runner    (1001) docker     (123)     2394 2023-06-07 14:03:19.000000 invenio-drafts-resources-1.4.1/tests/resources/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     6782 2023-06-07 14:03:19.000000 invenio-drafts-resources-1.4.1/tests/resources/test_files_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     7947 2023-06-07 14:03:19.000000 invenio-drafts-resources-1.4.1/tests/resources/test_record_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2326 2023-06-07 14:03:19.000000 invenio-drafts-resources-1.4.1/tests/resources/test_resource_links.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:03:25.000000 invenio-drafts-resources-1.4.1/tests/services/
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-06-07 14:03:19.000000 invenio-drafts-resources-1.4.1/tests/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-06-07 14:03:19.000000 invenio-drafts-resources-1.4.1/tests/services/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    13306 2023-06-07 14:03:19.000000 invenio-drafts-resources-1.4.1/tests/services/test_record_service.py
--rw-r--r--   0 runner    (1001) docker     (123)    15663 2023-06-07 14:03:19.000000 invenio-drafts-resources-1.4.1/tests/services/test_record_service_files.py
--rw-r--r--   0 runner    (1001) docker     (123)     1617 2023-06-07 14:03:19.000000 invenio-drafts-resources-1.4.1/tests/services/test_record_service_search.py
--rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-06-07 14:03:19.000000 invenio-drafts-resources-1.4.1/tests/services/test_record_service_tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)     1603 2023-06-07 14:03:19.000000 invenio-drafts-resources-1.4.1/tests/services/test_services.py
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-06-07 14:03:19.000000 invenio-drafts-resources-1.4.1/tests/services/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      667 2023-07-05 11:54:24.000000 invenio-drafts-resources-1.4.2/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-05 11:54:24.000000 invenio-drafts-resources-1.4.2/.git-blame-ignore-revs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-07-05 11:54:24.000000 invenio-drafts-resources-1.4.2/.github/workflows/i18n-pull.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-07-05 11:54:24.000000 invenio-drafts-resources-1.4.2/.github/workflows/i18n-push.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      868 2023-07-05 11:54:24.000000 invenio-drafts-resources-1.4.2/.github/workflows/pypi-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3134 2023-07-05 11:54:24.000000 invenio-drafts-resources-1.4.2/.github/workflows/tests.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/.tx/
+-rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-07-05 11:54:24.000000 invenio-drafts-resources-1.4.2/.tx/config
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-07-05 11:54:24.000000 invenio-drafts-resources-1.4.2/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-07-05 11:54:24.000000 invenio-drafts-resources-1.4.2/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3583 2023-07-05 11:54:24.000000 invenio-drafts-resources-1.4.2/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-07-05 11:54:24.000000 invenio-drafts-resources-1.4.2/INSTALL.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-07-05 11:54:24.000000 invenio-drafts-resources-1.4.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      886 2023-07-05 11:54:24.000000 invenio-drafts-resources-1.4.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4211 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-07-05 11:54:24.000000 invenio-drafts-resources-1.4.2/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-07-05 11:54:24.000000 invenio-drafts-resources-1.4.2/babel.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     7481 2023-07-05 11:54:24.000000 invenio-drafts-resources-1.4.2/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-07-05 11:54:24.000000 invenio-drafts-resources-1.4.2/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-07-05 11:54:24.000000 invenio-drafts-resources-1.4.2/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-07-05 11:54:24.000000 invenio-drafts-resources-1.4.2/docs/changes.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    10309 2023-07-05 11:54:24.000000 invenio-drafts-resources-1.4.2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-07-05 11:54:24.000000 invenio-drafts-resources-1.4.2/docs/configuration.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-07-05 11:54:24.000000 invenio-drafts-resources-1.4.2/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      819 2023-07-05 11:54:24.000000 invenio-drafts-resources-1.4.2/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-07-05 11:54:24.000000 invenio-drafts-resources-1.4.2/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-07-05 11:54:24.000000 invenio-drafts-resources-1.4.2/docs/license.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7017 2023-07-05 11:54:24.000000 invenio-drafts-resources-1.4.2/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-05 11:54:24.000000 invenio-drafts-resources-1.4.2/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-07-05 11:54:24.000000 invenio-drafts-resources-1.4.2/docs/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-07-05 11:54:24.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/records/
+-rw-r--r--   0 runner    (1001) docker     (123)      687 2023-07-05 11:54:24.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/records/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9005 2023-07-05 11:54:24.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/records/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4316 2023-07-05 11:54:24.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/records/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/records/systemfields/
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-07-05 11:54:24.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/records/systemfields/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4409 2023-07-05 11:54:24.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/records/systemfields/parent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7618 2023-07-05 11:54:24.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/records/systemfields/versions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-07-05 11:54:24.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/resources/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/resources/records/
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-07-05 11:54:24.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/resources/records/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-07-05 11:54:24.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/resources/records/args.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-07-05 11:54:24.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/resources/records/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-07-05 11:54:24.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/resources/records/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7603 2023-07-05 11:54:24.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/resources/records/resource.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/services/
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-07-05 11:54:24.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/services/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/services/records/
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-07-05 11:54:24.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/services/records/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/services/records/components/
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-07-05 11:54:24.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/services/records/components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1362 2023-07-05 11:54:24.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/services/records/components/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7891 2023-07-05 11:54:24.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/services/records/components/files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-07-05 11:54:24.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/services/records/components/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1209 2023-07-05 11:54:24.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/services/records/components/pid.py
+-rw-r--r--   0 runner    (1001) docker     (123)      591 2023-07-05 11:54:24.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/services/records/components/relations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5055 2023-07-05 11:54:24.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/services/records/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      988 2023-07-05 11:54:24.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/services/records/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      997 2023-07-05 11:54:24.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/services/records/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-07-05 11:54:24.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/services/records/search_params.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22127 2023-07-05 11:54:24.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/services/records/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-07-05 11:54:24.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/services/records/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/af/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/af/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      527 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/af/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-07-05 11:54:24.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/af/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/ar/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/ar/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-07-05 11:54:30.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/ar/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     2897 2023-07-05 11:54:24.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/ar/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/bg/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/bg/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      527 2023-07-05 11:54:30.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/bg/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-07-05 11:54:24.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/bg/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/ca/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/ca/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/ca/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     2283 2023-07-05 11:54:24.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/ca/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/cs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/cs/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      646 2023-07-05 11:54:30.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/cs/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     2353 2023-07-05 11:54:24.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/cs/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/da/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/da/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/da/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     2150 2023-07-05 11:54:24.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/da/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/de/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/de/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-07-05 11:54:30.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/de/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     2784 2023-07-05 11:54:24.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/de/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/de_AT/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/de_AT/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/de_AT/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-07-05 11:54:24.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/de_AT/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/de_DE/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/de_DE/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/de_DE/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-07-05 11:54:24.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/de_DE/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/el/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/el/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/el/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     2149 2023-07-05 11:54:24.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/el/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/en_AT/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/en_AT/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      541 2023-07-05 11:54:30.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/en_AT/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-07-05 11:54:24.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/en_AT/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/en_HU/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/en_HU/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/en_HU/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-07-05 11:54:24.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/en_HU/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/es/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/es/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-07-05 11:54:30.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/es/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     2670 2023-07-05 11:54:24.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/es/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/es_CU/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/es_CU/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-07-05 11:54:30.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/es_CU/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     2203 2023-07-05 11:54:24.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/es_CU/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/es_MX/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/es_MX/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/es_MX/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-07-05 11:54:24.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/es_MX/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/et/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/et/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/et/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     2588 2023-07-05 11:54:24.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/et/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/et_EE/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/et_EE/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      542 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/et_EE/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-07-05 11:54:24.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/et_EE/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/fa/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/fa/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2023-07-05 11:54:30.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/fa/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     2150 2023-07-05 11:54:24.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/fa/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/fa_IR/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/fa_IR/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-07-05 11:54:30.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/fa_IR/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     2163 2023-07-05 11:54:24.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/fa_IR/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/fr/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/fr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-07-05 11:54:30.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/fr/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     2333 2023-07-05 11:54:24.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/fr/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/fr_CI/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/fr_CI/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/fr_CI/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     2224 2023-07-05 11:54:24.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/fr_CI/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/fr_FR/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/fr_FR/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-07-05 11:54:30.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/fr_FR/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     2216 2023-07-05 11:54:24.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/fr_FR/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/gl/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/gl/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-07-05 11:54:30.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/gl/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-07-05 11:54:24.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/gl/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/hi_IN/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/hi_IN/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-07-05 11:54:30.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/hi_IN/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     2163 2023-07-05 11:54:24.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/hi_IN/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/hr/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/hr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/hr/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     2224 2023-07-05 11:54:24.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/hr/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/hu/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/hu/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/hu/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     2598 2023-07-05 11:54:24.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/hu/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/hu_HU/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/hu_HU/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      543 2023-07-05 11:54:30.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/hu_HU/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     2169 2023-07-05 11:54:24.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/hu_HU/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/it/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/it/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/it/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     2323 2023-07-05 11:54:24.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/it/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/ja/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/ja/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-07-05 11:54:30.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/ja/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     2145 2023-07-05 11:54:24.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/ja/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/ka/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/ka/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2023-07-05 11:54:30.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/ka/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     2150 2023-07-05 11:54:24.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/ka/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/lt/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/lt/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-07-05 11:54:30.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/lt/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     2285 2023-07-05 11:54:24.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/lt/LC_MESSAGES/messages.po
+-rw-r--r--   0 runner    (1001) docker     (123)     2087 2023-07-05 11:54:24.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/messages.pot
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/ne/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/ne/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2023-07-05 11:54:30.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/ne/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     2150 2023-07-05 11:54:24.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/ne/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/no/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/no/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      527 2023-07-05 11:54:30.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/no/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-07-05 11:54:24.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/no/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/pl/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/pl/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/pl/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     2296 2023-07-05 11:54:24.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/pl/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/pt/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/pt/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-07-05 11:54:30.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/pt/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-07-05 11:54:24.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/pt/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/ro/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/ro/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-07-05 11:54:30.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/ro/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-07-05 11:54:24.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/ro/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/ru/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/ru/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      663 2023-07-05 11:54:30.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/ru/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     2289 2023-07-05 11:54:24.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/ru/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/rw/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/rw/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/rw/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     2155 2023-07-05 11:54:24.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/rw/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/sk/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/sk/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-07-05 11:54:30.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/sk/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     2350 2023-07-05 11:54:24.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/sk/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/sv/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/sv/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-07-05 11:54:30.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/sv/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     2492 2023-07-05 11:54:24.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/sv/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/sv_SE/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/sv_SE/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-07-05 11:54:30.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/sv_SE/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-07-05 11:54:24.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/sv_SE/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/tr/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/tr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/tr/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     2696 2023-07-05 11:54:24.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/tr/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/uk/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/uk/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-07-05 11:54:30.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/uk/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     2728 2023-07-05 11:54:24.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/uk/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/uk_UA/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/uk_UA/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/uk_UA/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     2391 2023-07-05 11:54:24.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/uk_UA/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/zh_CN/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/zh_CN/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-07-05 11:54:30.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/zh_CN/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     2470 2023-07-05 11:54:24.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/zh_CN/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/zh_TW/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/zh_TW/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      533 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/zh_TW/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     2159 2023-07-05 11:54:24.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/zh_TW/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4211 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10132 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-05 11:54:24.000000 invenio-drafts-resources-1.4.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-07-05 11:54:24.000000 invenio-drafts-resources-1.4.2/requirements-devel.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1905 2023-07-05 11:54:24.000000 invenio-drafts-resources-1.4.2/run-tests.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     2297 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-07-05 11:54:24.000000 invenio-drafts-resources-1.4.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2438 2023-07-05 11:54:24.000000 invenio-drafts-resources-1.4.2/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/tests/mock_module/
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-07-05 11:54:24.000000 invenio-drafts-resources-1.4.2/tests/mock_module/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2619 2023-07-05 11:54:24.000000 invenio-drafts-resources-1.4.2/tests/mock_module/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/tests/mock_module/jsonschemas/
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-07-05 11:54:24.000000 invenio-drafts-resources-1.4.2/tests/mock_module/jsonschemas/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/tests/mock_module/jsonschemas/records/
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-07-05 11:54:24.000000 invenio-drafts-resources-1.4.2/tests/mock_module/jsonschemas/records/parent-v1.0.0.json
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-07-05 11:54:24.000000 invenio-drafts-resources-1.4.2/tests/mock_module/jsonschemas/records/record-v1.0.0.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/tests/mock_module/mappings/
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-07-05 11:54:24.000000 invenio-drafts-resources-1.4.2/tests/mock_module/mappings/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/tests/mock_module/mappings/os-v1/
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-07-05 11:54:24.000000 invenio-drafts-resources-1.4.2/tests/mock_module/mappings/os-v1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/tests/mock_module/mappings/os-v1/draftsresources/
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-07-05 11:54:24.000000 invenio-drafts-resources-1.4.2/tests/mock_module/mappings/os-v1/draftsresources/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/tests/mock_module/mappings/os-v1/draftsresources/drafts/
+-rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-07-05 11:54:24.000000 invenio-drafts-resources-1.4.2/tests/mock_module/mappings/os-v1/draftsresources/drafts/draft-v1.0.0.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/tests/mock_module/mappings/os-v1/draftsresources/records/
+-rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-07-05 11:54:24.000000 invenio-drafts-resources-1.4.2/tests/mock_module/mappings/os-v1/draftsresources/records/record-v1.0.0.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/tests/mock_module/mappings/os-v2/
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-07-05 11:54:24.000000 invenio-drafts-resources-1.4.2/tests/mock_module/mappings/os-v2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/tests/mock_module/mappings/os-v2/draftsresources/
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-07-05 11:54:24.000000 invenio-drafts-resources-1.4.2/tests/mock_module/mappings/os-v2/draftsresources/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/tests/mock_module/mappings/os-v2/draftsresources/drafts/
+-rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-07-05 11:54:24.000000 invenio-drafts-resources-1.4.2/tests/mock_module/mappings/os-v2/draftsresources/drafts/draft-v1.0.0.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/tests/mock_module/mappings/os-v2/draftsresources/records/
+-rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-07-05 11:54:24.000000 invenio-drafts-resources-1.4.2/tests/mock_module/mappings/os-v2/draftsresources/records/record-v1.0.0.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/tests/mock_module/mappings/v7/
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-07-05 11:54:24.000000 invenio-drafts-resources-1.4.2/tests/mock_module/mappings/v7/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/tests/mock_module/mappings/v7/draftsresources/
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-07-05 11:54:24.000000 invenio-drafts-resources-1.4.2/tests/mock_module/mappings/v7/draftsresources/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/tests/mock_module/mappings/v7/draftsresources/drafts/
+-rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-07-05 11:54:24.000000 invenio-drafts-resources-1.4.2/tests/mock_module/mappings/v7/draftsresources/drafts/draft-v1.0.0.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/tests/mock_module/mappings/v7/draftsresources/records/
+-rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-07-05 11:54:24.000000 invenio-drafts-resources-1.4.2/tests/mock_module/mappings/v7/draftsresources/records/record-v1.0.0.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-07-05 11:54:24.000000 invenio-drafts-resources-1.4.2/tests/mock_module/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-07-05 11:54:24.000000 invenio-drafts-resources-1.4.2/tests/mock_module/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-07-05 11:54:24.000000 invenio-drafts-resources-1.4.2/tests/mock_module/resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2252 2023-07-05 11:54:24.000000 invenio-drafts-resources-1.4.2/tests/mock_module/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-07-05 11:54:24.000000 invenio-drafts-resources-1.4.2/tests/mock_module/service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/tests/records/
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-07-05 11:54:24.000000 invenio-drafts-resources-1.4.2/tests/records/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11614 2023-07-05 11:54:24.000000 invenio-drafts-resources-1.4.2/tests/records/test_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/tests/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)     2394 2023-07-05 11:54:24.000000 invenio-drafts-resources-1.4.2/tests/resources/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6782 2023-07-05 11:54:24.000000 invenio-drafts-resources-1.4.2/tests/resources/test_files_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7947 2023-07-05 11:54:24.000000 invenio-drafts-resources-1.4.2/tests/resources/test_record_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2326 2023-07-05 11:54:24.000000 invenio-drafts-resources-1.4.2/tests/resources/test_resource_links.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/tests/services/
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-07-05 11:54:24.000000 invenio-drafts-resources-1.4.2/tests/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-07-05 11:54:24.000000 invenio-drafts-resources-1.4.2/tests/services/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13306 2023-07-05 11:54:24.000000 invenio-drafts-resources-1.4.2/tests/services/test_record_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15663 2023-07-05 11:54:24.000000 invenio-drafts-resources-1.4.2/tests/services/test_record_service_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1617 2023-07-05 11:54:24.000000 invenio-drafts-resources-1.4.2/tests/services/test_record_service_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-07-05 11:54:24.000000 invenio-drafts-resources-1.4.2/tests/services/test_record_service_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1603 2023-07-05 11:54:24.000000 invenio-drafts-resources-1.4.2/tests/services/test_services.py
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-07-05 11:54:24.000000 invenio-drafts-resources-1.4.2/tests/services/utils.py
```

### Comparing `invenio-drafts-resources-1.4.1/.editorconfig` & `invenio-drafts-resources-1.4.2/.editorconfig`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.1/.github/workflows/pypi-publish.yml` & `invenio-drafts-resources-1.4.2/.github/workflows/pypi-publish.yml`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.1/.github/workflows/tests.yml` & `invenio-drafts-resources-1.4.2/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.1/.tx/config` & `invenio-drafts-resources-1.4.2/.tx/config`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # -*- coding: utf-8 -*-
 #
 # Copyright (C) 2020 CERN.
+# Copyright (C) 2023 Graz University of Technology.
 #
 # Invenio-Drafts-Resources is free software; you can redistribute it and/or
 # modify it under the terms of the MIT License; see LICENSE file for more
 # details.
 #
 # 1) Create message catalog:
 #    $ python setup.py extract_messages
@@ -18,14 +19,14 @@
 #    $ tx push -s -t
 # 5) Pull translations for a single language from Transifex
 #    $ tx pull -l <lang>
 # 6) Pull translations for all languages from Transifex
 #    $ tx pull -a
 
 [main]
-host = https://www.transifex.com
+host = https://app.transifex.com
 
-[invenio.invenio_drafts_resources-messages]
+[o:inveniosoftware:p:invenio:r:invenio_drafts_resources-messages]
 file_filter = invenio_drafts_resources/translations/<lang>/LC_MESSAGES/messages.po
 source_file = invenio_drafts_resources/translations/messages.pot
 source_lang = en
 type = PO
```

### Comparing `invenio-drafts-resources-1.4.1/CHANGES.rst` & `invenio-drafts-resources-1.4.2/CHANGES.rst`

 * *Files 11% similar despite different names*

```diff
@@ -5,14 +5,19 @@
     Invenio-Drafts-Resources is free software; you can redistribute it and/or
     modify it under the terms of the MIT License; see LICENSE file for more
     details.
 
 Changes
 =======
 
+Version 1.4.2 (2023-07-05)
+
+- transifex: update config
+- components: add default files enabled variable
+
 Version 1.4.1 (2023-06-06)
 
 - fix permission check for managing files
 
 Version 1.4.0 (2023-04-25)
 
 - upgrade invenio-records-resources
```

### Comparing `invenio-drafts-resources-1.4.1/CONTRIBUTING.rst` & `invenio-drafts-resources-1.4.2/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.1/LICENSE` & `invenio-drafts-resources-1.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.1/MANIFEST.in` & `invenio-drafts-resources-1.4.2/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.1/PKG-INFO` & `invenio-drafts-resources-1.4.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invenio-drafts-resources
-Version: 1.4.1
+Version: 1.4.2
 Summary: Invenio Drafts Resources module to create REST APIs
 Home-page: https://github.com/inveniosoftware/Invenio-Drafts-Resources
 Author: CERN
 Author-email: info@inveniosoftware.org
 License: MIT
 Description: ..
             Copyright (C) 2020 CERN.
@@ -47,14 +47,19 @@
             Invenio-Drafts-Resources is free software; you can redistribute it and/or
             modify it under the terms of the MIT License; see LICENSE file for more
             details.
         
         Changes
         =======
         
+        Version 1.4.2 (2023-07-05)
+        
+        - transifex: update config
+        - components: add default files enabled variable
+        
         Version 1.4.1 (2023-06-06)
         
         - fix permission check for managing files
         
         Version 1.4.0 (2023-04-25)
         
         - upgrade invenio-records-resources
```

### Comparing `invenio-drafts-resources-1.4.1/README.rst` & `invenio-drafts-resources-1.4.2/README.rst`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.1/babel.ini` & `invenio-drafts-resources-1.4.2/babel.ini`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.1/docs/Makefile` & `invenio-drafts-resources-1.4.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.1/docs/conf.py` & `invenio-drafts-resources-1.4.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.1/docs/index.rst` & `invenio-drafts-resources-1.4.2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.1/docs/make.bat` & `invenio-drafts-resources-1.4.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.1/invenio_drafts_resources/records/__init__.py` & `invenio-drafts-resources-1.4.2/invenio_drafts_resources/records/__init__.py`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.1/invenio_drafts_resources/records/api.py` & `invenio-drafts-resources-1.4.2/invenio_drafts_resources/records/api.py`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.1/invenio_drafts_resources/records/models.py` & `invenio-drafts-resources-1.4.2/invenio_drafts_resources/records/models.py`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.1/invenio_drafts_resources/records/systemfields/parent.py` & `invenio-drafts-resources-1.4.2/invenio_drafts_resources/records/systemfields/parent.py`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.1/invenio_drafts_resources/records/systemfields/versions.py` & `invenio-drafts-resources-1.4.2/invenio_drafts_resources/records/systemfields/versions.py`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.1/invenio_drafts_resources/resources/records/args.py` & `invenio-drafts-resources-1.4.2/invenio_drafts_resources/resources/records/args.py`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.1/invenio_drafts_resources/resources/records/config.py` & `invenio-drafts-resources-1.4.2/invenio_drafts_resources/resources/records/config.py`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.1/invenio_drafts_resources/resources/records/errors.py` & `invenio-drafts-resources-1.4.2/invenio_drafts_resources/resources/records/errors.py`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.1/invenio_drafts_resources/resources/records/resource.py` & `invenio-drafts-resources-1.4.2/invenio_drafts_resources/resources/records/resource.py`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.1/invenio_drafts_resources/services/records/components/__init__.py` & `invenio-drafts-resources-1.4.2/invenio_drafts_resources/services/records/components/__init__.py`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.1/invenio_drafts_resources/services/records/components/base.py` & `invenio-drafts-resources-1.4.2/invenio_drafts_resources/services/records/components/base.py`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.1/invenio_drafts_resources/services/records/components/files.py` & `invenio-drafts-resources-1.4.2/invenio_drafts_resources/services/records/components/files.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,15 +32,17 @@
     def create(self, identity, data=None, record=None, errors=None):
         """Assigns files.enabled.
 
         NOTE: `record` actually refers to the draft
               (this interface is used in records-resources and rdm-records)
         """
         draft = record
-        enabled = data.get("files", {}).get("enabled", True)
+        enabled = data.get("files", {}).get(
+            "enabled", self.service.config.default_files_enabled
+        )
 
         if draft.files.enabled != enabled:
             if not self.service.check_permission(
                 identity, "manage_files", record=draft
             ):
                 errors.append(
                     {
```

### Comparing `invenio-drafts-resources-1.4.1/invenio_drafts_resources/services/records/components/metadata.py` & `invenio-drafts-resources-1.4.2/invenio_drafts_resources/services/records/components/metadata.py`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.1/invenio_drafts_resources/services/records/components/pid.py` & `invenio-drafts-resources-1.4.2/invenio_drafts_resources/services/records/components/pid.py`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.1/invenio_drafts_resources/services/records/components/relations.py` & `invenio-drafts-resources-1.4.2/invenio_drafts_resources/services/records/components/relations.py`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.1/invenio_drafts_resources/services/records/config.py` & `invenio-drafts-resources-1.4.2/invenio_drafts_resources/services/records/config.py`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.1/invenio_drafts_resources/services/records/permissions.py` & `invenio-drafts-resources-1.4.2/invenio_drafts_resources/services/records/permissions.py`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.1/invenio_drafts_resources/services/records/schema.py` & `invenio-drafts-resources-1.4.2/invenio_drafts_resources/services/records/schema.py`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.1/invenio_drafts_resources/services/records/search_params.py` & `invenio-drafts-resources-1.4.2/invenio_drafts_resources/services/records/search_params.py`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.1/invenio_drafts_resources/services/records/service.py` & `invenio-drafts-resources-1.4.2/invenio_drafts_resources/services/records/service.py`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.1/invenio_drafts_resources/services/records/tasks.py` & `invenio-drafts-resources-1.4.2/invenio_drafts_resources/services/records/tasks.py`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/af/LC_MESSAGES/messages.mo` & `invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/af/LC_MESSAGES/messages.mo`

 * *Format-specific differences are supported for Gettext message catalogues but no file-specific differences were detected; falling back to a binary diff. file(1) reports: GNU message catalog (little endian), revision 0.0, 1 message, Project-Id-Version: invenio-drafts-resources 0.18.2*

 * *Files 3% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 000000c0: 7369 6f6e 2d44 6174 653a 2032 3032 312d  sion-Date: 2021-
 000000d0: 3037 2d31 3320 3132 3a34 302b 3030 3030  07-13 12:40+0000
 000000e0: 0a4c 6173 742d 5472 616e 736c 6174 6f72  .Last-Translator
 000000f0: 3a20 4655 4c4c 204e 414d 4520 3c45 4d41  : FULL NAME <EMA
 00000100: 494c 4041 4444 5245 5353 3e0a 4c61 6e67  IL@ADDRESS>.Lang
 00000110: 7561 6765 3a20 6166 0a4c 616e 6775 6167  uage: af.Languag
 00000120: 652d 5465 616d 3a20 4166 7269 6b61 616e  e-Team: Afrikaan
-00000130: 7320 2868 7474 7073 3a2f 2f77 7777 2e74  s (https://www.t
+00000130: 7320 2868 7474 7073 3a2f 2f61 7070 2e74  s (https://app.t
 00000140: 7261 6e73 6966 6578 2e63 6f6d 2f69 6e76  ransifex.com/inv
 00000150: 656e 696f 736f 6674 7761 7265 2f74 6561  eniosoftware/tea
 00000160: 6d73 2f32 3335 3337 2f61 662f 290a 506c  ms/23537/af/).Pl
 00000170: 7572 616c 2d46 6f72 6d73 3a20 6e70 6c75  ural-Forms: nplu
 00000180: 7261 6c73 3d32 3b20 706c 7572 616c 3d28  rals=2; plural=(
 00000190: 6e20 213d 2031 293b 0a4d 494d 452d 5665  n != 1);.MIME-Ve
 000001a0: 7273 696f 6e3a 2031 2e30 0a43 6f6e 7465  rsion: 1.0.Conte
```

### Comparing `invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/af/LC_MESSAGES/messages.po` & `invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/af/LC_MESSAGES/messages.po`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-drafts-resources 0.18.2\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:07+0000\n"
 "PO-Revision-Date: 2021-07-13 12:40+0000\n"
-"Language-Team: Afrikaans (https://www.transifex.com/inveniosoftware/teams/23537/af/)\n"
+"Language-Team: Afrikaans (https://app.transifex.com/inveniosoftware/teams/23537/af/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.3\n"
 "Language: af\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
```

### Comparing `invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/ar/LC_MESSAGES/messages.mo` & `invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/ar/LC_MESSAGES/messages.mo`

 * *Files 11% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,50 +1,50 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-drafts-resources 0.18.2\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:07+0000\n"
 "PO-Revision-Date: 2021-07-13 12:40+0000\n"
-"Last-Translator: Bessem Aamira <bessemamira@gmail.com>, 2022\n"
+"Last-Translator: Salaheddine Ben Ali <salaheddine.benali@cnudst.tn>, 2022\n"
 "Language: ar\n"
-"Language-Team: Arabic (https://www.transifex.com/inveniosoftware/teams/23537/"
+"Language-Team: Arabic (https://app.transifex.com/inveniosoftware/teams/23537/"
 "ar/)\n"
 "Plural-Forms: nplurals=6; plural=n==0 ? 0 : n==1 ? 1 : n==2 ? 2 : n%100>=3 "
 "&& n%100<=10 ? 3 : n%100>=11 && n%100<=99 ? 4 : 5;\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.12.1\n"
 
 msgid "Best match"
 msgstr "أفضل تطابق "
 
 msgid "Files support must be enabled."
-msgstr "يجب أن يتم تفعيل دعم الملفات."
+msgstr "دعم الملفات يجب أن يكون مفعّلا ."
 
 msgid "Least recently updated"
-msgstr "الأقل تحيينا مؤخرًا"
+msgstr "التحيين الأحدث"
 
 msgid ""
 "Missing uploaded files. To disable files for this record please mark it as "
 "metadata-only."
 msgstr ""
-"الملفات التي تم تحميلها مفقودة. لتعطيل الملفات لهذا السجل ، يرجى تحديدها على "
-"أنها بيانات وصفية فقط."
+"الملفات التي تم تحميلها مفقودة. لتعطيل الملفات لهذه التّسجيلة ، يرجى تحديدها "
+"على أنها بيانات وصفية فقط."
 
 msgid "Newest"
-msgstr "الأجد"
+msgstr "الأحدث"
 
 msgid "Oldest"
 msgstr "الأقدم"
 
 msgid "Please remove all files first."
 msgstr "يرجى إزالة جميع الملفات أولاً."
 
 msgid "Recently updated"
-msgstr "المحيين مؤخرا"
+msgstr "المحيّن مؤخرا"
 
 msgid "The record has no files."
-msgstr "لا يحتوي السجل على ملفات."
+msgstr "التّسجيلة لا تحتوي على ملفات."
 
 msgid "Version"
 msgstr "نسخة"
```

### Comparing `invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/ar/LC_MESSAGES/messages.po` & `invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/sv/LC_MESSAGES/messages.po`

 * *Files 14% similar despite different names*

```diff
@@ -1,75 +1,75 @@
 # Translations template for invenio-drafts-resources.
 # Copyright (C) 2022 CERN
 # This file is distributed under the same license as the
 # invenio-drafts-resources project.
 # FIRST AUTHOR <EMAIL@ADDRESS>, 2022.
 # 
 # Translators:
-# Salaheddine Ben Ali <salaheddine.benali@cnudst.tn>, 2022
-# Bessem Aamira <bessemamira@gmail.com>, 2022
+# Sam Arbid, 2022
+# yyones, 2023
 # 
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-drafts-resources 0.18.2\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:07+0000\n"
 "PO-Revision-Date: 2021-07-13 12:40+0000\n"
-"Last-Translator: Bessem Aamira <bessemamira@gmail.com>, 2022\n"
-"Language-Team: Arabic (https://www.transifex.com/inveniosoftware/teams/23537/ar/)\n"
+"Last-Translator: yyones, 2023\n"
+"Language-Team: Swedish (https://app.transifex.com/inveniosoftware/teams/23537/sv/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.3\n"
-"Language: ar\n"
-"Plural-Forms: nplurals=6; plural=n==0 ? 0 : n==1 ? 1 : n==2 ? 2 : n%100>=3 && n%100<=10 ? 3 : n%100>=11 && n%100<=99 ? 4 : 5;\n"
+"Language: sv\n"
+"Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
 #: invenio_drafts_resources/services/records/config.py:42
 #: invenio_drafts_resources/services/records/config.py:71
 msgid "Best match"
-msgstr "أفضل تطابق "
+msgstr "Bästa matchningen"
 
 #: invenio_drafts_resources/services/records/config.py:46
 #: invenio_drafts_resources/services/records/config.py:83
 msgid "Newest"
-msgstr "الأجد"
+msgstr "Nyast"
 
 #: invenio_drafts_resources/services/records/config.py:50
 #: invenio_drafts_resources/services/records/config.py:87
 msgid "Oldest"
-msgstr "الأقدم"
+msgstr "Äldst"
 
 #: invenio_drafts_resources/services/records/config.py:54
 #: invenio_drafts_resources/services/records/config.py:91
 #: invenio_drafts_resources/services/records/config.py:108
 msgid "Version"
-msgstr "نسخة"
+msgstr "Version"
 
 #: invenio_drafts_resources/services/records/config.py:75
 msgid "Recently updated"
-msgstr "المحيين مؤخرا"
+msgstr "Nyligen uppdaterad"
 
 #: invenio_drafts_resources/services/records/config.py:79
 msgid "Least recently updated"
-msgstr "الأقل تحيينا مؤخرًا"
+msgstr "Senast uppdaterad"
 
 #: invenio_drafts_resources/services/records/components/files.py:60
 #: invenio_drafts_resources/services/records/components/files.py:127
 msgid ""
 "Missing uploaded files. To disable files for this record please mark it as "
 "metadata-only."
 msgstr ""
-"الملفات التي تم تحميلها مفقودة. لتعطيل الملفات لهذا السجل ، يرجى تحديدها على"
-" أنها بيانات وصفية فقط."
+"Uppladdade filer saknas. För att inaktivera filer för denna post, markera "
+"den som endast metadata."
 
 #: invenio_drafts_resources/services/records/components/files.py:153
 msgid "Files support must be enabled."
-msgstr "يجب أن يتم تفعيل دعم الملفات."
+msgstr "Filstöd måste vara aktiverat."
 
 #: invenio_drafts_resources/services/records/components/files.py:158
 msgid "Please remove all files first."
-msgstr "يرجى إزالة جميع الملفات أولاً."
+msgstr "Ta bort alla filer först."
 
 #: invenio_drafts_resources/services/records/components/files.py:163
 msgid "The record has no files."
-msgstr "لا يحتوي السجل على ملفات."
+msgstr "Posten har inga filer."
```

### Comparing `invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/bg/LC_MESSAGES/messages.mo` & `invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/de_AT/LC_MESSAGES/messages.mo`

 * *Format-specific differences are supported for Gettext message catalogues but no file-specific differences were detected; falling back to a binary diff. file(1) reports: GNU message catalog (little endian), revision 0.0, 1 message, Project-Id-Version: invenio-drafts-resources 0.18.2*

 * *Files 7% similar despite different names*

```diff
@@ -1,33 +1,34 @@
 00000000: de12 0495 0000 0000 0100 0000 1c00 0000  ................
 00000010: 2400 0000 0000 0000 0000 0000 0000 0000  $...............
-00000020: 2c00 0000 e101 0000 2d00 0000 0050 726f  ,.......-....Pro
+00000020: 2c00 0000 ee01 0000 2d00 0000 0050 726f  ,.......-....Pro
 00000030: 6a65 6374 2d49 642d 5665 7273 696f 6e3a  ject-Id-Version:
 00000040: 2069 6e76 656e 696f 2d64 7261 6674 732d   invenio-drafts-
 00000050: 7265 736f 7572 6365 7320 302e 3138 2e32  resources 0.18.2
 00000060: 0a52 6570 6f72 742d 4d73 6769 642d 4275  .Report-Msgid-Bu
 00000070: 6773 2d54 6f3a 2069 6e66 6f40 696e 7665  gs-To: info@inve
 00000080: 6e69 6f73 6f66 7477 6172 652e 6f72 670a  niosoftware.org.
 00000090: 504f 542d 4372 6561 7469 6f6e 2d44 6174  POT-Creation-Dat
 000000a0: 653a 2032 3032 322d 3130 2d31 3220 3039  e: 2022-10-12 09
 000000b0: 3a30 372b 3030 3030 0a50 4f2d 5265 7669  :07+0000.PO-Revi
 000000c0: 7369 6f6e 2d44 6174 653a 2032 3032 312d  sion-Date: 2021-
 000000d0: 3037 2d31 3320 3132 3a34 302b 3030 3030  07-13 12:40+0000
 000000e0: 0a4c 6173 742d 5472 616e 736c 6174 6f72  .Last-Translator
 000000f0: 3a20 4655 4c4c 204e 414d 4520 3c45 4d41  : FULL NAME <EMA
 00000100: 494c 4041 4444 5245 5353 3e0a 4c61 6e67  IL@ADDRESS>.Lang
-00000110: 7561 6765 3a20 6267 0a4c 616e 6775 6167  uage: bg.Languag
-00000120: 652d 5465 616d 3a20 4275 6c67 6172 6961  e-Team: Bulgaria
-00000130: 6e20 2868 7474 7073 3a2f 2f77 7777 2e74  n (https://www.t
-00000140: 7261 6e73 6966 6578 2e63 6f6d 2f69 6e76  ransifex.com/inv
-00000150: 656e 696f 736f 6674 7761 7265 2f74 6561  eniosoftware/tea
-00000160: 6d73 2f32 3335 3337 2f62 672f 290a 506c  ms/23537/bg/).Pl
-00000170: 7572 616c 2d46 6f72 6d73 3a20 6e70 6c75  ural-Forms: nplu
-00000180: 7261 6c73 3d32 3b20 706c 7572 616c 3d28  rals=2; plural=(
-00000190: 6e20 213d 2031 293b 0a4d 494d 452d 5665  n != 1);.MIME-Ve
-000001a0: 7273 696f 6e3a 2031 2e30 0a43 6f6e 7465  rsion: 1.0.Conte
-000001b0: 6e74 2d54 7970 653a 2074 6578 742f 706c  nt-Type: text/pl
-000001c0: 6169 6e3b 2063 6861 7273 6574 3d75 7466  ain; charset=utf
-000001d0: 2d38 0a43 6f6e 7465 6e74 2d54 7261 6e73  -8.Content-Trans
-000001e0: 6665 722d 456e 636f 6469 6e67 3a20 3862  fer-Encoding: 8b
-000001f0: 6974 0a47 656e 6572 6174 6564 2d42 793a  it.Generated-By:
-00000200: 2042 6162 656c 2032 2e31 322e 310a 00     Babel 2.12.1..
+00000110: 7561 6765 3a20 6465 5f41 540a 4c61 6e67  uage: de_AT.Lang
+00000120: 7561 6765 2d54 6561 6d3a 2047 6572 6d61  uage-Team: Germa
+00000130: 6e20 2841 7573 7472 6961 2920 2868 7474  n (Austria) (htt
+00000140: 7073 3a2f 2f61 7070 2e74 7261 6e73 6966  ps://app.transif
+00000150: 6578 2e63 6f6d 2f69 6e76 656e 696f 736f  ex.com/invenioso
+00000160: 6674 7761 7265 2f74 6561 6d73 2f32 3335  ftware/teams/235
+00000170: 3337 2f64 655f 4154 2f29 0a50 6c75 7261  37/de_AT/).Plura
+00000180: 6c2d 466f 726d 733a 206e 706c 7572 616c  l-Forms: nplural
+00000190: 733d 323b 2070 6c75 7261 6c3d 286e 2021  s=2; plural=(n !
+000001a0: 3d20 3129 3b0a 4d49 4d45 2d56 6572 7369  = 1);.MIME-Versi
+000001b0: 6f6e 3a20 312e 300a 436f 6e74 656e 742d  on: 1.0.Content-
+000001c0: 5479 7065 3a20 7465 7874 2f70 6c61 696e  Type: text/plain
+000001d0: 3b20 6368 6172 7365 743d 7574 662d 380a  ; charset=utf-8.
+000001e0: 436f 6e74 656e 742d 5472 616e 7366 6572  Content-Transfer
+000001f0: 2d45 6e63 6f64 696e 673a 2038 6269 740a  -Encoding: 8bit.
+00000200: 4765 6e65 7261 7465 642d 4279 3a20 4261  Generated-By: Ba
+00000210: 6265 6c20 322e 3132 2e31 0a00            bel 2.12.1..
```

### Comparing `invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/bg/LC_MESSAGES/messages.po` & `invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/bg/LC_MESSAGES/messages.po`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-drafts-resources 0.18.2\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:07+0000\n"
 "PO-Revision-Date: 2021-07-13 12:40+0000\n"
-"Language-Team: Bulgarian (https://www.transifex.com/inveniosoftware/teams/23537/bg/)\n"
+"Language-Team: Bulgarian (https://app.transifex.com/inveniosoftware/teams/23537/bg/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.3\n"
 "Language: bg\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
```

### Comparing `invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/ca/LC_MESSAGES/messages.mo` & `invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/ca/LC_MESSAGES/messages.mo`

 * *Files 2% similar despite different names*

#### msgunfmt {}

```diff
@@ -2,15 +2,15 @@
 msgstr ""
 "Project-Id-Version: invenio-drafts-resources 0.18.2\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:07+0000\n"
 "PO-Revision-Date: 2021-07-13 12:40+0000\n"
 "Last-Translator: Ferran Jorba <Ferran.Jorba@uab.cat>, 2021\n"
 "Language: ca\n"
-"Language-Team: Catalan (https://www.transifex.com/inveniosoftware/"
+"Language-Team: Catalan (https://app.transifex.com/inveniosoftware/"
 "teams/23537/ca/)\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.12.1\n"
```

### Comparing `invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/ca/LC_MESSAGES/messages.po` & `invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/ca/LC_MESSAGES/messages.po`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-drafts-resources 0.18.2\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:07+0000\n"
 "PO-Revision-Date: 2021-07-13 12:40+0000\n"
 "Last-Translator: Ferran Jorba <Ferran.Jorba@uab.cat>, 2021\n"
-"Language-Team: Catalan (https://www.transifex.com/inveniosoftware/teams/23537/ca/)\n"
+"Language-Team: Catalan (https://app.transifex.com/inveniosoftware/teams/23537/ca/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.3\n"
 "Language: ca\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
```

### Comparing `invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/cs/LC_MESSAGES/messages.mo` & `invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/es_MX/LC_MESSAGES/messages.mo`

 * *Files 20% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,19 +0,0 @@
-msgid ""
-msgstr ""
-"Project-Id-Version: invenio-drafts-resources 0.18.2\n"
-"Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
-"POT-Creation-Date: 2022-10-12 09:07+0000\n"
-"PO-Revision-Date: 2021-07-13 12:40+0000\n"
-"Last-Translator: Ivan Masár <helix84@centrum.sk>, 2021\n"
-"Language: cs\n"
-"Language-Team: Czech (https://www.transifex.com/inveniosoftware/teams/23537/"
-"cs/)\n"
-"Plural-Forms: nplurals=4; plural=(n == 1 && n % 1 == 0) ? 0 : (n >= 2 && n "
-"<= 4 && n % 1 == 0) ? 1: (n % 1 != 0 ) ? 2 : 3;\n"
-"MIME-Version: 1.0\n"
-"Content-Type: text/plain; charset=utf-8\n"
-"Content-Transfer-Encoding: 8bit\n"
-"Generated-By: Babel 2.12.1\n"
-
-msgid "Version"
-msgstr "Verze"
```

### Comparing `invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/cs/LC_MESSAGES/messages.po` & `invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/cs/LC_MESSAGES/messages.po`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-drafts-resources 0.18.2\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:07+0000\n"
 "PO-Revision-Date: 2021-07-13 12:40+0000\n"
 "Last-Translator: Ivan Masár <helix84@centrum.sk>, 2021\n"
-"Language-Team: Czech (https://www.transifex.com/inveniosoftware/teams/23537/cs/)\n"
+"Language-Team: Czech (https://app.transifex.com/inveniosoftware/teams/23537/cs/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.3\n"
 "Language: cs\n"
 "Plural-Forms: nplurals=4; plural=(n == 1 && n % 1 == 0) ? 0 : (n >= 2 && n <= 4 && n % 1 == 0) ? 1: (n % 1 != 0 ) ? 2 : 3;\n"
```

### Comparing `invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/da/LC_MESSAGES/messages.mo` & `invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/da/LC_MESSAGES/messages.mo`

 * *Format-specific differences are supported for Gettext message catalogues but no file-specific differences were detected; falling back to a binary diff. file(1) reports: GNU message catalog (little endian), revision 0.0, 1 message, Project-Id-Version: invenio-drafts-resources 0.18.2*

 * *Files 3% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 000000c0: 7369 6f6e 2d44 6174 653a 2032 3032 312d  sion-Date: 2021-
 000000d0: 3037 2d31 3320 3132 3a34 302b 3030 3030  07-13 12:40+0000
 000000e0: 0a4c 6173 742d 5472 616e 736c 6174 6f72  .Last-Translator
 000000f0: 3a20 4655 4c4c 204e 414d 4520 3c45 4d41  : FULL NAME <EMA
 00000100: 494c 4041 4444 5245 5353 3e0a 4c61 6e67  IL@ADDRESS>.Lang
 00000110: 7561 6765 3a20 6461 0a4c 616e 6775 6167  uage: da.Languag
 00000120: 652d 5465 616d 3a20 4461 6e69 7368 2028  e-Team: Danish (
-00000130: 6874 7470 733a 2f2f 7777 772e 7472 616e  https://www.tran
+00000130: 6874 7470 733a 2f2f 6170 702e 7472 616e  https://app.tran
 00000140: 7369 6665 782e 636f 6d2f 696e 7665 6e69  sifex.com/inveni
 00000150: 6f73 6f66 7477 6172 652f 7465 616d 732f  osoftware/teams/
 00000160: 3233 3533 372f 6461 2f29 0a50 6c75 7261  23537/da/).Plura
 00000170: 6c2d 466f 726d 733a 206e 706c 7572 616c  l-Forms: nplural
 00000180: 733d 323b 2070 6c75 7261 6c3d 286e 2021  s=2; plural=(n !
 00000190: 3d20 3129 3b0a 4d49 4d45 2d56 6572 7369  = 1);.MIME-Versi
 000001a0: 6f6e 3a20 312e 300a 436f 6e74 656e 742d  on: 1.0.Content-
```

### Comparing `invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/da/LC_MESSAGES/messages.po` & `invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/da/LC_MESSAGES/messages.po`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-drafts-resources 0.18.2\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:07+0000\n"
 "PO-Revision-Date: 2021-07-13 12:40+0000\n"
-"Language-Team: Danish (https://www.transifex.com/inveniosoftware/teams/23537/da/)\n"
+"Language-Team: Danish (https://app.transifex.com/inveniosoftware/teams/23537/da/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.3\n"
 "Language: da\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
```

### Comparing `invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/de/LC_MESSAGES/messages.mo` & `invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/de/LC_MESSAGES/messages.mo`

 * *Files 1% similar despite different names*

#### msgunfmt {}

```diff
@@ -2,15 +2,15 @@
 msgstr ""
 "Project-Id-Version: invenio-drafts-resources 0.18.2\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:07+0000\n"
 "PO-Revision-Date: 2021-07-13 12:40+0000\n"
 "Last-Translator: chriz_uniba <christina.zeller@uni-bamberg.de>, 2022\n"
 "Language: de\n"
-"Language-Team: German (https://www.transifex.com/inveniosoftware/teams/23537/"
+"Language-Team: German (https://app.transifex.com/inveniosoftware/teams/23537/"
 "de/)\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.12.1\n"
```

### Comparing `invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/de/LC_MESSAGES/messages.po` & `invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/de/LC_MESSAGES/messages.po`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-drafts-resources 0.18.2\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:07+0000\n"
 "PO-Revision-Date: 2021-07-13 12:40+0000\n"
 "Last-Translator: chriz_uniba <christina.zeller@uni-bamberg.de>, 2022\n"
-"Language-Team: German (https://www.transifex.com/inveniosoftware/teams/23537/de/)\n"
+"Language-Team: German (https://app.transifex.com/inveniosoftware/teams/23537/de/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.3\n"
 "Language: de\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
```

### Comparing `invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/el/LC_MESSAGES/messages.mo` & `invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/el/LC_MESSAGES/messages.mo`

 * *Format-specific differences are supported for Gettext message catalogues but no file-specific differences were detected; falling back to a binary diff. file(1) reports: GNU message catalog (little endian), revision 0.0, 1 message, Project-Id-Version: invenio-drafts-resources 0.18.2*

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 000000c0: 7369 6f6e 2d44 6174 653a 2032 3032 312d  sion-Date: 2021-
 000000d0: 3037 2d31 3320 3132 3a34 302b 3030 3030  07-13 12:40+0000
 000000e0: 0a4c 6173 742d 5472 616e 736c 6174 6f72  .Last-Translator
 000000f0: 3a20 4655 4c4c 204e 414d 4520 3c45 4d41  : FULL NAME <EMA
 00000100: 494c 4041 4444 5245 5353 3e0a 4c61 6e67  IL@ADDRESS>.Lang
 00000110: 7561 6765 3a20 656c 0a4c 616e 6775 6167  uage: el.Languag
 00000120: 652d 5465 616d 3a20 4772 6565 6b20 2868  e-Team: Greek (h
-00000130: 7474 7073 3a2f 2f77 7777 2e74 7261 6e73  ttps://www.trans
+00000130: 7474 7073 3a2f 2f61 7070 2e74 7261 6e73  ttps://app.trans
 00000140: 6966 6578 2e63 6f6d 2f69 6e76 656e 696f  ifex.com/invenio
 00000150: 736f 6674 7761 7265 2f74 6561 6d73 2f32  software/teams/2
 00000160: 3335 3337 2f65 6c2f 290a 506c 7572 616c  3537/el/).Plural
 00000170: 2d46 6f72 6d73 3a20 6e70 6c75 7261 6c73  -Forms: nplurals
 00000180: 3d32 3b20 706c 7572 616c 3d28 6e20 213d  =2; plural=(n !=
 00000190: 2031 293b 0a4d 494d 452d 5665 7273 696f   1);.MIME-Versio
 000001a0: 6e3a 2031 2e30 0a43 6f6e 7465 6e74 2d54  n: 1.0.Content-T
```

### Comparing `invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/el/LC_MESSAGES/messages.po` & `invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/zh_TW/LC_MESSAGES/messages.po`

 * *Files 2% similar despite different names*

```diff
@@ -7,21 +7,21 @@
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-drafts-resources 0.18.2\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:07+0000\n"
 "PO-Revision-Date: 2021-07-13 12:40+0000\n"
-"Language-Team: Greek (https://www.transifex.com/inveniosoftware/teams/23537/el/)\n"
+"Language-Team: Chinese (Taiwan) (https://app.transifex.com/inveniosoftware/teams/23537/zh_TW/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.3\n"
-"Language: el\n"
-"Plural-Forms: nplurals=2; plural=(n != 1);\n"
+"Language: zh_TW\n"
+"Plural-Forms: nplurals=1; plural=0;\n"
 
 #: invenio_drafts_resources/services/records/config.py:42
 #: invenio_drafts_resources/services/records/config.py:71
 msgid "Best match"
 msgstr ""
 
 #: invenio_drafts_resources/services/records/config.py:46
```

### Comparing `invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/es/LC_MESSAGES/messages.mo` & `invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/es/LC_MESSAGES/messages.mo`

 * *Files 19% similar despite different names*

#### msgunfmt {}

```diff
@@ -2,15 +2,15 @@
 msgstr ""
 "Project-Id-Version: invenio-drafts-resources 0.18.2\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:07+0000\n"
 "PO-Revision-Date: 2021-07-13 12:40+0000\n"
 "Last-Translator: Jesús Martín <jesusmartin@sallep.net>, 2021\n"
 "Language: es\n"
-"Language-Team: Spanish (https://www.transifex.com/inveniosoftware/"
+"Language-Team: Spanish (https://app.transifex.com/inveniosoftware/"
 "teams/23537/es/)\n"
 "Plural-Forms: nplurals=3; plural=n == 1 ? 0 : n != 0 && n % 1000000 == 0 ? "
 "1 : 2;\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.12.1\n"
```

### Comparing `invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/es/LC_MESSAGES/messages.po` & `invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/es/LC_MESSAGES/messages.po`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-drafts-resources 0.18.2\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:07+0000\n"
 "PO-Revision-Date: 2021-07-13 12:40+0000\n"
 "Last-Translator: Jesús Martín <jesusmartin@sallep.net>, 2021\n"
-"Language-Team: Spanish (https://www.transifex.com/inveniosoftware/teams/23537/es/)\n"
+"Language-Team: Spanish (https://app.transifex.com/inveniosoftware/teams/23537/es/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.3\n"
 "Language: es\n"
 "Plural-Forms: nplurals=3; plural=n == 1 ? 0 : n != 0 && n % 1000000 == 0 ? 1 : 2;\n"
```

### Comparing `invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/et/LC_MESSAGES/messages.mo` & `invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/et/LC_MESSAGES/messages.mo`

 * *Files 2% similar despite different names*

#### msgunfmt {}

```diff
@@ -2,15 +2,15 @@
 msgstr ""
 "Project-Id-Version: invenio-drafts-resources 0.18.2\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:07+0000\n"
 "PO-Revision-Date: 2021-07-13 12:40+0000\n"
 "Last-Translator: Martin Jantson <martinjantson97@gmail.com>, 2022\n"
 "Language: et\n"
-"Language-Team: Estonian (https://www.transifex.com/inveniosoftware/"
+"Language-Team: Estonian (https://app.transifex.com/inveniosoftware/"
 "teams/23537/et/)\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.12.1\n"
```

### Comparing `invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/et/LC_MESSAGES/messages.po` & `invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/et/LC_MESSAGES/messages.po`

 * *Files 4% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-drafts-resources 0.18.2\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:07+0000\n"
 "PO-Revision-Date: 2021-07-13 12:40+0000\n"
 "Last-Translator: Martin Jantson <martinjantson97@gmail.com>, 2022\n"
-"Language-Team: Estonian (https://www.transifex.com/inveniosoftware/teams/23537/et/)\n"
+"Language-Team: Estonian (https://app.transifex.com/inveniosoftware/teams/23537/et/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.3\n"
 "Language: et\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
```

### Comparing `invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/et_EE/LC_MESSAGES/messages.mo` & `invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/hi_IN/LC_MESSAGES/messages.mo`

 * *Format-specific differences are supported for Gettext message catalogues but no file-specific differences were detected; falling back to a binary diff. file(1) reports: GNU message catalog (little endian), revision 0.0, 1 message, Project-Id-Version: invenio-drafts-resources 0.18.2*

 * *Files 11% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 00000000: de12 0495 0000 0000 0100 0000 1c00 0000  ................
 00000010: 2400 0000 0000 0000 0000 0000 0000 0000  $...............
-00000020: 2c00 0000 f001 0000 2d00 0000 0050 726f  ,.......-....Pro
+00000020: 2c00 0000 eb01 0000 2d00 0000 0050 726f  ,.......-....Pro
 00000030: 6a65 6374 2d49 642d 5665 7273 696f 6e3a  ject-Id-Version:
 00000040: 2069 6e76 656e 696f 2d64 7261 6674 732d   invenio-drafts-
 00000050: 7265 736f 7572 6365 7320 302e 3138 2e32  resources 0.18.2
 00000060: 0a52 6570 6f72 742d 4d73 6769 642d 4275  .Report-Msgid-Bu
 00000070: 6773 2d54 6f3a 2069 6e66 6f40 696e 7665  gs-To: info@inve
 00000080: 6e69 6f73 6f66 7477 6172 652e 6f72 670a  niosoftware.org.
 00000090: 504f 542d 4372 6561 7469 6f6e 2d44 6174  POT-Creation-Dat
 000000a0: 653a 2032 3032 322d 3130 2d31 3220 3039  e: 2022-10-12 09
 000000b0: 3a30 372b 3030 3030 0a50 4f2d 5265 7669  :07+0000.PO-Revi
 000000c0: 7369 6f6e 2d44 6174 653a 2032 3032 312d  sion-Date: 2021-
 000000d0: 3037 2d31 3320 3132 3a34 302b 3030 3030  07-13 12:40+0000
 000000e0: 0a4c 6173 742d 5472 616e 736c 6174 6f72  .Last-Translator
 000000f0: 3a20 4655 4c4c 204e 414d 4520 3c45 4d41  : FULL NAME <EMA
 00000100: 494c 4041 4444 5245 5353 3e0a 4c61 6e67  IL@ADDRESS>.Lang
-00000110: 7561 6765 3a20 6574 5f45 450a 4c61 6e67  uage: et_EE.Lang
-00000120: 7561 6765 2d54 6561 6d3a 2045 7374 6f6e  uage-Team: Eston
-00000130: 6961 6e20 2845 7374 6f6e 6961 2920 2868  ian (Estonia) (h
-00000140: 7474 7073 3a2f 2f77 7777 2e74 7261 6e73  ttps://www.trans
-00000150: 6966 6578 2e63 6f6d 2f69 6e76 656e 696f  ifex.com/invenio
-00000160: 736f 6674 7761 7265 2f74 6561 6d73 2f32  software/teams/2
-00000170: 3335 3337 2f65 745f 4545 2f29 0a50 6c75  3537/et_EE/).Plu
-00000180: 7261 6c2d 466f 726d 733a 206e 706c 7572  ral-Forms: nplur
-00000190: 616c 733d 323b 2070 6c75 7261 6c3d 286e  als=2; plural=(n
-000001a0: 2021 3d20 3129 3b0a 4d49 4d45 2d56 6572   != 1);.MIME-Ver
-000001b0: 7369 6f6e 3a20 312e 300a 436f 6e74 656e  sion: 1.0.Conten
-000001c0: 742d 5479 7065 3a20 7465 7874 2f70 6c61  t-Type: text/pla
-000001d0: 696e 3b20 6368 6172 7365 743d 7574 662d  in; charset=utf-
-000001e0: 380a 436f 6e74 656e 742d 5472 616e 7366  8.Content-Transf
-000001f0: 6572 2d45 6e63 6f64 696e 673a 2038 6269  er-Encoding: 8bi
-00000200: 740a 4765 6e65 7261 7465 642d 4279 3a20  t.Generated-By: 
-00000210: 4261 6265 6c20 322e 3132 2e31 0a00       Babel 2.12.1..
+00000110: 7561 6765 3a20 6869 5f49 4e0a 4c61 6e67  uage: hi_IN.Lang
+00000120: 7561 6765 2d54 6561 6d3a 2048 696e 6469  uage-Team: Hindi
+00000130: 2028 496e 6469 6129 2028 6874 7470 733a   (India) (https:
+00000140: 2f2f 6170 702e 7472 616e 7369 6665 782e  //app.transifex.
+00000150: 636f 6d2f 696e 7665 6e69 6f73 6f66 7477  com/inveniosoftw
+00000160: 6172 652f 7465 616d 732f 3233 3533 372f  are/teams/23537/
+00000170: 6869 5f49 4e2f 290a 506c 7572 616c 2d46  hi_IN/).Plural-F
+00000180: 6f72 6d73 3a20 6e70 6c75 7261 6c73 3d32  orms: nplurals=2
+00000190: 3b20 706c 7572 616c 3d28 6e20 213d 2031  ; plural=(n != 1
+000001a0: 293b 0a4d 494d 452d 5665 7273 696f 6e3a  );.MIME-Version:
+000001b0: 2031 2e30 0a43 6f6e 7465 6e74 2d54 7970   1.0.Content-Typ
+000001c0: 653a 2074 6578 742f 706c 6169 6e3b 2063  e: text/plain; c
+000001d0: 6861 7273 6574 3d75 7466 2d38 0a43 6f6e  harset=utf-8.Con
+000001e0: 7465 6e74 2d54 7261 6e73 6665 722d 456e  tent-Transfer-En
+000001f0: 636f 6469 6e67 3a20 3862 6974 0a47 656e  coding: 8bit.Gen
+00000200: 6572 6174 6564 2d42 793a 2042 6162 656c  erated-By: Babel
+00000210: 2032 2e31 322e 310a 00                    2.12.1..
```

### Comparing `invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/et_EE/LC_MESSAGES/messages.po` & `invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/de_AT/LC_MESSAGES/messages.po`

 * *Files 2% similar despite different names*

```diff
@@ -7,20 +7,20 @@
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-drafts-resources 0.18.2\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:07+0000\n"
 "PO-Revision-Date: 2021-07-13 12:40+0000\n"
-"Language-Team: Estonian (Estonia) (https://www.transifex.com/inveniosoftware/teams/23537/et_EE/)\n"
+"Language-Team: German (Austria) (https://app.transifex.com/inveniosoftware/teams/23537/de_AT/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.3\n"
-"Language: et_EE\n"
+"Language: de_AT\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
 #: invenio_drafts_resources/services/records/config.py:42
 #: invenio_drafts_resources/services/records/config.py:71
 msgid "Best match"
 msgstr ""
```

### Comparing `invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/fa/LC_MESSAGES/messages.mo` & `invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/fa/LC_MESSAGES/messages.mo`

 * *Format-specific differences are supported for Gettext message catalogues but no file-specific differences were detected; falling back to a binary diff. file(1) reports: GNU message catalog (little endian), revision 0.0, 1 message, Project-Id-Version: invenio-drafts-resources 0.18.2*

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 000000c0: 7369 6f6e 2d44 6174 653a 2032 3032 312d  sion-Date: 2021-
 000000d0: 3037 2d31 3320 3132 3a34 302b 3030 3030  07-13 12:40+0000
 000000e0: 0a4c 6173 742d 5472 616e 736c 6174 6f72  .Last-Translator
 000000f0: 3a20 4655 4c4c 204e 414d 4520 3c45 4d41  : FULL NAME <EMA
 00000100: 494c 4041 4444 5245 5353 3e0a 4c61 6e67  IL@ADDRESS>.Lang
 00000110: 7561 6765 3a20 6661 0a4c 616e 6775 6167  uage: fa.Languag
 00000120: 652d 5465 616d 3a20 5065 7273 6961 6e20  e-Team: Persian 
-00000130: 2868 7474 7073 3a2f 2f77 7777 2e74 7261  (https://www.tra
+00000130: 2868 7474 7073 3a2f 2f61 7070 2e74 7261  (https://app.tra
 00000140: 6e73 6966 6578 2e63 6f6d 2f69 6e76 656e  nsifex.com/inven
 00000150: 696f 736f 6674 7761 7265 2f74 6561 6d73  iosoftware/teams
 00000160: 2f32 3335 3337 2f66 612f 290a 506c 7572  /23537/fa/).Plur
 00000170: 616c 2d46 6f72 6d73 3a20 6e70 6c75 7261  al-Forms: nplura
 00000180: 6c73 3d32 3b20 706c 7572 616c 3d28 6e20  ls=2; plural=(n 
 00000190: 3e20 3129 3b0a 4d49 4d45 2d56 6572 7369  > 1);.MIME-Versi
 000001a0: 6f6e 3a20 312e 300a 436f 6e74 656e 742d  on: 1.0.Content-
```

### Comparing `invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/fa/LC_MESSAGES/messages.po` & `invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/fa/LC_MESSAGES/messages.po`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-drafts-resources 0.18.2\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:07+0000\n"
 "PO-Revision-Date: 2021-07-13 12:40+0000\n"
-"Language-Team: Persian (https://www.transifex.com/inveniosoftware/teams/23537/fa/)\n"
+"Language-Team: Persian (https://app.transifex.com/inveniosoftware/teams/23537/fa/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.3\n"
 "Language: fa\n"
 "Plural-Forms: nplurals=2; plural=(n > 1);\n"
```

### Comparing `invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/fr/LC_MESSAGES/messages.mo` & `invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/fr/LC_MESSAGES/messages.mo`

 * *Files 2% similar despite different names*

#### msgunfmt {}

```diff
@@ -2,15 +2,15 @@
 msgstr ""
 "Project-Id-Version: invenio-drafts-resources 0.18.2\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:07+0000\n"
 "PO-Revision-Date: 2021-07-13 12:40+0000\n"
 "Last-Translator: Alizee Pace <alizee.pace@gmail.com>, 2021\n"
 "Language: fr\n"
-"Language-Team: French (https://www.transifex.com/inveniosoftware/teams/23537/"
+"Language-Team: French (https://app.transifex.com/inveniosoftware/teams/23537/"
 "fr/)\n"
 "Plural-Forms: nplurals=3; plural=(n == 0 || n == 1) ? 0 : n != 0 && n % "
 "1000000 == 0 ? 1 : 2;\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.12.1\n"
```

### Comparing `invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/fr/LC_MESSAGES/messages.po` & `invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/fr/LC_MESSAGES/messages.po`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-drafts-resources 0.18.2\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:07+0000\n"
 "PO-Revision-Date: 2021-07-13 12:40+0000\n"
 "Last-Translator: Alizee Pace <alizee.pace@gmail.com>, 2021\n"
-"Language-Team: French (https://www.transifex.com/inveniosoftware/teams/23537/fr/)\n"
+"Language-Team: French (https://app.transifex.com/inveniosoftware/teams/23537/fr/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.3\n"
 "Language: fr\n"
 "Plural-Forms: nplurals=3; plural=(n == 0 || n == 1) ? 0 : n != 0 && n % 1000000 == 0 ? 1 : 2;\n"
```

### Comparing `invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/gl/LC_MESSAGES/messages.mo` & `invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/gl/LC_MESSAGES/messages.mo`

 * *Format-specific differences are supported for Gettext message catalogues but no file-specific differences were detected; falling back to a binary diff. file(1) reports: GNU message catalog (little endian), revision 0.0, 1 message, Project-Id-Version: invenio-drafts-resources 0.18.2*

 * *Files 4% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 000000c0: 7369 6f6e 2d44 6174 653a 2032 3032 312d  sion-Date: 2021-
 000000d0: 3037 2d31 3320 3132 3a34 302b 3030 3030  07-13 12:40+0000
 000000e0: 0a4c 6173 742d 5472 616e 736c 6174 6f72  .Last-Translator
 000000f0: 3a20 4655 4c4c 204e 414d 4520 3c45 4d41  : FULL NAME <EMA
 00000100: 494c 4041 4444 5245 5353 3e0a 4c61 6e67  IL@ADDRESS>.Lang
 00000110: 7561 6765 3a20 676c 0a4c 616e 6775 6167  uage: gl.Languag
 00000120: 652d 5465 616d 3a20 4761 6c69 6369 616e  e-Team: Galician
-00000130: 2028 6874 7470 733a 2f2f 7777 772e 7472   (https://www.tr
+00000130: 2028 6874 7470 733a 2f2f 6170 702e 7472   (https://app.tr
 00000140: 616e 7369 6665 782e 636f 6d2f 696e 7665  ansifex.com/inve
 00000150: 6e69 6f73 6f66 7477 6172 652f 7465 616d  niosoftware/team
 00000160: 732f 3233 3533 372f 676c 2f29 0a50 6c75  s/23537/gl/).Plu
 00000170: 7261 6c2d 466f 726d 733a 206e 706c 7572  ral-Forms: nplur
 00000180: 616c 733d 323b 2070 6c75 7261 6c3d 286e  als=2; plural=(n
 00000190: 2021 3d20 3129 3b0a 4d49 4d45 2d56 6572   != 1);.MIME-Ver
 000001a0: 7369 6f6e 3a20 312e 300a 436f 6e74 656e  sion: 1.0.Conten
```

### Comparing `invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/gl/LC_MESSAGES/messages.po` & `invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/gl/LC_MESSAGES/messages.po`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-drafts-resources 0.18.2\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:07+0000\n"
 "PO-Revision-Date: 2021-07-13 12:40+0000\n"
-"Language-Team: Galician (https://www.transifex.com/inveniosoftware/teams/23537/gl/)\n"
+"Language-Team: Galician (https://app.transifex.com/inveniosoftware/teams/23537/gl/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.3\n"
 "Language: gl\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
```

### Comparing `invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/hr/LC_MESSAGES/messages.mo` & `invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/hr/LC_MESSAGES/messages.mo`

 * *Format-specific differences are supported for Gettext message catalogues but no file-specific differences were detected; falling back to a binary diff. file(1) reports: GNU message catalog (little endian), revision 0.0, 1 message, Project-Id-Version: invenio-drafts-resources 0.18.2*

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 000000c0: 7369 6f6e 2d44 6174 653a 2032 3032 312d  sion-Date: 2021-
 000000d0: 3037 2d31 3320 3132 3a34 302b 3030 3030  07-13 12:40+0000
 000000e0: 0a4c 6173 742d 5472 616e 736c 6174 6f72  .Last-Translator
 000000f0: 3a20 4655 4c4c 204e 414d 4520 3c45 4d41  : FULL NAME <EMA
 00000100: 494c 4041 4444 5245 5353 3e0a 4c61 6e67  IL@ADDRESS>.Lang
 00000110: 7561 6765 3a20 6872 0a4c 616e 6775 6167  uage: hr.Languag
 00000120: 652d 5465 616d 3a20 4372 6f61 7469 616e  e-Team: Croatian
-00000130: 2028 6874 7470 733a 2f2f 7777 772e 7472   (https://www.tr
+00000130: 2028 6874 7470 733a 2f2f 6170 702e 7472   (https://app.tr
 00000140: 616e 7369 6665 782e 636f 6d2f 696e 7665  ansifex.com/inve
 00000150: 6e69 6f73 6f66 7477 6172 652f 7465 616d  niosoftware/team
 00000160: 732f 3233 3533 372f 6872 2f29 0a50 6c75  s/23537/hr/).Plu
 00000170: 7261 6c2d 466f 726d 733a 206e 706c 7572  ral-Forms: nplur
 00000180: 616c 733d 333b 2070 6c75 7261 6c3d 6e25  als=3; plural=n%
 00000190: 3130 3d3d 3120 2626 206e 2531 3030 213d  10==1 && n%100!=
 000001a0: 3131 203f 2030 203a 206e 2531 303e 3d32  11 ? 0 : n%10>=2
```

### Comparing `invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/hr/LC_MESSAGES/messages.po` & `invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/hr/LC_MESSAGES/messages.po`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-drafts-resources 0.18.2\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:07+0000\n"
 "PO-Revision-Date: 2021-07-13 12:40+0000\n"
-"Language-Team: Croatian (https://www.transifex.com/inveniosoftware/teams/23537/hr/)\n"
+"Language-Team: Croatian (https://app.transifex.com/inveniosoftware/teams/23537/hr/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.3\n"
 "Language: hr\n"
 "Plural-Forms: nplurals=3; plural=n%10==1 && n%100!=11 ? 0 : n%10>=2 && n%10<=4 && (n%100<10 || n%100>=20) ? 1 : 2;\n"
```

### Comparing `invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/hu/LC_MESSAGES/messages.mo` & `invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/hu/LC_MESSAGES/messages.mo`

 * *Files 10% similar despite different names*

#### msgunfmt {}

```diff
@@ -2,15 +2,15 @@
 msgstr ""
 "Project-Id-Version: invenio-drafts-resources 0.18.2\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:07+0000\n"
 "PO-Revision-Date: 2021-07-13 12:40+0000\n"
 "Last-Translator: Andrea Dömötör, 2022\n"
 "Language: hu\n"
-"Language-Team: Hungarian (https://www.transifex.com/inveniosoftware/"
+"Language-Team: Hungarian (https://app.transifex.com/inveniosoftware/"
 "teams/23537/hu/)\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.12.1\n"
```

### Comparing `invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/hu/LC_MESSAGES/messages.po` & `invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/hu/LC_MESSAGES/messages.po`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-drafts-resources 0.18.2\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:07+0000\n"
 "PO-Revision-Date: 2021-07-13 12:40+0000\n"
 "Last-Translator: Andrea Dömötör, 2022\n"
-"Language-Team: Hungarian (https://www.transifex.com/inveniosoftware/teams/23537/hu/)\n"
+"Language-Team: Hungarian (https://app.transifex.com/inveniosoftware/teams/23537/hu/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.3\n"
 "Language: hu\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
```

### Comparing `invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/it/LC_MESSAGES/messages.mo` & `invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/it/LC_MESSAGES/messages.mo`

 * *Files 2% similar despite different names*

#### msgunfmt {}

```diff
@@ -2,15 +2,15 @@
 msgstr ""
 "Project-Id-Version: invenio-drafts-resources 0.18.2\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:07+0000\n"
 "PO-Revision-Date: 2021-07-13 12:40+0000\n"
 "Last-Translator: Alizee Pace <alizee.pace@gmail.com>, 2021\n"
 "Language: it\n"
-"Language-Team: Italian (https://www.transifex.com/inveniosoftware/"
+"Language-Team: Italian (https://app.transifex.com/inveniosoftware/"
 "teams/23537/it/)\n"
 "Plural-Forms: nplurals=3; plural=n == 1 ? 0 : n != 0 && n % 1000000 == 0 ? "
 "1 : 2;\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.12.1\n"
```

### Comparing `invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/it/LC_MESSAGES/messages.po` & `invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/it/LC_MESSAGES/messages.po`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-drafts-resources 0.18.2\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:07+0000\n"
 "PO-Revision-Date: 2021-07-13 12:40+0000\n"
 "Last-Translator: Alizee Pace <alizee.pace@gmail.com>, 2021\n"
-"Language-Team: Italian (https://www.transifex.com/inveniosoftware/teams/23537/it/)\n"
+"Language-Team: Italian (https://app.transifex.com/inveniosoftware/teams/23537/it/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.3\n"
 "Language: it\n"
 "Plural-Forms: nplurals=3; plural=n == 1 ? 0 : n != 0 && n % 1000000 == 0 ? 1 : 2;\n"
```

### Comparing `invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/ja/LC_MESSAGES/messages.mo` & `invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/ja/LC_MESSAGES/messages.mo`

 * *Format-specific differences are supported for Gettext message catalogues but no file-specific differences were detected; falling back to a binary diff. file(1) reports: GNU message catalog (little endian), revision 0.0, 1 message, Project-Id-Version: invenio-drafts-resources 0.18.2*

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 000000c0: 7369 6f6e 2d44 6174 653a 2032 3032 312d  sion-Date: 2021-
 000000d0: 3037 2d31 3320 3132 3a34 302b 3030 3030  07-13 12:40+0000
 000000e0: 0a4c 6173 742d 5472 616e 736c 6174 6f72  .Last-Translator
 000000f0: 3a20 4655 4c4c 204e 414d 4520 3c45 4d41  : FULL NAME <EMA
 00000100: 494c 4041 4444 5245 5353 3e0a 4c61 6e67  IL@ADDRESS>.Lang
 00000110: 7561 6765 3a20 6a61 0a4c 616e 6775 6167  uage: ja.Languag
 00000120: 652d 5465 616d 3a20 4a61 7061 6e65 7365  e-Team: Japanese
-00000130: 2028 6874 7470 733a 2f2f 7777 772e 7472   (https://www.tr
+00000130: 2028 6874 7470 733a 2f2f 6170 702e 7472   (https://app.tr
 00000140: 616e 7369 6665 782e 636f 6d2f 696e 7665  ansifex.com/inve
 00000150: 6e69 6f73 6f66 7477 6172 652f 7465 616d  niosoftware/team
 00000160: 732f 3233 3533 372f 6a61 2f29 0a50 6c75  s/23537/ja/).Plu
 00000170: 7261 6c2d 466f 726d 733a 206e 706c 7572  ral-Forms: nplur
 00000180: 616c 733d 313b 2070 6c75 7261 6c3d 303b  als=1; plural=0;
 00000190: 0a4d 494d 452d 5665 7273 696f 6e3a 2031  .MIME-Version: 1
 000001a0: 2e30 0a43 6f6e 7465 6e74 2d54 7970 653a  .0.Content-Type:
```

### Comparing `invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/ja/LC_MESSAGES/messages.po` & `invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/ja/LC_MESSAGES/messages.po`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-drafts-resources 0.18.2\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:07+0000\n"
 "PO-Revision-Date: 2021-07-13 12:40+0000\n"
-"Language-Team: Japanese (https://www.transifex.com/inveniosoftware/teams/23537/ja/)\n"
+"Language-Team: Japanese (https://app.transifex.com/inveniosoftware/teams/23537/ja/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.3\n"
 "Language: ja\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
```

### Comparing `invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/ka/LC_MESSAGES/messages.mo` & `invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/ka/LC_MESSAGES/messages.mo`

 * *Format-specific differences are supported for Gettext message catalogues but no file-specific differences were detected; falling back to a binary diff. file(1) reports: GNU message catalog (little endian), revision 0.0, 1 message, Project-Id-Version: invenio-drafts-resources 0.18.2*

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 000000c0: 7369 6f6e 2d44 6174 653a 2032 3032 312d  sion-Date: 2021-
 000000d0: 3037 2d31 3320 3132 3a34 302b 3030 3030  07-13 12:40+0000
 000000e0: 0a4c 6173 742d 5472 616e 736c 6174 6f72  .Last-Translator
 000000f0: 3a20 4655 4c4c 204e 414d 4520 3c45 4d41  : FULL NAME <EMA
 00000100: 494c 4041 4444 5245 5353 3e0a 4c61 6e67  IL@ADDRESS>.Lang
 00000110: 7561 6765 3a20 6b61 0a4c 616e 6775 6167  uage: ka.Languag
 00000120: 652d 5465 616d 3a20 4765 6f72 6769 616e  e-Team: Georgian
-00000130: 2028 6874 7470 733a 2f2f 7777 772e 7472   (https://www.tr
+00000130: 2028 6874 7470 733a 2f2f 6170 702e 7472   (https://app.tr
 00000140: 616e 7369 6665 782e 636f 6d2f 696e 7665  ansifex.com/inve
 00000150: 6e69 6f73 6f66 7477 6172 652f 7465 616d  niosoftware/team
 00000160: 732f 3233 3533 372f 6b61 2f29 0a50 6c75  s/23537/ka/).Plu
 00000170: 7261 6c2d 466f 726d 733a 206e 706c 7572  ral-Forms: nplur
 00000180: 616c 733d 323b 2070 6c75 7261 6c3d 286e  als=2; plural=(n
 00000190: 213d 3129 3b0a 4d49 4d45 2d56 6572 7369  !=1);.MIME-Versi
 000001a0: 6f6e 3a20 312e 300a 436f 6e74 656e 742d  on: 1.0.Content-
```

### Comparing `invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/ka/LC_MESSAGES/messages.po` & `invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/no/LC_MESSAGES/messages.po`

 * *Files 2% similar despite different names*

```diff
@@ -7,21 +7,21 @@
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-drafts-resources 0.18.2\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:07+0000\n"
 "PO-Revision-Date: 2021-07-13 12:40+0000\n"
-"Language-Team: Georgian (https://www.transifex.com/inveniosoftware/teams/23537/ka/)\n"
+"Language-Team: Norwegian (https://app.transifex.com/inveniosoftware/teams/23537/no/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.3\n"
-"Language: ka\n"
-"Plural-Forms: nplurals=2; plural=(n!=1);\n"
+"Language: no\n"
+"Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
 #: invenio_drafts_resources/services/records/config.py:42
 #: invenio_drafts_resources/services/records/config.py:71
 msgid "Best match"
 msgstr ""
 
 #: invenio_drafts_resources/services/records/config.py:46
```

### Comparing `invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/lt/LC_MESSAGES/messages.mo` & `invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/lt/LC_MESSAGES/messages.mo`

 * *Format-specific differences are supported for Gettext message catalogues but no file-specific differences were detected; falling back to a binary diff. file(1) reports: GNU message catalog (little endian), revision 0.0, 1 message, Project-Id-Version: invenio-drafts-resources 0.18.2*

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 000000c0: 7369 6f6e 2d44 6174 653a 2032 3032 312d  sion-Date: 2021-
 000000d0: 3037 2d31 3320 3132 3a34 302b 3030 3030  07-13 12:40+0000
 000000e0: 0a4c 6173 742d 5472 616e 736c 6174 6f72  .Last-Translator
 000000f0: 3a20 4655 4c4c 204e 414d 4520 3c45 4d41  : FULL NAME <EMA
 00000100: 494c 4041 4444 5245 5353 3e0a 4c61 6e67  IL@ADDRESS>.Lang
 00000110: 7561 6765 3a20 6c74 0a4c 616e 6775 6167  uage: lt.Languag
 00000120: 652d 5465 616d 3a20 4c69 7468 7561 6e69  e-Team: Lithuani
-00000130: 616e 2028 6874 7470 733a 2f2f 7777 772e  an (https://www.
+00000130: 616e 2028 6874 7470 733a 2f2f 6170 702e  an (https://app.
 00000140: 7472 616e 7369 6665 782e 636f 6d2f 696e  transifex.com/in
 00000150: 7665 6e69 6f73 6f66 7477 6172 652f 7465  veniosoftware/te
 00000160: 616d 732f 3233 3533 372f 6c74 2f29 0a50  ams/23537/lt/).P
 00000170: 6c75 7261 6c2d 466f 726d 733a 206e 706c  lural-Forms: npl
 00000180: 7572 616c 733d 343b 2070 6c75 7261 6c3d  urals=4; plural=
 00000190: 286e 2025 2031 3020 3d3d 2031 2026 2620  (n % 10 == 1 && 
 000001a0: 286e 2025 2031 3030 203e 2031 3920 7c7c  (n % 100 > 19 ||
```

### Comparing `invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/lt/LC_MESSAGES/messages.po` & `invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/lt/LC_MESSAGES/messages.po`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-drafts-resources 0.18.2\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:07+0000\n"
 "PO-Revision-Date: 2021-07-13 12:40+0000\n"
-"Language-Team: Lithuanian (https://www.transifex.com/inveniosoftware/teams/23537/lt/)\n"
+"Language-Team: Lithuanian (https://app.transifex.com/inveniosoftware/teams/23537/lt/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.3\n"
 "Language: lt\n"
 "Plural-Forms: nplurals=4; plural=(n % 10 == 1 && (n % 100 > 19 || n % 100 < 11) ? 0 : (n % 10 >= 2 && n % 10 <=9) && (n % 100 > 19 || n % 100 < 11) ? 1 : n % 1 != 0 ? 2: 3);\n"
```

### Comparing `invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/messages.pot` & `invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/messages.pot`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/no/LC_MESSAGES/messages.mo` & `invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/no/LC_MESSAGES/messages.mo`

 * *Format-specific differences are supported for Gettext message catalogues but no file-specific differences were detected; falling back to a binary diff. file(1) reports: GNU message catalog (little endian), revision 0.0, 1 message, Project-Id-Version: invenio-drafts-resources 0.18.2*

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 000000c0: 7369 6f6e 2d44 6174 653a 2032 3032 312d  sion-Date: 2021-
 000000d0: 3037 2d31 3320 3132 3a34 302b 3030 3030  07-13 12:40+0000
 000000e0: 0a4c 6173 742d 5472 616e 736c 6174 6f72  .Last-Translator
 000000f0: 3a20 4655 4c4c 204e 414d 4520 3c45 4d41  : FULL NAME <EMA
 00000100: 494c 4041 4444 5245 5353 3e0a 4c61 6e67  IL@ADDRESS>.Lang
 00000110: 7561 6765 3a20 6e6f 0a4c 616e 6775 6167  uage: no.Languag
 00000120: 652d 5465 616d 3a20 4e6f 7277 6567 6961  e-Team: Norwegia
-00000130: 6e20 2868 7474 7073 3a2f 2f77 7777 2e74  n (https://www.t
+00000130: 6e20 2868 7474 7073 3a2f 2f61 7070 2e74  n (https://app.t
 00000140: 7261 6e73 6966 6578 2e63 6f6d 2f69 6e76  ransifex.com/inv
 00000150: 656e 696f 736f 6674 7761 7265 2f74 6561  eniosoftware/tea
 00000160: 6d73 2f32 3335 3337 2f6e 6f2f 290a 506c  ms/23537/no/).Pl
 00000170: 7572 616c 2d46 6f72 6d73 3a20 6e70 6c75  ural-Forms: nplu
 00000180: 7261 6c73 3d32 3b20 706c 7572 616c 3d28  rals=2; plural=(
 00000190: 6e20 213d 2031 293b 0a4d 494d 452d 5665  n != 1);.MIME-Ve
 000001a0: 7273 696f 6e3a 2031 2e30 0a43 6f6e 7465  rsion: 1.0.Conte
```

### Comparing `invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/no/LC_MESSAGES/messages.po` & `invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/ro/LC_MESSAGES/messages.po`

 * *Files 4% similar despite different names*

```diff
@@ -7,21 +7,21 @@
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-drafts-resources 0.18.2\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:07+0000\n"
 "PO-Revision-Date: 2021-07-13 12:40+0000\n"
-"Language-Team: Norwegian (https://www.transifex.com/inveniosoftware/teams/23537/no/)\n"
+"Language-Team: Romanian (https://app.transifex.com/inveniosoftware/teams/23537/ro/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.3\n"
-"Language: no\n"
-"Plural-Forms: nplurals=2; plural=(n != 1);\n"
+"Language: ro\n"
+"Plural-Forms: nplurals=3; plural=(n==1?0:(((n%100>19)||((n%100==0)&&(n!=0)))?2:1));\n"
 
 #: invenio_drafts_resources/services/records/config.py:42
 #: invenio_drafts_resources/services/records/config.py:71
 msgid "Best match"
 msgstr ""
 
 #: invenio_drafts_resources/services/records/config.py:46
```

### Comparing `invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/pl/LC_MESSAGES/messages.mo` & `invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/ru/LC_MESSAGES/messages.mo`

 * *Format-specific differences are supported for Gettext message catalogues but no file-specific differences were detected; falling back to a binary diff. file(1) reports: GNU message catalog (little endian), revision 0.0, 1 message, Project-Id-Version: invenio-drafts-resources 0.18.2*

 * *Files 10% similar despite different names*

```diff
@@ -1,42 +1,42 @@
 00000000: de12 0495 0000 0000 0100 0000 1c00 0000  ................
 00000010: 2400 0000 0000 0000 0000 0000 0000 0000  $...............
-00000020: 2c00 0000 7002 0000 2d00 0000 0050 726f  ,...p...-....Pro
+00000020: 2c00 0000 6902 0000 2d00 0000 0050 726f  ,...i...-....Pro
 00000030: 6a65 6374 2d49 642d 5665 7273 696f 6e3a  ject-Id-Version:
 00000040: 2069 6e76 656e 696f 2d64 7261 6674 732d   invenio-drafts-
 00000050: 7265 736f 7572 6365 7320 302e 3138 2e32  resources 0.18.2
 00000060: 0a52 6570 6f72 742d 4d73 6769 642d 4275  .Report-Msgid-Bu
 00000070: 6773 2d54 6f3a 2069 6e66 6f40 696e 7665  gs-To: info@inve
 00000080: 6e69 6f73 6f66 7477 6172 652e 6f72 670a  niosoftware.org.
 00000090: 504f 542d 4372 6561 7469 6f6e 2d44 6174  POT-Creation-Dat
 000000a0: 653a 2032 3032 322d 3130 2d31 3220 3039  e: 2022-10-12 09
 000000b0: 3a30 372b 3030 3030 0a50 4f2d 5265 7669  :07+0000.PO-Revi
 000000c0: 7369 6f6e 2d44 6174 653a 2032 3032 312d  sion-Date: 2021-
 000000d0: 3037 2d31 3320 3132 3a34 302b 3030 3030  07-13 12:40+0000
 000000e0: 0a4c 6173 742d 5472 616e 736c 6174 6f72  .Last-Translator
 000000f0: 3a20 4655 4c4c 204e 414d 4520 3c45 4d41  : FULL NAME <EMA
 00000100: 494c 4041 4444 5245 5353 3e0a 4c61 6e67  IL@ADDRESS>.Lang
-00000110: 7561 6765 3a20 706c 0a4c 616e 6775 6167  uage: pl.Languag
-00000120: 652d 5465 616d 3a20 506f 6c69 7368 2028  e-Team: Polish (
-00000130: 6874 7470 733a 2f2f 7777 772e 7472 616e  https://www.tran
-00000140: 7369 6665 782e 636f 6d2f 696e 7665 6e69  sifex.com/inveni
-00000150: 6f73 6f66 7477 6172 652f 7465 616d 732f  osoftware/teams/
-00000160: 3233 3533 372f 706c 2f29 0a50 6c75 7261  23537/pl/).Plura
-00000170: 6c2d 466f 726d 733a 206e 706c 7572 616c  l-Forms: nplural
-00000180: 733d 343b 2070 6c75 7261 6c3d 286e 3d3d  s=4; plural=(n==
-00000190: 3120 3f20 3020 3a20 286e 2531 303e 3d32  1 ? 0 : (n%10>=2
-000001a0: 2026 2620 6e25 3130 3c3d 3429 2026 2620   && n%10<=4) && 
-000001b0: 286e 2531 3030 3c31 3220 7c7c 206e 2531  (n%100<12 || n%1
-000001c0: 3030 3e31 3429 203f 2031 203a 206e 213d  00>14) ? 1 : n!=
-000001d0: 3120 2626 2028 6e25 3130 3e3d 3020 2626  1 && (n%10>=0 &&
-000001e0: 206e 2531 303c 3d31 2920 7c7c 2028 6e25   n%10<=1) || (n%
-000001f0: 3130 3e3d 3520 2626 206e 2531 303c 3d39  10>=5 && n%10<=9
-00000200: 2920 7c7c 2028 6e25 3130 303e 3d31 3220  ) || (n%100>=12 
-00000210: 2626 206e 2531 3030 3c3d 3134 2920 3f20  && n%100<=14) ? 
-00000220: 3220 3a20 3329 3b0a 4d49 4d45 2d56 6572  2 : 3);.MIME-Ver
-00000230: 7369 6f6e 3a20 312e 300a 436f 6e74 656e  sion: 1.0.Conten
-00000240: 742d 5479 7065 3a20 7465 7874 2f70 6c61  t-Type: text/pla
-00000250: 696e 3b20 6368 6172 7365 743d 7574 662d  in; charset=utf-
-00000260: 380a 436f 6e74 656e 742d 5472 616e 7366  8.Content-Transf
-00000270: 6572 2d45 6e63 6f64 696e 673a 2038 6269  er-Encoding: 8bi
-00000280: 740a 4765 6e65 7261 7465 642d 4279 3a20  t.Generated-By: 
-00000290: 4261 6265 6c20 322e 3132 2e31 0a00       Babel 2.12.1..
+00000110: 7561 6765 3a20 7275 0a4c 616e 6775 6167  uage: ru.Languag
+00000120: 652d 5465 616d 3a20 5275 7373 6961 6e20  e-Team: Russian 
+00000130: 2868 7474 7073 3a2f 2f61 7070 2e74 7261  (https://app.tra
+00000140: 6e73 6966 6578 2e63 6f6d 2f69 6e76 656e  nsifex.com/inven
+00000150: 696f 736f 6674 7761 7265 2f74 6561 6d73  iosoftware/teams
+00000160: 2f32 3335 3337 2f72 752f 290a 506c 7572  /23537/ru/).Plur
+00000170: 616c 2d46 6f72 6d73 3a20 6e70 6c75 7261  al-Forms: nplura
+00000180: 6c73 3d34 3b20 706c 7572 616c 3d28 6e25  ls=4; plural=(n%
+00000190: 3130 3d3d 3120 2626 206e 2531 3030 213d  10==1 && n%100!=
+000001a0: 3131 203f 2030 203a 206e 2531 303e 3d32  11 ? 0 : n%10>=2
+000001b0: 2026 2620 6e25 3130 3c3d 3420 2626 2028   && n%10<=4 && (
+000001c0: 6e25 3130 303c 3132 207c 7c20 6e25 3130  n%100<12 || n%10
+000001d0: 303e 3134 2920 3f20 3120 3a20 6e25 3130  0>14) ? 1 : n%10
+000001e0: 3d3d 3020 7c7c 2028 6e25 3130 3e3d 3520  ==0 || (n%10>=5 
+000001f0: 2626 206e 2531 303c 3d39 2920 7c7c 2028  && n%10<=9) || (
+00000200: 6e25 3130 303e 3d31 3120 2626 206e 2531  n%100>=11 && n%1
+00000210: 3030 3c3d 3134 293f 2032 203a 2033 293b  00<=14)? 2 : 3);
+00000220: 0a4d 494d 452d 5665 7273 696f 6e3a 2031  .MIME-Version: 1
+00000230: 2e30 0a43 6f6e 7465 6e74 2d54 7970 653a  .0.Content-Type:
+00000240: 2074 6578 742f 706c 6169 6e3b 2063 6861   text/plain; cha
+00000250: 7273 6574 3d75 7466 2d38 0a43 6f6e 7465  rset=utf-8.Conte
+00000260: 6e74 2d54 7261 6e73 6665 722d 456e 636f  nt-Transfer-Enco
+00000270: 6469 6e67 3a20 3862 6974 0a47 656e 6572  ding: 8bit.Gener
+00000280: 6174 6564 2d42 793a 2042 6162 656c 2032  ated-By: Babel 2
+00000290: 2e31 322e 310a 00                        .12.1..
```

### Comparing `invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/pl/LC_MESSAGES/messages.po` & `invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/pl/LC_MESSAGES/messages.po`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-drafts-resources 0.18.2\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:07+0000\n"
 "PO-Revision-Date: 2021-07-13 12:40+0000\n"
-"Language-Team: Polish (https://www.transifex.com/inveniosoftware/teams/23537/pl/)\n"
+"Language-Team: Polish (https://app.transifex.com/inveniosoftware/teams/23537/pl/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.3\n"
 "Language: pl\n"
 "Plural-Forms: nplurals=4; plural=(n==1 ? 0 : (n%10>=2 && n%10<=4) && (n%100<12 || n%100>14) ? 1 : n!=1 && (n%10>=0 && n%10<=1) || (n%10>=5 && n%10<=9) || (n%100>=12 && n%100<=14) ? 2 : 3);\n"
```

### Comparing `invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/pt/LC_MESSAGES/messages.mo` & `invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/pt/LC_MESSAGES/messages.mo`

 * *Format-specific differences are supported for Gettext message catalogues but no file-specific differences were detected; falling back to a binary diff. file(1) reports: GNU message catalog (little endian), revision 0.0, 1 message, Project-Id-Version: invenio-drafts-resources 0.18.2*

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 000000c0: 7369 6f6e 2d44 6174 653a 2032 3032 312d  sion-Date: 2021-
 000000d0: 3037 2d31 3320 3132 3a34 302b 3030 3030  07-13 12:40+0000
 000000e0: 0a4c 6173 742d 5472 616e 736c 6174 6f72  .Last-Translator
 000000f0: 3a20 4655 4c4c 204e 414d 4520 3c45 4d41  : FULL NAME <EMA
 00000100: 494c 4041 4444 5245 5353 3e0a 4c61 6e67  IL@ADDRESS>.Lang
 00000110: 7561 6765 3a20 7074 0a4c 616e 6775 6167  uage: pt.Languag
 00000120: 652d 5465 616d 3a20 506f 7274 7567 7565  e-Team: Portugue
-00000130: 7365 2028 6874 7470 733a 2f2f 7777 772e  se (https://www.
+00000130: 7365 2028 6874 7470 733a 2f2f 6170 702e  se (https://app.
 00000140: 7472 616e 7369 6665 782e 636f 6d2f 696e  transifex.com/in
 00000150: 7665 6e69 6f73 6f66 7477 6172 652f 7465  veniosoftware/te
 00000160: 616d 732f 3233 3533 372f 7074 2f29 0a50  ams/23537/pt/).P
 00000170: 6c75 7261 6c2d 466f 726d 733a 206e 706c  lural-Forms: npl
 00000180: 7572 616c 733d 333b 2070 6c75 7261 6c3d  urals=3; plural=
 00000190: 286e 203d 3d20 3020 7c7c 206e 203d 3d20  (n == 0 || n == 
 000001a0: 3129 203f 2030 203a 206e 2021 3d20 3020  1) ? 0 : n != 0
```

### Comparing `invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/pt/LC_MESSAGES/messages.po` & `invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/es_MX/LC_MESSAGES/messages.po`

 * *Files 3% similar despite different names*

```diff
@@ -7,21 +7,21 @@
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-drafts-resources 0.18.2\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:07+0000\n"
 "PO-Revision-Date: 2021-07-13 12:40+0000\n"
-"Language-Team: Portuguese (https://www.transifex.com/inveniosoftware/teams/23537/pt/)\n"
+"Language-Team: Spanish (Mexico) (https://app.transifex.com/inveniosoftware/teams/23537/es_MX/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.3\n"
-"Language: pt\n"
-"Plural-Forms: nplurals=3; plural=(n == 0 || n == 1) ? 0 : n != 0 && n % 1000000 == 0 ? 1 : 2;\n"
+"Language: es_MX\n"
+"Plural-Forms: nplurals=3; plural=n == 1 ? 0 : n != 0 && n % 1000000 == 0 ? 1 : 2;\n"
 
 #: invenio_drafts_resources/services/records/config.py:42
 #: invenio_drafts_resources/services/records/config.py:71
 msgid "Best match"
 msgstr ""
 
 #: invenio_drafts_resources/services/records/config.py:46
```

### Comparing `invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/ro/LC_MESSAGES/messages.mo` & `invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/ro/LC_MESSAGES/messages.mo`

 * *Format-specific differences are supported for Gettext message catalogues but no file-specific differences were detected; falling back to a binary diff. file(1) reports: GNU message catalog (little endian), revision 0.0, 1 message, Project-Id-Version: invenio-drafts-resources 0.18.2*

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 000000c0: 7369 6f6e 2d44 6174 653a 2032 3032 312d  sion-Date: 2021-
 000000d0: 3037 2d31 3320 3132 3a34 302b 3030 3030  07-13 12:40+0000
 000000e0: 0a4c 6173 742d 5472 616e 736c 6174 6f72  .Last-Translator
 000000f0: 3a20 4655 4c4c 204e 414d 4520 3c45 4d41  : FULL NAME <EMA
 00000100: 494c 4041 4444 5245 5353 3e0a 4c61 6e67  IL@ADDRESS>.Lang
 00000110: 7561 6765 3a20 726f 0a4c 616e 6775 6167  uage: ro.Languag
 00000120: 652d 5465 616d 3a20 526f 6d61 6e69 616e  e-Team: Romanian
-00000130: 2028 6874 7470 733a 2f2f 7777 772e 7472   (https://www.tr
+00000130: 2028 6874 7470 733a 2f2f 6170 702e 7472   (https://app.tr
 00000140: 616e 7369 6665 782e 636f 6d2f 696e 7665  ansifex.com/inve
 00000150: 6e69 6f73 6f66 7477 6172 652f 7465 616d  niosoftware/team
 00000160: 732f 3233 3533 372f 726f 2f29 0a50 6c75  s/23537/ro/).Plu
 00000170: 7261 6c2d 466f 726d 733a 206e 706c 7572  ral-Forms: nplur
 00000180: 616c 733d 333b 2070 6c75 7261 6c3d 286e  als=3; plural=(n
 00000190: 3d3d 313f 303a 2828 286e 2531 3030 3e31  ==1?0:(((n%100>1
 000001a0: 3929 7c7c 2828 6e25 3130 303d 3d30 2926  9)||((n%100==0)&
```

### Comparing `invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/ro/LC_MESSAGES/messages.po` & `invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/de_DE/LC_MESSAGES/messages.po`

 * *Files 2% similar despite different names*

```diff
@@ -7,21 +7,21 @@
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-drafts-resources 0.18.2\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:07+0000\n"
 "PO-Revision-Date: 2021-07-13 12:40+0000\n"
-"Language-Team: Romanian (https://www.transifex.com/inveniosoftware/teams/23537/ro/)\n"
+"Language-Team: German (Germany) (https://app.transifex.com/inveniosoftware/teams/23537/de_DE/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.3\n"
-"Language: ro\n"
-"Plural-Forms: nplurals=3; plural=(n==1?0:(((n%100>19)||((n%100==0)&&(n!=0)))?2:1));\n"
+"Language: de_DE\n"
+"Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
 #: invenio_drafts_resources/services/records/config.py:42
 #: invenio_drafts_resources/services/records/config.py:71
 msgid "Best match"
 msgstr ""
 
 #: invenio_drafts_resources/services/records/config.py:46
```

### Comparing `invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/ru/LC_MESSAGES/messages.mo` & `invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/sk/LC_MESSAGES/messages.mo`

 * *Files 21% similar despite different names*

#### msgunfmt {}

```diff
@@ -0,0 +1,19 @@
+msgid ""
+msgstr ""
+"Project-Id-Version: invenio-drafts-resources 0.18.2\n"
+"Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
+"POT-Creation-Date: 2022-10-12 09:07+0000\n"
+"PO-Revision-Date: 2021-07-13 12:40+0000\n"
+"Last-Translator: Ivan Masár <helix84@centrum.sk>, 2021\n"
+"Language: sk\n"
+"Language-Team: Slovak (https://app.transifex.com/inveniosoftware/teams/23537/"
+"sk/)\n"
+"Plural-Forms: nplurals=4; plural=(n % 1 == 0 && n == 1 ? 0 : n % 1 == 0 && n "
+">= 2 && n <= 4 ? 1 : n % 1 != 0 ? 2: 3);\n"
+"MIME-Version: 1.0\n"
+"Content-Type: text/plain; charset=utf-8\n"
+"Content-Transfer-Encoding: 8bit\n"
+"Generated-By: Babel 2.12.1\n"
+
+msgid "Version"
+msgstr "Verzia"
```

### Comparing `invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/ru/LC_MESSAGES/messages.po` & `invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/ru/LC_MESSAGES/messages.po`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-drafts-resources 0.18.2\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:07+0000\n"
 "PO-Revision-Date: 2021-07-13 12:40+0000\n"
-"Language-Team: Russian (https://www.transifex.com/inveniosoftware/teams/23537/ru/)\n"
+"Language-Team: Russian (https://app.transifex.com/inveniosoftware/teams/23537/ru/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.3\n"
 "Language: ru\n"
 "Plural-Forms: nplurals=4; plural=(n%10==1 && n%100!=11 ? 0 : n%10>=2 && n%10<=4 && (n%100<12 || n%100>14) ? 1 : n%10==0 || (n%10>=5 && n%10<=9) || (n%100>=11 && n%100<=14)? 2 : 3);\n"
```

### Comparing `invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/rw/LC_MESSAGES/messages.mo` & `invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/rw/LC_MESSAGES/messages.mo`

 * *Format-specific differences are supported for Gettext message catalogues but no file-specific differences were detected; falling back to a binary diff. file(1) reports: GNU message catalog (little endian), revision 0.0, 1 message, Project-Id-Version: invenio-drafts-resources 0.18.2*

 * *Files 4% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 000000c0: 7369 6f6e 2d44 6174 653a 2032 3032 312d  sion-Date: 2021-
 000000d0: 3037 2d31 3320 3132 3a34 302b 3030 3030  07-13 12:40+0000
 000000e0: 0a4c 6173 742d 5472 616e 736c 6174 6f72  .Last-Translator
 000000f0: 3a20 4655 4c4c 204e 414d 4520 3c45 4d41  : FULL NAME <EMA
 00000100: 494c 4041 4444 5245 5353 3e0a 4c61 6e67  IL@ADDRESS>.Lang
 00000110: 7561 6765 3a20 7277 0a4c 616e 6775 6167  uage: rw.Languag
 00000120: 652d 5465 616d 3a20 4b69 6e79 6172 7761  e-Team: Kinyarwa
-00000130: 6e64 6120 2868 7474 7073 3a2f 2f77 7777  nda (https://www
+00000130: 6e64 6120 2868 7474 7073 3a2f 2f61 7070  nda (https://app
 00000140: 2e74 7261 6e73 6966 6578 2e63 6f6d 2f69  .transifex.com/i
 00000150: 6e76 656e 696f 736f 6674 7761 7265 2f74  nveniosoftware/t
 00000160: 6561 6d73 2f32 3335 3337 2f72 772f 290a  eams/23537/rw/).
 00000170: 506c 7572 616c 2d46 6f72 6d73 3a20 6e70  Plural-Forms: np
 00000180: 6c75 7261 6c73 3d32 3b20 706c 7572 616c  lurals=2; plural
 00000190: 3d28 6e20 213d 2031 293b 0a4d 494d 452d  =(n != 1);.MIME-
 000001a0: 5665 7273 696f 6e3a 2031 2e30 0a43 6f6e  Version: 1.0.Con
```

### Comparing `invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/rw/LC_MESSAGES/messages.po` & `invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/rw/LC_MESSAGES/messages.po`

 * *Files 4% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-drafts-resources 0.18.2\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:07+0000\n"
 "PO-Revision-Date: 2021-07-13 12:40+0000\n"
-"Language-Team: Kinyarwanda (https://www.transifex.com/inveniosoftware/teams/23537/rw/)\n"
+"Language-Team: Kinyarwanda (https://app.transifex.com/inveniosoftware/teams/23537/rw/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.3\n"
 "Language: rw\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
```

### Comparing `invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/sk/LC_MESSAGES/messages.mo` & `invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/cs/LC_MESSAGES/messages.mo`

 * *Files 13% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,19 +1,19 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-drafts-resources 0.18.2\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:07+0000\n"
 "PO-Revision-Date: 2021-07-13 12:40+0000\n"
 "Last-Translator: Ivan Masár <helix84@centrum.sk>, 2021\n"
-"Language: sk\n"
-"Language-Team: Slovak (https://www.transifex.com/inveniosoftware/teams/23537/"
-"sk/)\n"
-"Plural-Forms: nplurals=4; plural=(n % 1 == 0 && n == 1 ? 0 : n % 1 == 0 && n "
-">= 2 && n <= 4 ? 1 : n % 1 != 0 ? 2: 3);\n"
+"Language: cs\n"
+"Language-Team: Czech (https://app.transifex.com/inveniosoftware/teams/23537/"
+"cs/)\n"
+"Plural-Forms: nplurals=4; plural=(n == 1 && n % 1 == 0) ? 0 : (n >= 2 && n "
+"<= 4 && n % 1 == 0) ? 1: (n % 1 != 0 ) ? 2 : 3;\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.12.1\n"
 
 msgid "Version"
-msgstr "Verzia"
+msgstr "Verze"
```

### Comparing `invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/sk/LC_MESSAGES/messages.po` & `invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/sk/LC_MESSAGES/messages.po`

 * *Files 3% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-drafts-resources 0.18.2\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:07+0000\n"
 "PO-Revision-Date: 2021-07-13 12:40+0000\n"
 "Last-Translator: Ivan Masár <helix84@centrum.sk>, 2021\n"
-"Language-Team: Slovak (https://www.transifex.com/inveniosoftware/teams/23537/sk/)\n"
+"Language-Team: Slovak (https://app.transifex.com/inveniosoftware/teams/23537/sk/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.3\n"
 "Language: sk\n"
 "Plural-Forms: nplurals=4; plural=(n % 1 == 0 && n == 1 ? 0 : n % 1 == 0 && n >= 2 && n <= 4 ? 1 : n % 1 != 0 ? 2: 3);\n"
```

### Comparing `invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/sv/LC_MESSAGES/messages.mo` & `invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/sv/LC_MESSAGES/messages.mo`

 * *Files 5% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,16 +1,16 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-drafts-resources 0.18.2\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:07+0000\n"
 "PO-Revision-Date: 2021-07-13 12:40+0000\n"
-"Last-Translator: Sam Arbid, 2022\n"
+"Last-Translator: yyones, 2023\n"
 "Language: sv\n"
-"Language-Team: Swedish (https://www.transifex.com/inveniosoftware/"
+"Language-Team: Swedish (https://app.transifex.com/inveniosoftware/"
 "teams/23537/sv/)\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.12.1\n"
 
@@ -27,23 +27,23 @@
 "Missing uploaded files. To disable files for this record please mark it as "
 "metadata-only."
 msgstr ""
 "Uppladdade filer saknas. För att inaktivera filer för denna post, markera "
 "den som endast metadata."
 
 msgid "Newest"
-msgstr "Nyaste"
+msgstr "Nyast"
 
 msgid "Oldest"
 msgstr "Äldst"
 
 msgid "Please remove all files first."
 msgstr "Ta bort alla filer först."
 
 msgid "Recently updated"
 msgstr "Nyligen uppdaterad"
 
 msgid "The record has no files."
-msgstr "Rekorden har inga filer."
+msgstr "Posten har inga filer."
 
 msgid "Version"
 msgstr "Version"
```

### Comparing `invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/sv/LC_MESSAGES/messages.po` & `invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/uk/LC_MESSAGES/messages.po`

 * *Files 10% similar despite different names*

```diff
@@ -1,74 +1,72 @@
 # Translations template for invenio-drafts-resources.
 # Copyright (C) 2022 CERN
 # This file is distributed under the same license as the
 # invenio-drafts-resources project.
 # FIRST AUTHOR <EMAIL@ADDRESS>, 2022.
 # 
 # Translators:
-# Sam Arbid, 2022
+# Vasyl Ostrovskyi <vasyusya@yahoo.com>, 2023
 # 
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-drafts-resources 0.18.2\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:07+0000\n"
 "PO-Revision-Date: 2021-07-13 12:40+0000\n"
-"Last-Translator: Sam Arbid, 2022\n"
-"Language-Team: Swedish (https://www.transifex.com/inveniosoftware/teams/23537/sv/)\n"
+"Last-Translator: Vasyl Ostrovskyi <vasyusya@yahoo.com>, 2023\n"
+"Language-Team: Ukrainian (https://app.transifex.com/inveniosoftware/teams/23537/uk/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.3\n"
-"Language: sv\n"
-"Plural-Forms: nplurals=2; plural=(n != 1);\n"
+"Language: uk\n"
+"Plural-Forms: nplurals=4; plural=(n % 1 == 0 && n % 10 == 1 && n % 100 != 11 ? 0 : n % 1 == 0 && n % 10 >= 2 && n % 10 <= 4 && (n % 100 < 12 || n % 100 > 14) ? 1 : n % 1 == 0 && (n % 10 ==0 || (n % 10 >=5 && n % 10 <=9) || (n % 100 >=11 && n % 100 <=14 )) ? 2: 3);\n"
 
 #: invenio_drafts_resources/services/records/config.py:42
 #: invenio_drafts_resources/services/records/config.py:71
 msgid "Best match"
-msgstr "Bästa matchningen"
+msgstr "Найкраща відповідність"
 
 #: invenio_drafts_resources/services/records/config.py:46
 #: invenio_drafts_resources/services/records/config.py:83
 msgid "Newest"
-msgstr "Nyaste"
+msgstr "Найновіші"
 
 #: invenio_drafts_resources/services/records/config.py:50
 #: invenio_drafts_resources/services/records/config.py:87
 msgid "Oldest"
-msgstr "Äldst"
+msgstr "Найстаріші"
 
 #: invenio_drafts_resources/services/records/config.py:54
 #: invenio_drafts_resources/services/records/config.py:91
 #: invenio_drafts_resources/services/records/config.py:108
 msgid "Version"
-msgstr "Version"
+msgstr "Версія"
 
 #: invenio_drafts_resources/services/records/config.py:75
 msgid "Recently updated"
-msgstr "Nyligen uppdaterad"
+msgstr "Недавно оновлені"
 
 #: invenio_drafts_resources/services/records/config.py:79
 msgid "Least recently updated"
-msgstr "Senast uppdaterad"
+msgstr "Найбільш давно не оновлювались"
 
 #: invenio_drafts_resources/services/records/components/files.py:60
 #: invenio_drafts_resources/services/records/components/files.py:127
 msgid ""
 "Missing uploaded files. To disable files for this record please mark it as "
 "metadata-only."
 msgstr ""
-"Uppladdade filer saknas. För att inaktivera filer för denna post, markera "
-"den som endast metadata."
 
 #: invenio_drafts_resources/services/records/components/files.py:153
 msgid "Files support must be enabled."
-msgstr "Filstöd måste vara aktiverat."
+msgstr ""
 
 #: invenio_drafts_resources/services/records/components/files.py:158
 msgid "Please remove all files first."
-msgstr "Ta bort alla filer först."
+msgstr ""
 
 #: invenio_drafts_resources/services/records/components/files.py:163
 msgid "The record has no files."
-msgstr "Rekorden har inga filer."
+msgstr "Запис на містить файлів"
```

### Comparing `invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/tr/LC_MESSAGES/messages.mo` & `invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/tr/LC_MESSAGES/messages.mo`

 * *Files 1% similar despite different names*

#### msgunfmt {}

```diff
@@ -3,15 +3,15 @@
 "Project-Id-Version: invenio-drafts-resources 0.18.2\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:07+0000\n"
 "PO-Revision-Date: 2021-07-13 12:40+0000\n"
 "Last-Translator: Ben Translation and Interpreting Services <info@bentercume."
 "com>, 2021\n"
 "Language: tr\n"
-"Language-Team: Turkish (https://www.transifex.com/inveniosoftware/"
+"Language-Team: Turkish (https://app.transifex.com/inveniosoftware/"
 "teams/23537/tr/)\n"
 "Plural-Forms: nplurals=2; plural=(n > 1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.12.1\n"
```

### Comparing `invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/tr/LC_MESSAGES/messages.po` & `invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/tr/LC_MESSAGES/messages.po`

 * *Files 4% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-drafts-resources 0.18.2\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:07+0000\n"
 "PO-Revision-Date: 2021-07-13 12:40+0000\n"
 "Last-Translator: Ben Translation and Interpreting Services <info@bentercume.com>, 2021\n"
-"Language-Team: Turkish (https://www.transifex.com/inveniosoftware/teams/23537/tr/)\n"
+"Language-Team: Turkish (https://app.transifex.com/inveniosoftware/teams/23537/tr/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.3\n"
 "Language: tr\n"
 "Plural-Forms: nplurals=2; plural=(n > 1);\n"
```

### Comparing `invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/uk/LC_MESSAGES/messages.mo` & `invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/en_AT/LC_MESSAGES/messages.mo`

 * *Format-specific differences are supported for Gettext message catalogues but no file-specific differences were detected; falling back to a binary diff. file(1) reports: GNU message catalog (little endian), revision 0.0, 1 message, Project-Id-Version: invenio-drafts-resources 0.18.2*

 * *Files 24% similar despite different names*

```diff
@@ -1,47 +1,34 @@
 00000000: de12 0495 0000 0000 0100 0000 1c00 0000  ................
 00000010: 2400 0000 0000 0000 0000 0000 0000 0000  $...............
-00000020: 2c00 0000 bf02 0000 2d00 0000 0050 726f  ,.......-....Pro
+00000020: 2c00 0000 ef01 0000 2d00 0000 0050 726f  ,.......-....Pro
 00000030: 6a65 6374 2d49 642d 5665 7273 696f 6e3a  ject-Id-Version:
 00000040: 2069 6e76 656e 696f 2d64 7261 6674 732d   invenio-drafts-
 00000050: 7265 736f 7572 6365 7320 302e 3138 2e32  resources 0.18.2
 00000060: 0a52 6570 6f72 742d 4d73 6769 642d 4275  .Report-Msgid-Bu
 00000070: 6773 2d54 6f3a 2069 6e66 6f40 696e 7665  gs-To: info@inve
 00000080: 6e69 6f73 6f66 7477 6172 652e 6f72 670a  niosoftware.org.
 00000090: 504f 542d 4372 6561 7469 6f6e 2d44 6174  POT-Creation-Dat
 000000a0: 653a 2032 3032 322d 3130 2d31 3220 3039  e: 2022-10-12 09
 000000b0: 3a30 372b 3030 3030 0a50 4f2d 5265 7669  :07+0000.PO-Revi
 000000c0: 7369 6f6e 2d44 6174 653a 2032 3032 312d  sion-Date: 2021-
 000000d0: 3037 2d31 3320 3132 3a34 302b 3030 3030  07-13 12:40+0000
 000000e0: 0a4c 6173 742d 5472 616e 736c 6174 6f72  .Last-Translator
 000000f0: 3a20 4655 4c4c 204e 414d 4520 3c45 4d41  : FULL NAME <EMA
 00000100: 494c 4041 4444 5245 5353 3e0a 4c61 6e67  IL@ADDRESS>.Lang
-00000110: 7561 6765 3a20 756b 0a4c 616e 6775 6167  uage: uk.Languag
-00000120: 652d 5465 616d 3a20 556b 7261 696e 6961  e-Team: Ukrainia
-00000130: 6e20 2868 7474 7073 3a2f 2f77 7777 2e74  n (https://www.t
-00000140: 7261 6e73 6966 6578 2e63 6f6d 2f69 6e76  ransifex.com/inv
-00000150: 656e 696f 736f 6674 7761 7265 2f74 6561  eniosoftware/tea
-00000160: 6d73 2f32 3335 3337 2f75 6b2f 290a 506c  ms/23537/uk/).Pl
-00000170: 7572 616c 2d46 6f72 6d73 3a20 6e70 6c75  ural-Forms: nplu
-00000180: 7261 6c73 3d34 3b20 706c 7572 616c 3d28  rals=4; plural=(
-00000190: 6e20 2520 3120 3d3d 2030 2026 2620 6e20  n % 1 == 0 && n 
-000001a0: 2520 3130 203d 3d20 3120 2626 206e 2025  % 10 == 1 && n %
-000001b0: 2031 3030 2021 3d20 3131 203f 2030 203a   100 != 11 ? 0 :
-000001c0: 206e 2025 2031 203d 3d20 3020 2626 206e   n % 1 == 0 && n
-000001d0: 2025 2031 3020 3e3d 2032 2026 2620 6e20   % 10 >= 2 && n 
-000001e0: 2520 3130 203c 3d20 3420 2626 2028 6e20  % 10 <= 4 && (n 
-000001f0: 2520 3130 3020 3c20 3132 207c 7c20 6e20  % 100 < 12 || n 
-00000200: 2520 3130 3020 3e20 3134 2920 3f20 3120  % 100 > 14) ? 1 
-00000210: 3a20 6e20 2520 3120 3d3d 2030 2026 2620  : n % 1 == 0 && 
-00000220: 286e 2025 2031 3020 3d3d 3020 7c7c 2028  (n % 10 ==0 || (
-00000230: 6e20 2520 3130 203e 3d35 2026 2620 6e20  n % 10 >=5 && n 
-00000240: 2520 3130 203c 3d39 2920 7c7c 2028 6e20  % 10 <=9) || (n 
-00000250: 2520 3130 3020 3e3d 3131 2026 2620 6e20  % 100 >=11 && n 
-00000260: 2520 3130 3020 3c3d 3134 2029 2920 3f20  % 100 <=14 )) ? 
-00000270: 323a 2033 293b 0a4d 494d 452d 5665 7273  2: 3);.MIME-Vers
-00000280: 696f 6e3a 2031 2e30 0a43 6f6e 7465 6e74  ion: 1.0.Content
-00000290: 2d54 7970 653a 2074 6578 742f 706c 6169  -Type: text/plai
-000002a0: 6e3b 2063 6861 7273 6574 3d75 7466 2d38  n; charset=utf-8
-000002b0: 0a43 6f6e 7465 6e74 2d54 7261 6e73 6665  .Content-Transfe
-000002c0: 722d 456e 636f 6469 6e67 3a20 3862 6974  r-Encoding: 8bit
-000002d0: 0a47 656e 6572 6174 6564 2d42 793a 2042  .Generated-By: B
-000002e0: 6162 656c 2032 2e31 322e 310a 00         abel 2.12.1..
+00000110: 7561 6765 3a20 656e 5f41 540a 4c61 6e67  uage: en_AT.Lang
+00000120: 7561 6765 2d54 6561 6d3a 2045 6e67 6c69  uage-Team: Engli
+00000130: 7368 2028 4175 7374 7269 6129 2028 6874  sh (Austria) (ht
+00000140: 7470 733a 2f2f 6170 702e 7472 616e 7369  tps://app.transi
+00000150: 6665 782e 636f 6d2f 696e 7665 6e69 6f73  fex.com/invenios
+00000160: 6f66 7477 6172 652f 7465 616d 732f 3233  oftware/teams/23
+00000170: 3533 372f 656e 5f41 542f 290a 506c 7572  537/en_AT/).Plur
+00000180: 616c 2d46 6f72 6d73 3a20 6e70 6c75 7261  al-Forms: nplura
+00000190: 6c73 3d32 3b20 706c 7572 616c 3d28 6e20  ls=2; plural=(n 
+000001a0: 213d 2031 293b 0a4d 494d 452d 5665 7273  != 1);.MIME-Vers
+000001b0: 696f 6e3a 2031 2e30 0a43 6f6e 7465 6e74  ion: 1.0.Content
+000001c0: 2d54 7970 653a 2074 6578 742f 706c 6169  -Type: text/plai
+000001d0: 6e3b 2063 6861 7273 6574 3d75 7466 2d38  n; charset=utf-8
+000001e0: 0a43 6f6e 7465 6e74 2d54 7261 6e73 6665  .Content-Transfe
+000001f0: 722d 456e 636f 6469 6e67 3a20 3862 6974  r-Encoding: 8bit
+00000200: 0a47 656e 6572 6174 6564 2d42 793a 2042  .Generated-By: B
+00000210: 6162 656c 2032 2e31 322e 310a 00         abel 2.12.1..
```

### Comparing `invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/uk/LC_MESSAGES/messages.po` & `invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/uk_UA/LC_MESSAGES/messages.po`

 * *Files 2% similar despite different names*

```diff
@@ -7,20 +7,20 @@
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-drafts-resources 0.18.2\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:07+0000\n"
 "PO-Revision-Date: 2021-07-13 12:40+0000\n"
-"Language-Team: Ukrainian (https://www.transifex.com/inveniosoftware/teams/23537/uk/)\n"
+"Language-Team: Ukrainian (Ukraine) (https://app.transifex.com/inveniosoftware/teams/23537/uk_UA/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.3\n"
-"Language: uk\n"
+"Language: uk_UA\n"
 "Plural-Forms: nplurals=4; plural=(n % 1 == 0 && n % 10 == 1 && n % 100 != 11 ? 0 : n % 1 == 0 && n % 10 >= 2 && n % 10 <= 4 && (n % 100 < 12 || n % 100 > 14) ? 1 : n % 1 == 0 && (n % 10 ==0 || (n % 10 >=5 && n % 10 <=9) || (n % 100 >=11 && n % 100 <=14 )) ? 2: 3);\n"
 
 #: invenio_drafts_resources/services/records/config.py:42
 #: invenio_drafts_resources/services/records/config.py:71
 msgid "Best match"
 msgstr ""
```

### Comparing `invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/zh_CN/LC_MESSAGES/messages.mo` & `invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/zh_CN/LC_MESSAGES/messages.mo`

 * *Files 1% similar despite different names*

#### msgunfmt {}

```diff
@@ -2,15 +2,15 @@
 msgstr ""
 "Project-Id-Version: invenio-drafts-resources 0.18.2\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:07+0000\n"
 "PO-Revision-Date: 2021-07-13 12:40+0000\n"
 "Last-Translator: Kalven Richie, 2022\n"
 "Language: zh_CN\n"
-"Language-Team: Chinese (China) (https://www.transifex.com/inveniosoftware/"
+"Language-Team: Chinese (China) (https://app.transifex.com/inveniosoftware/"
 "teams/23537/zh_CN/)\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.12.1\n"
```

### Comparing `invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/zh_CN/LC_MESSAGES/messages.po` & `invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/zh_CN/LC_MESSAGES/messages.po`

 * *Files 4% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-drafts-resources 0.18.2\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:07+0000\n"
 "PO-Revision-Date: 2021-07-13 12:40+0000\n"
 "Last-Translator: Kalven Richie, 2022\n"
-"Language-Team: Chinese (China) (https://www.transifex.com/inveniosoftware/teams/23537/zh_CN/)\n"
+"Language-Team: Chinese (China) (https://app.transifex.com/inveniosoftware/teams/23537/zh_CN/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.3\n"
 "Language: zh_CN\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
```

### Comparing `invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/zh_TW/LC_MESSAGES/messages.mo` & `invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/zh_TW/LC_MESSAGES/messages.mo`

 * *Format-specific differences are supported for Gettext message catalogues but no file-specific differences were detected; falling back to a binary diff. file(1) reports: GNU message catalog (little endian), revision 0.0, 1 message, Project-Id-Version: invenio-drafts-resources 0.18.2*

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 000000d0: 3037 2d31 3320 3132 3a34 302b 3030 3030  07-13 12:40+0000
 000000e0: 0a4c 6173 742d 5472 616e 736c 6174 6f72  .Last-Translator
 000000f0: 3a20 4655 4c4c 204e 414d 4520 3c45 4d41  : FULL NAME <EMA
 00000100: 494c 4041 4444 5245 5353 3e0a 4c61 6e67  IL@ADDRESS>.Lang
 00000110: 7561 6765 3a20 7a68 5f54 570a 4c61 6e67  uage: zh_TW.Lang
 00000120: 7561 6765 2d54 6561 6d3a 2043 6869 6e65  uage-Team: Chine
 00000130: 7365 2028 5461 6977 616e 2920 2868 7474  se (Taiwan) (htt
-00000140: 7073 3a2f 2f77 7777 2e74 7261 6e73 6966  ps://www.transif
+00000140: 7073 3a2f 2f61 7070 2e74 7261 6e73 6966  ps://app.transif
 00000150: 6578 2e63 6f6d 2f69 6e76 656e 696f 736f  ex.com/invenioso
 00000160: 6674 7761 7265 2f74 6561 6d73 2f32 3335  ftware/teams/235
 00000170: 3337 2f7a 685f 5457 2f29 0a50 6c75 7261  37/zh_TW/).Plura
 00000180: 6c2d 466f 726d 733a 206e 706c 7572 616c  l-Forms: nplural
 00000190: 733d 313b 2070 6c75 7261 6c3d 303b 0a4d  s=1; plural=0;.M
 000001a0: 494d 452d 5665 7273 696f 6e3a 2031 2e30  IME-Version: 1.0
 000001b0: 0a43 6f6e 7465 6e74 2d54 7970 653a 2074  .Content-Type: t
```

### Comparing `invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/zh_TW/LC_MESSAGES/messages.po` & `invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/el/LC_MESSAGES/messages.po`

 * *Files 2% similar despite different names*

```diff
@@ -7,21 +7,21 @@
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-drafts-resources 0.18.2\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:07+0000\n"
 "PO-Revision-Date: 2021-07-13 12:40+0000\n"
-"Language-Team: Chinese (Taiwan) (https://www.transifex.com/inveniosoftware/teams/23537/zh_TW/)\n"
+"Language-Team: Greek (https://app.transifex.com/inveniosoftware/teams/23537/el/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.3\n"
-"Language: zh_TW\n"
-"Plural-Forms: nplurals=1; plural=0;\n"
+"Language: el\n"
+"Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
 #: invenio_drafts_resources/services/records/config.py:42
 #: invenio_drafts_resources/services/records/config.py:71
 msgid "Best match"
 msgstr ""
 
 #: invenio_drafts_resources/services/records/config.py:46
```

### Comparing `invenio-drafts-resources-1.4.1/invenio_drafts_resources.egg-info/PKG-INFO` & `invenio-drafts-resources-1.4.2/invenio_drafts_resources.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invenio-drafts-resources
-Version: 1.4.1
+Version: 1.4.2
 Summary: Invenio Drafts Resources module to create REST APIs
 Home-page: https://github.com/inveniosoftware/Invenio-Drafts-Resources
 Author: CERN
 Author-email: info@inveniosoftware.org
 License: MIT
 Description: ..
             Copyright (C) 2020 CERN.
@@ -47,14 +47,19 @@
             Invenio-Drafts-Resources is free software; you can redistribute it and/or
             modify it under the terms of the MIT License; see LICENSE file for more
             details.
         
         Changes
         =======
         
+        Version 1.4.2 (2023-07-05)
+        
+        - transifex: update config
+        - components: add default files enabled variable
+        
         Version 1.4.1 (2023-06-06)
         
         - fix permission check for managing files
         
         Version 1.4.0 (2023-04-25)
         
         - upgrade invenio-records-resources
```

### Comparing `invenio-drafts-resources-1.4.1/invenio_drafts_resources.egg-info/SOURCES.txt` & `invenio-drafts-resources-1.4.2/invenio_drafts_resources.egg-info/SOURCES.txt`

 * *Files 21% similar despite different names*

```diff
@@ -76,40 +76,64 @@
 invenio_drafts_resources/translations/ca/LC_MESSAGES/messages.po
 invenio_drafts_resources/translations/cs/LC_MESSAGES/messages.mo
 invenio_drafts_resources/translations/cs/LC_MESSAGES/messages.po
 invenio_drafts_resources/translations/da/LC_MESSAGES/messages.mo
 invenio_drafts_resources/translations/da/LC_MESSAGES/messages.po
 invenio_drafts_resources/translations/de/LC_MESSAGES/messages.mo
 invenio_drafts_resources/translations/de/LC_MESSAGES/messages.po
+invenio_drafts_resources/translations/de_AT/LC_MESSAGES/messages.mo
+invenio_drafts_resources/translations/de_AT/LC_MESSAGES/messages.po
+invenio_drafts_resources/translations/de_DE/LC_MESSAGES/messages.mo
+invenio_drafts_resources/translations/de_DE/LC_MESSAGES/messages.po
 invenio_drafts_resources/translations/el/LC_MESSAGES/messages.mo
 invenio_drafts_resources/translations/el/LC_MESSAGES/messages.po
+invenio_drafts_resources/translations/en_AT/LC_MESSAGES/messages.mo
+invenio_drafts_resources/translations/en_AT/LC_MESSAGES/messages.po
+invenio_drafts_resources/translations/en_HU/LC_MESSAGES/messages.mo
+invenio_drafts_resources/translations/en_HU/LC_MESSAGES/messages.po
 invenio_drafts_resources/translations/es/LC_MESSAGES/messages.mo
 invenio_drafts_resources/translations/es/LC_MESSAGES/messages.po
+invenio_drafts_resources/translations/es_CU/LC_MESSAGES/messages.mo
+invenio_drafts_resources/translations/es_CU/LC_MESSAGES/messages.po
+invenio_drafts_resources/translations/es_MX/LC_MESSAGES/messages.mo
+invenio_drafts_resources/translations/es_MX/LC_MESSAGES/messages.po
 invenio_drafts_resources/translations/et/LC_MESSAGES/messages.mo
 invenio_drafts_resources/translations/et/LC_MESSAGES/messages.po
 invenio_drafts_resources/translations/et_EE/LC_MESSAGES/messages.mo
 invenio_drafts_resources/translations/et_EE/LC_MESSAGES/messages.po
 invenio_drafts_resources/translations/fa/LC_MESSAGES/messages.mo
 invenio_drafts_resources/translations/fa/LC_MESSAGES/messages.po
+invenio_drafts_resources/translations/fa_IR/LC_MESSAGES/messages.mo
+invenio_drafts_resources/translations/fa_IR/LC_MESSAGES/messages.po
 invenio_drafts_resources/translations/fr/LC_MESSAGES/messages.mo
 invenio_drafts_resources/translations/fr/LC_MESSAGES/messages.po
+invenio_drafts_resources/translations/fr_CI/LC_MESSAGES/messages.mo
+invenio_drafts_resources/translations/fr_CI/LC_MESSAGES/messages.po
+invenio_drafts_resources/translations/fr_FR/LC_MESSAGES/messages.mo
+invenio_drafts_resources/translations/fr_FR/LC_MESSAGES/messages.po
 invenio_drafts_resources/translations/gl/LC_MESSAGES/messages.mo
 invenio_drafts_resources/translations/gl/LC_MESSAGES/messages.po
+invenio_drafts_resources/translations/hi_IN/LC_MESSAGES/messages.mo
+invenio_drafts_resources/translations/hi_IN/LC_MESSAGES/messages.po
 invenio_drafts_resources/translations/hr/LC_MESSAGES/messages.mo
 invenio_drafts_resources/translations/hr/LC_MESSAGES/messages.po
 invenio_drafts_resources/translations/hu/LC_MESSAGES/messages.mo
 invenio_drafts_resources/translations/hu/LC_MESSAGES/messages.po
+invenio_drafts_resources/translations/hu_HU/LC_MESSAGES/messages.mo
+invenio_drafts_resources/translations/hu_HU/LC_MESSAGES/messages.po
 invenio_drafts_resources/translations/it/LC_MESSAGES/messages.mo
 invenio_drafts_resources/translations/it/LC_MESSAGES/messages.po
 invenio_drafts_resources/translations/ja/LC_MESSAGES/messages.mo
 invenio_drafts_resources/translations/ja/LC_MESSAGES/messages.po
 invenio_drafts_resources/translations/ka/LC_MESSAGES/messages.mo
 invenio_drafts_resources/translations/ka/LC_MESSAGES/messages.po
 invenio_drafts_resources/translations/lt/LC_MESSAGES/messages.mo
 invenio_drafts_resources/translations/lt/LC_MESSAGES/messages.po
+invenio_drafts_resources/translations/ne/LC_MESSAGES/messages.mo
+invenio_drafts_resources/translations/ne/LC_MESSAGES/messages.po
 invenio_drafts_resources/translations/no/LC_MESSAGES/messages.mo
 invenio_drafts_resources/translations/no/LC_MESSAGES/messages.po
 invenio_drafts_resources/translations/pl/LC_MESSAGES/messages.mo
 invenio_drafts_resources/translations/pl/LC_MESSAGES/messages.po
 invenio_drafts_resources/translations/pt/LC_MESSAGES/messages.mo
 invenio_drafts_resources/translations/pt/LC_MESSAGES/messages.po
 invenio_drafts_resources/translations/ro/LC_MESSAGES/messages.mo
@@ -118,18 +142,22 @@
 invenio_drafts_resources/translations/ru/LC_MESSAGES/messages.po
 invenio_drafts_resources/translations/rw/LC_MESSAGES/messages.mo
 invenio_drafts_resources/translations/rw/LC_MESSAGES/messages.po
 invenio_drafts_resources/translations/sk/LC_MESSAGES/messages.mo
 invenio_drafts_resources/translations/sk/LC_MESSAGES/messages.po
 invenio_drafts_resources/translations/sv/LC_MESSAGES/messages.mo
 invenio_drafts_resources/translations/sv/LC_MESSAGES/messages.po
+invenio_drafts_resources/translations/sv_SE/LC_MESSAGES/messages.mo
+invenio_drafts_resources/translations/sv_SE/LC_MESSAGES/messages.po
 invenio_drafts_resources/translations/tr/LC_MESSAGES/messages.mo
 invenio_drafts_resources/translations/tr/LC_MESSAGES/messages.po
 invenio_drafts_resources/translations/uk/LC_MESSAGES/messages.mo
 invenio_drafts_resources/translations/uk/LC_MESSAGES/messages.po
+invenio_drafts_resources/translations/uk_UA/LC_MESSAGES/messages.mo
+invenio_drafts_resources/translations/uk_UA/LC_MESSAGES/messages.po
 invenio_drafts_resources/translations/zh_CN/LC_MESSAGES/messages.mo
 invenio_drafts_resources/translations/zh_CN/LC_MESSAGES/messages.po
 invenio_drafts_resources/translations/zh_TW/LC_MESSAGES/messages.mo
 invenio_drafts_resources/translations/zh_TW/LC_MESSAGES/messages.po
 tests/conftest.py
 tests/mock_module/__init__.py
 tests/mock_module/api.py
```

### Comparing `invenio-drafts-resources-1.4.1/run-tests.sh` & `invenio-drafts-resources-1.4.2/run-tests.sh`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 #!/usr/bin/env bash
 # -*- coding: utf-8 -*-
 #
 # Copyright (C) 2020-2021 CERN.
 # Copyright (C) 2020 Northwestern University.
 # Copyright (C) 2021 TU Wien.
+# Copyright (C) 2023 Graz University of Technology.
 #
 # Invenio-Drafts-Resources is free software; you can redistribute it and/or modify
 # it under the terms of the MIT License; see LICENSE file for more details.
 
 # Usage:
 #   ./run-tests.sh [pytest options and args...]
 #
```

### Comparing `invenio-drafts-resources-1.4.1/setup.cfg` & `invenio-drafts-resources-1.4.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.1/tests/conftest.py` & `invenio-drafts-resources-1.4.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.1/tests/mock_module/api.py` & `invenio-drafts-resources-1.4.2/tests/mock_module/api.py`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.1/tests/mock_module/mappings/os-v1/draftsresources/drafts/draft-v1.0.0.json` & `invenio-drafts-resources-1.4.2/tests/mock_module/mappings/os-v1/draftsresources/drafts/draft-v1.0.0.json`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.1/tests/mock_module/mappings/os-v1/draftsresources/records/record-v1.0.0.json` & `invenio-drafts-resources-1.4.2/tests/mock_module/mappings/os-v1/draftsresources/records/record-v1.0.0.json`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.1/tests/mock_module/mappings/os-v2/draftsresources/drafts/draft-v1.0.0.json` & `invenio-drafts-resources-1.4.2/tests/mock_module/mappings/os-v2/draftsresources/drafts/draft-v1.0.0.json`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.1/tests/mock_module/mappings/os-v2/draftsresources/records/record-v1.0.0.json` & `invenio-drafts-resources-1.4.2/tests/mock_module/mappings/os-v2/draftsresources/records/record-v1.0.0.json`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.1/tests/mock_module/mappings/v7/draftsresources/drafts/draft-v1.0.0.json` & `invenio-drafts-resources-1.4.2/tests/mock_module/mappings/v7/draftsresources/drafts/draft-v1.0.0.json`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.1/tests/mock_module/mappings/v7/draftsresources/records/record-v1.0.0.json` & `invenio-drafts-resources-1.4.2/tests/mock_module/mappings/v7/draftsresources/records/record-v1.0.0.json`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.1/tests/mock_module/models.py` & `invenio-drafts-resources-1.4.2/tests/mock_module/models.py`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.1/tests/mock_module/permissions.py` & `invenio-drafts-resources-1.4.2/tests/mock_module/permissions.py`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.1/tests/mock_module/resource.py` & `invenio-drafts-resources-1.4.2/tests/mock_module/resource.py`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.1/tests/mock_module/schemas.py` & `invenio-drafts-resources-1.4.2/tests/mock_module/schemas.py`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.1/tests/mock_module/service.py` & `invenio-drafts-resources-1.4.2/tests/mock_module/service.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,14 +19,15 @@
     """Mock service configuration."""
 
     permission_policy_cls = PermissionPolicy
     record_cls = Record
     draft_cls = Draft
 
     schema = RecordSchema
+    default_files_enabled = True
 
     components = RecordServiceConfig.components + [DraftFilesComponent]
 
     links_item = {
         "self": ConditionalLink(
             cond=is_record,
             if_=RecordLink("{+api}/mocks/{id}"),
```

### Comparing `invenio-drafts-resources-1.4.1/tests/records/conftest.py` & `invenio-drafts-resources-1.4.2/tests/records/conftest.py`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.1/tests/records/test_api.py` & `invenio-drafts-resources-1.4.2/tests/records/test_api.py`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.1/tests/resources/conftest.py` & `invenio-drafts-resources-1.4.2/tests/resources/conftest.py`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.1/tests/resources/test_files_resource.py` & `invenio-drafts-resources-1.4.2/tests/resources/test_files_resource.py`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.1/tests/resources/test_record_resource.py` & `invenio-drafts-resources-1.4.2/tests/resources/test_record_resource.py`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.1/tests/resources/test_resource_links.py` & `invenio-drafts-resources-1.4.2/tests/resources/test_resource_links.py`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.1/tests/services/conftest.py` & `invenio-drafts-resources-1.4.2/tests/services/conftest.py`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.1/tests/services/test_record_service.py` & `invenio-drafts-resources-1.4.2/tests/services/test_record_service.py`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.1/tests/services/test_record_service_files.py` & `invenio-drafts-resources-1.4.2/tests/services/test_record_service_files.py`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.1/tests/services/test_record_service_search.py` & `invenio-drafts-resources-1.4.2/tests/services/test_record_service_search.py`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.1/tests/services/test_record_service_tasks.py` & `invenio-drafts-resources-1.4.2/tests/services/test_record_service_tasks.py`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.1/tests/services/test_services.py` & `invenio-drafts-resources-1.4.2/tests/services/test_services.py`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.1/tests/services/utils.py` & `invenio-drafts-resources-1.4.2/tests/services/utils.py`

 * *Files identical despite different names*

