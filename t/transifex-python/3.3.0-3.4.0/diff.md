# Comparing `tmp/transifex-python-3.3.0.tar.gz` & `tmp/transifex-python-3.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/transifex-python-3.3.0.tar", last modified: Tue Mar 21 09:04:59 2023, max compression
+gzip compressed data, was "dist/transifex-python-3.4.0.tar", last modified: Wed Jul  5 13:01:58 2023, max compression
```

## Comparing `transifex-python-3.3.0.tar` & `transifex-python-3.4.0.tar`

### file list

```diff
@@ -1,138 +1,138 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 09:04:59.000000 transifex-python-3.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-03-21 09:04:56.000000 transifex-python-3.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3250 2023-03-21 09:04:59.000000 transifex-python-3.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2415 2023-03-21 09:04:56.000000 transifex-python-3.3.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-03-21 09:04:59.000000 transifex-python-3.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      809 2023-03-21 09:04:56.000000 transifex-python-3.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 09:04:59.000000 transifex-python-3.3.0/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 09:04:59.000000 transifex-python-3.3.0/tests/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-21 09:04:56.000000 transifex-python-3.3.0/tests/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-03-21 09:04:56.000000 transifex-python-3.3.0/tests/api/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-03-21 09:04:56.000000 transifex-python-3.3.0/tests/api/payloads.py
--rw-r--r--   0 runner    (1001) docker     (123)     1624 2023-03-21 09:04:56.000000 transifex-python-3.3.0/tests/api/test_apis.py
--rw-r--r--   0 runner    (1001) docker     (123)     4231 2023-03-21 09:04:56.000000 transifex-python-3.3.0/tests/api/test_bulk.py
--rw-r--r--   0 runner    (1001) docker     (123)     2617 2023-03-21 09:04:56.000000 transifex-python-3.3.0/tests/api/test_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2341 2023-03-21 09:04:56.000000 transifex-python-3.3.0/tests/api/test_plural_lists.py
--rw-r--r--   0 runner    (1001) docker     (123)     6168 2023-03-21 09:04:56.000000 transifex-python-3.3.0/tests/api/test_queryset.py
--rw-r--r--   0 runner    (1001) docker     (123)     5946 2023-03-21 09:04:56.000000 transifex-python-3.3.0/tests/api/test_relationships.py
--rw-r--r--   0 runner    (1001) docker     (123)     7560 2023-03-21 09:04:56.000000 transifex-python-3.3.0/tests/api/test_single_resource.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 09:04:59.000000 transifex-python-3.3.0/tests/common/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-21 09:04:56.000000 transifex-python-3.3.0/tests/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1781 2023-03-21 09:04:56.000000 transifex-python-3.3.0/tests/common/test_is_plural.py
--rw-r--r--   0 runner    (1001) docker     (123)    11401 2023-03-21 09:04:56.000000 transifex-python-3.3.0/tests/common/test_strings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 09:04:59.000000 transifex-python-3.3.0/tests/native/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-21 09:04:56.000000 transifex-python-3.3.0/tests/native/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-03-21 09:04:56.000000 transifex-python-3.3.0/tests/native/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 09:04:59.000000 transifex-python-3.3.0/tests/native/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-21 09:04:56.000000 transifex-python-3.3.0/tests/native/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-03-21 09:04:56.000000 transifex-python-3.3.0/tests/native/core/test_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)    19402 2023-03-21 09:04:56.000000 transifex-python-3.3.0/tests/native/core/test_cds.py
--rw-r--r--   0 runner    (1001) docker     (123)    14928 2023-03-21 09:04:56.000000 transifex-python-3.3.0/tests/native/core/test_core.py
--rw-r--r--   0 runner    (1001) docker     (123)     1610 2023-03-21 09:04:56.000000 transifex-python-3.3.0/tests/native/core/test_daemon.py
--rw-r--r--   0 runner    (1001) docker     (123)     2039 2023-03-21 09:04:56.000000 transifex-python-3.3.0/tests/native/core/test_init.py
--rw-r--r--   0 runner    (1001) docker     (123)     4498 2023-03-21 09:04:56.000000 transifex-python-3.3.0/tests/native/core/test_parsing.py
--rw-r--r--   0 runner    (1001) docker     (123)    10082 2023-03-21 09:04:56.000000 transifex-python-3.3.0/tests/native/core/test_rendering.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 09:04:59.000000 transifex-python-3.3.0/tests/native/core/test_tools/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-21 09:04:56.000000 transifex-python-3.3.0/tests/native/core/test_tools/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 09:04:59.000000 transifex-python-3.3.0/tests/native/core/test_tools/test_migrations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-21 09:04:56.000000 transifex-python-3.3.0/tests/native/core/test_tools/test_migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3366 2023-03-21 09:04:56.000000 transifex-python-3.3.0/tests/native/core/test_tools/test_migrations/test_mark.py
--rw-r--r--   0 runner    (1001) docker     (123)     3768 2023-03-21 09:04:56.000000 transifex-python-3.3.0/tests/native/core/test_tools/test_migrations/test_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     5632 2023-03-21 09:04:56.000000 transifex-python-3.3.0/tests/native/core/test_tools/test_migrations/test_review.py
--rw-r--r--   0 runner    (1001) docker     (123)     3441 2023-03-21 09:04:56.000000 transifex-python-3.3.0/tests/native/core/test_tools/test_migrations/test_save.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 09:04:59.000000 transifex-python-3.3.0/tests/native/django/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-21 09:04:56.000000 transifex-python-3.3.0/tests/native/django/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      658 2023-03-21 09:04:56.000000 transifex-python-3.3.0/tests/native/django/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 09:04:59.000000 transifex-python-3.3.0/tests/native/django/test_commands/
--rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-03-21 09:04:56.000000 transifex-python-3.3.0/tests/native/django/test_commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2693 2023-03-21 09:04:56.000000 transifex-python-3.3.0/tests/native/django/test_commands/test_invalidatetransifex.py
--rw-r--r--   0 runner    (1001) docker     (123)    15314 2023-03-21 09:04:56.000000 transifex-python-3.3.0/tests/native/django/test_commands/test_migratetransifex.py
--rw-r--r--   0 runner    (1001) docker     (123)    14797 2023-03-21 09:04:56.000000 transifex-python-3.3.0/tests/native/django/test_commands/test_pushtransifex.py
--rw-r--r--   0 runner    (1001) docker     (123)    20355 2023-03-21 09:04:56.000000 transifex-python-3.3.0/tests/native/django/test_templatetag.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 09:04:59.000000 transifex-python-3.3.0/tests/native/django/test_tools/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-21 09:04:56.000000 transifex-python-3.3.0/tests/native/django/test_tools/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 09:04:59.000000 transifex-python-3.3.0/tests/native/django/test_tools/test_migrations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-21 09:04:56.000000 transifex-python-3.3.0/tests/native/django/test_tools/test_migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3575 2023-03-21 09:04:56.000000 transifex-python-3.3.0/tests/native/django/test_tools/test_migrations/test_templatetags.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 09:04:59.000000 transifex-python-3.3.0/tests/native/django/test_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-21 09:04:56.000000 transifex-python-3.3.0/tests/native/django/test_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-03-21 09:04:56.000000 transifex-python-3.3.0/tests/native/django/test_utils/test_init.py
--rw-r--r--   0 runner    (1001) docker     (123)     2818 2023-03-21 09:04:56.000000 transifex-python-3.3.0/tests/native/django/test_utils/test_templates.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 09:04:59.000000 transifex-python-3.3.0/transifex/
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-03-21 09:04:56.000000 transifex-python-3.3.0/transifex/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-03-21 09:04:59.000000 transifex-python-3.3.0/transifex/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 09:04:59.000000 transifex-python-3.3.0/transifex/api/
--rw-r--r--   0 runner    (1001) docker     (123)     8677 2023-03-21 09:04:56.000000 transifex-python-3.3.0/transifex/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      979 2023-03-21 09:04:56.000000 transifex-python-3.3.0/transifex/api/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 09:04:59.000000 transifex-python-3.3.0/transifex/api/jsonapi/
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-03-21 09:04:56.000000 transifex-python-3.3.0/transifex/api/jsonapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7548 2023-03-21 09:04:56.000000 transifex-python-3.3.0/transifex/api/jsonapi/apis.py
--rw-r--r--   0 runner    (1001) docker     (123)     2556 2023-03-21 09:04:56.000000 transifex-python-3.3.0/transifex/api/jsonapi/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     5969 2023-03-21 09:04:56.000000 transifex-python-3.3.0/transifex/api/jsonapi/collections.py
--rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-03-21 09:04:56.000000 transifex-python-3.3.0/transifex/api/jsonapi/compat.py
--rw-r--r--   0 runner    (1001) docker     (123)     5892 2023-03-21 09:04:56.000000 transifex-python-3.3.0/transifex/api/jsonapi/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    31687 2023-03-21 09:04:56.000000 transifex-python-3.3.0/transifex/api/jsonapi/resources.py
--rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-03-21 09:04:56.000000 transifex-python-3.3.0/transifex/api/jsonapi/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 09:04:59.000000 transifex-python-3.3.0/transifex/common/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-21 09:04:56.000000 transifex-python-3.3.0/transifex/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-03-21 09:04:56.000000 transifex-python-3.3.0/transifex/common/_compat.py
--rw-r--r--   0 runner    (1001) docker     (123)     2779 2023-03-21 09:04:56.000000 transifex-python-3.3.0/transifex/common/console.py
--rw-r--r--   0 runner    (1001) docker     (123)     6811 2023-03-21 09:04:56.000000 transifex-python-3.3.0/transifex/common/strings.py
--rw-r--r--   0 runner    (1001) docker     (123)     7311 2023-03-21 09:04:56.000000 transifex-python-3.3.0/transifex/common/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 09:04:59.000000 transifex-python-3.3.0/transifex/native/
--rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-03-21 09:04:56.000000 transifex-python-3.3.0/transifex/native/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2502 2023-03-21 09:04:56.000000 transifex-python-3.3.0/transifex/native/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)    13093 2023-03-21 09:04:56.000000 transifex-python-3.3.0/transifex/native/cds.py
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-03-21 09:04:56.000000 transifex-python-3.3.0/transifex/native/consts.py
--rw-r--r--   0 runner    (1001) docker     (123)    10102 2023-03-21 09:04:56.000000 transifex-python-3.3.0/transifex/native/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     2477 2023-03-21 09:04:56.000000 transifex-python-3.3.0/transifex/native/daemon.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 09:04:59.000000 transifex-python-3.3.0/transifex/native/django/
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-03-21 09:04:56.000000 transifex-python-3.3.0/transifex/native/django/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4552 2023-03-21 09:04:56.000000 transifex-python-3.3.0/transifex/native/django/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-03-21 09:04:56.000000 transifex-python-3.3.0/transifex/native/django/compat.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 09:04:59.000000 transifex-python-3.3.0/transifex/native/django/management/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-21 09:04:56.000000 transifex-python-3.3.0/transifex/native/django/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 09:04:59.000000 transifex-python-3.3.0/transifex/native/django/management/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-21 09:04:56.000000 transifex-python-3.3.0/transifex/native/django/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2661 2023-03-21 09:04:56.000000 transifex-python-3.3.0/transifex/native/django/management/commands/transifex.py
--rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-03-21 09:04:56.000000 transifex-python-3.3.0/transifex/native/django/management/common.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 09:04:59.000000 transifex-python-3.3.0/transifex/native/django/management/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-21 09:04:56.000000 transifex-python-3.3.0/transifex/native/django/management/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5010 2023-03-21 09:04:56.000000 transifex-python-3.3.0/transifex/native/django/management/utils/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2872 2023-03-21 09:04:56.000000 transifex-python-3.3.0/transifex/native/django/management/utils/invalidate.py
--rw-r--r--   0 runner    (1001) docker     (123)     8356 2023-03-21 09:04:56.000000 transifex-python-3.3.0/transifex/native/django/management/utils/migrate.py
--rw-r--r--   0 runner    (1001) docker     (123)    15301 2023-03-21 09:04:56.000000 transifex-python-3.3.0/transifex/native/django/management/utils/push.py
--rw-r--r--   0 runner    (1001) docker     (123)    15293 2023-03-21 09:04:56.000000 transifex-python-3.3.0/transifex/native/django/management/utils/try_templatetag.py
--rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-03-21 09:04:56.000000 transifex-python-3.3.0/transifex/native/django/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 09:04:59.000000 transifex-python-3.3.0/transifex/native/django/templatetags/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-21 09:04:56.000000 transifex-python-3.3.0/transifex/native/django/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12422 2023-03-21 09:04:56.000000 transifex-python-3.3.0/transifex/native/django/templatetags/transifex.py
--rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-03-21 09:04:56.000000 transifex-python-3.3.0/transifex/native/django/templatetags/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 09:04:59.000000 transifex-python-3.3.0/transifex/native/django/tools/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-21 09:04:56.000000 transifex-python-3.3.0/transifex/native/django/tools/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 09:04:59.000000 transifex-python-3.3.0/transifex/native/django/tools/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-21 09:04:56.000000 transifex-python-3.3.0/transifex/native/django/tools/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26025 2023-03-21 09:04:56.000000 transifex-python-3.3.0/transifex/native/django/tools/migrations/templatetags.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 09:04:59.000000 transifex-python-3.3.0/transifex/native/django/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     3045 2023-03-21 09:04:56.000000 transifex-python-3.3.0/transifex/native/django/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4158 2023-03-21 09:04:56.000000 transifex-python-3.3.0/transifex/native/django/utils/templates.py
--rw-r--r--   0 runner    (1001) docker     (123)    18581 2023-03-21 09:04:56.000000 transifex-python-3.3.0/transifex/native/parsing.py
--rw-r--r--   0 runner    (1001) docker     (123)     9795 2023-03-21 09:04:56.000000 transifex-python-3.3.0/transifex/native/rendering.py
--rw-r--r--   0 runner    (1001) docker     (123)     2337 2023-03-21 09:04:56.000000 transifex-python-3.3.0/transifex/native/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 09:04:59.000000 transifex-python-3.3.0/transifex/native/tools/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-21 09:04:56.000000 transifex-python-3.3.0/transifex/native/tools/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 09:04:59.000000 transifex-python-3.3.0/transifex/native/tools/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-21 09:04:56.000000 transifex-python-3.3.0/transifex/native/tools/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18197 2023-03-21 09:04:56.000000 transifex-python-3.3.0/transifex/native/tools/migrations/execution.py
--rw-r--r--   0 runner    (1001) docker     (123)    34399 2023-03-21 09:04:56.000000 transifex-python-3.3.0/transifex/native/tools/migrations/gettext.py
--rw-r--r--   0 runner    (1001) docker     (123)     5065 2023-03-21 09:04:56.000000 transifex-python-3.3.0/transifex/native/tools/migrations/mark.py
--rw-r--r--   0 runner    (1001) docker     (123)     5615 2023-03-21 09:04:56.000000 transifex-python-3.3.0/transifex/native/tools/migrations/models.py
--rw-r--r--   0 runner    (1001) docker     (123)    19611 2023-03-21 09:04:56.000000 transifex-python-3.3.0/transifex/native/tools/migrations/review.py
--rw-r--r--   0 runner    (1001) docker     (123)     6226 2023-03-21 09:04:56.000000 transifex-python-3.3.0/transifex/native/tools/migrations/save.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 09:04:59.000000 transifex-python-3.3.0/transifex_python.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3250 2023-03-21 09:04:59.000000 transifex-python-3.3.0/transifex_python.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4013 2023-03-21 09:04:59.000000 transifex-python-3.3.0/transifex_python.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-21 09:04:59.000000 transifex-python-3.3.0/transifex_python.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-03-21 09:04:59.000000 transifex-python-3.3.0/transifex_python.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-03-21 09:04:59.000000 transifex-python-3.3.0/transifex_python.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    68611 2023-03-21 09:04:56.000000 transifex-python-3.3.0/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 13:01:58.000000 transifex-python-3.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-05 13:01:56.000000 transifex-python-3.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3250 2023-07-05 13:01:58.000000 transifex-python-3.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2415 2023-07-05 13:01:56.000000 transifex-python-3.4.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-07-05 13:01:58.000000 transifex-python-3.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      809 2023-07-05 13:01:56.000000 transifex-python-3.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 13:01:58.000000 transifex-python-3.4.0/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 13:01:58.000000 transifex-python-3.4.0/tests/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 13:01:56.000000 transifex-python-3.4.0/tests/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-07-05 13:01:56.000000 transifex-python-3.4.0/tests/api/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-07-05 13:01:56.000000 transifex-python-3.4.0/tests/api/payloads.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1624 2023-07-05 13:01:56.000000 transifex-python-3.4.0/tests/api/test_apis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4231 2023-07-05 13:01:56.000000 transifex-python-3.4.0/tests/api/test_bulk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2617 2023-07-05 13:01:56.000000 transifex-python-3.4.0/tests/api/test_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2341 2023-07-05 13:01:56.000000 transifex-python-3.4.0/tests/api/test_plural_lists.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6168 2023-07-05 13:01:56.000000 transifex-python-3.4.0/tests/api/test_queryset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5946 2023-07-05 13:01:56.000000 transifex-python-3.4.0/tests/api/test_relationships.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7560 2023-07-05 13:01:56.000000 transifex-python-3.4.0/tests/api/test_single_resource.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 13:01:58.000000 transifex-python-3.4.0/tests/common/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 13:01:56.000000 transifex-python-3.4.0/tests/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1781 2023-07-05 13:01:56.000000 transifex-python-3.4.0/tests/common/test_is_plural.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11401 2023-07-05 13:01:56.000000 transifex-python-3.4.0/tests/common/test_strings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 13:01:58.000000 transifex-python-3.4.0/tests/native/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 13:01:56.000000 transifex-python-3.4.0/tests/native/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-07-05 13:01:56.000000 transifex-python-3.4.0/tests/native/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 13:01:58.000000 transifex-python-3.4.0/tests/native/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 13:01:56.000000 transifex-python-3.4.0/tests/native/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-07-05 13:01:56.000000 transifex-python-3.4.0/tests/native/core/test_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19402 2023-07-05 13:01:56.000000 transifex-python-3.4.0/tests/native/core/test_cds.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14940 2023-07-05 13:01:56.000000 transifex-python-3.4.0/tests/native/core/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1610 2023-07-05 13:01:56.000000 transifex-python-3.4.0/tests/native/core/test_daemon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2039 2023-07-05 13:01:56.000000 transifex-python-3.4.0/tests/native/core/test_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4498 2023-07-05 13:01:56.000000 transifex-python-3.4.0/tests/native/core/test_parsing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10082 2023-07-05 13:01:56.000000 transifex-python-3.4.0/tests/native/core/test_rendering.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 13:01:58.000000 transifex-python-3.4.0/tests/native/core/test_tools/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 13:01:56.000000 transifex-python-3.4.0/tests/native/core/test_tools/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 13:01:58.000000 transifex-python-3.4.0/tests/native/core/test_tools/test_migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 13:01:56.000000 transifex-python-3.4.0/tests/native/core/test_tools/test_migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3366 2023-07-05 13:01:56.000000 transifex-python-3.4.0/tests/native/core/test_tools/test_migrations/test_mark.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3768 2023-07-05 13:01:56.000000 transifex-python-3.4.0/tests/native/core/test_tools/test_migrations/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5632 2023-07-05 13:01:56.000000 transifex-python-3.4.0/tests/native/core/test_tools/test_migrations/test_review.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3441 2023-07-05 13:01:56.000000 transifex-python-3.4.0/tests/native/core/test_tools/test_migrations/test_save.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 13:01:58.000000 transifex-python-3.4.0/tests/native/django/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 13:01:56.000000 transifex-python-3.4.0/tests/native/django/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      658 2023-07-05 13:01:56.000000 transifex-python-3.4.0/tests/native/django/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 13:01:58.000000 transifex-python-3.4.0/tests/native/django/test_commands/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-05 13:01:56.000000 transifex-python-3.4.0/tests/native/django/test_commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2693 2023-07-05 13:01:56.000000 transifex-python-3.4.0/tests/native/django/test_commands/test_invalidatetransifex.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15314 2023-07-05 13:01:56.000000 transifex-python-3.4.0/tests/native/django/test_commands/test_migratetransifex.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14797 2023-07-05 13:01:56.000000 transifex-python-3.4.0/tests/native/django/test_commands/test_pushtransifex.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20355 2023-07-05 13:01:56.000000 transifex-python-3.4.0/tests/native/django/test_templatetag.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 13:01:58.000000 transifex-python-3.4.0/tests/native/django/test_tools/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 13:01:56.000000 transifex-python-3.4.0/tests/native/django/test_tools/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 13:01:58.000000 transifex-python-3.4.0/tests/native/django/test_tools/test_migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 13:01:56.000000 transifex-python-3.4.0/tests/native/django/test_tools/test_migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3575 2023-07-05 13:01:56.000000 transifex-python-3.4.0/tests/native/django/test_tools/test_migrations/test_templatetags.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 13:01:58.000000 transifex-python-3.4.0/tests/native/django/test_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 13:01:56.000000 transifex-python-3.4.0/tests/native/django/test_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-07-05 13:01:56.000000 transifex-python-3.4.0/tests/native/django/test_utils/test_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2818 2023-07-05 13:01:56.000000 transifex-python-3.4.0/tests/native/django/test_utils/test_templates.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 13:01:58.000000 transifex-python-3.4.0/transifex/
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-05 13:01:56.000000 transifex-python-3.4.0/transifex/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-07-05 13:01:58.000000 transifex-python-3.4.0/transifex/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 13:01:58.000000 transifex-python-3.4.0/transifex/api/
+-rw-r--r--   0 runner    (1001) docker     (123)     8677 2023-07-05 13:01:56.000000 transifex-python-3.4.0/transifex/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      979 2023-07-05 13:01:56.000000 transifex-python-3.4.0/transifex/api/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 13:01:58.000000 transifex-python-3.4.0/transifex/api/jsonapi/
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-07-05 13:01:56.000000 transifex-python-3.4.0/transifex/api/jsonapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7548 2023-07-05 13:01:56.000000 transifex-python-3.4.0/transifex/api/jsonapi/apis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2556 2023-07-05 13:01:56.000000 transifex-python-3.4.0/transifex/api/jsonapi/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5877 2023-07-05 13:01:56.000000 transifex-python-3.4.0/transifex/api/jsonapi/collections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-07-05 13:01:56.000000 transifex-python-3.4.0/transifex/api/jsonapi/compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5892 2023-07-05 13:01:56.000000 transifex-python-3.4.0/transifex/api/jsonapi/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31687 2023-07-05 13:01:56.000000 transifex-python-3.4.0/transifex/api/jsonapi/resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-07-05 13:01:56.000000 transifex-python-3.4.0/transifex/api/jsonapi/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 13:01:58.000000 transifex-python-3.4.0/transifex/common/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 13:01:56.000000 transifex-python-3.4.0/transifex/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-07-05 13:01:56.000000 transifex-python-3.4.0/transifex/common/_compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2779 2023-07-05 13:01:56.000000 transifex-python-3.4.0/transifex/common/console.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6811 2023-07-05 13:01:56.000000 transifex-python-3.4.0/transifex/common/strings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7311 2023-07-05 13:01:56.000000 transifex-python-3.4.0/transifex/common/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 13:01:58.000000 transifex-python-3.4.0/transifex/native/
+-rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-07-05 13:01:56.000000 transifex-python-3.4.0/transifex/native/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2502 2023-07-05 13:01:56.000000 transifex-python-3.4.0/transifex/native/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13370 2023-07-05 13:01:56.000000 transifex-python-3.4.0/transifex/native/cds.py
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-07-05 13:01:56.000000 transifex-python-3.4.0/transifex/native/consts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10331 2023-07-05 13:01:56.000000 transifex-python-3.4.0/transifex/native/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2477 2023-07-05 13:01:56.000000 transifex-python-3.4.0/transifex/native/daemon.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 13:01:58.000000 transifex-python-3.4.0/transifex/native/django/
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-07-05 13:01:56.000000 transifex-python-3.4.0/transifex/native/django/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4552 2023-07-05 13:01:56.000000 transifex-python-3.4.0/transifex/native/django/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-07-05 13:01:56.000000 transifex-python-3.4.0/transifex/native/django/compat.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 13:01:58.000000 transifex-python-3.4.0/transifex/native/django/management/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 13:01:56.000000 transifex-python-3.4.0/transifex/native/django/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 13:01:58.000000 transifex-python-3.4.0/transifex/native/django/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 13:01:56.000000 transifex-python-3.4.0/transifex/native/django/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2661 2023-07-05 13:01:56.000000 transifex-python-3.4.0/transifex/native/django/management/commands/transifex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-07-05 13:01:56.000000 transifex-python-3.4.0/transifex/native/django/management/common.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 13:01:58.000000 transifex-python-3.4.0/transifex/native/django/management/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 13:01:56.000000 transifex-python-3.4.0/transifex/native/django/management/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5010 2023-07-05 13:01:56.000000 transifex-python-3.4.0/transifex/native/django/management/utils/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2872 2023-07-05 13:01:56.000000 transifex-python-3.4.0/transifex/native/django/management/utils/invalidate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8356 2023-07-05 13:01:56.000000 transifex-python-3.4.0/transifex/native/django/management/utils/migrate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15614 2023-07-05 13:01:56.000000 transifex-python-3.4.0/transifex/native/django/management/utils/push.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15293 2023-07-05 13:01:56.000000 transifex-python-3.4.0/transifex/native/django/management/utils/try_templatetag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-07-05 13:01:56.000000 transifex-python-3.4.0/transifex/native/django/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 13:01:58.000000 transifex-python-3.4.0/transifex/native/django/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 13:01:56.000000 transifex-python-3.4.0/transifex/native/django/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12422 2023-07-05 13:01:56.000000 transifex-python-3.4.0/transifex/native/django/templatetags/transifex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-07-05 13:01:56.000000 transifex-python-3.4.0/transifex/native/django/templatetags/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 13:01:58.000000 transifex-python-3.4.0/transifex/native/django/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 13:01:56.000000 transifex-python-3.4.0/transifex/native/django/tools/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 13:01:58.000000 transifex-python-3.4.0/transifex/native/django/tools/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 13:01:56.000000 transifex-python-3.4.0/transifex/native/django/tools/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26025 2023-07-05 13:01:56.000000 transifex-python-3.4.0/transifex/native/django/tools/migrations/templatetags.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 13:01:58.000000 transifex-python-3.4.0/transifex/native/django/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     3045 2023-07-05 13:01:56.000000 transifex-python-3.4.0/transifex/native/django/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4158 2023-07-05 13:01:56.000000 transifex-python-3.4.0/transifex/native/django/utils/templates.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18581 2023-07-05 13:01:56.000000 transifex-python-3.4.0/transifex/native/parsing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9795 2023-07-05 13:01:56.000000 transifex-python-3.4.0/transifex/native/rendering.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2337 2023-07-05 13:01:56.000000 transifex-python-3.4.0/transifex/native/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 13:01:58.000000 transifex-python-3.4.0/transifex/native/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 13:01:56.000000 transifex-python-3.4.0/transifex/native/tools/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 13:01:58.000000 transifex-python-3.4.0/transifex/native/tools/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 13:01:56.000000 transifex-python-3.4.0/transifex/native/tools/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18197 2023-07-05 13:01:56.000000 transifex-python-3.4.0/transifex/native/tools/migrations/execution.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34399 2023-07-05 13:01:56.000000 transifex-python-3.4.0/transifex/native/tools/migrations/gettext.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5065 2023-07-05 13:01:56.000000 transifex-python-3.4.0/transifex/native/tools/migrations/mark.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5615 2023-07-05 13:01:56.000000 transifex-python-3.4.0/transifex/native/tools/migrations/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19611 2023-07-05 13:01:56.000000 transifex-python-3.4.0/transifex/native/tools/migrations/review.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6226 2023-07-05 13:01:56.000000 transifex-python-3.4.0/transifex/native/tools/migrations/save.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 13:01:58.000000 transifex-python-3.4.0/transifex_python.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3250 2023-07-05 13:01:58.000000 transifex-python-3.4.0/transifex_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4013 2023-07-05 13:01:58.000000 transifex-python-3.4.0/transifex_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 13:01:58.000000 transifex-python-3.4.0/transifex_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-05 13:01:58.000000 transifex-python-3.4.0/transifex_python.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-05 13:01:58.000000 transifex-python-3.4.0/transifex_python.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    68611 2023-07-05 13:01:56.000000 transifex-python-3.4.0/versioneer.py
```

### Comparing `transifex-python-3.3.0/PKG-INFO` & `transifex-python-3.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: transifex-python
-Version: 3.3.0
+Version: 3.4.0
 Summary: Transifex Python Toolkit
 Home-page: https://github.com/transifex/transifex-python
 Author: Transifex
 Author-email: info@transifex.com
 License: UNKNOWN
 Description: ![Test suite](https://github.com/transifex/transifex-python/workflows/Test%20suite/badge.svg?branch=master)
         [![codecov](https://codecov.io/gh/transifex/transifex-python/branch/master/graph/badge.svg)](https://codecov.io/gh/transifex/transifex-python)
```

### Comparing `transifex-python-3.3.0/README.md` & `transifex-python-3.4.0/README.md`

 * *Files identical despite different names*

### Comparing `transifex-python-3.3.0/setup.py` & `transifex-python-3.4.0/setup.py`

 * *Files identical despite different names*

### Comparing `transifex-python-3.3.0/tests/api/payloads.py` & `transifex-python-3.4.0/tests/api/payloads.py`

 * *Files identical despite different names*

### Comparing `transifex-python-3.3.0/tests/api/test_apis.py` & `transifex-python-3.4.0/tests/api/test_apis.py`

 * *Files identical despite different names*

### Comparing `transifex-python-3.3.0/tests/api/test_bulk.py` & `transifex-python-3.4.0/tests/api/test_bulk.py`

 * *Files identical despite different names*

### Comparing `transifex-python-3.3.0/tests/api/test_exceptions.py` & `transifex-python-3.4.0/tests/api/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `transifex-python-3.3.0/tests/api/test_plural_lists.py` & `transifex-python-3.4.0/tests/api/test_plural_lists.py`

 * *Files identical despite different names*

### Comparing `transifex-python-3.3.0/tests/api/test_queryset.py` & `transifex-python-3.4.0/tests/api/test_queryset.py`

 * *Files identical despite different names*

### Comparing `transifex-python-3.3.0/tests/api/test_relationships.py` & `transifex-python-3.4.0/tests/api/test_relationships.py`

 * *Files identical despite different names*

### Comparing `transifex-python-3.3.0/tests/api/test_single_resource.py` & `transifex-python-3.4.0/tests/api/test_single_resource.py`

 * *Files identical despite different names*

### Comparing `transifex-python-3.3.0/tests/common/test_is_plural.py` & `transifex-python-3.4.0/tests/common/test_is_plural.py`

 * *Files identical despite different names*

### Comparing `transifex-python-3.3.0/tests/common/test_strings.py` & `transifex-python-3.4.0/tests/common/test_strings.py`

 * *Files identical despite different names*

### Comparing `transifex-python-3.3.0/tests/native/core/test_cache.py` & `transifex-python-3.4.0/tests/native/core/test_cache.py`

 * *Files identical despite different names*

### Comparing `transifex-python-3.3.0/tests/native/core/test_cds.py` & `transifex-python-3.4.0/tests/native/core/test_cds.py`

 * *Files identical despite different names*

### Comparing `transifex-python-3.3.0/tests/native/core/test_core.py` & `transifex-python-3.4.0/tests/native/core/test_core.py`

 * *Files 0% similar despite different names*

```diff
@@ -376,16 +376,16 @@
         response = MagicMock()
         response.status_code = 200
         response.content = '{"data":{"status":"completed","details":{}}}'
         mock_get_status.return_value = response
 
         strings = [SourceString('a'), SourceString('b')]
         mytx = self._get_tx()
-        mytx.push_source_strings(strings, False, True, True)
-        mock_push_strings.assert_called_once_with(strings, False, True, True)
+        mytx.push_source_strings(strings, False, True, True, True)
+        mock_push_strings.assert_called_once_with(strings, False, True, True, True)
 
     @patch('transifex.native.core.MemoryCache.update')
     @patch('transifex.native.core.CDSHandler.fetch_translations')
     def test_fetch_translations_reaches_cds_handler_and_cache(self, mock_cds,
                                                               mock_cache):
         mytx = self._get_tx()
         mytx.fetch_translations()
```

### Comparing `transifex-python-3.3.0/tests/native/core/test_daemon.py` & `transifex-python-3.4.0/tests/native/core/test_daemon.py`

 * *Files identical despite different names*

### Comparing `transifex-python-3.3.0/tests/native/core/test_init.py` & `transifex-python-3.4.0/tests/native/core/test_init.py`

 * *Files identical despite different names*

### Comparing `transifex-python-3.3.0/tests/native/core/test_parsing.py` & `transifex-python-3.4.0/tests/native/core/test_parsing.py`

 * *Files identical despite different names*

### Comparing `transifex-python-3.3.0/tests/native/core/test_rendering.py` & `transifex-python-3.4.0/tests/native/core/test_rendering.py`

 * *Files identical despite different names*

### Comparing `transifex-python-3.3.0/tests/native/core/test_tools/test_migrations/test_mark.py` & `transifex-python-3.4.0/tests/native/core/test_tools/test_migrations/test_mark.py`

 * *Files identical despite different names*

### Comparing `transifex-python-3.3.0/tests/native/core/test_tools/test_migrations/test_models.py` & `transifex-python-3.4.0/tests/native/core/test_tools/test_migrations/test_models.py`

 * *Files identical despite different names*

### Comparing `transifex-python-3.3.0/tests/native/core/test_tools/test_migrations/test_review.py` & `transifex-python-3.4.0/tests/native/core/test_tools/test_migrations/test_review.py`

 * *Files identical despite different names*

### Comparing `transifex-python-3.3.0/tests/native/core/test_tools/test_migrations/test_save.py` & `transifex-python-3.4.0/tests/native/core/test_tools/test_migrations/test_save.py`

 * *Files identical despite different names*

### Comparing `transifex-python-3.3.0/tests/native/django/settings.py` & `transifex-python-3.4.0/tests/native/django/settings.py`

 * *Files identical despite different names*

### Comparing `transifex-python-3.3.0/tests/native/django/test_commands/__init__.py` & `transifex-python-3.4.0/tests/native/django/test_commands/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -27,14 +27,15 @@
         # Push
         'extension',
         'append_tags',
         'with_tags_only',
         'without_tags_only',
         'dry_run',
         'override_tags',
+        'override_occurrences',
         'do_not_keep_translations',
         'symlinks',
 
         # Invalidate
         'purge',
     )
     return command
```

### Comparing `transifex-python-3.3.0/tests/native/django/test_commands/test_invalidatetransifex.py` & `transifex-python-3.4.0/tests/native/django/test_commands/test_invalidatetransifex.py`

 * *Files identical despite different names*

### Comparing `transifex-python-3.3.0/tests/native/django/test_commands/test_migratetransifex.py` & `transifex-python-3.4.0/tests/native/django/test_commands/test_migratetransifex.py`

 * *Files identical despite different names*

### Comparing `transifex-python-3.3.0/tests/native/django/test_commands/test_pushtransifex.py` & `transifex-python-3.4.0/tests/native/django/test_commands/test_pushtransifex.py`

 * *Files identical despite different names*

### Comparing `transifex-python-3.3.0/tests/native/django/test_templatetag.py` & `transifex-python-3.4.0/tests/native/django/test_templatetag.py`

 * *Files identical despite different names*

### Comparing `transifex-python-3.3.0/tests/native/django/test_tools/test_migrations/test_templatetags.py` & `transifex-python-3.4.0/tests/native/django/test_tools/test_migrations/test_templatetags.py`

 * *Files identical despite different names*

### Comparing `transifex-python-3.3.0/tests/native/django/test_utils/test_init.py` & `transifex-python-3.4.0/tests/native/django/test_utils/test_init.py`

 * *Files identical despite different names*

### Comparing `transifex-python-3.3.0/tests/native/django/test_utils/test_templates.py` & `transifex-python-3.4.0/tests/native/django/test_utils/test_templates.py`

 * *Files identical despite different names*

### Comparing `transifex-python-3.3.0/transifex/api/__init__.py` & `transifex-python-3.4.0/transifex/api/__init__.py`

 * *Files identical despite different names*

### Comparing `transifex-python-3.3.0/transifex/api/exceptions.py` & `transifex-python-3.4.0/transifex/api/exceptions.py`

 * *Files identical despite different names*

### Comparing `transifex-python-3.3.0/transifex/api/jsonapi/apis.py` & `transifex-python-3.4.0/transifex/api/jsonapi/apis.py`

 * *Files identical despite different names*

### Comparing `transifex-python-3.3.0/transifex/api/jsonapi/auth.py` & `transifex-python-3.4.0/transifex/api/jsonapi/auth.py`

 * *Files identical despite different names*

### Comparing `transifex-python-3.3.0/transifex/api/jsonapi/collections.py` & `transifex-python-3.4.0/transifex/api/jsonapi/collections.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 from .exceptions import DoesNotExist, MultipleObjectsReturned
 
 
 class Collection(abc.MutableSequence):
     def __init__(self, API, url, params=None):
         if params is None:
             params = {}
+        else:
+            params = dict(params)
 
         parsed = urlparse(url)
         path, query = parsed.path, parsed.query
         query_params = parse_qs(query)
         query_params = {
             key: value[0] if len(value) == 1 else value
             for key, value in list(query_params.items())
@@ -51,36 +53,33 @@
         return self._previous_url
 
     def _evaluate(self, response_body=None):
         if self._data is not None:
             return
 
         if response_body is None:
-            response_body = self.API.request(
-                "get", self._url, params=self._params)
+            response_body = self.API.request("get", self._url, params=self._params)
         included = {}
         if "included" in response_body:
             included = {
                 (item["type"], item["id"]): item for item in response_body["included"]
             }
 
         self._data = []
         for item in response_body["data"]:
             related = {}
             for (name, relationship) in item.get("relationships", {}).items():
                 if relationship is None or "data" not in relationship:
                     continue
-                key = (relationship["data"]["type"],
-                       relationship["data"]["id"])
+                key = (relationship["data"]["type"], relationship["data"]["id"])
                 if key in included:
                     related[name] = self.API.new(included[key])
             relationships = item.pop("relationships", {})
             relationships.update(related)
-            self._data.append(self.API.new(
-                relationships=relationships, **item))
+            self._data.append(self.API.new(relationships=relationships, **item))
 
         self._next_url = response_body.get("links", {}).get("next")
         self._previous_url = response_body.get("links", {}).get("previous")
 
     # Make it look like a list
     def __getitem__(self, index):
         return self.data[index]
@@ -100,16 +99,15 @@
     def __repr__(self):
         return repr(self.data)
 
     def to_dict(self):
         self_url = self._url
         if self._params:
             self_url += "?" + "&".join(
-                ("{}={}".format(key, value)
-                 for key, value in self._params.items())
+                ("{}={}".format(key, value) for key, value in self._params.items())
             )
 
         links = {"self": self_url}
         if self.has_next():
             links["next"] = self.next_url()
         else:
             links["next"] = None
@@ -121,21 +119,21 @@
         return {"data": [item.to_dict() for item in self.data], "links": links}
 
     # Pagination
     def has_next(self):
         return bool(self.next_url)
 
     def next(self):
-        return self.__class__(self.API, self.next_url, self._params)
+        return self.__class__(self.API, self.next_url)
 
     def has_previous(self):
         return bool(self.previous_url)
 
     def previous(self):
-        return self.__class__(self.API, self.previous_url, self._params)
+        return self.__class__(self.API, self.previous_url)
 
     def all_pages(self):
         if self.data:
             yield self
         page = self
         while page.has_next():
             page = page.next()
@@ -149,16 +147,15 @@
     # Filters etc
     def filter(self, **filters):
         from .resources import Resource
 
         params = dict(self._params)
 
         for key, value in filters.items():
-            key = "filter" + "".join(("[{}]".format(part)
-                                      for part in key.split("__")))
+            key = "filter" + "".join(("[{}]".format(part) for part in key.split("__")))
             if isinstance(value, Resource):
                 value = value.id
 
             params[key] = value
 
         return self.__class__(self.API, self._url, params)
```

### Comparing `transifex-python-3.3.0/transifex/api/jsonapi/compat.py` & `transifex-python-3.4.0/transifex/api/jsonapi/compat.py`

 * *Files identical despite different names*

### Comparing `transifex-python-3.3.0/transifex/api/jsonapi/exceptions.py` & `transifex-python-3.4.0/transifex/api/jsonapi/exceptions.py`

 * *Files identical despite different names*

### Comparing `transifex-python-3.3.0/transifex/api/jsonapi/resources.py` & `transifex-python-3.4.0/transifex/api/jsonapi/resources.py`

 * *Files identical despite different names*

### Comparing `transifex-python-3.3.0/transifex/api/jsonapi/utils.py` & `transifex-python-3.4.0/transifex/api/jsonapi/utils.py`

 * *Files identical despite different names*

### Comparing `transifex-python-3.3.0/transifex/common/console.py` & `transifex-python-3.4.0/transifex/common/console.py`

 * *Files identical despite different names*

### Comparing `transifex-python-3.3.0/transifex/common/strings.py` & `transifex-python-3.4.0/transifex/common/strings.py`

 * *Files identical despite different names*

### Comparing `transifex-python-3.3.0/transifex/common/utils.py` & `transifex-python-3.4.0/transifex/common/utils.py`

 * *Files identical despite different names*

### Comparing `transifex-python-3.3.0/transifex/native/__init__.py` & `transifex-python-3.4.0/transifex/native/__init__.py`

 * *Files identical despite different names*

### Comparing `transifex-python-3.3.0/transifex/native/cache.py` & `transifex-python-3.4.0/transifex/native/cache.py`

 * *Files identical despite different names*

### Comparing `transifex-python-3.3.0/transifex/native/cds.py` & `transifex-python-3.4.0/transifex/native/cds.py`

 * *Files 3% similar despite different names*

```diff
@@ -200,26 +200,29 @@
                 )  # pragma no cover
                 translations[language_code] = (False, {})
 
         return translations
 
     def push_source_strings(self, strings, purge=False,
                             do_not_keep_translations=False,
-                            override_tags=False):
+                            override_tags=False,
+                            override_occurrences=False):
         """Push source strings to CDS.
 
         :param list(SourceString) strings: a list of `SourceString` objects
             holding source strings
         :param bool purge: True deletes destination source content not included
             in pushed content. False appends the pushed content to destination
             source content.
         :param bool do_not_keep_translations: True deletes translations when the
             source strings of existing keys are updated. False preserves them.
         :param bool override_tags: True replaces all the tags of pushed strings.
             False appends them to existing tags.
+        :param bool override_occurrences: True replaces all the occurrences of pushed strings.
+            False appends them to existing occurrences.
         :return: the HTTP response object
         :rtype: requests.Response
         """
         if not self.secret:
             raise Exception('You need to use `TRANSIFEX_SECRET` when pushing '
                             'source content')
 
@@ -234,14 +237,15 @@
                 headers=self._get_headers(use_secret=True),
                 json={
                     'data': data,
                     'meta': {
                         'purge': purge,
                         'keep_translations': not do_not_keep_translations,
                         'override_tags': override_tags,
+                        'override_occurrences': override_occurrences,
                     },
                 }
             )
             response.raise_for_status()
 
         except requests.ConnectionError:
             logger.error(
```

### Comparing `transifex-python-3.3.0/transifex/native/core.py` & `transifex-python-3.4.0/transifex/native/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -194,32 +194,35 @@
     def fetch_translations(self):
         """Fetch fresh content from the CDS."""
         self._check_initialization()
         self._cache.update(self._cds_handler.fetch_translations())
 
     def push_source_strings(self, strings, purge=False,
                             do_not_keep_translations=False,
-                            override_tags=False):
+                            override_tags=False,
+                            override_occurrences=False):
         """Push the given source strings to the CDS.
 
         :param list strings: a list of SourceString objects
         :param bool purge: True deletes destination source content not included
             in pushed content. False appends the pushed content to destination
             source content.
         :param bool do_not_keep_translations: True deletes translations when the
             source strings of existing keys are updated. False preserves them.
         :param bool override_tags: True replaces all the tags of pushed strings.
             False appends them to existing tags.
+        :param bool override_occurrences: True replaces all the occurrences of pushed strings.
+            False appends them to existing occurrences.
         :return: a tuple containing the status code and the content of the
             response
         :rtype: tuple
         """
         self._check_initialization()
         response = self._cds_handler.push_source_strings(
-            strings, purge, do_not_keep_translations, override_tags)
+            strings, purge, do_not_keep_translations, override_tags, override_occurrences)
         return response.status_code, json.loads(response.content)
 
     def get_push_status(self, job_path):
         """Push the given source strings to the CDS.
 
         :param str job_path: Job url path
         :return: a tuple containing the status code and the content of the
```

### Comparing `transifex-python-3.3.0/transifex/native/daemon.py` & `transifex-python-3.4.0/transifex/native/daemon.py`

 * *Files identical despite different names*

### Comparing `transifex-python-3.3.0/transifex/native/django/apps.py` & `transifex-python-3.4.0/transifex/native/django/apps.py`

 * *Files identical despite different names*

### Comparing `transifex-python-3.3.0/transifex/native/django/management/commands/transifex.py` & `transifex-python-3.4.0/transifex/native/django/management/commands/transifex.py`

 * *Files identical despite different names*

### Comparing `transifex-python-3.3.0/transifex/native/django/management/common.py` & `transifex-python-3.4.0/transifex/native/django/management/common.py`

 * *Files identical despite different names*

### Comparing `transifex-python-3.3.0/transifex/native/django/management/utils/base.py` & `transifex-python-3.4.0/transifex/native/django/management/utils/base.py`

 * *Files identical despite different names*

### Comparing `transifex-python-3.3.0/transifex/native/django/management/utils/invalidate.py` & `transifex-python-3.4.0/transifex/native/django/management/utils/invalidate.py`

 * *Files identical despite different names*

### Comparing `transifex-python-3.3.0/transifex/native/django/management/utils/migrate.py` & `transifex-python-3.4.0/transifex/native/django/management/utils/migrate.py`

 * *Files identical despite different names*

### Comparing `transifex-python-3.3.0/transifex/native/django/management/utils/push.py` & `transifex-python-3.4.0/transifex/native/django/management/utils/push.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,14 +64,18 @@
             help=('Disable polling for upload results'),
         )
         parser.add_argument(
             '--override-tags', action='store_true', dest='override_tags', default=False,
             help=('Override tags when pushing content'),
         )
         parser.add_argument(
+            '--override-occurrences', action='store_true', dest='override_occurrences', default=False,
+            help=('Override occurrences when pushing content'),
+        )
+        parser.add_argument(
             '--do-not-keep-translations', action='store_true', dest='do_not_keep_translations', default=False,
             help=('Remove translations when source strings change'),
         )
         parser.add_argument(
             '--verbose', '-v', action='store_true',
             dest='verbose_output', default=False,
             help=('Verbose output'),
@@ -95,14 +99,15 @@
         self.purge = options['purge']
         self.symlinks = options['symlinks']
         self.append_tags = options['append_tags']
         self.with_tags_only = options['with_tags_only']
         self.without_tags_only = options['without_tags_only']
         self.dry_run = options['dry_run']
         self.override_tags = options['override_tags']
+        self.override_occurrences = options['override_occurrences']
         self.do_not_keep_translations = options['do_not_keep_translations']
         self.no_wait = options['no_wait']
         self.key_generator = options['key_generator']
         extensions = options['extensions']
         if self.domain == 'djangojs':
             exts = extensions if extensions else ['js']
         else:
@@ -189,15 +194,16 @@
 
         Color.echo(
             'Pushing [warn]{}[end] unique translatable strings '
             'to Transifex...'.format(total)
         )
         status_code, response_content = tx.push_source_strings(
             self.string_collection.strings.values(), self.purge,
-            self.do_not_keep_translations, self.override_tags
+            self.do_not_keep_translations, self.override_tags,
+            self.override_occurrences
         )
 
         if self.no_wait:
             Color.echo('Queued')
             return
 
         job_url = response_content['data']['links']['job']
```

### Comparing `transifex-python-3.3.0/transifex/native/django/management/utils/try_templatetag.py` & `transifex-python-3.4.0/transifex/native/django/management/utils/try_templatetag.py`

 * *Files identical despite different names*

### Comparing `transifex-python-3.3.0/transifex/native/django/settings.py` & `transifex-python-3.4.0/transifex/native/django/settings.py`

 * *Files identical despite different names*

### Comparing `transifex-python-3.3.0/transifex/native/django/templatetags/transifex.py` & `transifex-python-3.4.0/transifex/native/django/templatetags/transifex.py`

 * *Files identical despite different names*

### Comparing `transifex-python-3.3.0/transifex/native/django/templatetags/utils.py` & `transifex-python-3.4.0/transifex/native/django/templatetags/utils.py`

 * *Files identical despite different names*

### Comparing `transifex-python-3.3.0/transifex/native/django/tools/migrations/templatetags.py` & `transifex-python-3.4.0/transifex/native/django/tools/migrations/templatetags.py`

 * *Files identical despite different names*

### Comparing `transifex-python-3.3.0/transifex/native/django/utils/__init__.py` & `transifex-python-3.4.0/transifex/native/django/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `transifex-python-3.3.0/transifex/native/django/utils/templates.py` & `transifex-python-3.4.0/transifex/native/django/utils/templates.py`

 * *Files identical despite different names*

### Comparing `transifex-python-3.3.0/transifex/native/parsing.py` & `transifex-python-3.4.0/transifex/native/parsing.py`

 * *Files identical despite different names*

### Comparing `transifex-python-3.3.0/transifex/native/rendering.py` & `transifex-python-3.4.0/transifex/native/rendering.py`

 * *Files identical despite different names*

### Comparing `transifex-python-3.3.0/transifex/native/settings.py` & `transifex-python-3.4.0/transifex/native/settings.py`

 * *Files identical despite different names*

### Comparing `transifex-python-3.3.0/transifex/native/tools/migrations/execution.py` & `transifex-python-3.4.0/transifex/native/tools/migrations/execution.py`

 * *Files identical despite different names*

### Comparing `transifex-python-3.3.0/transifex/native/tools/migrations/gettext.py` & `transifex-python-3.4.0/transifex/native/tools/migrations/gettext.py`

 * *Files identical despite different names*

### Comparing `transifex-python-3.3.0/transifex/native/tools/migrations/mark.py` & `transifex-python-3.4.0/transifex/native/tools/migrations/mark.py`

 * *Files identical despite different names*

### Comparing `transifex-python-3.3.0/transifex/native/tools/migrations/models.py` & `transifex-python-3.4.0/transifex/native/tools/migrations/models.py`

 * *Files identical despite different names*

### Comparing `transifex-python-3.3.0/transifex/native/tools/migrations/review.py` & `transifex-python-3.4.0/transifex/native/tools/migrations/review.py`

 * *Files identical despite different names*

### Comparing `transifex-python-3.3.0/transifex/native/tools/migrations/save.py` & `transifex-python-3.4.0/transifex/native/tools/migrations/save.py`

 * *Files identical despite different names*

### Comparing `transifex-python-3.3.0/transifex_python.egg-info/PKG-INFO` & `transifex-python-3.4.0/transifex_python.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: transifex-python
-Version: 3.3.0
+Version: 3.4.0
 Summary: Transifex Python Toolkit
 Home-page: https://github.com/transifex/transifex-python
 Author: Transifex
 Author-email: info@transifex.com
 License: UNKNOWN
 Description: ![Test suite](https://github.com/transifex/transifex-python/workflows/Test%20suite/badge.svg?branch=master)
         [![codecov](https://codecov.io/gh/transifex/transifex-python/branch/master/graph/badge.svg)](https://codecov.io/gh/transifex/transifex-python)
```

### Comparing `transifex-python-3.3.0/transifex_python.egg-info/SOURCES.txt` & `transifex-python-3.4.0/transifex_python.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `transifex-python-3.3.0/versioneer.py` & `transifex-python-3.4.0/versioneer.py`

 * *Files identical despite different names*

