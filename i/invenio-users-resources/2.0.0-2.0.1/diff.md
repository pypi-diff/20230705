# Comparing `tmp/invenio-users-resources-2.0.0.tar.gz` & `tmp/invenio-users-resources-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/invenio-users-resources-2.0.0.tar", last modified: Fri Jun 30 15:24:34 2023, max compression
+gzip compressed data, was "dist/invenio-users-resources-2.0.1.tar", last modified: Wed Jul  5 14:29:19 2023, max compression
```

## Comparing `invenio-users-resources-2.0.0.tar` & `invenio-users-resources-2.0.1.tar`

### file list

```diff
@@ -1,265 +1,321 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:24:34.000000 invenio-users-resources-2.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-06-30 15:24:25.000000 invenio-users-resources-2.0.0/.dockerignore
--rw-r--r--   0 runner    (1001) docker     (123)      646 2023-06-30 15:24:25.000000 invenio-users-resources-2.0.0/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-30 15:24:25.000000 invenio-users-resources-2.0.0/.git-blame-ignore-revs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:24:34.000000 invenio-users-resources-2.0.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:24:34.000000 invenio-users-resources-2.0.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-06-30 15:24:25.000000 invenio-users-resources-2.0.0/.github/workflows/i18n-pull.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2013 2023-06-30 15:24:25.000000 invenio-users-resources-2.0.0/.github/workflows/i18n-push.yml
--rw-r--r--   0 runner    (1001) docker     (123)      651 2023-06-30 15:24:25.000000 invenio-users-resources-2.0.0/.github/workflows/pypi-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3436 2023-06-30 15:24:25.000000 invenio-users-resources-2.0.0/.github/workflows/tests.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:24:34.000000 invenio-users-resources-2.0.0/.tx/
--rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-06-30 15:24:25.000000 invenio-users-resources-2.0.0/.tx/config
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-06-30 15:24:25.000000 invenio-users-resources-2.0.0/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-06-30 15:24:25.000000 invenio-users-resources-2.0.0/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3612 2023-06-30 15:24:25.000000 invenio-users-resources-2.0.0/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-06-30 15:24:25.000000 invenio-users-resources-2.0.0/INSTALL.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-06-30 15:24:25.000000 invenio-users-resources-2.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      984 2023-06-30 15:24:25.000000 invenio-users-resources-2.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4071 2023-06-30 15:24:34.000000 invenio-users-resources-2.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-06-30 15:24:25.000000 invenio-users-resources-2.0.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      480 2023-06-30 15:24:25.000000 invenio-users-resources-2.0.0/babel.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:24:34.000000 invenio-users-resources-2.0.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     7477 2023-06-30 15:24:25.000000 invenio-users-resources-2.0.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-06-30 15:24:25.000000 invenio-users-resources-2.0.0/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-06-30 15:24:25.000000 invenio-users-resources-2.0.0/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-06-30 15:24:25.000000 invenio-users-resources-2.0.0/docs/changes.rst
--rw-r--r--   0 runner    (1001) docker     (123)    10463 2023-06-30 15:24:25.000000 invenio-users-resources-2.0.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-06-30 15:24:25.000000 invenio-users-resources-2.0.0/docs/configuration.rst
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-30 15:24:25.000000 invenio-users-resources-2.0.0/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      817 2023-06-30 15:24:25.000000 invenio-users-resources-2.0.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-06-30 15:24:25.000000 invenio-users-resources-2.0.0/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-06-30 15:24:25.000000 invenio-users-resources-2.0.0/docs/license.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7015 2023-06-30 15:24:25.000000 invenio-users-resources-2.0.0/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-30 15:24:25.000000 invenio-users-resources-2.0.0/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-06-30 15:24:25.000000 invenio-users-resources-2.0.0/docs/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:24:34.000000 invenio-users-resources-2.0.0/invenio_users_resources/
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-06-30 15:24:25.000000 invenio-users-resources-2.0.0/invenio_users_resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      914 2023-06-30 15:24:25.000000 invenio-users-resources-2.0.0/invenio_users_resources/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3432 2023-06-30 15:24:25.000000 invenio-users-resources-2.0.0/invenio_users_resources/entity_resolvers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3105 2023-06-30 15:24:25.000000 invenio-users-resources-2.0.0/invenio_users_resources/ext.py
--rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-06-30 15:24:25.000000 invenio-users-resources-2.0.0/invenio_users_resources/forms.py
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-06-30 15:24:25.000000 invenio-users-resources-2.0.0/invenio_users_resources/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:24:34.000000 invenio-users-resources-2.0.0/invenio_users_resources/notifications/
--rw-r--r--   0 runner    (1001) docker     (123)      293 2023-06-30 15:24:25.000000 invenio-users-resources-2.0.0/invenio_users_resources/notifications/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      866 2023-06-30 15:24:25.000000 invenio-users-resources-2.0.0/invenio_users_resources/notifications/filters.py
--rw-r--r--   0 runner    (1001) docker     (123)      900 2023-06-30 15:24:25.000000 invenio-users-resources-2.0.0/invenio_users_resources/notifications/generators.py
--rw-r--r--   0 runner    (1001) docker     (123)      871 2023-06-30 15:24:25.000000 invenio-users-resources-2.0.0/invenio_users_resources/proxies.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:24:34.000000 invenio-users-resources-2.0.0/invenio_users_resources/records/
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-06-30 15:24:25.000000 invenio-users-resources-2.0.0/invenio_users_resources/records/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8281 2023-06-30 15:24:25.000000 invenio-users-resources-2.0.0/invenio_users_resources/records/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:24:34.000000 invenio-users-resources-2.0.0/invenio_users_resources/records/dumpers/
--rw-r--r--   0 runner    (1001) docker     (123)      365 2023-06-30 15:24:25.000000 invenio-users-resources-2.0.0/invenio_users_resources/records/dumpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-06-30 15:24:25.000000 invenio-users-resources-2.0.0/invenio_users_resources/records/dumpers/email.py
--rw-r--r--   0 runner    (1001) docker     (123)     2718 2023-06-30 15:24:25.000000 invenio-users-resources-2.0.0/invenio_users_resources/records/hooks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:24:34.000000 invenio-users-resources-2.0.0/invenio_users_resources/records/mappings/
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-06-30 15:24:25.000000 invenio-users-resources-2.0.0/invenio_users_resources/records/mappings/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:24:34.000000 invenio-users-resources-2.0.0/invenio_users_resources/records/mappings/os-v1/
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-06-30 15:24:25.000000 invenio-users-resources-2.0.0/invenio_users_resources/records/mappings/os-v1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:24:34.000000 invenio-users-resources-2.0.0/invenio_users_resources/records/mappings/os-v1/groups/
--rw-r--r--   0 runner    (1001) docker     (123)      695 2023-06-30 15:24:25.000000 invenio-users-resources-2.0.0/invenio_users_resources/records/mappings/os-v1/groups/group-v1.0.0.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:24:34.000000 invenio-users-resources-2.0.0/invenio_users_resources/records/mappings/os-v1/users/
--rw-r--r--   0 runner    (1001) docker     (123)     1995 2023-06-30 15:24:25.000000 invenio-users-resources-2.0.0/invenio_users_resources/records/mappings/os-v1/users/user-v1.0.0.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:24:34.000000 invenio-users-resources-2.0.0/invenio_users_resources/records/mappings/os-v2/
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-06-30 15:24:25.000000 invenio-users-resources-2.0.0/invenio_users_resources/records/mappings/os-v2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:24:34.000000 invenio-users-resources-2.0.0/invenio_users_resources/records/mappings/os-v2/groups/
--rw-r--r--   0 runner    (1001) docker     (123)      695 2023-06-30 15:24:25.000000 invenio-users-resources-2.0.0/invenio_users_resources/records/mappings/os-v2/groups/group-v1.0.0.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:24:34.000000 invenio-users-resources-2.0.0/invenio_users_resources/records/mappings/os-v2/users/
--rw-r--r--   0 runner    (1001) docker     (123)     1995 2023-06-30 15:24:25.000000 invenio-users-resources-2.0.0/invenio_users_resources/records/mappings/os-v2/users/user-v1.0.0.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:24:34.000000 invenio-users-resources-2.0.0/invenio_users_resources/records/mappings/v7/
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-06-30 15:24:25.000000 invenio-users-resources-2.0.0/invenio_users_resources/records/mappings/v7/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:24:34.000000 invenio-users-resources-2.0.0/invenio_users_resources/records/mappings/v7/groups/
--rw-r--r--   0 runner    (1001) docker     (123)      695 2023-06-30 15:24:25.000000 invenio-users-resources-2.0.0/invenio_users_resources/records/mappings/v7/groups/group-v1.0.0.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:24:34.000000 invenio-users-resources-2.0.0/invenio_users_resources/records/mappings/v7/users/
--rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-06-30 15:24:25.000000 invenio-users-resources-2.0.0/invenio_users_resources/records/mappings/v7/users/user-v1.0.0.json
--rw-r--r--   0 runner    (1001) docker     (123)     2870 2023-06-30 15:24:25.000000 invenio-users-resources-2.0.0/invenio_users_resources/records/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:24:34.000000 invenio-users-resources-2.0.0/invenio_users_resources/resources/
--rw-r--r--   0 runner    (1001) docker     (123)      488 2023-06-30 15:24:25.000000 invenio-users-resources-2.0.0/invenio_users_resources/resources/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:24:34.000000 invenio-users-resources-2.0.0/invenio_users_resources/resources/groups/
--rw-r--r--   0 runner    (1001) docker     (123)      402 2023-06-30 15:24:25.000000 invenio-users-resources-2.0.0/invenio_users_resources/resources/groups/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      981 2023-06-30 15:24:25.000000 invenio-users-resources-2.0.0/invenio_users_resources/resources/groups/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2230 2023-06-30 15:24:25.000000 invenio-users-resources-2.0.0/invenio_users_resources/resources/groups/resource.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:24:34.000000 invenio-users-resources-2.0.0/invenio_users_resources/resources/users/
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-06-30 15:24:25.000000 invenio-users-resources-2.0.0/invenio_users_resources/resources/users/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      801 2023-06-30 15:24:25.000000 invenio-users-resources-2.0.0/invenio_users_resources/resources/users/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2323 2023-06-30 15:24:25.000000 invenio-users-resources-2.0.0/invenio_users_resources/resources/users/resource.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:24:34.000000 invenio-users-resources-2.0.0/invenio_users_resources/services/
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-06-30 15:24:25.000000 invenio-users-resources-2.0.0/invenio_users_resources/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      553 2023-06-30 15:24:25.000000 invenio-users-resources-2.0.0/invenio_users_resources/services/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     3523 2023-06-30 15:24:25.000000 invenio-users-resources-2.0.0/invenio_users_resources/services/generators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:24:34.000000 invenio-users-resources-2.0.0/invenio_users_resources/services/groups/
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-06-30 15:24:25.000000 invenio-users-resources-2.0.0/invenio_users_resources/services/groups/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2331 2023-06-30 15:24:25.000000 invenio-users-resources-2.0.0/invenio_users_resources/services/groups/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3453 2023-06-30 15:24:25.000000 invenio-users-resources-2.0.0/invenio_users_resources/services/groups/results.py
--rw-r--r--   0 runner    (1001) docker     (123)     1923 2023-06-30 15:24:25.000000 invenio-users-resources-2.0.0/invenio_users_resources/services/groups/service.py
--rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-06-30 15:24:25.000000 invenio-users-resources-2.0.0/invenio_users_resources/services/groups/tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)      868 2023-06-30 15:24:25.000000 invenio-users-resources-2.0.0/invenio_users_resources/services/params.py
--rw-r--r--   0 runner    (1001) docker     (123)     1283 2023-06-30 15:24:25.000000 invenio-users-resources-2.0.0/invenio_users_resources/services/permissions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1711 2023-06-30 15:24:25.000000 invenio-users-resources-2.0.0/invenio_users_resources/services/results.py
--rw-r--r--   0 runner    (1001) docker     (123)     3287 2023-06-30 15:24:25.000000 invenio-users-resources-2.0.0/invenio_users_resources/services/schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:24:34.000000 invenio-users-resources-2.0.0/invenio_users_resources/services/users/
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-06-30 15:24:25.000000 invenio-users-resources-2.0.0/invenio_users_resources/services/users/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2522 2023-06-30 15:24:25.000000 invenio-users-resources-2.0.0/invenio_users_resources/services/users/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3396 2023-06-30 15:24:25.000000 invenio-users-resources-2.0.0/invenio_users_resources/services/users/results.py
--rw-r--r--   0 runner    (1001) docker     (123)     3357 2023-06-30 15:24:25.000000 invenio-users-resources-2.0.0/invenio_users_resources/services/users/service.py
--rw-r--r--   0 runner    (1001) docker     (123)     1886 2023-06-30 15:24:25.000000 invenio-users-resources-2.0.0/invenio_users_resources/services/users/tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:24:34.000000 invenio-users-resources-2.0.0/invenio_users_resources/templates/
--rw-r--r--   0 runner    (1001) docker     (123)      377 2023-06-30 15:24:25.000000 invenio-users-resources-2.0.0/invenio_users_resources/templates/avatar.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:24:34.000000 invenio-users-resources-2.0.0/invenio_users_resources/templates/semantic-ui/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:24:34.000000 invenio-users-resources-2.0.0/invenio_users_resources/templates/semantic-ui/invenio_users_resources/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:24:34.000000 invenio-users-resources-2.0.0/invenio_users_resources/templates/semantic-ui/invenio_users_resources/settings/
--rw-r--r--   0 runner    (1001) docker     (123)     2731 2023-06-30 15:24:25.000000 invenio-users-resources-2.0.0/invenio_users_resources/templates/semantic-ui/invenio_users_resources/settings/notifications.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:24:34.000000 invenio-users-resources-2.0.0/invenio_users_resources/translations/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:24:34.000000 invenio-users-resources-2.0.0/invenio_users_resources/translations/af/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:24:34.000000 invenio-users-resources-2.0.0/invenio_users_resources/translations/af/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-06-30 15:24:33.000000 invenio-users-resources-2.0.0/invenio_users_resources/translations/af/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-06-30 15:24:25.000000 invenio-users-resources-2.0.0/invenio_users_resources/translations/af/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:24:34.000000 invenio-users-resources-2.0.0/invenio_users_resources/translations/ar/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:24:34.000000 invenio-users-resources-2.0.0/invenio_users_resources/translations/ar/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      829 2023-06-30 15:24:33.000000 invenio-users-resources-2.0.0/invenio_users_resources/translations/ar/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)     1349 2023-06-30 15:24:25.000000 invenio-users-resources-2.0.0/invenio_users_resources/translations/ar/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:24:34.000000 invenio-users-resources-2.0.0/invenio_users_resources/translations/bg/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:24:34.000000 invenio-users-resources-2.0.0/invenio_users_resources/translations/bg/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      567 2023-06-30 15:24:33.000000 invenio-users-resources-2.0.0/invenio_users_resources/translations/bg/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-06-30 15:24:25.000000 invenio-users-resources-2.0.0/invenio_users_resources/translations/bg/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:24:34.000000 invenio-users-resources-2.0.0/invenio_users_resources/translations/ca/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:24:34.000000 invenio-users-resources-2.0.0/invenio_users_resources/translations/ca/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      562 2023-06-30 15:24:33.000000 invenio-users-resources-2.0.0/invenio_users_resources/translations/ca/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-06-30 15:24:25.000000 invenio-users-resources-2.0.0/invenio_users_resources/translations/ca/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:24:34.000000 invenio-users-resources-2.0.0/invenio_users_resources/translations/cs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:24:34.000000 invenio-users-resources-2.0.0/invenio_users_resources/translations/cs/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      643 2023-06-30 15:24:33.000000 invenio-users-resources-2.0.0/invenio_users_resources/translations/cs/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-06-30 15:24:25.000000 invenio-users-resources-2.0.0/invenio_users_resources/translations/cs/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:24:34.000000 invenio-users-resources-2.0.0/invenio_users_resources/translations/da/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:24:34.000000 invenio-users-resources-2.0.0/invenio_users_resources/translations/da/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      522 2023-06-30 15:24:33.000000 invenio-users-resources-2.0.0/invenio_users_resources/translations/da/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)      999 2023-06-30 15:24:25.000000 invenio-users-resources-2.0.0/invenio_users_resources/translations/da/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:24:34.000000 invenio-users-resources-2.0.0/invenio_users_resources/translations/de/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:24:34.000000 invenio-users-resources-2.0.0/invenio_users_resources/translations/de/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-06-30 15:24:33.000000 invenio-users-resources-2.0.0/invenio_users_resources/translations/de/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-06-30 15:24:25.000000 invenio-users-resources-2.0.0/invenio_users_resources/translations/de/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:24:34.000000 invenio-users-resources-2.0.0/invenio_users_resources/translations/el/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:24:34.000000 invenio-users-resources-2.0.0/invenio_users_resources/translations/el/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      567 2023-06-30 15:24:33.000000 invenio-users-resources-2.0.0/invenio_users_resources/translations/el/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-06-30 15:24:25.000000 invenio-users-resources-2.0.0/invenio_users_resources/translations/el/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:24:34.000000 invenio-users-resources-2.0.0/invenio_users_resources/translations/es/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:24:34.000000 invenio-users-resources-2.0.0/invenio_users_resources/translations/es/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      763 2023-06-30 15:24:33.000000 invenio-users-resources-2.0.0/invenio_users_resources/translations/es/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)     1283 2023-06-30 15:24:25.000000 invenio-users-resources-2.0.0/invenio_users_resources/translations/es/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:24:34.000000 invenio-users-resources-2.0.0/invenio_users_resources/translations/et/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:24:34.000000 invenio-users-resources-2.0.0/invenio_users_resources/translations/et/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-06-30 15:24:33.000000 invenio-users-resources-2.0.0/invenio_users_resources/translations/et/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-06-30 15:24:25.000000 invenio-users-resources-2.0.0/invenio_users_resources/translations/et/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:24:34.000000 invenio-users-resources-2.0.0/invenio_users_resources/translations/et_EE/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:24:34.000000 invenio-users-resources-2.0.0/invenio_users_resources/translations/et_EE/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-06-30 15:24:33.000000 invenio-users-resources-2.0.0/invenio_users_resources/translations/et_EE/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-06-30 15:24:25.000000 invenio-users-resources-2.0.0/invenio_users_resources/translations/et_EE/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:24:34.000000 invenio-users-resources-2.0.0/invenio_users_resources/translations/fa/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:24:34.000000 invenio-users-resources-2.0.0/invenio_users_resources/translations/fa/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      564 2023-06-30 15:24:33.000000 invenio-users-resources-2.0.0/invenio_users_resources/translations/fa/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-06-30 15:24:25.000000 invenio-users-resources-2.0.0/invenio_users_resources/translations/fa/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:24:34.000000 invenio-users-resources-2.0.0/invenio_users_resources/translations/fr/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:24:34.000000 invenio-users-resources-2.0.0/invenio_users_resources/translations/fr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      614 2023-06-30 15:24:33.000000 invenio-users-resources-2.0.0/invenio_users_resources/translations/fr/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-06-30 15:24:25.000000 invenio-users-resources-2.0.0/invenio_users_resources/translations/fr/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:24:34.000000 invenio-users-resources-2.0.0/invenio_users_resources/translations/gl/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:24:34.000000 invenio-users-resources-2.0.0/invenio_users_resources/translations/gl/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      524 2023-06-30 15:24:33.000000 invenio-users-resources-2.0.0/invenio_users_resources/translations/gl/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-06-30 15:24:25.000000 invenio-users-resources-2.0.0/invenio_users_resources/translations/gl/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:24:34.000000 invenio-users-resources-2.0.0/invenio_users_resources/translations/hr/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:24:34.000000 invenio-users-resources-2.0.0/invenio_users_resources/translations/hr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      635 2023-06-30 15:24:33.000000 invenio-users-resources-2.0.0/invenio_users_resources/translations/hr/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-06-30 15:24:25.000000 invenio-users-resources-2.0.0/invenio_users_resources/translations/hr/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:24:34.000000 invenio-users-resources-2.0.0/invenio_users_resources/translations/hu/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:24:34.000000 invenio-users-resources-2.0.0/invenio_users_resources/translations/hu/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      707 2023-06-30 15:24:33.000000 invenio-users-resources-2.0.0/invenio_users_resources/translations/hu/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-06-30 15:24:25.000000 invenio-users-resources-2.0.0/invenio_users_resources/translations/hu/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:24:34.000000 invenio-users-resources-2.0.0/invenio_users_resources/translations/it/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:24:34.000000 invenio-users-resources-2.0.0/invenio_users_resources/translations/it/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-06-30 15:24:33.000000 invenio-users-resources-2.0.0/invenio_users_resources/translations/it/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-06-30 15:24:25.000000 invenio-users-resources-2.0.0/invenio_users_resources/translations/it/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:24:34.000000 invenio-users-resources-2.0.0/invenio_users_resources/translations/ja/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:24:34.000000 invenio-users-resources-2.0.0/invenio_users_resources/translations/ja/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-06-30 15:24:33.000000 invenio-users-resources-2.0.0/invenio_users_resources/translations/ja/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-06-30 15:24:25.000000 invenio-users-resources-2.0.0/invenio_users_resources/translations/ja/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:24:34.000000 invenio-users-resources-2.0.0/invenio_users_resources/translations/ka/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:24:34.000000 invenio-users-resources-2.0.0/invenio_users_resources/translations/ka/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      576 2023-06-30 15:24:33.000000 invenio-users-resources-2.0.0/invenio_users_resources/translations/ka/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-06-30 15:24:25.000000 invenio-users-resources-2.0.0/invenio_users_resources/translations/ka/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:24:34.000000 invenio-users-resources-2.0.0/invenio_users_resources/translations/lt/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:24:34.000000 invenio-users-resources-2.0.0/invenio_users_resources/translations/lt/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      704 2023-06-30 15:24:33.000000 invenio-users-resources-2.0.0/invenio_users_resources/translations/lt/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)     1266 2023-06-30 15:24:25.000000 invenio-users-resources-2.0.0/invenio_users_resources/translations/lt/LC_MESSAGES/messages.po
--rw-r--r--   0 runner    (1001) docker     (123)      936 2023-06-30 15:24:25.000000 invenio-users-resources-2.0.0/invenio_users_resources/translations/messages.pot
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:24:34.000000 invenio-users-resources-2.0.0/invenio_users_resources/translations/no/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:24:34.000000 invenio-users-resources-2.0.0/invenio_users_resources/translations/no/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      565 2023-06-30 15:24:33.000000 invenio-users-resources-2.0.0/invenio_users_resources/translations/no/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-06-30 15:24:25.000000 invenio-users-resources-2.0.0/invenio_users_resources/translations/no/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:24:34.000000 invenio-users-resources-2.0.0/invenio_users_resources/translations/pl/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:24:34.000000 invenio-users-resources-2.0.0/invenio_users_resources/translations/pl/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-06-30 15:24:33.000000 invenio-users-resources-2.0.0/invenio_users_resources/translations/pl/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-06-30 15:24:25.000000 invenio-users-resources-2.0.0/invenio_users_resources/translations/pl/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:24:34.000000 invenio-users-resources-2.0.0/invenio_users_resources/translations/pt/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:24:34.000000 invenio-users-resources-2.0.0/invenio_users_resources/translations/pt/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-06-30 15:24:33.000000 invenio-users-resources-2.0.0/invenio_users_resources/translations/pt/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-06-30 15:24:25.000000 invenio-users-resources-2.0.0/invenio_users_resources/translations/pt/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:24:34.000000 invenio-users-resources-2.0.0/invenio_users_resources/translations/ro/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:24:34.000000 invenio-users-resources-2.0.0/invenio_users_resources/translations/ro/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      605 2023-06-30 15:24:33.000000 invenio-users-resources-2.0.0/invenio_users_resources/translations/ro/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-06-30 15:24:25.000000 invenio-users-resources-2.0.0/invenio_users_resources/translations/ro/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:24:34.000000 invenio-users-resources-2.0.0/invenio_users_resources/translations/ru/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:24:34.000000 invenio-users-resources-2.0.0/invenio_users_resources/translations/ru/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      703 2023-06-30 15:24:33.000000 invenio-users-resources-2.0.0/invenio_users_resources/translations/ru/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-06-30 15:24:25.000000 invenio-users-resources-2.0.0/invenio_users_resources/translations/ru/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:24:34.000000 invenio-users-resources-2.0.0/invenio_users_resources/translations/rw/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:24:34.000000 invenio-users-resources-2.0.0/invenio_users_resources/translations/rw/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      527 2023-06-30 15:24:33.000000 invenio-users-resources-2.0.0/invenio_users_resources/translations/rw/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-06-30 15:24:25.000000 invenio-users-resources-2.0.0/invenio_users_resources/translations/rw/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:24:34.000000 invenio-users-resources-2.0.0/invenio_users_resources/translations/sk/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:24:34.000000 invenio-users-resources-2.0.0/invenio_users_resources/translations/sk/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      637 2023-06-30 15:24:33.000000 invenio-users-resources-2.0.0/invenio_users_resources/translations/sk/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-06-30 15:24:25.000000 invenio-users-resources-2.0.0/invenio_users_resources/translations/sk/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:24:34.000000 invenio-users-resources-2.0.0/invenio_users_resources/translations/sv/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:24:34.000000 invenio-users-resources-2.0.0/invenio_users_resources/translations/sv/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      710 2023-06-30 15:24:33.000000 invenio-users-resources-2.0.0/invenio_users_resources/translations/sv/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-06-30 15:24:25.000000 invenio-users-resources-2.0.0/invenio_users_resources/translations/sv/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:24:34.000000 invenio-users-resources-2.0.0/invenio_users_resources/translations/tr/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:24:34.000000 invenio-users-resources-2.0.0/invenio_users_resources/translations/tr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-06-30 15:24:33.000000 invenio-users-resources-2.0.0/invenio_users_resources/translations/tr/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-06-30 15:24:25.000000 invenio-users-resources-2.0.0/invenio_users_resources/translations/tr/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:24:34.000000 invenio-users-resources-2.0.0/invenio_users_resources/translations/uk/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:24:34.000000 invenio-users-resources-2.0.0/invenio_users_resources/translations/uk/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      747 2023-06-30 15:24:33.000000 invenio-users-resources-2.0.0/invenio_users_resources/translations/uk/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-06-30 15:24:25.000000 invenio-users-resources-2.0.0/invenio_users_resources/translations/uk/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:24:34.000000 invenio-users-resources-2.0.0/invenio_users_resources/translations/zh_CN/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:24:34.000000 invenio-users-resources-2.0.0/invenio_users_resources/translations/zh_CN/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      702 2023-06-30 15:24:33.000000 invenio-users-resources-2.0.0/invenio_users_resources/translations/zh_CN/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-06-30 15:24:25.000000 invenio-users-resources-2.0.0/invenio_users_resources/translations/zh_CN/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:24:34.000000 invenio-users-resources-2.0.0/invenio_users_resources/translations/zh_TW/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:24:34.000000 invenio-users-resources-2.0.0/invenio_users_resources/translations/zh_TW/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-06-30 15:24:33.000000 invenio-users-resources-2.0.0/invenio_users_resources/translations/zh_TW/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-06-30 15:24:25.000000 invenio-users-resources-2.0.0/invenio_users_resources/translations/zh_TW/LC_MESSAGES/messages.po
--rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-06-30 15:24:25.000000 invenio-users-resources-2.0.0/invenio_users_resources/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:24:34.000000 invenio-users-resources-2.0.0/invenio_users_resources.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4071 2023-06-30 15:24:33.000000 invenio-users-resources-2.0.0/invenio_users_resources.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7970 2023-06-30 15:24:33.000000 invenio-users-resources-2.0.0/invenio_users_resources.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 15:24:33.000000 invenio-users-resources-2.0.0/invenio_users_resources.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-06-30 15:24:33.000000 invenio-users-resources-2.0.0/invenio_users_resources.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 15:24:33.000000 invenio-users-resources-2.0.0/invenio_users_resources.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-06-30 15:24:33.000000 invenio-users-resources-2.0.0/invenio_users_resources.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-30 15:24:33.000000 invenio-users-resources-2.0.0/invenio_users_resources.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-30 15:24:25.000000 invenio-users-resources-2.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-06-30 15:24:25.000000 invenio-users-resources-2.0.0/requirements-devel.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)     1401 2023-06-30 15:24:25.000000 invenio-users-resources-2.0.0/run-tests.sh
--rw-r--r--   0 runner    (1001) docker     (123)     2878 2023-06-30 15:24:34.000000 invenio-users-resources-2.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-06-30 15:24:25.000000 invenio-users-resources-2.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:24:34.000000 invenio-users-resources-2.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     7924 2023-06-30 15:24:25.000000 invenio-users-resources-2.0.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:24:34.000000 invenio-users-resources-2.0.0/tests/resources/
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-06-30 15:24:25.000000 invenio-users-resources-2.0.0/tests/resources/test_resources_groups.py
--rw-r--r--   0 runner    (1001) docker     (123)     2911 2023-06-30 15:24:25.000000 invenio-users-resources-2.0.0/tests/resources/test_resources_users.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:24:34.000000 invenio-users-resources-2.0.0/tests/services/
--rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-06-30 15:24:25.000000 invenio-users-resources-2.0.0/tests/services/test_service_groups.py
--rw-r--r--   0 runner    (1001) docker     (123)     3967 2023-06-30 15:24:25.000000 invenio-users-resources-2.0.0/tests/services/test_service_users.py
--rw-r--r--   0 runner    (1001) docker     (123)      830 2023-06-30 15:24:25.000000 invenio-users-resources-2.0.0/tests/test_invenio_users_resources.py
--rw-r--r--   0 runner    (1001) docker     (123)     2801 2023-06-30 15:24:25.000000 invenio-users-resources-2.0.0/tests/test_notifications.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:29:19.000000 invenio-users-resources-2.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-05 14:29:11.000000 invenio-users-resources-2.0.1/.dockerignore
+-rw-r--r--   0 runner    (1001) docker     (123)      646 2023-07-05 14:29:11.000000 invenio-users-resources-2.0.1/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-05 14:29:11.000000 invenio-users-resources-2.0.1/.git-blame-ignore-revs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:29:19.000000 invenio-users-resources-2.0.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:29:19.000000 invenio-users-resources-2.0.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-07-05 14:29:11.000000 invenio-users-resources-2.0.1/.github/workflows/i18n-pull.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-07-05 14:29:11.000000 invenio-users-resources-2.0.1/.github/workflows/i18n-push.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-07-05 14:29:11.000000 invenio-users-resources-2.0.1/.github/workflows/pypi-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3436 2023-07-05 14:29:11.000000 invenio-users-resources-2.0.1/.github/workflows/tests.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:29:19.000000 invenio-users-resources-2.0.1/.tx/
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-07-05 14:29:11.000000 invenio-users-resources-2.0.1/.tx/config
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-07-05 14:29:11.000000 invenio-users-resources-2.0.1/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1591 2023-07-05 14:29:11.000000 invenio-users-resources-2.0.1/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3612 2023-07-05 14:29:11.000000 invenio-users-resources-2.0.1/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-07-05 14:29:11.000000 invenio-users-resources-2.0.1/INSTALL.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-07-05 14:29:11.000000 invenio-users-resources-2.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-07-05 14:29:11.000000 invenio-users-resources-2.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4183 2023-07-05 14:29:19.000000 invenio-users-resources-2.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-07-05 14:29:11.000000 invenio-users-resources-2.0.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      480 2023-07-05 14:29:11.000000 invenio-users-resources-2.0.1/babel.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:29:19.000000 invenio-users-resources-2.0.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     7477 2023-07-05 14:29:11.000000 invenio-users-resources-2.0.1/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-07-05 14:29:11.000000 invenio-users-resources-2.0.1/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-07-05 14:29:11.000000 invenio-users-resources-2.0.1/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-07-05 14:29:11.000000 invenio-users-resources-2.0.1/docs/changes.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    10463 2023-07-05 14:29:11.000000 invenio-users-resources-2.0.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-07-05 14:29:11.000000 invenio-users-resources-2.0.1/docs/configuration.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-05 14:29:11.000000 invenio-users-resources-2.0.1/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-07-05 14:29:11.000000 invenio-users-resources-2.0.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-07-05 14:29:11.000000 invenio-users-resources-2.0.1/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-07-05 14:29:11.000000 invenio-users-resources-2.0.1/docs/license.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7015 2023-07-05 14:29:11.000000 invenio-users-resources-2.0.1/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-05 14:29:11.000000 invenio-users-resources-2.0.1/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-07-05 14:29:11.000000 invenio-users-resources-2.0.1/docs/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:29:19.000000 invenio-users-resources-2.0.1/invenio_users_resources/
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-07-05 14:29:11.000000 invenio-users-resources-2.0.1/invenio_users_resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      914 2023-07-05 14:29:11.000000 invenio-users-resources-2.0.1/invenio_users_resources/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3432 2023-07-05 14:29:11.000000 invenio-users-resources-2.0.1/invenio_users_resources/entity_resolvers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3105 2023-07-05 14:29:11.000000 invenio-users-resources-2.0.1/invenio_users_resources/ext.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-07-05 14:29:11.000000 invenio-users-resources-2.0.1/invenio_users_resources/forms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-07-05 14:29:11.000000 invenio-users-resources-2.0.1/invenio_users_resources/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:29:19.000000 invenio-users-resources-2.0.1/invenio_users_resources/notifications/
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-07-05 14:29:11.000000 invenio-users-resources-2.0.1/invenio_users_resources/notifications/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      866 2023-07-05 14:29:11.000000 invenio-users-resources-2.0.1/invenio_users_resources/notifications/filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-07-05 14:29:11.000000 invenio-users-resources-2.0.1/invenio_users_resources/notifications/generators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-07-05 14:29:11.000000 invenio-users-resources-2.0.1/invenio_users_resources/proxies.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:29:19.000000 invenio-users-resources-2.0.1/invenio_users_resources/records/
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-07-05 14:29:11.000000 invenio-users-resources-2.0.1/invenio_users_resources/records/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8281 2023-07-05 14:29:11.000000 invenio-users-resources-2.0.1/invenio_users_resources/records/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:29:19.000000 invenio-users-resources-2.0.1/invenio_users_resources/records/dumpers/
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-07-05 14:29:11.000000 invenio-users-resources-2.0.1/invenio_users_resources/records/dumpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-07-05 14:29:11.000000 invenio-users-resources-2.0.1/invenio_users_resources/records/dumpers/email.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2566 2023-07-05 14:29:11.000000 invenio-users-resources-2.0.1/invenio_users_resources/records/hooks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:29:19.000000 invenio-users-resources-2.0.1/invenio_users_resources/records/mappings/
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-07-05 14:29:11.000000 invenio-users-resources-2.0.1/invenio_users_resources/records/mappings/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:29:19.000000 invenio-users-resources-2.0.1/invenio_users_resources/records/mappings/os-v1/
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-07-05 14:29:11.000000 invenio-users-resources-2.0.1/invenio_users_resources/records/mappings/os-v1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:29:19.000000 invenio-users-resources-2.0.1/invenio_users_resources/records/mappings/os-v1/groups/
+-rw-r--r--   0 runner    (1001) docker     (123)      695 2023-07-05 14:29:11.000000 invenio-users-resources-2.0.1/invenio_users_resources/records/mappings/os-v1/groups/group-v1.0.0.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:29:19.000000 invenio-users-resources-2.0.1/invenio_users_resources/records/mappings/os-v1/users/
+-rw-r--r--   0 runner    (1001) docker     (123)     1995 2023-07-05 14:29:11.000000 invenio-users-resources-2.0.1/invenio_users_resources/records/mappings/os-v1/users/user-v1.0.0.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:29:19.000000 invenio-users-resources-2.0.1/invenio_users_resources/records/mappings/os-v2/
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-07-05 14:29:11.000000 invenio-users-resources-2.0.1/invenio_users_resources/records/mappings/os-v2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:29:19.000000 invenio-users-resources-2.0.1/invenio_users_resources/records/mappings/os-v2/groups/
+-rw-r--r--   0 runner    (1001) docker     (123)      695 2023-07-05 14:29:11.000000 invenio-users-resources-2.0.1/invenio_users_resources/records/mappings/os-v2/groups/group-v1.0.0.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:29:19.000000 invenio-users-resources-2.0.1/invenio_users_resources/records/mappings/os-v2/users/
+-rw-r--r--   0 runner    (1001) docker     (123)     1995 2023-07-05 14:29:11.000000 invenio-users-resources-2.0.1/invenio_users_resources/records/mappings/os-v2/users/user-v1.0.0.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:29:19.000000 invenio-users-resources-2.0.1/invenio_users_resources/records/mappings/v7/
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-07-05 14:29:11.000000 invenio-users-resources-2.0.1/invenio_users_resources/records/mappings/v7/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:29:19.000000 invenio-users-resources-2.0.1/invenio_users_resources/records/mappings/v7/groups/
+-rw-r--r--   0 runner    (1001) docker     (123)      695 2023-07-05 14:29:11.000000 invenio-users-resources-2.0.1/invenio_users_resources/records/mappings/v7/groups/group-v1.0.0.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:29:19.000000 invenio-users-resources-2.0.1/invenio_users_resources/records/mappings/v7/users/
+-rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-07-05 14:29:11.000000 invenio-users-resources-2.0.1/invenio_users_resources/records/mappings/v7/users/user-v1.0.0.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2870 2023-07-05 14:29:11.000000 invenio-users-resources-2.0.1/invenio_users_resources/records/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:29:19.000000 invenio-users-resources-2.0.1/invenio_users_resources/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)      488 2023-07-05 14:29:11.000000 invenio-users-resources-2.0.1/invenio_users_resources/resources/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:29:19.000000 invenio-users-resources-2.0.1/invenio_users_resources/resources/groups/
+-rw-r--r--   0 runner    (1001) docker     (123)      402 2023-07-05 14:29:11.000000 invenio-users-resources-2.0.1/invenio_users_resources/resources/groups/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      981 2023-07-05 14:29:11.000000 invenio-users-resources-2.0.1/invenio_users_resources/resources/groups/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2230 2023-07-05 14:29:11.000000 invenio-users-resources-2.0.1/invenio_users_resources/resources/groups/resource.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:29:19.000000 invenio-users-resources-2.0.1/invenio_users_resources/resources/users/
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-07-05 14:29:11.000000 invenio-users-resources-2.0.1/invenio_users_resources/resources/users/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      801 2023-07-05 14:29:11.000000 invenio-users-resources-2.0.1/invenio_users_resources/resources/users/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2323 2023-07-05 14:29:11.000000 invenio-users-resources-2.0.1/invenio_users_resources/resources/users/resource.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:29:19.000000 invenio-users-resources-2.0.1/invenio_users_resources/services/
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-07-05 14:29:11.000000 invenio-users-resources-2.0.1/invenio_users_resources/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-07-05 14:29:11.000000 invenio-users-resources-2.0.1/invenio_users_resources/services/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3523 2023-07-05 14:29:11.000000 invenio-users-resources-2.0.1/invenio_users_resources/services/generators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:29:19.000000 invenio-users-resources-2.0.1/invenio_users_resources/services/groups/
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-07-05 14:29:11.000000 invenio-users-resources-2.0.1/invenio_users_resources/services/groups/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2331 2023-07-05 14:29:11.000000 invenio-users-resources-2.0.1/invenio_users_resources/services/groups/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3453 2023-07-05 14:29:11.000000 invenio-users-resources-2.0.1/invenio_users_resources/services/groups/results.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1975 2023-07-05 14:29:11.000000 invenio-users-resources-2.0.1/invenio_users_resources/services/groups/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-07-05 14:29:11.000000 invenio-users-resources-2.0.1/invenio_users_resources/services/groups/tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      868 2023-07-05 14:29:11.000000 invenio-users-resources-2.0.1/invenio_users_resources/services/params.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1283 2023-07-05 14:29:11.000000 invenio-users-resources-2.0.1/invenio_users_resources/services/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1711 2023-07-05 14:29:11.000000 invenio-users-resources-2.0.1/invenio_users_resources/services/results.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3287 2023-07-05 14:29:11.000000 invenio-users-resources-2.0.1/invenio_users_resources/services/schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:29:19.000000 invenio-users-resources-2.0.1/invenio_users_resources/services/users/
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-07-05 14:29:11.000000 invenio-users-resources-2.0.1/invenio_users_resources/services/users/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2522 2023-07-05 14:29:11.000000 invenio-users-resources-2.0.1/invenio_users_resources/services/users/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3396 2023-07-05 14:29:11.000000 invenio-users-resources-2.0.1/invenio_users_resources/services/users/results.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3407 2023-07-05 14:29:11.000000 invenio-users-resources-2.0.1/invenio_users_resources/services/users/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1886 2023-07-05 14:29:11.000000 invenio-users-resources-2.0.1/invenio_users_resources/services/users/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:29:19.000000 invenio-users-resources-2.0.1/invenio_users_resources/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-07-05 14:29:11.000000 invenio-users-resources-2.0.1/invenio_users_resources/templates/avatar.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:29:19.000000 invenio-users-resources-2.0.1/invenio_users_resources/templates/semantic-ui/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:29:19.000000 invenio-users-resources-2.0.1/invenio_users_resources/templates/semantic-ui/invenio_users_resources/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:29:19.000000 invenio-users-resources-2.0.1/invenio_users_resources/templates/semantic-ui/invenio_users_resources/settings/
+-rw-r--r--   0 runner    (1001) docker     (123)     2731 2023-07-05 14:29:11.000000 invenio-users-resources-2.0.1/invenio_users_resources/templates/semantic-ui/invenio_users_resources/settings/notifications.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:29:19.000000 invenio-users-resources-2.0.1/invenio_users_resources/translations/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:29:19.000000 invenio-users-resources-2.0.1/invenio_users_resources/translations/af/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:29:19.000000 invenio-users-resources-2.0.1/invenio_users_resources/translations/af/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-07-05 14:29:19.000000 invenio-users-resources-2.0.1/invenio_users_resources/translations/af/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-07-05 14:29:11.000000 invenio-users-resources-2.0.1/invenio_users_resources/translations/af/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:29:19.000000 invenio-users-resources-2.0.1/invenio_users_resources/translations/ar/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:29:19.000000 invenio-users-resources-2.0.1/invenio_users_resources/translations/ar/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      846 2023-07-05 14:29:19.000000 invenio-users-resources-2.0.1/invenio_users_resources/translations/ar/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-07-05 14:29:11.000000 invenio-users-resources-2.0.1/invenio_users_resources/translations/ar/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:29:19.000000 invenio-users-resources-2.0.1/invenio_users_resources/translations/bg/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:29:19.000000 invenio-users-resources-2.0.1/invenio_users_resources/translations/bg/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-07-05 14:29:19.000000 invenio-users-resources-2.0.1/invenio_users_resources/translations/bg/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-07-05 14:29:11.000000 invenio-users-resources-2.0.1/invenio_users_resources/translations/bg/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:29:19.000000 invenio-users-resources-2.0.1/invenio_users_resources/translations/ca/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:29:19.000000 invenio-users-resources-2.0.1/invenio_users_resources/translations/ca/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      562 2023-07-05 14:29:19.000000 invenio-users-resources-2.0.1/invenio_users_resources/translations/ca/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-07-05 14:29:11.000000 invenio-users-resources-2.0.1/invenio_users_resources/translations/ca/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:29:19.000000 invenio-users-resources-2.0.1/invenio_users_resources/translations/cs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:29:19.000000 invenio-users-resources-2.0.1/invenio_users_resources/translations/cs/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-07-05 14:29:19.000000 invenio-users-resources-2.0.1/invenio_users_resources/translations/cs/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-07-05 14:29:11.000000 invenio-users-resources-2.0.1/invenio_users_resources/translations/cs/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:29:19.000000 invenio-users-resources-2.0.1/invenio_users_resources/translations/da/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:29:19.000000 invenio-users-resources-2.0.1/invenio_users_resources/translations/da/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      522 2023-07-05 14:29:19.000000 invenio-users-resources-2.0.1/invenio_users_resources/translations/da/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)      999 2023-07-05 14:29:11.000000 invenio-users-resources-2.0.1/invenio_users_resources/translations/da/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:29:19.000000 invenio-users-resources-2.0.1/invenio_users_resources/translations/de/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:29:19.000000 invenio-users-resources-2.0.1/invenio_users_resources/translations/de/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-07-05 14:29:19.000000 invenio-users-resources-2.0.1/invenio_users_resources/translations/de/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-07-05 14:29:11.000000 invenio-users-resources-2.0.1/invenio_users_resources/translations/de/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:29:19.000000 invenio-users-resources-2.0.1/invenio_users_resources/translations/de_AT/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:29:19.000000 invenio-users-resources-2.0.1/invenio_users_resources/translations/de_AT/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      538 2023-07-05 14:29:19.000000 invenio-users-resources-2.0.1/invenio_users_resources/translations/de_AT/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-07-05 14:29:11.000000 invenio-users-resources-2.0.1/invenio_users_resources/translations/de_AT/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:29:19.000000 invenio-users-resources-2.0.1/invenio_users_resources/translations/de_DE/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:29:19.000000 invenio-users-resources-2.0.1/invenio_users_resources/translations/de_DE/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      538 2023-07-05 14:29:19.000000 invenio-users-resources-2.0.1/invenio_users_resources/translations/de_DE/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-07-05 14:29:11.000000 invenio-users-resources-2.0.1/invenio_users_resources/translations/de_DE/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:29:19.000000 invenio-users-resources-2.0.1/invenio_users_resources/translations/el/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:29:19.000000 invenio-users-resources-2.0.1/invenio_users_resources/translations/el/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-07-05 14:29:19.000000 invenio-users-resources-2.0.1/invenio_users_resources/translations/el/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-07-05 14:29:11.000000 invenio-users-resources-2.0.1/invenio_users_resources/translations/el/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:29:19.000000 invenio-users-resources-2.0.1/invenio_users_resources/translations/en_AT/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:29:19.000000 invenio-users-resources-2.0.1/invenio_users_resources/translations/en_AT/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2023-07-05 14:29:19.000000 invenio-users-resources-2.0.1/invenio_users_resources/translations/en_AT/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-07-05 14:29:11.000000 invenio-users-resources-2.0.1/invenio_users_resources/translations/en_AT/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:29:19.000000 invenio-users-resources-2.0.1/invenio_users_resources/translations/en_HU/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:29:19.000000 invenio-users-resources-2.0.1/invenio_users_resources/translations/en_HU/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-07-05 14:29:19.000000 invenio-users-resources-2.0.1/invenio_users_resources/translations/en_HU/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-07-05 14:29:11.000000 invenio-users-resources-2.0.1/invenio_users_resources/translations/en_HU/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:29:19.000000 invenio-users-resources-2.0.1/invenio_users_resources/translations/es/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:29:19.000000 invenio-users-resources-2.0.1/invenio_users_resources/translations/es/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      763 2023-07-05 14:29:19.000000 invenio-users-resources-2.0.1/invenio_users_resources/translations/es/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1283 2023-07-05 14:29:11.000000 invenio-users-resources-2.0.1/invenio_users_resources/translations/es/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:29:19.000000 invenio-users-resources-2.0.1/invenio_users_resources/translations/es_CU/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:29:19.000000 invenio-users-resources-2.0.1/invenio_users_resources/translations/es_CU/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-07-05 14:29:19.000000 invenio-users-resources-2.0.1/invenio_users_resources/translations/es_CU/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-07-05 14:29:11.000000 invenio-users-resources-2.0.1/invenio_users_resources/translations/es_CU/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:29:19.000000 invenio-users-resources-2.0.1/invenio_users_resources/translations/es_MX/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:29:19.000000 invenio-users-resources-2.0.1/invenio_users_resources/translations/es_MX/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-07-05 14:29:19.000000 invenio-users-resources-2.0.1/invenio_users_resources/translations/es_MX/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-07-05 14:29:11.000000 invenio-users-resources-2.0.1/invenio_users_resources/translations/es_MX/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:29:19.000000 invenio-users-resources-2.0.1/invenio_users_resources/translations/et/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:29:19.000000 invenio-users-resources-2.0.1/invenio_users_resources/translations/et/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-07-05 14:29:19.000000 invenio-users-resources-2.0.1/invenio_users_resources/translations/et/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-07-05 14:29:11.000000 invenio-users-resources-2.0.1/invenio_users_resources/translations/et/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:29:19.000000 invenio-users-resources-2.0.1/invenio_users_resources/translations/et_EE/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:29:19.000000 invenio-users-resources-2.0.1/invenio_users_resources/translations/et_EE/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-07-05 14:29:19.000000 invenio-users-resources-2.0.1/invenio_users_resources/translations/et_EE/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-07-05 14:29:11.000000 invenio-users-resources-2.0.1/invenio_users_resources/translations/et_EE/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:29:19.000000 invenio-users-resources-2.0.1/invenio_users_resources/translations/fa/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:29:19.000000 invenio-users-resources-2.0.1/invenio_users_resources/translations/fa/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-07-05 14:29:19.000000 invenio-users-resources-2.0.1/invenio_users_resources/translations/fa/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-07-05 14:29:11.000000 invenio-users-resources-2.0.1/invenio_users_resources/translations/fa/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:29:19.000000 invenio-users-resources-2.0.1/invenio_users_resources/translations/fa_IR/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:29:19.000000 invenio-users-resources-2.0.1/invenio_users_resources/translations/fa_IR/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-07-05 14:29:19.000000 invenio-users-resources-2.0.1/invenio_users_resources/translations/fa_IR/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-07-05 14:29:11.000000 invenio-users-resources-2.0.1/invenio_users_resources/translations/fa_IR/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:29:19.000000 invenio-users-resources-2.0.1/invenio_users_resources/translations/fr/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:29:19.000000 invenio-users-resources-2.0.1/invenio_users_resources/translations/fr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      614 2023-07-05 14:29:19.000000 invenio-users-resources-2.0.1/invenio_users_resources/translations/fr/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-07-05 14:29:11.000000 invenio-users-resources-2.0.1/invenio_users_resources/translations/fr/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:29:19.000000 invenio-users-resources-2.0.1/invenio_users_resources/translations/fr_CI/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:29:19.000000 invenio-users-resources-2.0.1/invenio_users_resources/translations/fr_CI/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-07-05 14:29:19.000000 invenio-users-resources-2.0.1/invenio_users_resources/translations/fr_CI/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-07-05 14:29:11.000000 invenio-users-resources-2.0.1/invenio_users_resources/translations/fr_CI/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:29:19.000000 invenio-users-resources-2.0.1/invenio_users_resources/translations/fr_FR/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:29:19.000000 invenio-users-resources-2.0.1/invenio_users_resources/translations/fr_FR/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-07-05 14:29:19.000000 invenio-users-resources-2.0.1/invenio_users_resources/translations/fr_FR/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-07-05 14:29:11.000000 invenio-users-resources-2.0.1/invenio_users_resources/translations/fr_FR/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:29:19.000000 invenio-users-resources-2.0.1/invenio_users_resources/translations/gl/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:29:19.000000 invenio-users-resources-2.0.1/invenio_users_resources/translations/gl/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2023-07-05 14:29:19.000000 invenio-users-resources-2.0.1/invenio_users_resources/translations/gl/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-07-05 14:29:11.000000 invenio-users-resources-2.0.1/invenio_users_resources/translations/gl/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:29:19.000000 invenio-users-resources-2.0.1/invenio_users_resources/translations/hi_IN/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:29:19.000000 invenio-users-resources-2.0.1/invenio_users_resources/translations/hi_IN/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-07-05 14:29:19.000000 invenio-users-resources-2.0.1/invenio_users_resources/translations/hi_IN/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-07-05 14:29:11.000000 invenio-users-resources-2.0.1/invenio_users_resources/translations/hi_IN/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:29:19.000000 invenio-users-resources-2.0.1/invenio_users_resources/translations/hr/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:29:19.000000 invenio-users-resources-2.0.1/invenio_users_resources/translations/hr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      635 2023-07-05 14:29:19.000000 invenio-users-resources-2.0.1/invenio_users_resources/translations/hr/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-07-05 14:29:11.000000 invenio-users-resources-2.0.1/invenio_users_resources/translations/hr/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:29:19.000000 invenio-users-resources-2.0.1/invenio_users_resources/translations/hu/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:29:19.000000 invenio-users-resources-2.0.1/invenio_users_resources/translations/hu/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      707 2023-07-05 14:29:19.000000 invenio-users-resources-2.0.1/invenio_users_resources/translations/hu/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-07-05 14:29:11.000000 invenio-users-resources-2.0.1/invenio_users_resources/translations/hu/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:29:19.000000 invenio-users-resources-2.0.1/invenio_users_resources/translations/hu_HU/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:29:19.000000 invenio-users-resources-2.0.1/invenio_users_resources/translations/hu_HU/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      541 2023-07-05 14:29:19.000000 invenio-users-resources-2.0.1/invenio_users_resources/translations/hu_HU/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-07-05 14:29:11.000000 invenio-users-resources-2.0.1/invenio_users_resources/translations/hu_HU/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:29:19.000000 invenio-users-resources-2.0.1/invenio_users_resources/translations/it/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:29:19.000000 invenio-users-resources-2.0.1/invenio_users_resources/translations/it/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-07-05 14:29:19.000000 invenio-users-resources-2.0.1/invenio_users_resources/translations/it/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-07-05 14:29:11.000000 invenio-users-resources-2.0.1/invenio_users_resources/translations/it/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:29:19.000000 invenio-users-resources-2.0.1/invenio_users_resources/translations/ja/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:29:19.000000 invenio-users-resources-2.0.1/invenio_users_resources/translations/ja/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-07-05 14:29:19.000000 invenio-users-resources-2.0.1/invenio_users_resources/translations/ja/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-07-05 14:29:11.000000 invenio-users-resources-2.0.1/invenio_users_resources/translations/ja/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:29:19.000000 invenio-users-resources-2.0.1/invenio_users_resources/translations/ka/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:29:19.000000 invenio-users-resources-2.0.1/invenio_users_resources/translations/ka/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-07-05 14:29:19.000000 invenio-users-resources-2.0.1/invenio_users_resources/translations/ka/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-07-05 14:29:11.000000 invenio-users-resources-2.0.1/invenio_users_resources/translations/ka/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:29:19.000000 invenio-users-resources-2.0.1/invenio_users_resources/translations/lt/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:29:19.000000 invenio-users-resources-2.0.1/invenio_users_resources/translations/lt/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      704 2023-07-05 14:29:19.000000 invenio-users-resources-2.0.1/invenio_users_resources/translations/lt/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1266 2023-07-05 14:29:11.000000 invenio-users-resources-2.0.1/invenio_users_resources/translations/lt/LC_MESSAGES/messages.po
+-rw-r--r--   0 runner    (1001) docker     (123)      936 2023-07-05 14:29:11.000000 invenio-users-resources-2.0.1/invenio_users_resources/translations/messages.pot
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:29:19.000000 invenio-users-resources-2.0.1/invenio_users_resources/translations/ne/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:29:19.000000 invenio-users-resources-2.0.1/invenio_users_resources/translations/ne/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      522 2023-07-05 14:29:19.000000 invenio-users-resources-2.0.1/invenio_users_resources/translations/ne/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)      999 2023-07-05 14:29:11.000000 invenio-users-resources-2.0.1/invenio_users_resources/translations/ne/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:29:19.000000 invenio-users-resources-2.0.1/invenio_users_resources/translations/no/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:29:19.000000 invenio-users-resources-2.0.1/invenio_users_resources/translations/no/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      565 2023-07-05 14:29:19.000000 invenio-users-resources-2.0.1/invenio_users_resources/translations/no/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-07-05 14:29:11.000000 invenio-users-resources-2.0.1/invenio_users_resources/translations/no/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:29:19.000000 invenio-users-resources-2.0.1/invenio_users_resources/translations/pl/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:29:19.000000 invenio-users-resources-2.0.1/invenio_users_resources/translations/pl/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-07-05 14:29:19.000000 invenio-users-resources-2.0.1/invenio_users_resources/translations/pl/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-07-05 14:29:11.000000 invenio-users-resources-2.0.1/invenio_users_resources/translations/pl/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:29:19.000000 invenio-users-resources-2.0.1/invenio_users_resources/translations/pt/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:29:19.000000 invenio-users-resources-2.0.1/invenio_users_resources/translations/pt/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-07-05 14:29:19.000000 invenio-users-resources-2.0.1/invenio_users_resources/translations/pt/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-07-05 14:29:11.000000 invenio-users-resources-2.0.1/invenio_users_resources/translations/pt/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:29:19.000000 invenio-users-resources-2.0.1/invenio_users_resources/translations/ro/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:29:19.000000 invenio-users-resources-2.0.1/invenio_users_resources/translations/ro/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      725 2023-07-05 14:29:19.000000 invenio-users-resources-2.0.1/invenio_users_resources/translations/ro/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-07-05 14:29:11.000000 invenio-users-resources-2.0.1/invenio_users_resources/translations/ro/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:29:19.000000 invenio-users-resources-2.0.1/invenio_users_resources/translations/ru/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:29:19.000000 invenio-users-resources-2.0.1/invenio_users_resources/translations/ru/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2023-07-05 14:29:19.000000 invenio-users-resources-2.0.1/invenio_users_resources/translations/ru/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-07-05 14:29:11.000000 invenio-users-resources-2.0.1/invenio_users_resources/translations/ru/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:29:19.000000 invenio-users-resources-2.0.1/invenio_users_resources/translations/rw/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:29:19.000000 invenio-users-resources-2.0.1/invenio_users_resources/translations/rw/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      527 2023-07-05 14:29:19.000000 invenio-users-resources-2.0.1/invenio_users_resources/translations/rw/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-07-05 14:29:11.000000 invenio-users-resources-2.0.1/invenio_users_resources/translations/rw/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:29:19.000000 invenio-users-resources-2.0.1/invenio_users_resources/translations/sk/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:29:19.000000 invenio-users-resources-2.0.1/invenio_users_resources/translations/sk/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      637 2023-07-05 14:29:19.000000 invenio-users-resources-2.0.1/invenio_users_resources/translations/sk/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-07-05 14:29:11.000000 invenio-users-resources-2.0.1/invenio_users_resources/translations/sk/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:29:19.000000 invenio-users-resources-2.0.1/invenio_users_resources/translations/sv/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:29:19.000000 invenio-users-resources-2.0.1/invenio_users_resources/translations/sv/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      710 2023-07-05 14:29:19.000000 invenio-users-resources-2.0.1/invenio_users_resources/translations/sv/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-07-05 14:29:11.000000 invenio-users-resources-2.0.1/invenio_users_resources/translations/sv/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:29:19.000000 invenio-users-resources-2.0.1/invenio_users_resources/translations/sv_SE/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:29:19.000000 invenio-users-resources-2.0.1/invenio_users_resources/translations/sv_SE/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      538 2023-07-05 14:29:19.000000 invenio-users-resources-2.0.1/invenio_users_resources/translations/sv_SE/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-07-05 14:29:11.000000 invenio-users-resources-2.0.1/invenio_users_resources/translations/sv_SE/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:29:19.000000 invenio-users-resources-2.0.1/invenio_users_resources/translations/tr/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:29:19.000000 invenio-users-resources-2.0.1/invenio_users_resources/translations/tr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-07-05 14:29:19.000000 invenio-users-resources-2.0.1/invenio_users_resources/translations/tr/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-07-05 14:29:11.000000 invenio-users-resources-2.0.1/invenio_users_resources/translations/tr/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:29:19.000000 invenio-users-resources-2.0.1/invenio_users_resources/translations/uk/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:29:19.000000 invenio-users-resources-2.0.1/invenio_users_resources/translations/uk/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      868 2023-07-05 14:29:19.000000 invenio-users-resources-2.0.1/invenio_users_resources/translations/uk/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-07-05 14:29:11.000000 invenio-users-resources-2.0.1/invenio_users_resources/translations/uk/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:29:19.000000 invenio-users-resources-2.0.1/invenio_users_resources/translations/uk_UA/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:29:19.000000 invenio-users-resources-2.0.1/invenio_users_resources/translations/uk_UA/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      763 2023-07-05 14:29:19.000000 invenio-users-resources-2.0.1/invenio_users_resources/translations/uk_UA/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-07-05 14:29:11.000000 invenio-users-resources-2.0.1/invenio_users_resources/translations/uk_UA/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:29:19.000000 invenio-users-resources-2.0.1/invenio_users_resources/translations/zh_CN/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:29:19.000000 invenio-users-resources-2.0.1/invenio_users_resources/translations/zh_CN/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      702 2023-07-05 14:29:19.000000 invenio-users-resources-2.0.1/invenio_users_resources/translations/zh_CN/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-07-05 14:29:11.000000 invenio-users-resources-2.0.1/invenio_users_resources/translations/zh_CN/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:29:19.000000 invenio-users-resources-2.0.1/invenio_users_resources/translations/zh_TW/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:29:19.000000 invenio-users-resources-2.0.1/invenio_users_resources/translations/zh_TW/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-07-05 14:29:19.000000 invenio-users-resources-2.0.1/invenio_users_resources/translations/zh_TW/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-07-05 14:29:11.000000 invenio-users-resources-2.0.1/invenio_users_resources/translations/zh_TW/LC_MESSAGES/messages.po
+-rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-07-05 14:29:11.000000 invenio-users-resources-2.0.1/invenio_users_resources/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:29:19.000000 invenio-users-resources-2.0.1/invenio_users_resources.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4183 2023-07-05 14:29:19.000000 invenio-users-resources-2.0.1/invenio_users_resources.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9840 2023-07-05 14:29:19.000000 invenio-users-resources-2.0.1/invenio_users_resources.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 14:29:19.000000 invenio-users-resources-2.0.1/invenio_users_resources.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-07-05 14:29:19.000000 invenio-users-resources-2.0.1/invenio_users_resources.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 14:29:19.000000 invenio-users-resources-2.0.1/invenio_users_resources.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-07-05 14:29:19.000000 invenio-users-resources-2.0.1/invenio_users_resources.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-05 14:29:19.000000 invenio-users-resources-2.0.1/invenio_users_resources.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-05 14:29:11.000000 invenio-users-resources-2.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-07-05 14:29:11.000000 invenio-users-resources-2.0.1/requirements-devel.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1401 2023-07-05 14:29:11.000000 invenio-users-resources-2.0.1/run-tests.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     2878 2023-07-05 14:29:19.000000 invenio-users-resources-2.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-07-05 14:29:11.000000 invenio-users-resources-2.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:29:19.000000 invenio-users-resources-2.0.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     7924 2023-07-05 14:29:11.000000 invenio-users-resources-2.0.1/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:29:19.000000 invenio-users-resources-2.0.1/tests/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-07-05 14:29:11.000000 invenio-users-resources-2.0.1/tests/resources/test_resources_groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2911 2023-07-05 14:29:11.000000 invenio-users-resources-2.0.1/tests/resources/test_resources_users.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:29:19.000000 invenio-users-resources-2.0.1/tests/services/
+-rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-07-05 14:29:11.000000 invenio-users-resources-2.0.1/tests/services/test_service_groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3967 2023-07-05 14:29:11.000000 invenio-users-resources-2.0.1/tests/services/test_service_users.py
+-rw-r--r--   0 runner    (1001) docker     (123)      830 2023-07-05 14:29:11.000000 invenio-users-resources-2.0.1/tests/test_invenio_users_resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2801 2023-07-05 14:29:11.000000 invenio-users-resources-2.0.1/tests/test_notifications.py
```

### Comparing `invenio-users-resources-2.0.0/.editorconfig` & `invenio-users-resources-2.0.1/.editorconfig`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-2.0.0/.github/workflows/pypi-publish.yml` & `invenio-users-resources-2.0.1/.github/workflows/pypi-publish.yml`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-2.0.0/.github/workflows/tests.yml` & `invenio-users-resources-2.0.1/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-2.0.0/.tx/config` & `invenio-users-resources-2.0.1/.tx/config`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # -*- coding: utf-8 -*-
 #
 # Copyright (C) 2022 CERN.
+# Copyright (C) 2023 Graz University of Technology.
 #
 # Invenio-Users-Resources is free software; you can redistribute it and/or
 # modify it under the terms of the MIT License; see LICENSE file for more
 # details.
 
 #
 # 1) Create message catalog:
@@ -19,14 +20,14 @@
 #    $ tx push -s -t
 # 5) Pull translations for a single language from Transifex
 #    $ tx pull -l <lang>
 # 6) Pull translations for all languages from Transifex
 #    $ tx pull -a
 
 [main]
-host = https://www.transifex.com
+host = https://app.transifex.com
 
-[invenio.invenio-users-resources-messages]
+[o:inveniosoftware:p:invenio:r:invenio-users-resources-messages]
 file_filter = invenio_users_resources/translations/<lang>/LC_MESSAGES/messages.po
 source_file = invenio_users_resources/translations/messages.pot
 source_lang = en
 type = PO
```

### Comparing `invenio-users-resources-2.0.0/CHANGES.rst` & `invenio-users-resources-2.0.1/CHANGES.rst`

 * *Files 9% similar despite different names*

```diff
@@ -4,14 +4,19 @@
     Invenio-Users-Resources is free software; you can redistribute it
     and/or modify it under the terms of the MIT License; see LICENSE file for
     more details.
 
 Changes
 =======
 
+Version 2.0.1 (2023-07-05)
+
+- fix post_commit hooks
+- add translations
+
 Version 2.0.0 (2023-06-30)
 
 - changing the groups tasks interface to use bulk indexing as default
 
 Version 1.9.0 (2023-06-15)
 
 - groups: add description field
```

### Comparing `invenio-users-resources-2.0.0/CONTRIBUTING.rst` & `invenio-users-resources-2.0.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-2.0.0/LICENSE` & `invenio-users-resources-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-2.0.0/MANIFEST.in` & `invenio-users-resources-2.0.1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-2.0.0/PKG-INFO` & `invenio-users-resources-2.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invenio-users-resources
-Version: 2.0.0
+Version: 2.0.1
 Summary: Invenio module providing management APIs for users and roles/groups.
 Home-page: https://github.com/inveniosoftware/invenio-users-resources
 Author: CERN/TU Wien/JRC
 Author-email: info@inveniosoftware.org
 License: MIT
 Description: ..
             Copyright (C) 2022 CERN.
@@ -42,14 +42,19 @@
             Invenio-Users-Resources is free software; you can redistribute it
             and/or modify it under the terms of the MIT License; see LICENSE file for
             more details.
         
         Changes
         =======
         
+        Version 2.0.1 (2023-07-05)
+        
+        - fix post_commit hooks
+        - add translations
+        
         Version 2.0.0 (2023-06-30)
         
         - changing the groups tasks interface to use bulk indexing as default
         
         Version 1.9.0 (2023-06-15)
         
         - groups: add description field
```

### Comparing `invenio-users-resources-2.0.0/README.rst` & `invenio-users-resources-2.0.1/README.rst`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-2.0.0/docs/Makefile` & `invenio-users-resources-2.0.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-2.0.0/docs/conf.py` & `invenio-users-resources-2.0.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-2.0.0/docs/index.rst` & `invenio-users-resources-2.0.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-2.0.0/docs/make.bat` & `invenio-users-resources-2.0.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-2.0.0/invenio_users_resources/config.py` & `invenio-users-resources-2.0.1/invenio_users_resources/config.py`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-2.0.0/invenio_users_resources/entity_resolvers.py` & `invenio-users-resources-2.0.1/invenio_users_resources/entity_resolvers.py`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-2.0.0/invenio_users_resources/ext.py` & `invenio-users-resources-2.0.1/invenio_users_resources/ext.py`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-2.0.0/invenio_users_resources/forms.py` & `invenio-users-resources-2.0.1/invenio_users_resources/forms.py`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-2.0.0/invenio_users_resources/models.py` & `invenio-users-resources-2.0.1/invenio_users_resources/models.py`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-2.0.0/invenio_users_resources/notifications/filters.py` & `invenio-users-resources-2.0.1/invenio_users_resources/notifications/filters.py`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-2.0.0/invenio_users_resources/notifications/generators.py` & `invenio-users-resources-2.0.1/invenio_users_resources/notifications/generators.py`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-2.0.0/invenio_users_resources/proxies.py` & `invenio-users-resources-2.0.1/invenio_users_resources/proxies.py`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-2.0.0/invenio_users_resources/records/api.py` & `invenio-users-resources-2.0.1/invenio_users_resources/records/api.py`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-2.0.0/invenio_users_resources/records/dumpers/email.py` & `invenio-users-resources-2.0.1/invenio_users_resources/records/dumpers/email.py`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-2.0.0/invenio_users_resources/records/hooks.py` & `invenio-users-resources-2.0.1/invenio_users_resources/records/hooks.py`

 * *Files 9% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 # details.
 
 """Invenio users DB hooks."""
 
 from invenio_accounts.models import Role, User
 from invenio_accounts.proxies import current_db_change_history
 
-from ..proxies import current_groups_service, current_users_service
 from ..services.groups.tasks import reindex_groups, unindex_groups
 from ..services.users.tasks import reindex_users, unindex_users
 
 
 def pre_commit(sender, session):
     """Find out which entities need indexing before commit."""
     # it seems that the {dirty,new,deleted} sets aren't populated
@@ -50,19 +49,19 @@
     # since this function is called after the commit, no more
     # DB operations are allowed here, not even lazy-loading of
     # properties!
     sid = id(session)
 
     if current_db_change_history.sessions.get(sid):
         # Handle updates
-        current_session = list(current_db_change_history.sessions[sid].updated_users)
-        current_users_service.indexer.bulk_index(current_session)
+        user_ids_updated = list(current_db_change_history.sessions[sid].updated_users)
+        reindex_users.delay(user_ids_updated)
 
         group_ids_updated = list(current_db_change_history.sessions[sid].updated_roles)
-        current_groups_service.indexer.bulk_index(group_ids_updated)
+        reindex_groups.delay(group_ids_updated)
 
         # Handle deletes
         user_ids_deleted = list(current_db_change_history.sessions[sid].deleted_users)
-        current_users_service.indexer.bulk_delete(user_ids_deleted)
+        unindex_users.delay(user_ids_deleted)
 
         group_ids_deleted = list(current_db_change_history.sessions[sid].deleted_roles)
-        current_groups_service.indexer.bulk_delete(group_ids_deleted)
+        unindex_groups.delay(group_ids_deleted)
```

### Comparing `invenio-users-resources-2.0.0/invenio_users_resources/records/mappings/os-v1/groups/group-v1.0.0.json` & `invenio-users-resources-2.0.1/invenio_users_resources/records/mappings/os-v1/groups/group-v1.0.0.json`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-2.0.0/invenio_users_resources/records/mappings/os-v1/users/user-v1.0.0.json` & `invenio-users-resources-2.0.1/invenio_users_resources/records/mappings/os-v1/users/user-v1.0.0.json`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-2.0.0/invenio_users_resources/records/mappings/os-v2/groups/group-v1.0.0.json` & `invenio-users-resources-2.0.1/invenio_users_resources/records/mappings/os-v2/groups/group-v1.0.0.json`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-2.0.0/invenio_users_resources/records/mappings/os-v2/users/user-v1.0.0.json` & `invenio-users-resources-2.0.1/invenio_users_resources/records/mappings/os-v2/users/user-v1.0.0.json`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-2.0.0/invenio_users_resources/records/mappings/v7/groups/group-v1.0.0.json` & `invenio-users-resources-2.0.1/invenio_users_resources/records/mappings/v7/groups/group-v1.0.0.json`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-2.0.0/invenio_users_resources/records/mappings/v7/users/user-v1.0.0.json` & `invenio-users-resources-2.0.1/invenio_users_resources/records/mappings/v7/users/user-v1.0.0.json`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-2.0.0/invenio_users_resources/records/models.py` & `invenio-users-resources-2.0.1/invenio_users_resources/records/models.py`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-2.0.0/invenio_users_resources/resources/groups/config.py` & `invenio-users-resources-2.0.1/invenio_users_resources/resources/groups/config.py`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-2.0.0/invenio_users_resources/resources/groups/resource.py` & `invenio-users-resources-2.0.1/invenio_users_resources/resources/groups/resource.py`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-2.0.0/invenio_users_resources/resources/users/config.py` & `invenio-users-resources-2.0.1/invenio_users_resources/resources/users/config.py`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-2.0.0/invenio_users_resources/resources/users/resource.py` & `invenio-users-resources-2.0.1/invenio_users_resources/resources/users/resource.py`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-2.0.0/invenio_users_resources/services/common.py` & `invenio-users-resources-2.0.1/invenio_users_resources/services/common.py`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-2.0.0/invenio_users_resources/services/generators.py` & `invenio-users-resources-2.0.1/invenio_users_resources/services/generators.py`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-2.0.0/invenio_users_resources/services/groups/config.py` & `invenio-users-resources-2.0.1/invenio_users_resources/services/groups/config.py`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-2.0.0/invenio_users_resources/services/groups/results.py` & `invenio-users-resources-2.0.1/invenio_users_resources/services/groups/results.py`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-2.0.0/invenio_users_resources/services/groups/service.py` & `invenio-users-resources-2.0.1/invenio_users_resources/services/groups/service.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 # Invenio-Users-Resources is free software; you can redistribute it and/or
 # modify it under the terms of the MIT License; see LICENSE file for more
 # details.
 
 """Groups service."""
 
 from invenio_accounts.models import Role
+from invenio_db import db
 from invenio_records_resources.resources.errors import PermissionDeniedError
 from invenio_records_resources.services import RecordService
 
 from ...records.api import GroupAggregate
 from ..results import AvatarResult
 
 
@@ -46,11 +47,12 @@
             # return 403 even on empty resource due to security implications
             raise PermissionDeniedError()
         self.require_permission(identity, "read", record=group)
         return AvatarResult(group)
 
     def rebuild_index(self, identity, uow=None):
         """Reindex all user groups managed by this service."""
-        roles = Role.query.all()
+        roles = db.session.query(Role.id).yield_per(1000)
+
         self.indexer.bulk_index([r.id for r in roles])
 
         return True
```

### Comparing `invenio-users-resources-2.0.0/invenio_users_resources/services/groups/tasks.py` & `invenio-users-resources-2.0.1/invenio_users_resources/services/groups/tasks.py`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-2.0.0/invenio_users_resources/services/params.py` & `invenio-users-resources-2.0.1/invenio_users_resources/services/params.py`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-2.0.0/invenio_users_resources/services/permissions.py` & `invenio-users-resources-2.0.1/invenio_users_resources/services/permissions.py`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-2.0.0/invenio_users_resources/services/results.py` & `invenio-users-resources-2.0.1/invenio_users_resources/services/results.py`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-2.0.0/invenio_users_resources/services/schemas.py` & `invenio-users-resources-2.0.1/invenio_users_resources/services/schemas.py`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-2.0.0/invenio_users_resources/services/users/config.py` & `invenio-users-resources-2.0.1/invenio_users_resources/services/users/config.py`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-2.0.0/invenio_users_resources/services/users/results.py` & `invenio-users-resources-2.0.1/invenio_users_resources/services/users/results.py`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-2.0.0/invenio_users_resources/services/users/service.py` & `invenio-users-resources-2.0.1/invenio_users_resources/services/users/service.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 # Invenio-Users-Resources is free software; you can redistribute it and/or
 # modify it under the terms of the MIT License; see LICENSE file for more
 # details.
 
 """Users service."""
 
 from invenio_accounts.models import User
+from invenio_db import db
 from invenio_records_resources.resources.errors import PermissionDeniedError
 from invenio_records_resources.services import RecordService
 from invenio_records_resources.services.uow import RecordCommitOp, unit_of_work
 from invenio_search.engine import dsl
 
 from invenio_users_resources.services.results import AvatarResult
 
@@ -95,11 +96,10 @@
             # return 403 even on empty resource due to security implications
             raise PermissionDeniedError()
         self.require_permission(identity, "read", record=user)
         return AvatarResult(user)
 
     def rebuild_index(self, identity, uow=None):
         """Reindex all users managed by this service."""
-        users = User.query.all()
+        users = db.session.query(User.id).yield_per(1000)
         self.indexer.bulk_index([u.id for u in users])
-
         return True
```

### Comparing `invenio-users-resources-2.0.0/invenio_users_resources/services/users/tasks.py` & `invenio-users-resources-2.0.1/invenio_users_resources/services/users/tasks.py`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-2.0.0/invenio_users_resources/templates/semantic-ui/invenio_users_resources/settings/notifications.html` & `invenio-users-resources-2.0.1/invenio_users_resources/templates/semantic-ui/invenio_users_resources/settings/notifications.html`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-2.0.0/invenio_users_resources/translations/af/LC_MESSAGES/messages.mo` & `invenio-users-resources-2.0.1/invenio_users_resources/translations/af/LC_MESSAGES/messages.mo`

 * *Format-specific differences are supported for Gettext message catalogues but no file-specific differences were detected; falling back to a binary diff. file(1) reports: GNU message catalog (little endian), revision 0.0, 1 message, Project-Id-Version: invenio-users-resources 0.3.2*

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 000000c0: 6f6e 2d44 6174 653a 2032 3032 322d 3032  on-Date: 2022-02
 000000d0: 2d31 3620 3131 3a35 382b 3030 3030 0a4c  -16 11:58+0000.L
 000000e0: 6173 742d 5472 616e 736c 6174 6f72 3a20  ast-Translator: 
 000000f0: 4655 4c4c 204e 414d 4520 3c45 4d41 494c  FULL NAME <EMAIL
 00000100: 4041 4444 5245 5353 3e0a 4c61 6e67 7561  @ADDRESS>.Langua
 00000110: 6765 3a20 6166 0a4c 616e 6775 6167 652d  ge: af.Language-
 00000120: 5465 616d 3a20 4166 7269 6b61 616e 7320  Team: Afrikaans 
-00000130: 2868 7474 7073 3a2f 2f77 7777 2e74 7261  (https://www.tra
+00000130: 2868 7474 7073 3a2f 2f61 7070 2e74 7261  (https://app.tra
 00000140: 6e73 6966 6578 2e63 6f6d 2f69 6e76 656e  nsifex.com/inven
 00000150: 696f 736f 6674 7761 7265 2f74 6561 6d73  iosoftware/teams
 00000160: 2f32 3335 3337 2f61 662f 290a 506c 7572  /23537/af/).Plur
 00000170: 616c 2d46 6f72 6d73 3a20 6e70 6c75 7261  al-Forms: nplura
 00000180: 6c73 3d32 3b20 706c 7572 616c 3d28 6e20  ls=2; plural=(n 
 00000190: 213d 2031 293b 0a4d 494d 452d 5665 7273  != 1);.MIME-Vers
 000001a0: 696f 6e3a 2031 2e30 0a43 6f6e 7465 6e74  ion: 1.0.Content
```

### Comparing `invenio-users-resources-2.0.0/invenio_users_resources/translations/af/LC_MESSAGES/messages.po` & `invenio-users-resources-2.0.1/invenio_users_resources/translations/ca/LC_MESSAGES/messages.po`

 * *Files 11% similar despite different names*

```diff
@@ -1,32 +1,36 @@
 # Translations template for invenio-users-resources.
 # Copyright (C) 2022 CERN
 # This file is distributed under the same license as the
 # invenio-users-resources project.
 # FIRST AUTHOR <EMAIL@ADDRESS>, 2022.
 # 
+# Translators:
+# Tibor Simko <tibor.simko@cern.ch>, 2022
+# 
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-users-resources 0.3.2\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 12:12+0000\n"
 "PO-Revision-Date: 2022-02-16 11:58+0000\n"
-"Language-Team: Afrikaans (https://www.transifex.com/inveniosoftware/teams/23537/af/)\n"
+"Last-Translator: Tibor Simko <tibor.simko@cern.ch>, 2022\n"
+"Language-Team: Catalan (https://app.transifex.com/inveniosoftware/teams/23537/ca/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.3\n"
-"Language: af\n"
+"Language: ca\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
 #: invenio_users_resources/services/schemas.py:21
 msgid "Value must be either 'public' or 'restricted'."
 msgstr ""
 
 #: invenio_users_resources/services/groups/config.py:43
 msgid "Best match"
 msgstr ""
 
 #: invenio_users_resources/services/groups/config.py:47
 msgid "Name"
-msgstr ""
+msgstr "Nom"
```

### Comparing `invenio-users-resources-2.0.0/invenio_users_resources/translations/ar/LC_MESSAGES/messages.mo` & `invenio-users-resources-2.0.1/invenio_users_resources/translations/ar/LC_MESSAGES/messages.mo`

 * *Files 23% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,25 +1,25 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-users-resources 0.3.2\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 12:12+0000\n"
 "PO-Revision-Date: 2022-02-16 11:58+0000\n"
-"Last-Translator: Tibor Simko <tibor.simko@cern.ch>, 2022\n"
+"Last-Translator: Salaheddine Ben Ali <salaheddine.benali@cnudst.tn>, 2023\n"
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
 
 msgid "Name"
-msgstr "اسم"
+msgstr "إسم"
 
 msgid "Value must be either 'public' or 'restricted'."
-msgstr "يجب أن تكون القيمة إما \"عامة\" أو \"مقيدة\"."
+msgstr "يجب أن تكون القيمة إما 'عامة' أو 'مقيدة'."
```

### Comparing `invenio-users-resources-2.0.0/invenio_users_resources/translations/ar/LC_MESSAGES/messages.po` & `invenio-users-resources-2.0.1/invenio_users_resources/translations/hu/LC_MESSAGES/messages.po`

 * *Files 15% similar despite different names*

```diff
@@ -1,37 +1,36 @@
 # Translations template for invenio-users-resources.
 # Copyright (C) 2022 CERN
 # This file is distributed under the same license as the
 # invenio-users-resources project.
 # FIRST AUTHOR <EMAIL@ADDRESS>, 2022.
 # 
 # Translators:
-# Bessem Aamira <bessemamira@gmail.com>, 2022
-# Tibor Simko <tibor.simko@cern.ch>, 2022
+# Andrea Dömötör, 2022
 # 
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-users-resources 0.3.2\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 12:12+0000\n"
 "PO-Revision-Date: 2022-02-16 11:58+0000\n"
-"Last-Translator: Tibor Simko <tibor.simko@cern.ch>, 2022\n"
-"Language-Team: Arabic (https://www.transifex.com/inveniosoftware/teams/23537/ar/)\n"
+"Last-Translator: Andrea Dömötör, 2022\n"
+"Language-Team: Hungarian (https://app.transifex.com/inveniosoftware/teams/23537/hu/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.3\n"
-"Language: ar\n"
-"Plural-Forms: nplurals=6; plural=n==0 ? 0 : n==1 ? 1 : n==2 ? 2 : n%100>=3 && n%100<=10 ? 3 : n%100>=11 && n%100<=99 ? 4 : 5;\n"
+"Language: hu\n"
+"Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
 #: invenio_users_resources/services/schemas.py:21
 msgid "Value must be either 'public' or 'restricted'."
-msgstr "يجب أن تكون القيمة إما \"عامة\" أو \"مقيدة\"."
+msgstr "Az érték 'nyilvános' vagy 'korlátozott' lehet."
 
 #: invenio_users_resources/services/groups/config.py:43
 msgid "Best match"
-msgstr "أفضل تطابق "
+msgstr "Legjobb találat"
 
 #: invenio_users_resources/services/groups/config.py:47
 msgid "Name"
-msgstr "اسم"
+msgstr "Név"
```

### Comparing `invenio-users-resources-2.0.0/invenio_users_resources/translations/bg/LC_MESSAGES/messages.mo` & `invenio-users-resources-2.0.1/invenio_users_resources/translations/bg/LC_MESSAGES/messages.mo`

 * *Files 2% similar despite different names*

#### msgunfmt {}

```diff
@@ -2,15 +2,15 @@
 msgstr ""
 "Project-Id-Version: invenio-users-resources 0.3.2\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 12:12+0000\n"
 "PO-Revision-Date: 2022-02-16 11:58+0000\n"
 "Last-Translator: Tibor Simko <tibor.simko@cern.ch>, 2022\n"
 "Language: bg\n"
-"Language-Team: Bulgarian (https://www.transifex.com/inveniosoftware/"
+"Language-Team: Bulgarian (https://app.transifex.com/inveniosoftware/"
 "teams/23537/bg/)\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.12.1\n"
```

### Comparing `invenio-users-resources-2.0.0/invenio_users_resources/translations/bg/LC_MESSAGES/messages.po` & `invenio-users-resources-2.0.1/invenio_users_resources/translations/bg/LC_MESSAGES/messages.po`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-users-resources 0.3.2\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 12:12+0000\n"
 "PO-Revision-Date: 2022-02-16 11:58+0000\n"
 "Last-Translator: Tibor Simko <tibor.simko@cern.ch>, 2022\n"
-"Language-Team: Bulgarian (https://www.transifex.com/inveniosoftware/teams/23537/bg/)\n"
+"Language-Team: Bulgarian (https://app.transifex.com/inveniosoftware/teams/23537/bg/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.3\n"
 "Language: bg\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
```

### Comparing `invenio-users-resources-2.0.0/invenio_users_resources/translations/ca/LC_MESSAGES/messages.mo` & `invenio-users-resources-2.0.1/invenio_users_resources/translations/ca/LC_MESSAGES/messages.mo`

 * *Files 4% similar despite different names*

#### msgunfmt {}

```diff
@@ -2,15 +2,15 @@
 msgstr ""
 "Project-Id-Version: invenio-users-resources 0.3.2\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 12:12+0000\n"
 "PO-Revision-Date: 2022-02-16 11:58+0000\n"
 "Last-Translator: Tibor Simko <tibor.simko@cern.ch>, 2022\n"
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

### Comparing `invenio-users-resources-2.0.0/invenio_users_resources/translations/ca/LC_MESSAGES/messages.po` & `invenio-users-resources-2.0.1/invenio_users_resources/translations/ja/LC_MESSAGES/messages.po`

 * *Files 4% similar despite different names*

```diff
@@ -11,26 +11,26 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-users-resources 0.3.2\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 12:12+0000\n"
 "PO-Revision-Date: 2022-02-16 11:58+0000\n"
 "Last-Translator: Tibor Simko <tibor.simko@cern.ch>, 2022\n"
-"Language-Team: Catalan (https://www.transifex.com/inveniosoftware/teams/23537/ca/)\n"
+"Language-Team: Japanese (https://app.transifex.com/inveniosoftware/teams/23537/ja/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.3\n"
-"Language: ca\n"
-"Plural-Forms: nplurals=2; plural=(n != 1);\n"
+"Language: ja\n"
+"Plural-Forms: nplurals=1; plural=0;\n"
 
 #: invenio_users_resources/services/schemas.py:21
 msgid "Value must be either 'public' or 'restricted'."
 msgstr ""
 
 #: invenio_users_resources/services/groups/config.py:43
 msgid "Best match"
 msgstr ""
 
 #: invenio_users_resources/services/groups/config.py:47
 msgid "Name"
-msgstr "Nom"
+msgstr "名前"
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `invenio-users-resources-2.0.0/invenio_users_resources/translations/cs/LC_MESSAGES/messages.mo` & `invenio-users-resources-2.0.1/invenio_users_resources/translations/fr/LC_MESSAGES/messages.mo`

 * *Files 13% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,19 +1,19 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-users-resources 0.3.2\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 12:12+0000\n"
 "PO-Revision-Date: 2022-02-16 11:58+0000\n"
-"Last-Translator: Tibor Simko <tibor.simko@cern.ch>, 2022\n"
-"Language: cs\n"
-"Language-Team: Czech (https://www.transifex.com/inveniosoftware/teams/23537/"
-"cs/)\n"
-"Plural-Forms: nplurals=4; plural=(n == 1 && n % 1 == 0) ? 0 : (n >= 2 && n "
-"<= 4 && n % 1 == 0) ? 1: (n % 1 != 0 ) ? 2 : 3;\n"
+"Last-Translator: Alizee Pace <alizee.pace@gmail.com>, 2022\n"
+"Language: fr\n"
+"Language-Team: French (https://app.transifex.com/inveniosoftware/teams/23537/"
+"fr/)\n"
+"Plural-Forms: nplurals=3; plural=(n == 0 || n == 1) ? 0 : n != 0 && n % "
+"1000000 == 0 ? 1 : 2;\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.12.1\n"
 
 msgid "Name"
-msgstr "Název"
+msgstr "Nom"
```

### Comparing `invenio-users-resources-2.0.0/invenio_users_resources/translations/cs/LC_MESSAGES/messages.po` & `invenio-users-resources-2.0.1/invenio_users_resources/translations/cs/LC_MESSAGES/messages.po`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-users-resources 0.3.2\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 12:12+0000\n"
 "PO-Revision-Date: 2022-02-16 11:58+0000\n"
 "Last-Translator: Tibor Simko <tibor.simko@cern.ch>, 2022\n"
-"Language-Team: Czech (https://www.transifex.com/inveniosoftware/teams/23537/cs/)\n"
+"Language-Team: Czech (https://app.transifex.com/inveniosoftware/teams/23537/cs/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.3\n"
 "Language: cs\n"
 "Plural-Forms: nplurals=4; plural=(n == 1 && n % 1 == 0) ? 0 : (n >= 2 && n <= 4 && n % 1 == 0) ? 1: (n % 1 != 0 ) ? 2 : 3;\n"
```

### Comparing `invenio-users-resources-2.0.0/invenio_users_resources/translations/da/LC_MESSAGES/messages.mo` & `invenio-users-resources-2.0.1/invenio_users_resources/translations/da/LC_MESSAGES/messages.mo`

 * *Format-specific differences are supported for Gettext message catalogues but no file-specific differences were detected; falling back to a binary diff. file(1) reports: GNU message catalog (little endian), revision 0.0, 1 message, Project-Id-Version: invenio-users-resources 0.3.2*

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 000000c0: 6f6e 2d44 6174 653a 2032 3032 322d 3032  on-Date: 2022-02
 000000d0: 2d31 3620 3131 3a35 382b 3030 3030 0a4c  -16 11:58+0000.L
 000000e0: 6173 742d 5472 616e 736c 6174 6f72 3a20  ast-Translator: 
 000000f0: 4655 4c4c 204e 414d 4520 3c45 4d41 494c  FULL NAME <EMAIL
 00000100: 4041 4444 5245 5353 3e0a 4c61 6e67 7561  @ADDRESS>.Langua
 00000110: 6765 3a20 6461 0a4c 616e 6775 6167 652d  ge: da.Language-
 00000120: 5465 616d 3a20 4461 6e69 7368 2028 6874  Team: Danish (ht
-00000130: 7470 733a 2f2f 7777 772e 7472 616e 7369  tps://www.transi
+00000130: 7470 733a 2f2f 6170 702e 7472 616e 7369  tps://app.transi
 00000140: 6665 782e 636f 6d2f 696e 7665 6e69 6f73  fex.com/invenios
 00000150: 6f66 7477 6172 652f 7465 616d 732f 3233  oftware/teams/23
 00000160: 3533 372f 6461 2f29 0a50 6c75 7261 6c2d  537/da/).Plural-
 00000170: 466f 726d 733a 206e 706c 7572 616c 733d  Forms: nplurals=
 00000180: 323b 2070 6c75 7261 6c3d 286e 2021 3d20  2; plural=(n != 
 00000190: 3129 3b0a 4d49 4d45 2d56 6572 7369 6f6e  1);.MIME-Version
 000001a0: 3a20 312e 300a 436f 6e74 656e 742d 5479  : 1.0.Content-Ty
```

### Comparing `invenio-users-resources-2.0.0/invenio_users_resources/translations/da/LC_MESSAGES/messages.po` & `invenio-users-resources-2.0.1/invenio_users_resources/translations/da/LC_MESSAGES/messages.po`

 * *Files 11% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-users-resources 0.3.2\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 12:12+0000\n"
 "PO-Revision-Date: 2022-02-16 11:58+0000\n"
-"Language-Team: Danish (https://www.transifex.com/inveniosoftware/teams/23537/da/)\n"
+"Language-Team: Danish (https://app.transifex.com/inveniosoftware/teams/23537/da/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.3\n"
 "Language: da\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
```

### Comparing `invenio-users-resources-2.0.0/invenio_users_resources/translations/de/LC_MESSAGES/messages.mo` & `invenio-users-resources-2.0.1/invenio_users_resources/translations/de/LC_MESSAGES/messages.mo`

 * *Files 2% similar despite different names*

#### msgunfmt {}

```diff
@@ -2,15 +2,15 @@
 msgstr ""
 "Project-Id-Version: invenio-users-resources 0.3.2\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 12:12+0000\n"
 "PO-Revision-Date: 2022-02-16 11:58+0000\n"
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

### Comparing `invenio-users-resources-2.0.0/invenio_users_resources/translations/de/LC_MESSAGES/messages.po` & `invenio-users-resources-2.0.1/invenio_users_resources/translations/de/LC_MESSAGES/messages.po`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-users-resources 0.3.2\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 12:12+0000\n"
 "PO-Revision-Date: 2022-02-16 11:58+0000\n"
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

### Comparing `invenio-users-resources-2.0.0/invenio_users_resources/translations/el/LC_MESSAGES/messages.mo` & `invenio-users-resources-2.0.1/invenio_users_resources/translations/el/LC_MESSAGES/messages.mo`

 * *Files 2% similar despite different names*

#### msgunfmt {}

```diff
@@ -2,15 +2,15 @@
 msgstr ""
 "Project-Id-Version: invenio-users-resources 0.3.2\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 12:12+0000\n"
 "PO-Revision-Date: 2022-02-16 11:58+0000\n"
 "Last-Translator: Tibor Simko <tibor.simko@cern.ch>, 2022\n"
 "Language: el\n"
-"Language-Team: Greek (https://www.transifex.com/inveniosoftware/teams/23537/"
+"Language-Team: Greek (https://app.transifex.com/inveniosoftware/teams/23537/"
 "el/)\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.12.1\n"
```

### Comparing `invenio-users-resources-2.0.0/invenio_users_resources/translations/el/LC_MESSAGES/messages.po` & `invenio-users-resources-2.0.1/invenio_users_resources/translations/el/LC_MESSAGES/messages.po`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-users-resources 0.3.2\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 12:12+0000\n"
 "PO-Revision-Date: 2022-02-16 11:58+0000\n"
 "Last-Translator: Tibor Simko <tibor.simko@cern.ch>, 2022\n"
-"Language-Team: Greek (https://www.transifex.com/inveniosoftware/teams/23537/el/)\n"
+"Language-Team: Greek (https://app.transifex.com/inveniosoftware/teams/23537/el/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.3\n"
 "Language: el\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
```

### Comparing `invenio-users-resources-2.0.0/invenio_users_resources/translations/es/LC_MESSAGES/messages.mo` & `invenio-users-resources-2.0.1/invenio_users_resources/translations/es/LC_MESSAGES/messages.mo`

 * *Files 2% similar despite different names*

#### msgunfmt {}

```diff
@@ -2,15 +2,15 @@
 msgstr ""
 "Project-Id-Version: invenio-users-resources 0.3.2\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 12:12+0000\n"
 "PO-Revision-Date: 2022-02-16 11:58+0000\n"
 "Last-Translator: Alizee Pace <alizee.pace@gmail.com>, 2022\n"
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

### Comparing `invenio-users-resources-2.0.0/invenio_users_resources/translations/es/LC_MESSAGES/messages.po` & `invenio-users-resources-2.0.1/invenio_users_resources/translations/es/LC_MESSAGES/messages.po`

 * *Files 8% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-users-resources 0.3.2\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 12:12+0000\n"
 "PO-Revision-Date: 2022-02-16 11:58+0000\n"
 "Last-Translator: Alizee Pace <alizee.pace@gmail.com>, 2022\n"
-"Language-Team: Spanish (https://www.transifex.com/inveniosoftware/teams/23537/es/)\n"
+"Language-Team: Spanish (https://app.transifex.com/inveniosoftware/teams/23537/es/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.3\n"
 "Language: es\n"
 "Plural-Forms: nplurals=3; plural=n == 1 ? 0 : n != 0 && n % 1000000 == 0 ? 1 : 2;\n"
```

### Comparing `invenio-users-resources-2.0.0/invenio_users_resources/translations/et/LC_MESSAGES/messages.mo` & `invenio-users-resources-2.0.1/invenio_users_resources/translations/et/LC_MESSAGES/messages.mo`

 * *Files 2% similar despite different names*

#### msgunfmt {}

```diff
@@ -2,15 +2,15 @@
 msgstr ""
 "Project-Id-Version: invenio-users-resources 0.3.2\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 12:12+0000\n"
 "PO-Revision-Date: 2022-02-16 11:58+0000\n"
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

### Comparing `invenio-users-resources-2.0.0/invenio_users_resources/translations/et/LC_MESSAGES/messages.po` & `invenio-users-resources-2.0.1/invenio_users_resources/translations/et/LC_MESSAGES/messages.po`

 * *Files 8% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-users-resources 0.3.2\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 12:12+0000\n"
 "PO-Revision-Date: 2022-02-16 11:58+0000\n"
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

### Comparing `invenio-users-resources-2.0.0/invenio_users_resources/translations/et_EE/LC_MESSAGES/messages.mo` & `invenio-users-resources-2.0.1/invenio_users_resources/translations/et_EE/LC_MESSAGES/messages.mo`

 * *Format-specific differences are supported for Gettext message catalogues but no file-specific differences were detected; falling back to a binary diff. file(1) reports: GNU message catalog (little endian), revision 0.0, 1 message, Project-Id-Version: invenio-users-resources 0.3.2*

 * *Files 3% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 000000d0: 2d31 3620 3131 3a35 382b 3030 3030 0a4c  -16 11:58+0000.L
 000000e0: 6173 742d 5472 616e 736c 6174 6f72 3a20  ast-Translator: 
 000000f0: 4655 4c4c 204e 414d 4520 3c45 4d41 494c  FULL NAME <EMAIL
 00000100: 4041 4444 5245 5353 3e0a 4c61 6e67 7561  @ADDRESS>.Langua
 00000110: 6765 3a20 6574 5f45 450a 4c61 6e67 7561  ge: et_EE.Langua
 00000120: 6765 2d54 6561 6d3a 2045 7374 6f6e 6961  ge-Team: Estonia
 00000130: 6e20 2845 7374 6f6e 6961 2920 2868 7474  n (Estonia) (htt
-00000140: 7073 3a2f 2f77 7777 2e74 7261 6e73 6966  ps://www.transif
+00000140: 7073 3a2f 2f61 7070 2e74 7261 6e73 6966  ps://app.transif
 00000150: 6578 2e63 6f6d 2f69 6e76 656e 696f 736f  ex.com/invenioso
 00000160: 6674 7761 7265 2f74 6561 6d73 2f32 3335  ftware/teams/235
 00000170: 3337 2f65 745f 4545 2f29 0a50 6c75 7261  37/et_EE/).Plura
 00000180: 6c2d 466f 726d 733a 206e 706c 7572 616c  l-Forms: nplural
 00000190: 733d 323b 2070 6c75 7261 6c3d 286e 2021  s=2; plural=(n !
 000001a0: 3d20 3129 3b0a 4d49 4d45 2d56 6572 7369  = 1);.MIME-Versi
 000001b0: 6f6e 3a20 312e 300a 436f 6e74 656e 742d  on: 1.0.Content-
```

### Comparing `invenio-users-resources-2.0.0/invenio_users_resources/translations/et_EE/LC_MESSAGES/messages.po` & `invenio-users-resources-2.0.1/invenio_users_resources/translations/et_EE/LC_MESSAGES/messages.po`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-users-resources 0.3.2\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 12:12+0000\n"
 "PO-Revision-Date: 2022-02-16 11:58+0000\n"
-"Language-Team: Estonian (Estonia) (https://www.transifex.com/inveniosoftware/teams/23537/et_EE/)\n"
+"Language-Team: Estonian (Estonia) (https://app.transifex.com/inveniosoftware/teams/23537/et_EE/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.3\n"
 "Language: et_EE\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
```

### Comparing `invenio-users-resources-2.0.0/invenio_users_resources/translations/fa/LC_MESSAGES/messages.mo` & `invenio-users-resources-2.0.1/invenio_users_resources/translations/fa/LC_MESSAGES/messages.mo`

 * *Files 2% similar despite different names*

#### msgunfmt {}

```diff
@@ -2,15 +2,15 @@
 msgstr ""
 "Project-Id-Version: invenio-users-resources 0.3.2\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 12:12+0000\n"
 "PO-Revision-Date: 2022-02-16 11:58+0000\n"
 "Last-Translator: Tibor Simko <tibor.simko@cern.ch>, 2022\n"
 "Language: fa\n"
-"Language-Team: Persian (https://www.transifex.com/inveniosoftware/"
+"Language-Team: Persian (https://app.transifex.com/inveniosoftware/"
 "teams/23537/fa/)\n"
 "Plural-Forms: nplurals=2; plural=(n > 1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.12.1\n"
```

### Comparing `invenio-users-resources-2.0.0/invenio_users_resources/translations/fa/LC_MESSAGES/messages.po` & `invenio-users-resources-2.0.1/invenio_users_resources/translations/fa/LC_MESSAGES/messages.po`

 * *Files 8% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-users-resources 0.3.2\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 12:12+0000\n"
 "PO-Revision-Date: 2022-02-16 11:58+0000\n"
 "Last-Translator: Tibor Simko <tibor.simko@cern.ch>, 2022\n"
-"Language-Team: Persian (https://www.transifex.com/inveniosoftware/teams/23537/fa/)\n"
+"Language-Team: Persian (https://app.transifex.com/inveniosoftware/teams/23537/fa/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.3\n"
 "Language: fa\n"
 "Plural-Forms: nplurals=2; plural=(n > 1);\n"
```

### Comparing `invenio-users-resources-2.0.0/invenio_users_resources/translations/fr/LC_MESSAGES/messages.mo` & `invenio-users-resources-2.0.1/invenio_users_resources/translations/pt/LC_MESSAGES/messages.mo`

 * *Files 13% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,19 +1,19 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-users-resources 0.3.2\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 12:12+0000\n"
 "PO-Revision-Date: 2022-02-16 11:58+0000\n"
-"Last-Translator: Alizee Pace <alizee.pace@gmail.com>, 2022\n"
-"Language: fr\n"
-"Language-Team: French (https://www.transifex.com/inveniosoftware/teams/23537/"
-"fr/)\n"
+"Last-Translator: Tibor Simko <tibor.simko@cern.ch>, 2022\n"
+"Language: pt\n"
+"Language-Team: Portuguese (https://app.transifex.com/inveniosoftware/"
+"teams/23537/pt/)\n"
 "Plural-Forms: nplurals=3; plural=(n == 0 || n == 1) ? 0 : n != 0 && n % "
 "1000000 == 0 ? 1 : 2;\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.12.1\n"
 
 msgid "Name"
-msgstr "Nom"
+msgstr "Nome"
```

### Comparing `invenio-users-resources-2.0.0/invenio_users_resources/translations/fr/LC_MESSAGES/messages.po` & `invenio-users-resources-2.0.1/invenio_users_resources/translations/fr/LC_MESSAGES/messages.po`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-users-resources 0.3.2\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 12:12+0000\n"
 "PO-Revision-Date: 2022-02-16 11:58+0000\n"
 "Last-Translator: Alizee Pace <alizee.pace@gmail.com>, 2022\n"
-"Language-Team: French (https://www.transifex.com/inveniosoftware/teams/23537/fr/)\n"
+"Language-Team: French (https://app.transifex.com/inveniosoftware/teams/23537/fr/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.3\n"
 "Language: fr\n"
 "Plural-Forms: nplurals=3; plural=(n == 0 || n == 1) ? 0 : n != 0 && n % 1000000 == 0 ? 1 : 2;\n"
```

### Comparing `invenio-users-resources-2.0.0/invenio_users_resources/translations/gl/LC_MESSAGES/messages.mo` & `invenio-users-resources-2.0.1/invenio_users_resources/translations/gl/LC_MESSAGES/messages.mo`

 * *Format-specific differences are supported for Gettext message catalogues but no file-specific differences were detected; falling back to a binary diff. file(1) reports: GNU message catalog (little endian), revision 0.0, 1 message, Project-Id-Version: invenio-users-resources 0.3.2*

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 000000c0: 6f6e 2d44 6174 653a 2032 3032 322d 3032  on-Date: 2022-02
 000000d0: 2d31 3620 3131 3a35 382b 3030 3030 0a4c  -16 11:58+0000.L
 000000e0: 6173 742d 5472 616e 736c 6174 6f72 3a20  ast-Translator: 
 000000f0: 4655 4c4c 204e 414d 4520 3c45 4d41 494c  FULL NAME <EMAIL
 00000100: 4041 4444 5245 5353 3e0a 4c61 6e67 7561  @ADDRESS>.Langua
 00000110: 6765 3a20 676c 0a4c 616e 6775 6167 652d  ge: gl.Language-
 00000120: 5465 616d 3a20 4761 6c69 6369 616e 2028  Team: Galician (
-00000130: 6874 7470 733a 2f2f 7777 772e 7472 616e  https://www.tran
+00000130: 6874 7470 733a 2f2f 6170 702e 7472 616e  https://app.tran
 00000140: 7369 6665 782e 636f 6d2f 696e 7665 6e69  sifex.com/inveni
 00000150: 6f73 6f66 7477 6172 652f 7465 616d 732f  osoftware/teams/
 00000160: 3233 3533 372f 676c 2f29 0a50 6c75 7261  23537/gl/).Plura
 00000170: 6c2d 466f 726d 733a 206e 706c 7572 616c  l-Forms: nplural
 00000180: 733d 323b 2070 6c75 7261 6c3d 286e 2021  s=2; plural=(n !
 00000190: 3d20 3129 3b0a 4d49 4d45 2d56 6572 7369  = 1);.MIME-Versi
 000001a0: 6f6e 3a20 312e 300a 436f 6e74 656e 742d  on: 1.0.Content-
```

### Comparing `invenio-users-resources-2.0.0/invenio_users_resources/translations/gl/LC_MESSAGES/messages.po` & `invenio-users-resources-2.0.1/invenio_users_resources/translations/gl/LC_MESSAGES/messages.po`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-users-resources 0.3.2\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 12:12+0000\n"
 "PO-Revision-Date: 2022-02-16 11:58+0000\n"
-"Language-Team: Galician (https://www.transifex.com/inveniosoftware/teams/23537/gl/)\n"
+"Language-Team: Galician (https://app.transifex.com/inveniosoftware/teams/23537/gl/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.3\n"
 "Language: gl\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
```

### Comparing `invenio-users-resources-2.0.0/invenio_users_resources/translations/hr/LC_MESSAGES/messages.mo` & `invenio-users-resources-2.0.1/invenio_users_resources/translations/hr/LC_MESSAGES/messages.mo`

 * *Files 2% similar despite different names*

#### msgunfmt {}

```diff
@@ -2,15 +2,15 @@
 msgstr ""
 "Project-Id-Version: invenio-users-resources 0.3.2\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 12:12+0000\n"
 "PO-Revision-Date: 2022-02-16 11:58+0000\n"
 "Last-Translator: Tibor Simko <tibor.simko@cern.ch>, 2022\n"
 "Language: hr\n"
-"Language-Team: Croatian (https://www.transifex.com/inveniosoftware/"
+"Language-Team: Croatian (https://app.transifex.com/inveniosoftware/"
 "teams/23537/hr/)\n"
 "Plural-Forms: nplurals=3; plural=n%10==1 && n%100!=11 ? 0 : n%10>=2 && "
 "n%10<=4 && (n%100<10 || n%100>=20) ? 1 : 2;\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.12.1\n"
```

### Comparing `invenio-users-resources-2.0.0/invenio_users_resources/translations/hr/LC_MESSAGES/messages.po` & `invenio-users-resources-2.0.1/invenio_users_resources/translations/hr/LC_MESSAGES/messages.po`

 * *Files 9% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-users-resources 0.3.2\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 12:12+0000\n"
 "PO-Revision-Date: 2022-02-16 11:58+0000\n"
 "Last-Translator: Tibor Simko <tibor.simko@cern.ch>, 2022\n"
-"Language-Team: Croatian (https://www.transifex.com/inveniosoftware/teams/23537/hr/)\n"
+"Language-Team: Croatian (https://app.transifex.com/inveniosoftware/teams/23537/hr/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.3\n"
 "Language: hr\n"
 "Plural-Forms: nplurals=3; plural=n%10==1 && n%100!=11 ? 0 : n%10>=2 && n%10<=4 && (n%100<10 || n%100>=20) ? 1 : 2;\n"
```

### Comparing `invenio-users-resources-2.0.0/invenio_users_resources/translations/hu/LC_MESSAGES/messages.mo` & `invenio-users-resources-2.0.1/invenio_users_resources/translations/zh_CN/LC_MESSAGES/messages.mo`

 * *Files 16% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,24 +1,24 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-users-resources 0.3.2\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 12:12+0000\n"
 "PO-Revision-Date: 2022-02-16 11:58+0000\n"
-"Last-Translator: Andrea Dömötör, 2022\n"
-"Language: hu\n"
-"Language-Team: Hungarian (https://www.transifex.com/inveniosoftware/"
-"teams/23537/hu/)\n"
-"Plural-Forms: nplurals=2; plural=(n != 1);\n"
+"Last-Translator: Kalven Richie, 2022\n"
+"Language: zh_CN\n"
+"Language-Team: Chinese (China) (https://app.transifex.com/inveniosoftware/"
+"teams/23537/zh_CN/)\n"
+"Plural-Forms: nplurals=1; plural=0;\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.12.1\n"
 
 msgid "Best match"
-msgstr "Legjobb találat"
+msgstr "最佳匹配"
 
 msgid "Name"
-msgstr "Név"
+msgstr "名称"
 
 msgid "Value must be either 'public' or 'restricted'."
-msgstr "Az érték 'nyilvános' vagy 'korlátozott' lehet."
+msgstr "值必须为“public”或“restricted”。"
```

### Comparing `invenio-users-resources-2.0.0/invenio_users_resources/translations/hu/LC_MESSAGES/messages.po` & `invenio-users-resources-2.0.1/invenio_users_resources/translations/rw/LC_MESSAGES/messages.po`

 * *Files 10% similar despite different names*

```diff
@@ -1,36 +1,32 @@
 # Translations template for invenio-users-resources.
 # Copyright (C) 2022 CERN
 # This file is distributed under the same license as the
 # invenio-users-resources project.
 # FIRST AUTHOR <EMAIL@ADDRESS>, 2022.
 # 
-# Translators:
-# Andrea Dömötör, 2022
-# 
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-users-resources 0.3.2\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 12:12+0000\n"
 "PO-Revision-Date: 2022-02-16 11:58+0000\n"
-"Last-Translator: Andrea Dömötör, 2022\n"
-"Language-Team: Hungarian (https://www.transifex.com/inveniosoftware/teams/23537/hu/)\n"
+"Language-Team: Kinyarwanda (https://app.transifex.com/inveniosoftware/teams/23537/rw/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.3\n"
-"Language: hu\n"
+"Language: rw\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
 #: invenio_users_resources/services/schemas.py:21
 msgid "Value must be either 'public' or 'restricted'."
-msgstr "Az érték 'nyilvános' vagy 'korlátozott' lehet."
+msgstr ""
 
 #: invenio_users_resources/services/groups/config.py:43
 msgid "Best match"
-msgstr "Legjobb találat"
+msgstr ""
 
 #: invenio_users_resources/services/groups/config.py:47
 msgid "Name"
-msgstr "Név"
+msgstr ""
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `invenio-users-resources-2.0.0/invenio_users_resources/translations/it/LC_MESSAGES/messages.mo` & `invenio-users-resources-2.0.1/invenio_users_resources/translations/it/LC_MESSAGES/messages.mo`

 * *Files 3% similar despite different names*

#### msgunfmt {}

```diff
@@ -2,15 +2,15 @@
 msgstr ""
 "Project-Id-Version: invenio-users-resources 0.3.2\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 12:12+0000\n"
 "PO-Revision-Date: 2022-02-16 11:58+0000\n"
 "Last-Translator: Alizee Pace <alizee.pace@gmail.com>, 2022\n"
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

### Comparing `invenio-users-resources-2.0.0/invenio_users_resources/translations/it/LC_MESSAGES/messages.po` & `invenio-users-resources-2.0.1/invenio_users_resources/translations/it/LC_MESSAGES/messages.po`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-users-resources 0.3.2\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 12:12+0000\n"
 "PO-Revision-Date: 2022-02-16 11:58+0000\n"
 "Last-Translator: Alizee Pace <alizee.pace@gmail.com>, 2022\n"
-"Language-Team: Italian (https://www.transifex.com/inveniosoftware/teams/23537/it/)\n"
+"Language-Team: Italian (https://app.transifex.com/inveniosoftware/teams/23537/it/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.3\n"
 "Language: it\n"
 "Plural-Forms: nplurals=3; plural=n == 1 ? 0 : n != 0 && n % 1000000 == 0 ? 1 : 2;\n"
```

### Comparing `invenio-users-resources-2.0.0/invenio_users_resources/translations/ja/LC_MESSAGES/messages.mo` & `invenio-users-resources-2.0.1/invenio_users_resources/translations/sv_SE/LC_MESSAGES/messages.mo`

 * *Files 16% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,18 +0,0 @@
-msgid ""
-msgstr ""
-"Project-Id-Version: invenio-users-resources 0.3.2\n"
-"Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
-"POT-Creation-Date: 2022-10-12 12:12+0000\n"
-"PO-Revision-Date: 2022-02-16 11:58+0000\n"
-"Last-Translator: Tibor Simko <tibor.simko@cern.ch>, 2022\n"
-"Language: ja\n"
-"Language-Team: Japanese (https://www.transifex.com/inveniosoftware/"
-"teams/23537/ja/)\n"
-"Plural-Forms: nplurals=1; plural=0;\n"
-"MIME-Version: 1.0\n"
-"Content-Type: text/plain; charset=utf-8\n"
-"Content-Transfer-Encoding: 8bit\n"
-"Generated-By: Babel 2.12.1\n"
-
-msgid "Name"
-msgstr "名前"
```

### Comparing `invenio-users-resources-2.0.0/invenio_users_resources/translations/ja/LC_MESSAGES/messages.po` & `invenio-users-resources-2.0.1/invenio_users_resources/translations/ka/LC_MESSAGES/messages.po`

 * *Files 10% similar despite different names*

```diff
@@ -11,26 +11,26 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-users-resources 0.3.2\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 12:12+0000\n"
 "PO-Revision-Date: 2022-02-16 11:58+0000\n"
 "Last-Translator: Tibor Simko <tibor.simko@cern.ch>, 2022\n"
-"Language-Team: Japanese (https://www.transifex.com/inveniosoftware/teams/23537/ja/)\n"
+"Language-Team: Georgian (https://app.transifex.com/inveniosoftware/teams/23537/ka/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.3\n"
-"Language: ja\n"
-"Plural-Forms: nplurals=1; plural=0;\n"
+"Language: ka\n"
+"Plural-Forms: nplurals=2; plural=(n!=1);\n"
 
 #: invenio_users_resources/services/schemas.py:21
 msgid "Value must be either 'public' or 'restricted'."
 msgstr ""
 
 #: invenio_users_resources/services/groups/config.py:43
 msgid "Best match"
 msgstr ""
 
 #: invenio_users_resources/services/groups/config.py:47
 msgid "Name"
-msgstr "名前"
+msgstr "სახელი"
```

### Comparing `invenio-users-resources-2.0.0/invenio_users_resources/translations/ka/LC_MESSAGES/messages.mo` & `invenio-users-resources-2.0.1/invenio_users_resources/translations/ka/LC_MESSAGES/messages.mo`

 * *Files 3% similar despite different names*

#### msgunfmt {}

```diff
@@ -2,15 +2,15 @@
 msgstr ""
 "Project-Id-Version: invenio-users-resources 0.3.2\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 12:12+0000\n"
 "PO-Revision-Date: 2022-02-16 11:58+0000\n"
 "Last-Translator: Tibor Simko <tibor.simko@cern.ch>, 2022\n"
 "Language: ka\n"
-"Language-Team: Georgian (https://www.transifex.com/inveniosoftware/"
+"Language-Team: Georgian (https://app.transifex.com/inveniosoftware/"
 "teams/23537/ka/)\n"
 "Plural-Forms: nplurals=2; plural=(n!=1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.12.1\n"
```

### Comparing `invenio-users-resources-2.0.0/invenio_users_resources/translations/ka/LC_MESSAGES/messages.po` & `invenio-users-resources-2.0.1/invenio_users_resources/translations/zh_TW/LC_MESSAGES/messages.po`

 * *Files 12% similar despite different names*

```diff
@@ -11,26 +11,26 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-users-resources 0.3.2\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 12:12+0000\n"
 "PO-Revision-Date: 2022-02-16 11:58+0000\n"
 "Last-Translator: Tibor Simko <tibor.simko@cern.ch>, 2022\n"
-"Language-Team: Georgian (https://www.transifex.com/inveniosoftware/teams/23537/ka/)\n"
+"Language-Team: Chinese (Taiwan) (https://app.transifex.com/inveniosoftware/teams/23537/zh_TW/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.3\n"
-"Language: ka\n"
-"Plural-Forms: nplurals=2; plural=(n!=1);\n"
+"Language: zh_TW\n"
+"Plural-Forms: nplurals=1; plural=0;\n"
 
 #: invenio_users_resources/services/schemas.py:21
 msgid "Value must be either 'public' or 'restricted'."
 msgstr ""
 
 #: invenio_users_resources/services/groups/config.py:43
 msgid "Best match"
 msgstr ""
 
 #: invenio_users_resources/services/groups/config.py:47
 msgid "Name"
-msgstr "სახელი"
+msgstr "名稱"
```

### Comparing `invenio-users-resources-2.0.0/invenio_users_resources/translations/lt/LC_MESSAGES/messages.mo` & `invenio-users-resources-2.0.1/invenio_users_resources/translations/lt/LC_MESSAGES/messages.mo`

 * *Files 21% similar despite different names*

#### msgunfmt {}

```diff
@@ -2,15 +2,15 @@
 msgstr ""
 "Project-Id-Version: invenio-users-resources 0.3.2\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 12:12+0000\n"
 "PO-Revision-Date: 2022-02-16 11:58+0000\n"
 "Last-Translator: Tibor Simko <tibor.simko@cern.ch>, 2022\n"
 "Language: lt\n"
-"Language-Team: Lithuanian (https://www.transifex.com/inveniosoftware/"
+"Language-Team: Lithuanian (https://app.transifex.com/inveniosoftware/"
 "teams/23537/lt/)\n"
 "Plural-Forms: nplurals=4; plural=(n % 10 == 1 && (n % 100 > 19 || n % 100 < "
 "11) ? 0 : (n % 10 >= 2 && n % 10 <=9) && (n % 100 > 19 || n % 100 < 11) ? "
 "1 : n % 1 != 0 ? 2: 3);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
```

### Comparing `invenio-users-resources-2.0.0/invenio_users_resources/translations/lt/LC_MESSAGES/messages.po` & `invenio-users-resources-2.0.1/invenio_users_resources/translations/lt/LC_MESSAGES/messages.po`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-users-resources 0.3.2\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 12:12+0000\n"
 "PO-Revision-Date: 2022-02-16 11:58+0000\n"
 "Last-Translator: Tibor Simko <tibor.simko@cern.ch>, 2022\n"
-"Language-Team: Lithuanian (https://www.transifex.com/inveniosoftware/teams/23537/lt/)\n"
+"Language-Team: Lithuanian (https://app.transifex.com/inveniosoftware/teams/23537/lt/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.3\n"
 "Language: lt\n"
 "Plural-Forms: nplurals=4; plural=(n % 10 == 1 && (n % 100 > 19 || n % 100 < 11) ? 0 : (n % 10 >= 2 && n % 10 <=9) && (n % 100 > 19 || n % 100 < 11) ? 1 : n % 1 != 0 ? 2: 3);\n"
```

### Comparing `invenio-users-resources-2.0.0/invenio_users_resources/translations/messages.pot` & `invenio-users-resources-2.0.1/invenio_users_resources/translations/messages.pot`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-2.0.0/invenio_users_resources/translations/no/LC_MESSAGES/messages.mo` & `invenio-users-resources-2.0.1/invenio_users_resources/translations/no/LC_MESSAGES/messages.mo`

 * *Files 3% similar despite different names*

#### msgunfmt {}

```diff
@@ -2,15 +2,15 @@
 msgstr ""
 "Project-Id-Version: invenio-users-resources 0.3.2\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 12:12+0000\n"
 "PO-Revision-Date: 2022-02-16 11:58+0000\n"
 "Last-Translator: Tibor Simko <tibor.simko@cern.ch>, 2022\n"
 "Language: no\n"
-"Language-Team: Norwegian (https://www.transifex.com/inveniosoftware/"
+"Language-Team: Norwegian (https://app.transifex.com/inveniosoftware/"
 "teams/23537/no/)\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.12.1\n"
```

### Comparing `invenio-users-resources-2.0.0/invenio_users_resources/translations/no/LC_MESSAGES/messages.po` & `invenio-users-resources-2.0.1/invenio_users_resources/translations/no/LC_MESSAGES/messages.po`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-users-resources 0.3.2\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 12:12+0000\n"
 "PO-Revision-Date: 2022-02-16 11:58+0000\n"
 "Last-Translator: Tibor Simko <tibor.simko@cern.ch>, 2022\n"
-"Language-Team: Norwegian (https://www.transifex.com/inveniosoftware/teams/23537/no/)\n"
+"Language-Team: Norwegian (https://app.transifex.com/inveniosoftware/teams/23537/no/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.3\n"
 "Language: no\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
```

### Comparing `invenio-users-resources-2.0.0/invenio_users_resources/translations/pl/LC_MESSAGES/messages.mo` & `invenio-users-resources-2.0.1/invenio_users_resources/translations/pl/LC_MESSAGES/messages.mo`

 * *Files 14% similar despite different names*

#### msgunfmt {}

```diff
@@ -2,15 +2,15 @@
 msgstr ""
 "Project-Id-Version: invenio-users-resources 0.3.2\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 12:12+0000\n"
 "PO-Revision-Date: 2022-02-16 11:58+0000\n"
 "Last-Translator: Tibor Simko <tibor.simko@cern.ch>, 2022\n"
 "Language: pl\n"
-"Language-Team: Polish (https://www.transifex.com/inveniosoftware/teams/23537/"
+"Language-Team: Polish (https://app.transifex.com/inveniosoftware/teams/23537/"
 "pl/)\n"
 "Plural-Forms: nplurals=4; plural=(n==1 ? 0 : (n%10>=2 && n%10<=4) && "
 "(n%100<12 || n%100>14) ? 1 : n!=1 && (n%10>=0 && n%10<=1) || (n%10>=5 && "
 "n%10<=9) || (n%100>=12 && n%100<=14) ? 2 : 3);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
```

### Comparing `invenio-users-resources-2.0.0/invenio_users_resources/translations/pl/LC_MESSAGES/messages.po` & `invenio-users-resources-2.0.1/invenio_users_resources/translations/pl/LC_MESSAGES/messages.po`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-users-resources 0.3.2\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 12:12+0000\n"
 "PO-Revision-Date: 2022-02-16 11:58+0000\n"
 "Last-Translator: Tibor Simko <tibor.simko@cern.ch>, 2022\n"
-"Language-Team: Polish (https://www.transifex.com/inveniosoftware/teams/23537/pl/)\n"
+"Language-Team: Polish (https://app.transifex.com/inveniosoftware/teams/23537/pl/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.3\n"
 "Language: pl\n"
 "Plural-Forms: nplurals=4; plural=(n==1 ? 0 : (n%10>=2 && n%10<=4) && (n%100<12 || n%100>14) ? 1 : n!=1 && (n%10>=0 && n%10<=1) || (n%10>=5 && n%10<=9) || (n%100>=12 && n%100<=14) ? 2 : 3);\n"
```

### Comparing `invenio-users-resources-2.0.0/invenio_users_resources/translations/pt/LC_MESSAGES/messages.mo` & `invenio-users-resources-2.0.1/invenio_users_resources/translations/es_MX/LC_MESSAGES/messages.mo`

 * *Files 19% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,19 +0,0 @@
-msgid ""
-msgstr ""
-"Project-Id-Version: invenio-users-resources 0.3.2\n"
-"Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
-"POT-Creation-Date: 2022-10-12 12:12+0000\n"
-"PO-Revision-Date: 2022-02-16 11:58+0000\n"
-"Last-Translator: Tibor Simko <tibor.simko@cern.ch>, 2022\n"
-"Language: pt\n"
-"Language-Team: Portuguese (https://www.transifex.com/inveniosoftware/"
-"teams/23537/pt/)\n"
-"Plural-Forms: nplurals=3; plural=(n == 0 || n == 1) ? 0 : n != 0 && n % "
-"1000000 == 0 ? 1 : 2;\n"
-"MIME-Version: 1.0\n"
-"Content-Type: text/plain; charset=utf-8\n"
-"Content-Transfer-Encoding: 8bit\n"
-"Generated-By: Babel 2.12.1\n"
-
-msgid "Name"
-msgstr "Nome"
```

### Comparing `invenio-users-resources-2.0.0/invenio_users_resources/translations/pt/LC_MESSAGES/messages.po` & `invenio-users-resources-2.0.1/invenio_users_resources/translations/pt/LC_MESSAGES/messages.po`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-users-resources 0.3.2\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 12:12+0000\n"
 "PO-Revision-Date: 2022-02-16 11:58+0000\n"
 "Last-Translator: Tibor Simko <tibor.simko@cern.ch>, 2022\n"
-"Language-Team: Portuguese (https://www.transifex.com/inveniosoftware/teams/23537/pt/)\n"
+"Language-Team: Portuguese (https://app.transifex.com/inveniosoftware/teams/23537/pt/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.3\n"
 "Language: pt\n"
 "Plural-Forms: nplurals=3; plural=(n == 0 || n == 1) ? 0 : n != 0 && n % 1000000 == 0 ? 1 : 2;\n"
```

### Comparing `invenio-users-resources-2.0.0/invenio_users_resources/translations/ro/LC_MESSAGES/messages.mo` & `invenio-users-resources-2.0.1/invenio_users_resources/translations/fr_CI/LC_MESSAGES/messages.mo`

 * *Files 20% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,19 +0,0 @@
-msgid ""
-msgstr ""
-"Project-Id-Version: invenio-users-resources 0.3.2\n"
-"Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
-"POT-Creation-Date: 2022-10-12 12:12+0000\n"
-"PO-Revision-Date: 2022-02-16 11:58+0000\n"
-"Last-Translator: Tibor Simko <tibor.simko@cern.ch>, 2022\n"
-"Language: ro\n"
-"Language-Team: Romanian (https://www.transifex.com/inveniosoftware/"
-"teams/23537/ro/)\n"
-"Plural-Forms: nplurals=3; plural=(n==1?0:(((n%100>19)||((n%100==0)&&(n!=0)))?"
-"2:1));\n"
-"MIME-Version: 1.0\n"
-"Content-Type: text/plain; charset=utf-8\n"
-"Content-Transfer-Encoding: 8bit\n"
-"Generated-By: Babel 2.12.1\n"
-
-msgid "Name"
-msgstr "Nume"
```

### Comparing `invenio-users-resources-2.0.0/invenio_users_resources/translations/ro/LC_MESSAGES/messages.po` & `invenio-users-resources-2.0.1/invenio_users_resources/translations/tr/LC_MESSAGES/messages.po`

 * *Files 15% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 # Translations template for invenio-users-resources.
 # Copyright (C) 2022 CERN
 # This file is distributed under the same license as the
 # invenio-users-resources project.
 # FIRST AUTHOR <EMAIL@ADDRESS>, 2022.
 # 
 # Translators:
-# Tibor Simko <tibor.simko@cern.ch>, 2022
+# Ben Translation and Interpreting Services <info@bentercume.com>, 2022
 # 
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-users-resources 0.3.2\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 12:12+0000\n"
 "PO-Revision-Date: 2022-02-16 11:58+0000\n"
-"Last-Translator: Tibor Simko <tibor.simko@cern.ch>, 2022\n"
-"Language-Team: Romanian (https://www.transifex.com/inveniosoftware/teams/23537/ro/)\n"
+"Last-Translator: Ben Translation and Interpreting Services <info@bentercume.com>, 2022\n"
+"Language-Team: Turkish (https://app.transifex.com/inveniosoftware/teams/23537/tr/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.3\n"
-"Language: ro\n"
-"Plural-Forms: nplurals=3; plural=(n==1?0:(((n%100>19)||((n%100==0)&&(n!=0)))?2:1));\n"
+"Language: tr\n"
+"Plural-Forms: nplurals=2; plural=(n > 1);\n"
 
 #: invenio_users_resources/services/schemas.py:21
 msgid "Value must be either 'public' or 'restricted'."
 msgstr ""
 
 #: invenio_users_resources/services/groups/config.py:43
 msgid "Best match"
-msgstr ""
+msgstr "En iyi eşleşme"
 
 #: invenio_users_resources/services/groups/config.py:47
 msgid "Name"
-msgstr "Nume"
+msgstr "Ad"
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `invenio-users-resources-2.0.0/invenio_users_resources/translations/ru/LC_MESSAGES/messages.mo` & `invenio-users-resources-2.0.1/invenio_users_resources/translations/ru/LC_MESSAGES/messages.mo`

 * *Files 0% similar despite different names*

#### msgunfmt {}

```diff
@@ -2,15 +2,15 @@
 msgstr ""
 "Project-Id-Version: invenio-users-resources 0.3.2\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 12:12+0000\n"
 "PO-Revision-Date: 2022-02-16 11:58+0000\n"
 "Last-Translator: Tibor Simko <tibor.simko@cern.ch>, 2022\n"
 "Language: ru\n"
-"Language-Team: Russian (https://www.transifex.com/inveniosoftware/"
+"Language-Team: Russian (https://app.transifex.com/inveniosoftware/"
 "teams/23537/ru/)\n"
 "Plural-Forms: nplurals=4; plural=(n%10==1 && n%100!=11 ? 0 : n%10>=2 && "
 "n%10<=4 && (n%100<12 || n%100>14) ? 1 : n%10==0 || (n%10>=5 && n%10<=9) || "
 "(n%100>=11 && n%100<=14)? 2 : 3);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
```

### Comparing `invenio-users-resources-2.0.0/invenio_users_resources/translations/ru/LC_MESSAGES/messages.po` & `invenio-users-resources-2.0.1/invenio_users_resources/translations/ru/LC_MESSAGES/messages.po`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-users-resources 0.3.2\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 12:12+0000\n"
 "PO-Revision-Date: 2022-02-16 11:58+0000\n"
 "Last-Translator: Tibor Simko <tibor.simko@cern.ch>, 2022\n"
-"Language-Team: Russian (https://www.transifex.com/inveniosoftware/teams/23537/ru/)\n"
+"Language-Team: Russian (https://app.transifex.com/inveniosoftware/teams/23537/ru/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.3\n"
 "Language: ru\n"
 "Plural-Forms: nplurals=4; plural=(n%10==1 && n%100!=11 ? 0 : n%10>=2 && n%10<=4 && (n%100<12 || n%100>14) ? 1 : n%10==0 || (n%10>=5 && n%10<=9) || (n%100>=11 && n%100<=14)? 2 : 3);\n"
```

### Comparing `invenio-users-resources-2.0.0/invenio_users_resources/translations/rw/LC_MESSAGES/messages.mo` & `invenio-users-resources-2.0.1/invenio_users_resources/translations/rw/LC_MESSAGES/messages.mo`

 * *Format-specific differences are supported for Gettext message catalogues but no file-specific differences were detected; falling back to a binary diff. file(1) reports: GNU message catalog (little endian), revision 0.0, 1 message, Project-Id-Version: invenio-users-resources 0.3.2*

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 000000c0: 6f6e 2d44 6174 653a 2032 3032 322d 3032  on-Date: 2022-02
 000000d0: 2d31 3620 3131 3a35 382b 3030 3030 0a4c  -16 11:58+0000.L
 000000e0: 6173 742d 5472 616e 736c 6174 6f72 3a20  ast-Translator: 
 000000f0: 4655 4c4c 204e 414d 4520 3c45 4d41 494c  FULL NAME <EMAIL
 00000100: 4041 4444 5245 5353 3e0a 4c61 6e67 7561  @ADDRESS>.Langua
 00000110: 6765 3a20 7277 0a4c 616e 6775 6167 652d  ge: rw.Language-
 00000120: 5465 616d 3a20 4b69 6e79 6172 7761 6e64  Team: Kinyarwand
-00000130: 6120 2868 7474 7073 3a2f 2f77 7777 2e74  a (https://www.t
+00000130: 6120 2868 7474 7073 3a2f 2f61 7070 2e74  a (https://app.t
 00000140: 7261 6e73 6966 6578 2e63 6f6d 2f69 6e76  ransifex.com/inv
 00000150: 656e 696f 736f 6674 7761 7265 2f74 6561  eniosoftware/tea
 00000160: 6d73 2f32 3335 3337 2f72 772f 290a 506c  ms/23537/rw/).Pl
 00000170: 7572 616c 2d46 6f72 6d73 3a20 6e70 6c75  ural-Forms: nplu
 00000180: 7261 6c73 3d32 3b20 706c 7572 616c 3d28  rals=2; plural=(
 00000190: 6e20 213d 2031 293b 0a4d 494d 452d 5665  n != 1);.MIME-Ve
 000001a0: 7273 696f 6e3a 2031 2e30 0a43 6f6e 7465  rsion: 1.0.Conte
```

### Comparing `invenio-users-resources-2.0.0/invenio_users_resources/translations/rw/LC_MESSAGES/messages.po` & `invenio-users-resources-2.0.1/invenio_users_resources/translations/fr_CI/LC_MESSAGES/messages.po`

 * *Files 10% similar despite different names*

```diff
@@ -7,21 +7,21 @@
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-users-resources 0.3.2\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 12:12+0000\n"
 "PO-Revision-Date: 2022-02-16 11:58+0000\n"
-"Language-Team: Kinyarwanda (https://www.transifex.com/inveniosoftware/teams/23537/rw/)\n"
+"Language-Team: French (Côte d'Ivoire) (https://app.transifex.com/inveniosoftware/teams/23537/fr_CI/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.3\n"
-"Language: rw\n"
-"Plural-Forms: nplurals=2; plural=(n != 1);\n"
+"Language: fr_CI\n"
+"Plural-Forms: nplurals=3; plural=(n == 0 || n == 1) ? 0 : n != 0 && n % 1000000 == 0 ? 1 : 2;\n"
 
 #: invenio_users_resources/services/schemas.py:21
 msgid "Value must be either 'public' or 'restricted'."
 msgstr ""
 
 #: invenio_users_resources/services/groups/config.py:43
 msgid "Best match"
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `invenio-users-resources-2.0.0/invenio_users_resources/translations/sk/LC_MESSAGES/messages.mo` & `invenio-users-resources-2.0.1/invenio_users_resources/translations/sk/LC_MESSAGES/messages.mo`

 * *Files 2% similar despite different names*

#### msgunfmt {}

```diff
@@ -2,15 +2,15 @@
 msgstr ""
 "Project-Id-Version: invenio-users-resources 0.3.2\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 12:12+0000\n"
 "PO-Revision-Date: 2022-02-16 11:58+0000\n"
 "Last-Translator: Tibor Simko <tibor.simko@cern.ch>, 2022\n"
 "Language: sk\n"
-"Language-Team: Slovak (https://www.transifex.com/inveniosoftware/teams/23537/"
+"Language-Team: Slovak (https://app.transifex.com/inveniosoftware/teams/23537/"
 "sk/)\n"
 "Plural-Forms: nplurals=4; plural=(n % 1 == 0 && n == 1 ? 0 : n % 1 == 0 && n "
 ">= 2 && n <= 4 ? 1 : n % 1 != 0 ? 2: 3);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.12.1\n"
```

### Comparing `invenio-users-resources-2.0.0/invenio_users_resources/translations/sk/LC_MESSAGES/messages.po` & `invenio-users-resources-2.0.1/invenio_users_resources/translations/sk/LC_MESSAGES/messages.po`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-users-resources 0.3.2\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 12:12+0000\n"
 "PO-Revision-Date: 2022-02-16 11:58+0000\n"
 "Last-Translator: Tibor Simko <tibor.simko@cern.ch>, 2022\n"
-"Language-Team: Slovak (https://www.transifex.com/inveniosoftware/teams/23537/sk/)\n"
+"Language-Team: Slovak (https://app.transifex.com/inveniosoftware/teams/23537/sk/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.3\n"
 "Language: sk\n"
 "Plural-Forms: nplurals=4; plural=(n % 1 == 0 && n == 1 ? 0 : n % 1 == 0 && n >= 2 && n <= 4 ? 1 : n % 1 != 0 ? 2: 3);\n"
```

### Comparing `invenio-users-resources-2.0.0/invenio_users_resources/translations/sv/LC_MESSAGES/messages.mo` & `invenio-users-resources-2.0.1/invenio_users_resources/translations/sv/LC_MESSAGES/messages.mo`

 * *Files 2% similar despite different names*

#### msgunfmt {}

```diff
@@ -2,15 +2,15 @@
 msgstr ""
 "Project-Id-Version: invenio-users-resources 0.3.2\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 12:12+0000\n"
 "PO-Revision-Date: 2022-02-16 11:58+0000\n"
 "Last-Translator: Sam Arbid, 2022\n"
 "Language: sv\n"
-"Language-Team: Swedish (https://www.transifex.com/inveniosoftware/"
+"Language-Team: Swedish (https://app.transifex.com/inveniosoftware/"
 "teams/23537/sv/)\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.12.1\n"
```

### Comparing `invenio-users-resources-2.0.0/invenio_users_resources/translations/sv/LC_MESSAGES/messages.po` & `invenio-users-resources-2.0.1/invenio_users_resources/translations/sv/LC_MESSAGES/messages.po`

 * *Files 9% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-users-resources 0.3.2\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 12:12+0000\n"
 "PO-Revision-Date: 2022-02-16 11:58+0000\n"
 "Last-Translator: Sam Arbid, 2022\n"
-"Language-Team: Swedish (https://www.transifex.com/inveniosoftware/teams/23537/sv/)\n"
+"Language-Team: Swedish (https://app.transifex.com/inveniosoftware/teams/23537/sv/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.3\n"
 "Language: sv\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
```

### Comparing `invenio-users-resources-2.0.0/invenio_users_resources/translations/tr/LC_MESSAGES/messages.mo` & `invenio-users-resources-2.0.1/invenio_users_resources/translations/tr/LC_MESSAGES/messages.mo`

 * *Files 2% similar despite different names*

#### msgunfmt {}

```diff
@@ -3,15 +3,15 @@
 "Project-Id-Version: invenio-users-resources 0.3.2\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 12:12+0000\n"
 "PO-Revision-Date: 2022-02-16 11:58+0000\n"
 "Last-Translator: Ben Translation and Interpreting Services <info@bentercume."
 "com>, 2022\n"
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

### Comparing `invenio-users-resources-2.0.0/invenio_users_resources/translations/tr/LC_MESSAGES/messages.po` & `invenio-users-resources-2.0.1/invenio_users_resources/translations/ne/LC_MESSAGES/messages.po`

 * *Files 18% similar despite different names*

```diff
@@ -1,36 +1,32 @@
 # Translations template for invenio-users-resources.
 # Copyright (C) 2022 CERN
 # This file is distributed under the same license as the
 # invenio-users-resources project.
 # FIRST AUTHOR <EMAIL@ADDRESS>, 2022.
 # 
-# Translators:
-# Ben Translation and Interpreting Services <info@bentercume.com>, 2022
-# 
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-users-resources 0.3.2\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 12:12+0000\n"
 "PO-Revision-Date: 2022-02-16 11:58+0000\n"
-"Last-Translator: Ben Translation and Interpreting Services <info@bentercume.com>, 2022\n"
-"Language-Team: Turkish (https://www.transifex.com/inveniosoftware/teams/23537/tr/)\n"
+"Language-Team: Nepali (https://app.transifex.com/inveniosoftware/teams/23537/ne/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.3\n"
-"Language: tr\n"
-"Plural-Forms: nplurals=2; plural=(n > 1);\n"
+"Language: ne\n"
+"Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
 #: invenio_users_resources/services/schemas.py:21
 msgid "Value must be either 'public' or 'restricted'."
 msgstr ""
 
 #: invenio_users_resources/services/groups/config.py:43
 msgid "Best match"
-msgstr "En iyi eşleşme"
+msgstr ""
 
 #: invenio_users_resources/services/groups/config.py:47
 msgid "Name"
-msgstr "Ad"
+msgstr ""
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `invenio-users-resources-2.0.0/invenio_users_resources/translations/uk/LC_MESSAGES/messages.mo` & `invenio-users-resources-2.0.1/invenio_users_resources/translations/uk_UA/LC_MESSAGES/messages.mo`

 * *Format-specific differences are supported for Gettext message catalogues but no file-specific differences were detected; falling back to a binary diff. file(1) reports: GNU message catalog (little endian), revision 0.0, 1 message, Project-Id-Version: invenio-users-resources 0.3.2*

 * *Files 18% similar despite different names*

```diff
@@ -1,47 +1,48 @@
 00000000: de12 0495 0000 0000 0100 0000 1c00 0000  ................
 00000010: 2400 0000 0000 0000 0000 0000 0000 0000  $...............
-00000020: 2c00 0000 bd02 0000 2d00 0000 0050 726f  ,.......-....Pro
+00000020: 2c00 0000 cd02 0000 2d00 0000 0050 726f  ,.......-....Pro
 00000030: 6a65 6374 2d49 642d 5665 7273 696f 6e3a  ject-Id-Version:
 00000040: 2069 6e76 656e 696f 2d75 7365 7273 2d72   invenio-users-r
 00000050: 6573 6f75 7263 6573 2030 2e33 2e32 0a52  esources 0.3.2.R
 00000060: 6570 6f72 742d 4d73 6769 642d 4275 6773  eport-Msgid-Bugs
 00000070: 2d54 6f3a 2069 6e66 6f40 696e 7665 6e69  -To: info@inveni
 00000080: 6f73 6f66 7477 6172 652e 6f72 670a 504f  osoftware.org.PO
 00000090: 542d 4372 6561 7469 6f6e 2d44 6174 653a  T-Creation-Date:
 000000a0: 2032 3032 322d 3130 2d31 3220 3132 3a31   2022-10-12 12:1
 000000b0: 322b 3030 3030 0a50 4f2d 5265 7669 7369  2+0000.PO-Revisi
 000000c0: 6f6e 2d44 6174 653a 2032 3032 322d 3032  on-Date: 2022-02
 000000d0: 2d31 3620 3131 3a35 382b 3030 3030 0a4c  -16 11:58+0000.L
 000000e0: 6173 742d 5472 616e 736c 6174 6f72 3a20  ast-Translator: 
 000000f0: 4655 4c4c 204e 414d 4520 3c45 4d41 494c  FULL NAME <EMAIL
 00000100: 4041 4444 5245 5353 3e0a 4c61 6e67 7561  @ADDRESS>.Langua
-00000110: 6765 3a20 756b 0a4c 616e 6775 6167 652d  ge: uk.Language-
-00000120: 5465 616d 3a20 556b 7261 696e 6961 6e20  Team: Ukrainian 
-00000130: 2868 7474 7073 3a2f 2f77 7777 2e74 7261  (https://www.tra
-00000140: 6e73 6966 6578 2e63 6f6d 2f69 6e76 656e  nsifex.com/inven
-00000150: 696f 736f 6674 7761 7265 2f74 6561 6d73  iosoftware/teams
-00000160: 2f32 3335 3337 2f75 6b2f 290a 506c 7572  /23537/uk/).Plur
-00000170: 616c 2d46 6f72 6d73 3a20 6e70 6c75 7261  al-Forms: nplura
-00000180: 6c73 3d34 3b20 706c 7572 616c 3d28 6e20  ls=4; plural=(n 
-00000190: 2520 3120 3d3d 2030 2026 2620 6e20 2520  % 1 == 0 && n % 
-000001a0: 3130 203d 3d20 3120 2626 206e 2025 2031  10 == 1 && n % 1
-000001b0: 3030 2021 3d20 3131 203f 2030 203a 206e  00 != 11 ? 0 : n
-000001c0: 2025 2031 203d 3d20 3020 2626 206e 2025   % 1 == 0 && n %
-000001d0: 2031 3020 3e3d 2032 2026 2620 6e20 2520   10 >= 2 && n % 
-000001e0: 3130 203c 3d20 3420 2626 2028 6e20 2520  10 <= 4 && (n % 
-000001f0: 3130 3020 3c20 3132 207c 7c20 6e20 2520  100 < 12 || n % 
-00000200: 3130 3020 3e20 3134 2920 3f20 3120 3a20  100 > 14) ? 1 : 
-00000210: 6e20 2520 3120 3d3d 2030 2026 2620 286e  n % 1 == 0 && (n
-00000220: 2025 2031 3020 3d3d 3020 7c7c 2028 6e20   % 10 ==0 || (n 
-00000230: 2520 3130 203e 3d35 2026 2620 6e20 2520  % 10 >=5 && n % 
-00000240: 3130 203c 3d39 2920 7c7c 2028 6e20 2520  10 <=9) || (n % 
-00000250: 3130 3020 3e3d 3131 2026 2620 6e20 2520  100 >=11 && n % 
-00000260: 3130 3020 3c3d 3134 2029 2920 3f20 323a  100 <=14 )) ? 2:
-00000270: 2033 293b 0a4d 494d 452d 5665 7273 696f   3);.MIME-Versio
-00000280: 6e3a 2031 2e30 0a43 6f6e 7465 6e74 2d54  n: 1.0.Content-T
-00000290: 7970 653a 2074 6578 742f 706c 6169 6e3b  ype: text/plain;
-000002a0: 2063 6861 7273 6574 3d75 7466 2d38 0a43   charset=utf-8.C
-000002b0: 6f6e 7465 6e74 2d54 7261 6e73 6665 722d  ontent-Transfer-
-000002c0: 456e 636f 6469 6e67 3a20 3862 6974 0a47  Encoding: 8bit.G
-000002d0: 656e 6572 6174 6564 2d42 793a 2042 6162  enerated-By: Bab
-000002e0: 656c 2032 2e31 322e 310a 00              el 2.12.1..
+00000110: 6765 3a20 756b 5f55 410a 4c61 6e67 7561  ge: uk_UA.Langua
+00000120: 6765 2d54 6561 6d3a 2055 6b72 6169 6e69  ge-Team: Ukraini
+00000130: 616e 2028 556b 7261 696e 6529 2028 6874  an (Ukraine) (ht
+00000140: 7470 733a 2f2f 6170 702e 7472 616e 7369  tps://app.transi
+00000150: 6665 782e 636f 6d2f 696e 7665 6e69 6f73  fex.com/invenios
+00000160: 6f66 7477 6172 652f 7465 616d 732f 3233  oftware/teams/23
+00000170: 3533 372f 756b 5f55 412f 290a 506c 7572  537/uk_UA/).Plur
+00000180: 616c 2d46 6f72 6d73 3a20 6e70 6c75 7261  al-Forms: nplura
+00000190: 6c73 3d34 3b20 706c 7572 616c 3d28 6e20  ls=4; plural=(n 
+000001a0: 2520 3120 3d3d 2030 2026 2620 6e20 2520  % 1 == 0 && n % 
+000001b0: 3130 203d 3d20 3120 2626 206e 2025 2031  10 == 1 && n % 1
+000001c0: 3030 2021 3d20 3131 203f 2030 203a 206e  00 != 11 ? 0 : n
+000001d0: 2025 2031 203d 3d20 3020 2626 206e 2025   % 1 == 0 && n %
+000001e0: 2031 3020 3e3d 2032 2026 2620 6e20 2520   10 >= 2 && n % 
+000001f0: 3130 203c 3d20 3420 2626 2028 6e20 2520  10 <= 4 && (n % 
+00000200: 3130 3020 3c20 3132 207c 7c20 6e20 2520  100 < 12 || n % 
+00000210: 3130 3020 3e20 3134 2920 3f20 3120 3a20  100 > 14) ? 1 : 
+00000220: 6e20 2520 3120 3d3d 2030 2026 2620 286e  n % 1 == 0 && (n
+00000230: 2025 2031 3020 3d3d 3020 7c7c 2028 6e20   % 10 ==0 || (n 
+00000240: 2520 3130 203e 3d35 2026 2620 6e20 2520  % 10 >=5 && n % 
+00000250: 3130 203c 3d39 2920 7c7c 2028 6e20 2520  10 <=9) || (n % 
+00000260: 3130 3020 3e3d 3131 2026 2620 6e20 2520  100 >=11 && n % 
+00000270: 3130 3020 3c3d 3134 2029 2920 3f20 323a  100 <=14 )) ? 2:
+00000280: 2033 293b 0a4d 494d 452d 5665 7273 696f   3);.MIME-Versio
+00000290: 6e3a 2031 2e30 0a43 6f6e 7465 6e74 2d54  n: 1.0.Content-T
+000002a0: 7970 653a 2074 6578 742f 706c 6169 6e3b  ype: text/plain;
+000002b0: 2063 6861 7273 6574 3d75 7466 2d38 0a43   charset=utf-8.C
+000002c0: 6f6e 7465 6e74 2d54 7261 6e73 6665 722d  ontent-Transfer-
+000002d0: 456e 636f 6469 6e67 3a20 3862 6974 0a47  Encoding: 8bit.G
+000002e0: 656e 6572 6174 6564 2d42 793a 2042 6162  enerated-By: Bab
+000002f0: 656c 2032 2e31 322e 310a 00              el 2.12.1..
```

### Comparing `invenio-users-resources-2.0.0/invenio_users_resources/translations/uk/LC_MESSAGES/messages.po` & `invenio-users-resources-2.0.1/invenio_users_resources/translations/fr_FR/LC_MESSAGES/messages.po`

 * *Files 10% similar despite different names*

```diff
@@ -7,21 +7,21 @@
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-users-resources 0.3.2\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 12:12+0000\n"
 "PO-Revision-Date: 2022-02-16 11:58+0000\n"
-"Language-Team: Ukrainian (https://www.transifex.com/inveniosoftware/teams/23537/uk/)\n"
+"Language-Team: French (France) (https://app.transifex.com/inveniosoftware/teams/23537/fr_FR/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.3\n"
-"Language: uk\n"
-"Plural-Forms: nplurals=4; plural=(n % 1 == 0 && n % 10 == 1 && n % 100 != 11 ? 0 : n % 1 == 0 && n % 10 >= 2 && n % 10 <= 4 && (n % 100 < 12 || n % 100 > 14) ? 1 : n % 1 == 0 && (n % 10 ==0 || (n % 10 >=5 && n % 10 <=9) || (n % 100 >=11 && n % 100 <=14 )) ? 2: 3);\n"
+"Language: fr_FR\n"
+"Plural-Forms: nplurals=3; plural=(n == 0 || n == 1) ? 0 : n != 0 && n % 1000000 == 0 ? 1 : 2;\n"
 
 #: invenio_users_resources/services/schemas.py:21
 msgid "Value must be either 'public' or 'restricted'."
 msgstr ""
 
 #: invenio_users_resources/services/groups/config.py:43
 msgid "Best match"
```

### Comparing `invenio-users-resources-2.0.0/invenio_users_resources/translations/zh_CN/LC_MESSAGES/messages.mo` & `invenio-users-resources-2.0.1/invenio_users_resources/translations/fa_IR/LC_MESSAGES/messages.mo`

 * *Files 20% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,24 +0,0 @@
-msgid ""
-msgstr ""
-"Project-Id-Version: invenio-users-resources 0.3.2\n"
-"Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
-"POT-Creation-Date: 2022-10-12 12:12+0000\n"
-"PO-Revision-Date: 2022-02-16 11:58+0000\n"
-"Last-Translator: Kalven Richie, 2022\n"
-"Language: zh_CN\n"
-"Language-Team: Chinese (China) (https://www.transifex.com/inveniosoftware/"
-"teams/23537/zh_CN/)\n"
-"Plural-Forms: nplurals=1; plural=0;\n"
-"MIME-Version: 1.0\n"
-"Content-Type: text/plain; charset=utf-8\n"
-"Content-Transfer-Encoding: 8bit\n"
-"Generated-By: Babel 2.12.1\n"
-
-msgid "Best match"
-msgstr "最佳匹配"
-
-msgid "Name"
-msgstr "名称"
-
-msgid "Value must be either 'public' or 'restricted'."
-msgstr "值必须为“public”或“restricted”。"
```

### Comparing `invenio-users-resources-2.0.0/invenio_users_resources/translations/zh_CN/LC_MESSAGES/messages.po` & `invenio-users-resources-2.0.1/invenio_users_resources/translations/zh_CN/LC_MESSAGES/messages.po`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-users-resources 0.3.2\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 12:12+0000\n"
 "PO-Revision-Date: 2022-02-16 11:58+0000\n"
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

### Comparing `invenio-users-resources-2.0.0/invenio_users_resources/translations/zh_TW/LC_MESSAGES/messages.mo` & `invenio-users-resources-2.0.1/invenio_users_resources/translations/zh_TW/LC_MESSAGES/messages.mo`

 * *Files 2% similar despite different names*

#### msgunfmt {}

```diff
@@ -2,15 +2,15 @@
 msgstr ""
 "Project-Id-Version: invenio-users-resources 0.3.2\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 12:12+0000\n"
 "PO-Revision-Date: 2022-02-16 11:58+0000\n"
 "Last-Translator: Tibor Simko <tibor.simko@cern.ch>, 2022\n"
 "Language: zh_TW\n"
-"Language-Team: Chinese (Taiwan) (https://www.transifex.com/inveniosoftware/"
+"Language-Team: Chinese (Taiwan) (https://app.transifex.com/inveniosoftware/"
 "teams/23537/zh_TW/)\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.12.1\n"
```

### Comparing `invenio-users-resources-2.0.0/invenio_users_resources/translations/zh_TW/LC_MESSAGES/messages.po` & `invenio-users-resources-2.0.1/invenio_users_resources/translations/fa_IR/LC_MESSAGES/messages.po`

 * *Files 12% similar despite different names*

```diff
@@ -1,36 +1,32 @@
 # Translations template for invenio-users-resources.
 # Copyright (C) 2022 CERN
 # This file is distributed under the same license as the
 # invenio-users-resources project.
 # FIRST AUTHOR <EMAIL@ADDRESS>, 2022.
 # 
-# Translators:
-# Tibor Simko <tibor.simko@cern.ch>, 2022
-# 
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-users-resources 0.3.2\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 12:12+0000\n"
 "PO-Revision-Date: 2022-02-16 11:58+0000\n"
-"Last-Translator: Tibor Simko <tibor.simko@cern.ch>, 2022\n"
-"Language-Team: Chinese (Taiwan) (https://www.transifex.com/inveniosoftware/teams/23537/zh_TW/)\n"
+"Language-Team: Persian (Iran) (https://app.transifex.com/inveniosoftware/teams/23537/fa_IR/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.3\n"
-"Language: zh_TW\n"
-"Plural-Forms: nplurals=1; plural=0;\n"
+"Language: fa_IR\n"
+"Plural-Forms: nplurals=2; plural=(n > 1);\n"
 
 #: invenio_users_resources/services/schemas.py:21
 msgid "Value must be either 'public' or 'restricted'."
 msgstr ""
 
 #: invenio_users_resources/services/groups/config.py:43
 msgid "Best match"
 msgstr ""
 
 #: invenio_users_resources/services/groups/config.py:47
 msgid "Name"
-msgstr "名稱"
+msgstr ""
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `invenio-users-resources-2.0.0/invenio_users_resources/views.py` & `invenio-users-resources-2.0.1/invenio_users_resources/views.py`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-2.0.0/invenio_users_resources.egg-info/PKG-INFO` & `invenio-users-resources-2.0.1/invenio_users_resources.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invenio-users-resources
-Version: 2.0.0
+Version: 2.0.1
 Summary: Invenio module providing management APIs for users and roles/groups.
 Home-page: https://github.com/inveniosoftware/invenio-users-resources
 Author: CERN/TU Wien/JRC
 Author-email: info@inveniosoftware.org
 License: MIT
 Description: ..
             Copyright (C) 2022 CERN.
@@ -42,14 +42,19 @@
             Invenio-Users-Resources is free software; you can redistribute it
             and/or modify it under the terms of the MIT License; see LICENSE file for
             more details.
         
         Changes
         =======
         
+        Version 2.0.1 (2023-07-05)
+        
+        - fix post_commit hooks
+        - add translations
+        
         Version 2.0.0 (2023-06-30)
         
         - changing the groups tasks interface to use bulk indexing as default
         
         Version 1.9.0 (2023-06-15)
         
         - groups: add description field
```

### Comparing `invenio-users-resources-2.0.0/invenio_users_resources.egg-info/SOURCES.txt` & `invenio-users-resources-2.0.1/invenio_users_resources.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -103,40 +103,64 @@
 invenio_users_resources/translations/ca/LC_MESSAGES/messages.po
 invenio_users_resources/translations/cs/LC_MESSAGES/messages.mo
 invenio_users_resources/translations/cs/LC_MESSAGES/messages.po
 invenio_users_resources/translations/da/LC_MESSAGES/messages.mo
 invenio_users_resources/translations/da/LC_MESSAGES/messages.po
 invenio_users_resources/translations/de/LC_MESSAGES/messages.mo
 invenio_users_resources/translations/de/LC_MESSAGES/messages.po
+invenio_users_resources/translations/de_AT/LC_MESSAGES/messages.mo
+invenio_users_resources/translations/de_AT/LC_MESSAGES/messages.po
+invenio_users_resources/translations/de_DE/LC_MESSAGES/messages.mo
+invenio_users_resources/translations/de_DE/LC_MESSAGES/messages.po
 invenio_users_resources/translations/el/LC_MESSAGES/messages.mo
 invenio_users_resources/translations/el/LC_MESSAGES/messages.po
+invenio_users_resources/translations/en_AT/LC_MESSAGES/messages.mo
+invenio_users_resources/translations/en_AT/LC_MESSAGES/messages.po
+invenio_users_resources/translations/en_HU/LC_MESSAGES/messages.mo
+invenio_users_resources/translations/en_HU/LC_MESSAGES/messages.po
 invenio_users_resources/translations/es/LC_MESSAGES/messages.mo
 invenio_users_resources/translations/es/LC_MESSAGES/messages.po
+invenio_users_resources/translations/es_CU/LC_MESSAGES/messages.mo
+invenio_users_resources/translations/es_CU/LC_MESSAGES/messages.po
+invenio_users_resources/translations/es_MX/LC_MESSAGES/messages.mo
+invenio_users_resources/translations/es_MX/LC_MESSAGES/messages.po
 invenio_users_resources/translations/et/LC_MESSAGES/messages.mo
 invenio_users_resources/translations/et/LC_MESSAGES/messages.po
 invenio_users_resources/translations/et_EE/LC_MESSAGES/messages.mo
 invenio_users_resources/translations/et_EE/LC_MESSAGES/messages.po
 invenio_users_resources/translations/fa/LC_MESSAGES/messages.mo
 invenio_users_resources/translations/fa/LC_MESSAGES/messages.po
+invenio_users_resources/translations/fa_IR/LC_MESSAGES/messages.mo
+invenio_users_resources/translations/fa_IR/LC_MESSAGES/messages.po
 invenio_users_resources/translations/fr/LC_MESSAGES/messages.mo
 invenio_users_resources/translations/fr/LC_MESSAGES/messages.po
+invenio_users_resources/translations/fr_CI/LC_MESSAGES/messages.mo
+invenio_users_resources/translations/fr_CI/LC_MESSAGES/messages.po
+invenio_users_resources/translations/fr_FR/LC_MESSAGES/messages.mo
+invenio_users_resources/translations/fr_FR/LC_MESSAGES/messages.po
 invenio_users_resources/translations/gl/LC_MESSAGES/messages.mo
 invenio_users_resources/translations/gl/LC_MESSAGES/messages.po
+invenio_users_resources/translations/hi_IN/LC_MESSAGES/messages.mo
+invenio_users_resources/translations/hi_IN/LC_MESSAGES/messages.po
 invenio_users_resources/translations/hr/LC_MESSAGES/messages.mo
 invenio_users_resources/translations/hr/LC_MESSAGES/messages.po
 invenio_users_resources/translations/hu/LC_MESSAGES/messages.mo
 invenio_users_resources/translations/hu/LC_MESSAGES/messages.po
+invenio_users_resources/translations/hu_HU/LC_MESSAGES/messages.mo
+invenio_users_resources/translations/hu_HU/LC_MESSAGES/messages.po
 invenio_users_resources/translations/it/LC_MESSAGES/messages.mo
 invenio_users_resources/translations/it/LC_MESSAGES/messages.po
 invenio_users_resources/translations/ja/LC_MESSAGES/messages.mo
 invenio_users_resources/translations/ja/LC_MESSAGES/messages.po
 invenio_users_resources/translations/ka/LC_MESSAGES/messages.mo
 invenio_users_resources/translations/ka/LC_MESSAGES/messages.po
 invenio_users_resources/translations/lt/LC_MESSAGES/messages.mo
 invenio_users_resources/translations/lt/LC_MESSAGES/messages.po
+invenio_users_resources/translations/ne/LC_MESSAGES/messages.mo
+invenio_users_resources/translations/ne/LC_MESSAGES/messages.po
 invenio_users_resources/translations/no/LC_MESSAGES/messages.mo
 invenio_users_resources/translations/no/LC_MESSAGES/messages.po
 invenio_users_resources/translations/pl/LC_MESSAGES/messages.mo
 invenio_users_resources/translations/pl/LC_MESSAGES/messages.po
 invenio_users_resources/translations/pt/LC_MESSAGES/messages.mo
 invenio_users_resources/translations/pt/LC_MESSAGES/messages.po
 invenio_users_resources/translations/ro/LC_MESSAGES/messages.mo
@@ -145,18 +169,22 @@
 invenio_users_resources/translations/ru/LC_MESSAGES/messages.po
 invenio_users_resources/translations/rw/LC_MESSAGES/messages.mo
 invenio_users_resources/translations/rw/LC_MESSAGES/messages.po
 invenio_users_resources/translations/sk/LC_MESSAGES/messages.mo
 invenio_users_resources/translations/sk/LC_MESSAGES/messages.po
 invenio_users_resources/translations/sv/LC_MESSAGES/messages.mo
 invenio_users_resources/translations/sv/LC_MESSAGES/messages.po
+invenio_users_resources/translations/sv_SE/LC_MESSAGES/messages.mo
+invenio_users_resources/translations/sv_SE/LC_MESSAGES/messages.po
 invenio_users_resources/translations/tr/LC_MESSAGES/messages.mo
 invenio_users_resources/translations/tr/LC_MESSAGES/messages.po
 invenio_users_resources/translations/uk/LC_MESSAGES/messages.mo
 invenio_users_resources/translations/uk/LC_MESSAGES/messages.po
+invenio_users_resources/translations/uk_UA/LC_MESSAGES/messages.mo
+invenio_users_resources/translations/uk_UA/LC_MESSAGES/messages.po
 invenio_users_resources/translations/zh_CN/LC_MESSAGES/messages.mo
 invenio_users_resources/translations/zh_CN/LC_MESSAGES/messages.po
 invenio_users_resources/translations/zh_TW/LC_MESSAGES/messages.mo
 invenio_users_resources/translations/zh_TW/LC_MESSAGES/messages.po
 tests/conftest.py
 tests/test_invenio_users_resources.py
 tests/test_notifications.py
```

### Comparing `invenio-users-resources-2.0.0/invenio_users_resources.egg-info/entry_points.txt` & `invenio-users-resources-2.0.1/invenio_users_resources.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-2.0.0/run-tests.sh` & `invenio-users-resources-2.0.1/run-tests.sh`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-2.0.0/setup.cfg` & `invenio-users-resources-2.0.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-2.0.0/tests/conftest.py` & `invenio-users-resources-2.0.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-2.0.0/tests/resources/test_resources_groups.py` & `invenio-users-resources-2.0.1/tests/resources/test_resources_groups.py`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-2.0.0/tests/resources/test_resources_users.py` & `invenio-users-resources-2.0.1/tests/resources/test_resources_users.py`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-2.0.0/tests/services/test_service_groups.py` & `invenio-users-resources-2.0.1/tests/services/test_service_groups.py`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-2.0.0/tests/services/test_service_users.py` & `invenio-users-resources-2.0.1/tests/services/test_service_users.py`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-2.0.0/tests/test_invenio_users_resources.py` & `invenio-users-resources-2.0.1/tests/test_invenio_users_resources.py`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-2.0.0/tests/test_notifications.py` & `invenio-users-resources-2.0.1/tests/test_notifications.py`

 * *Files identical despite different names*

